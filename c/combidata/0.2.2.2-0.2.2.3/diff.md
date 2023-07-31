# Comparing `tmp/combidata-0.2.2.2.tar.gz` & `tmp/combidata-0.2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combidata-0.2.2.2.tar", last modified: Mon Jul 31 14:10:05 2023, max compression
+gzip compressed data, was "combidata-0.2.2.3.tar", last modified: Mon Jul 31 14:42:26 2023, max compression
```

## Comparing `combidata-0.2.2.2.tar` & `combidata-0.2.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:10:05.752617 combidata-0.2.2.2/
--rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.2.2/LICENSE
--rw-rw-rw-   0        0        0    10605 2023-07-31 14:10:05.752411 combidata-0.2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9822 2023-07-30 14:49:48.000000 combidata-0.2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 14:10:05.710978 combidata-0.2.2.2/combidata/
--rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.2.2/combidata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:10:05.743260 combidata-0.2.2.2/combidata/classes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2.2/combidata/classes/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-07-29 20:41:49.000000 combidata-0.2.2.2/combidata/classes/case.py
--rw-rw-rw-   0        0        0     3205 2023-07-31 13:54:33.000000 combidata-0.2.2.2/combidata/classes/combination.py
--rw-rw-rw-   0        0        0    12143 2023-07-31 12:40:31.000000 combidata-0.2.2.2/combidata/classes/data_generator.py
--rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.2.2/combidata/classes/process.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:10:05.749260 combidata-0.2.2.2/combidata/processes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2.2/combidata/processes/__init__.py
--rw-rw-rw-   0        0        0     3474 2023-07-31 12:32:53.000000 combidata-0.2.2.2/combidata/processes/combine.py
--rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.2.2/combidata/processes/form.py
--rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.2.2/combidata/processes/genetate.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:10:05.737257 combidata-0.2.2.2/combidata.egg-info/
--rw-rw-rw-   0        0        0    10605 2023-07-31 14:10:05.000000 combidata-0.2.2.2/combidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-31 14:10:05.000000 combidata-0.2.2.2/combidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:10:05.000000 combidata-0.2.2.2/combidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 14:10:05.000000 combidata-0.2.2.2/combidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      555 2023-07-31 14:08:31.000000 combidata-0.2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 14:10:05.752617 combidata-0.2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-07-31 14:08:31.000000 combidata-0.2.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:10:05.750258 combidata-0.2.2.2/tests/
--rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.2.2/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:26.141180 combidata-0.2.2.3/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.2.3/LICENSE
+-rw-rw-rw-   0        0        0    10605 2023-07-31 14:42:26.140184 combidata-0.2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9822 2023-07-30 14:49:48.000000 combidata-0.2.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:26.065182 combidata-0.2.2.3/combidata/
+-rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.2.3/combidata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:26.120178 combidata-0.2.2.3/combidata/classes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2.3/combidata/classes/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-07-29 20:41:49.000000 combidata-0.2.2.3/combidata/classes/case.py
+-rw-rw-rw-   0        0        0     3233 2023-07-31 14:38:13.000000 combidata-0.2.2.3/combidata/classes/combination.py
+-rw-rw-rw-   0        0        0    12143 2023-07-31 12:40:31.000000 combidata-0.2.2.3/combidata/classes/data_generator.py
+-rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.2.3/combidata/classes/process.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:26.134180 combidata-0.2.2.3/combidata/processes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2.3/combidata/processes/__init__.py
+-rw-rw-rw-   0        0        0     3474 2023-07-31 12:32:53.000000 combidata-0.2.2.3/combidata/processes/combine.py
+-rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.2.3/combidata/processes/form.py
+-rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.2.3/combidata/processes/genetate.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:26.093178 combidata-0.2.2.3/combidata.egg-info/
+-rw-rw-rw-   0        0        0    10605 2023-07-31 14:42:26.000000 combidata-0.2.2.3/combidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-31 14:42:26.000000 combidata-0.2.2.3/combidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:42:26.000000 combidata-0.2.2.3/combidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 14:42:26.000000 combidata-0.2.2.3/combidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2023-07-31 14:41:46.000000 combidata-0.2.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:42:26.142179 combidata-0.2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-31 14:41:46.000000 combidata-0.2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:26.138184 combidata-0.2.2.3/tests/
+-rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.2.3/tests/test_generator.py
```

### Comparing `combidata-0.2.2.2/LICENSE` & `combidata-0.2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2.2/PKG-INFO` & `combidata-0.2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.2.2
+Version: 0.2.2.3
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.2.2/README.md` & `combidata-0.2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2.2/combidata/classes/case.py` & `combidata-0.2.2.3/combidata/classes/case.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2.2/combidata/classes/combination.py` & `combidata-0.2.2.3/combidata/classes/combination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import traceback
 
 
 def step_not_done(current_step_name, combi):
     if isinstance(combi, list):
         for combination in combi:
             if combination.step_done != current_step_name and combination.step_done != "STOP":
@@ -34,15 +35,15 @@
     """
     test_seed = None
     formed_data = None
 
     step_done = None  # last passed step
 
     def __init__(self, case, workflow, init_lib, template, tools, logger, generator_id):
-        self.init_lib = init_lib
+        self.init_lib = copy.deepcopy(init_lib)
         self.main_case = case
         self.template = template
         self.tools = tools
         self.logger = logger
         self.generator_id = generator_id
 
         self.generated_data = {}
```

### Comparing `combidata-0.2.2.2/combidata/classes/data_generator.py` & `combidata-0.2.2.3/combidata/classes/data_generator.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2.2/combidata/processes/combine.py` & `combidata-0.2.2.3/combidata/processes/combine.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2.2/combidata/processes/form.py` & `combidata-0.2.2.3/combidata/processes/form.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2.2/combidata/processes/genetate.py` & `combidata-0.2.2.3/combidata/processes/genetate.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2.2/combidata.egg-info/PKG-INFO` & `combidata-0.2.2.3/combidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.2.2
+Version: 0.2.2.3
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.2.2/pyproject.toml` & `combidata-0.2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     "testing API",
     "testing",
     "autotesting"
 ]
 urls = {Homepage = "https://github.com/Warrfie/combidata"}
 authors = [{name = "MaximKuklikov(Warrfie)", email = "warrfie@gmail.com"}]
 requires-python = ">=3.10"
-version="0.2.2.2"
+version="0.2.2.3"
```

### Comparing `combidata-0.2.2.2/setup.py` & `combidata-0.2.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="combidata",
-    version="0.2.2.2",
+    version="0.2.2.3",
     description="Package for random data generation and combination different cases",
     long_description=long_description,
     url="https://github.com/Warrfie/combidata",
     author="Kuklikov Maxim (Warrfie)",
     author_email="warrfie@gmail.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `combidata-0.2.2.2/tests/test_generator.py` & `combidata-0.2.2.3/tests/test_generator.py`

 * *Files identical despite different names*

