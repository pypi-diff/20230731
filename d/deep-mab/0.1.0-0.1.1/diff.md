# Comparing `tmp/deep_mab-0.1.0.tar.gz` & `tmp/deep_mab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_mab-0.1.0.tar", last modified: Mon Jul 31 01:29:10 2023, max compression
+gzip compressed data, was "deep_mab-0.1.1.tar", last modified: Mon Jul 31 02:35:59 2023, max compression
```

## Comparing `deep_mab-0.1.0.tar` & `deep_mab-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:29:10.887172 deep_mab-0.1.0/
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:15:16.000000 deep_mab-0.1.0/Dockerfile
--rw-r--r--   0 samsonqian   (501) staff       (20)     1067 2023-07-31 01:15:35.000000 deep_mab-0.1.0/LICENSE
--rw-r--r--   0 samsonqian   (501) staff       (20)       61 2023-07-31 01:15:55.000000 deep_mab-0.1.0/MANIFEST.in
--rw-r--r--   0 samsonqian   (501) staff       (20)     1508 2023-07-31 01:29:10.887254 deep_mab-0.1.0/PKG-INFO
--rw-r--r--   0 samsonqian   (501) staff       (20)     1154 2023-07-31 01:25:44.000000 deep_mab-0.1.0/README.md
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:29:10.883147 deep_mab-0.1.0/deep_mab/
--rw-r--r--   0 samsonqian   (501) staff       (20)       47 2023-07-31 01:08:35.000000 deep_mab-0.1.0/deep_mab/__init__.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:29:10.885658 deep_mab-0.1.0/deep_mab/cmab/
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:00:32.000000 deep_mab-0.1.0/deep_mab/cmab/__init__.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     1320 2023-07-31 01:09:15.000000 deep_mab-0.1.0/deep_mab/cmab/cbandit.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     1777 2023-07-31 01:11:10.000000 deep_mab-0.1.0/deep_mab/cmab/lin_ucb.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     2463 2023-07-31 01:14:44.000000 deep_mab-0.1.0/deep_mab/cmab/nn_epsilon_greedy.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     2615 2023-07-31 01:12:50.000000 deep_mab-0.1.0/deep_mab/cmab/nn_ucb.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:29:10.886940 deep_mab-0.1.0/deep_mab/mab/
--rw-r--r--   0 samsonqian   (501) staff       (20)       20 2023-07-31 01:04:29.000000 deep_mab-0.1.0/deep_mab/mab/__init__.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     1617 2023-07-31 01:04:29.000000 deep_mab-0.1.0/deep_mab/mab/bandit.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     1425 2023-07-31 01:05:42.000000 deep_mab-0.1.0/deep_mab/mab/epsilon_greedy.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     1416 2023-07-31 01:07:27.000000 deep_mab-0.1.0/deep_mab/mab/thompson_sampling.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     1433 2023-07-31 01:06:27.000000 deep_mab-0.1.0/deep_mab/mab/ucb.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:29:10.883957 deep_mab-0.1.0/deep_mab.egg-info/
--rw-r--r--   0 samsonqian   (501) staff       (20)     1508 2023-07-31 01:29:10.000000 deep_mab-0.1.0/deep_mab.egg-info/PKG-INFO
--rw-r--r--   0 samsonqian   (501) staff       (20)      493 2023-07-31 01:29:10.000000 deep_mab-0.1.0/deep_mab.egg-info/SOURCES.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)        1 2023-07-31 01:29:10.000000 deep_mab-0.1.0/deep_mab.egg-info/dependency_links.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)        9 2023-07-31 01:29:10.000000 deep_mab-0.1.0/deep_mab.egg-info/top_level.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)      203 2023-07-31 01:16:20.000000 deep_mab-0.1.0/requirements.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)      141 2023-07-31 01:29:10.887575 deep_mab-0.1.0/setup.cfg
--rw-r--r--   0 samsonqian   (501) staff       (20)     1385 2023-07-31 01:29:02.000000 deep_mab-0.1.0/setup.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:35:59.653011 deep_mab-0.1.1/
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:31:33.000000 deep_mab-0.1.1/Dockerfile
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1067 2023-07-31 01:31:33.000000 deep_mab-0.1.1/LICENSE
+-rw-r--r--   0 samsonqian   (501) staff       (20)       61 2023-07-31 01:31:33.000000 deep_mab-0.1.1/MANIFEST.in
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1465 2023-07-31 02:35:59.653099 deep_mab-0.1.1/PKG-INFO
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1111 2023-07-31 01:31:33.000000 deep_mab-0.1.1/README.md
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:35:59.650046 deep_mab-0.1.1/deep_mab/
+-rw-r--r--   0 samsonqian   (501) staff       (20)       47 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/__init__.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:35:59.651727 deep_mab-0.1.1/deep_mab/cmab/
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/cmab/__init__.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1320 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/cmab/cbandit.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1777 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/cmab/lin_ucb.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     2463 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/cmab/nn_epsilon_greedy.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     2615 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/cmab/nn_ucb.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:35:59.652848 deep_mab-0.1.1/deep_mab/mab/
+-rw-r--r--   0 samsonqian   (501) staff       (20)       20 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/mab/__init__.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1617 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/mab/bandit.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1425 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/mab/epsilon_greedy.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1416 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/mab/thompson_sampling.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1433 2023-07-31 01:31:33.000000 deep_mab-0.1.1/deep_mab/mab/ucb.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:35:59.650761 deep_mab-0.1.1/deep_mab.egg-info/
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1465 2023-07-31 02:35:59.000000 deep_mab-0.1.1/deep_mab.egg-info/PKG-INFO
+-rw-r--r--   0 samsonqian   (501) staff       (20)      493 2023-07-31 02:35:59.000000 deep_mab-0.1.1/deep_mab.egg-info/SOURCES.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)        1 2023-07-31 02:35:59.000000 deep_mab-0.1.1/deep_mab.egg-info/dependency_links.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)        9 2023-07-31 02:35:59.000000 deep_mab-0.1.1/deep_mab.egg-info/top_level.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)      203 2023-07-31 01:31:33.000000 deep_mab-0.1.1/requirements.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)      141 2023-07-31 02:35:59.653432 deep_mab-0.1.1/setup.cfg
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1385 2023-07-31 02:35:39.000000 deep_mab-0.1.1/setup.py
```

### Comparing `deep_mab-0.1.0/LICENSE` & `deep_mab-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/PKG-INFO` & `deep_mab-0.1.1/deep_mab.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: deep_mab
-Version: 0.1.0
+Name: deep-mab
+Version: 0.1.1
 Summary: Contextual MAB algorithms
 Home-page: https://github.com/samsonq/contextual-bandits
 Author: Samson Qian
 Author-email: samsonqian@gmail.com
 License: MIT
 Keywords: mab deep_mab deep_mab reinforcement-learning
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Contextual MAB
+# Deep Contextual MAB
 MAB and linear/non-linear Contextual MAB algorithms.
 
 ## Algorithms
 
 #### Multi-Arm Bandits
 * [x] Epsilon Greedy
 * [x] UCB
@@ -23,36 +23,36 @@
 
 #### Contextual Multi-Arm Bandits
 * [x] Neural Net Epsilon Greedy
 * [x] LinUCB
 * [x] Neural Net UCB
 
 ## Usage Instructions
-* This project is published on [PyPI](https://pypi.org/project/contextual-mab/). To install package, run:
+* This project is published on [PyPI](https://pypi.org/project/deep-mab/). To install package, run:
 
   ```
-  pip install contextual-mab
+  pip install deep-mab
   ```
 * To run the algorithms, import the package and call the respective functions. For example, to run the LinUCB algorithm, run:
 
   ```
-  from contextual_bandits.algorithms import LinUCB
+  from deep_mab.cmab import LinUCB
   model = LinUCB(n_arms=10, alpha=1, fit_intercept=True)
   model.fit(X_train, y_train)
   model.predict(X_test)
   ```
 * For more details, refer to the [documentation](https://contextual-bandits.readthedocs.io/en/latest/).
 * To run the examples, clone the repository and run the following commands:
 
   ```
-  cd contextual-bandits
+  cd deep-mab
   pip install -r requirements.txt
   python examples/linucb_example.py
   ```
 * To run the tests, run the following commands:
 
   ```
-  cd contextual-bandits
+  cd deep-mab
   pip install -r requirements.txt
   pytest
   ```
```

### Comparing `deep_mab-0.1.0/README.md` & `deep_mab-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Contextual MAB
+# Deep Contextual MAB
 MAB and linear/non-linear Contextual MAB algorithms.
 
 ## Algorithms
 
 #### Multi-Arm Bandits
 * [x] Epsilon Greedy
 * [x] UCB
@@ -10,36 +10,36 @@
 
 #### Contextual Multi-Arm Bandits
 * [x] Neural Net Epsilon Greedy
 * [x] LinUCB
 * [x] Neural Net UCB
 
 ## Usage Instructions
-* This project is published on [PyPI](https://pypi.org/project/contextual-mab/). To install package, run:
+* This project is published on [PyPI](https://pypi.org/project/deep-mab/). To install package, run:
 
   ```
-  pip install contextual-mab
+  pip install deep-mab
   ```
 * To run the algorithms, import the package and call the respective functions. For example, to run the LinUCB algorithm, run:
 
   ```
-  from contextual_bandits.algorithms import LinUCB
+  from deep_mab.cmab import LinUCB
   model = LinUCB(n_arms=10, alpha=1, fit_intercept=True)
   model.fit(X_train, y_train)
   model.predict(X_test)
   ```
 * For more details, refer to the [documentation](https://contextual-bandits.readthedocs.io/en/latest/).
 * To run the examples, clone the repository and run the following commands:
 
   ```
-  cd contextual-bandits
+  cd deep-mab
   pip install -r requirements.txt
   python examples/linucb_example.py
   ```
 * To run the tests, run the following commands:
 
   ```
-  cd contextual-bandits
+  cd deep-mab
   pip install -r requirements.txt
   pytest
   ```
```

### Comparing `deep_mab-0.1.0/deep_mab/cmab/cbandit.py` & `deep_mab-0.1.1/deep_mab/cmab/cbandit.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab/cmab/lin_ucb.py` & `deep_mab-0.1.1/deep_mab/cmab/lin_ucb.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab/cmab/nn_epsilon_greedy.py` & `deep_mab-0.1.1/deep_mab/cmab/nn_epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab/cmab/nn_ucb.py` & `deep_mab-0.1.1/deep_mab/cmab/nn_ucb.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab/mab/bandit.py` & `deep_mab-0.1.1/deep_mab/mab/bandit.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab/mab/epsilon_greedy.py` & `deep_mab-0.1.1/deep_mab/mab/epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab/mab/thompson_sampling.py` & `deep_mab-0.1.1/deep_mab/mab/thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab/mab/ucb.py` & `deep_mab-0.1.1/deep_mab/mab/ucb.py`

 * *Files identical despite different names*

### Comparing `deep_mab-0.1.0/deep_mab.egg-info/PKG-INFO` & `deep_mab-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: deep-mab
-Version: 0.1.0
+Name: deep_mab
+Version: 0.1.1
 Summary: Contextual MAB algorithms
 Home-page: https://github.com/samsonq/contextual-bandits
 Author: Samson Qian
 Author-email: samsonqian@gmail.com
 License: MIT
 Keywords: mab deep_mab deep_mab reinforcement-learning
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Contextual MAB
+# Deep Contextual MAB
 MAB and linear/non-linear Contextual MAB algorithms.
 
 ## Algorithms
 
 #### Multi-Arm Bandits
 * [x] Epsilon Greedy
 * [x] UCB
@@ -23,36 +23,36 @@
 
 #### Contextual Multi-Arm Bandits
 * [x] Neural Net Epsilon Greedy
 * [x] LinUCB
 * [x] Neural Net UCB
 
 ## Usage Instructions
-* This project is published on [PyPI](https://pypi.org/project/contextual-mab/). To install package, run:
+* This project is published on [PyPI](https://pypi.org/project/deep-mab/). To install package, run:
 
   ```
-  pip install contextual-mab
+  pip install deep-mab
   ```
 * To run the algorithms, import the package and call the respective functions. For example, to run the LinUCB algorithm, run:
 
   ```
-  from contextual_bandits.algorithms import LinUCB
+  from deep_mab.cmab import LinUCB
   model = LinUCB(n_arms=10, alpha=1, fit_intercept=True)
   model.fit(X_train, y_train)
   model.predict(X_test)
   ```
 * For more details, refer to the [documentation](https://contextual-bandits.readthedocs.io/en/latest/).
 * To run the examples, clone the repository and run the following commands:
 
   ```
-  cd contextual-bandits
+  cd deep-mab
   pip install -r requirements.txt
   python examples/linucb_example.py
   ```
 * To run the tests, run the following commands:
 
   ```
-  cd contextual-bandits
+  cd deep-mab
   pip install -r requirements.txt
   pytest
   ```
```

### Comparing `deep_mab-0.1.0/setup.py` & `deep_mab-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     install_reqs = _parse_requirements("requirements.txt")
 except Exception as e:
     logging.warning('Fail load requirements file, so using default ones.')
     install_reqs = []
 
 setup(
     name="deep_mab",
-    version="0.1.0",
+    version="0.1.1",
     author="Samson Qian",
     author_email="samsonqian@gmail.com",
     packages=["deep_mab", "deep_mab.cmab", "deep_mab.mab"],
     url="https://github.com/samsonq/contextual-bandits",
     license="MIT",
     description="Contextual MAB algorithms",
     long_description=README,
```

