# Comparing `tmp/combidata-0.2.2.tar.gz` & `tmp/combidata-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combidata-0.2.2.tar", last modified: Sun Jul 30 14:50:50 2023, max compression
+gzip compressed data, was "combidata-0.2.2.1.tar", last modified: Mon Jul 31 12:56:56 2023, max compression
```

## Comparing `combidata-0.2.2.tar` & `combidata-0.2.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.320017 combidata-0.2.2/
--rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    10603 2023-07-30 14:50:50.319014 combidata-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9822 2023-07-30 14:49:48.000000 combidata-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.218012 combidata-0.2.2/combidata/
--rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.2/combidata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.276017 combidata-0.2.2/combidata/classes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2/combidata/classes/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-07-29 20:41:49.000000 combidata-0.2.2/combidata/classes/case.py
--rw-rw-rw-   0        0        0     3107 2023-07-30 08:57:21.000000 combidata-0.2.2/combidata/classes/combination.py
--rw-rw-rw-   0        0        0    11849 2023-07-30 14:42:10.000000 combidata-0.2.2/combidata/classes/data_generator.py
--rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.2/combidata/classes/process.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.305014 combidata-0.2.2/combidata/processes/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2/combidata/processes/__init__.py
--rw-rw-rw-   0        0        0     3516 2023-07-30 10:12:58.000000 combidata-0.2.2/combidata/processes/combine.py
--rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.2/combidata/processes/form.py
--rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.2/combidata/processes/genetate.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.247015 combidata-0.2.2/combidata.egg-info/
--rw-rw-rw-   0        0        0    10603 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-30 14:50:50.000000 combidata-0.2.2/combidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      553 2023-07-30 14:49:48.000000 combidata-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 14:50:50.321017 combidata-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1073 2023-07-30 14:49:48.000000 combidata-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:50:50.318015 combidata-0.2.2/tests/
--rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.2/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:56:56.782153 combidata-0.2.2.1/
+-rw-rw-rw-   0        0        0     1083 2022-11-07 15:57:18.000000 combidata-0.2.2.1/LICENSE
+-rw-rw-rw-   0        0        0    10605 2023-07-31 12:56:56.782153 combidata-0.2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9822 2023-07-30 14:49:48.000000 combidata-0.2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 12:56:56.740159 combidata-0.2.2.1/combidata/
+-rw-rw-rw-   0        0        0      395 2023-02-10 13:56:29.000000 combidata-0.2.2.1/combidata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:56:56.774150 combidata-0.2.2.1/combidata/classes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2.1/combidata/classes/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-07-29 20:41:49.000000 combidata-0.2.2.1/combidata/classes/case.py
+-rw-rw-rw-   0        0        0     3107 2023-07-30 08:57:21.000000 combidata-0.2.2.1/combidata/classes/combination.py
+-rw-rw-rw-   0        0        0    12143 2023-07-31 12:40:31.000000 combidata-0.2.2.1/combidata/classes/data_generator.py
+-rw-rw-rw-   0        0        0      351 2023-03-02 16:58:22.000000 combidata-0.2.2.1/combidata/classes/process.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:56:56.779152 combidata-0.2.2.1/combidata/processes/
+-rw-rw-rw-   0        0        0        0 2023-02-03 08:57:32.000000 combidata-0.2.2.1/combidata/processes/__init__.py
+-rw-rw-rw-   0        0        0     3474 2023-07-31 12:32:53.000000 combidata-0.2.2.1/combidata/processes/combine.py
+-rw-rw-rw-   0        0        0      655 2023-02-16 18:09:16.000000 combidata-0.2.2.1/combidata/processes/form.py
+-rw-rw-rw-   0        0        0     1924 2023-04-01 06:30:40.000000 combidata-0.2.2.1/combidata/processes/genetate.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:56:56.767159 combidata-0.2.2.1/combidata.egg-info/
+-rw-rw-rw-   0        0        0    10605 2023-07-31 12:56:56.000000 combidata-0.2.2.1/combidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-31 12:56:56.000000 combidata-0.2.2.1/combidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:56:56.000000 combidata-0.2.2.1/combidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 12:56:56.000000 combidata-0.2.2.1/combidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2023-07-31 12:56:30.000000 combidata-0.2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:56:56.782153 combidata-0.2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-31 12:56:30.000000 combidata-0.2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:56:56.780152 combidata-0.2.2.1/tests/
+-rw-rw-rw-   0        0        0     3511 2023-06-30 13:59:13.000000 combidata-0.2.2.1/tests/test_generator.py
```

### Comparing `combidata-0.2.2/LICENSE` & `combidata-0.2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2/PKG-INFO` & `combidata-0.2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.2/README.md` & `combidata-0.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2/combidata/classes/case.py` & `combidata-0.2.2.1/combidata/classes/case.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2/combidata/classes/combination.py` & `combidata-0.2.2.1/combidata/classes/combination.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2/combidata/classes/data_generator.py` & `combidata-0.2.2.1/combidata/classes/data_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import random
 import traceback
+from pprint import pprint
 
 from combidata.classes.case import Case
 from combidata.classes.combination import Combination, step_not_done
 
 
 def crop_types(current_dict, poss_types):
     for unit, modes in current_dict.items():
@@ -133,22 +134,28 @@
         self.workflow = self.get_workflow(library["workflow"], type_of_cases)
 
         type_of_cases = type_of_cases if type_of_cases else "standard"
         if types_for_generation is None:
             types_for_generation = ["standard"]
         if not isinstance(types_for_generation, list):
             types_for_generation = [types_for_generation]
-        neutral_lib = self.form_neutral_lib(self.init_lib, types_for_generation)
+        neutral_lib = self.form_neutral_lib(self.init_lib)
+        self.spread_requirements(neutral_lib)
+        crop_types(neutral_lib, types_for_generation)
 
         self.combinations = self.find_combinations(neutral_lib, type_of_cases)
 
-        assert self.combinations, "No combinations for tests"
+        assert self.combinations, "No combinations for tests" #TODO deep logging needed
 
         if amount is not None:
             self.combinations = extend_dict(self.combinations, amount)
+    def spread_requirements(self, neutral_lib):
+        for field, modes in neutral_lib.items():
+            for mode, case in modes.items():
+                self.init_lib[field][mode].requirements = case.requirements
 
     def find_combinations(self, neutral_lib, type_of_cases):
         all_combinations = {}
         for field_name, cases in self.init_lib.items():
             for field_mode, case in cases.items():
                 if case.type_of_case == type_of_cases and can_combine(neutral_lib, case):
                     current_combination = Combination(case, self.workflow, neutral_lib,
@@ -230,15 +237,15 @@
     def dell_fields(self, possible_fields, banned_fields):
         if possible_fields is not None or banned_fields is not None:
             banned_fields = banned_fields if possible_fields is None else [field for field in self.init_lib.keys() if
                                                                            field not in possible_fields]
             for field in banned_fields:
                 del self.init_lib[field]
 
-    def form_neutral_lib(self, init_lib, neutral_types):
+    def form_neutral_lib(self, init_lib):
         neutral_lib = form_template(init_lib)
 
         for field, modes in init_lib.items():
             for mode in modes:
                 if init_lib[field][mode].requirements:
                     for req_unit, req_modes in init_lib[field][mode].requirements.items():
                         if req_unit in neutral_lib.keys() and mode in neutral_lib[field].keys():
@@ -256,10 +263,10 @@
                                     neutral_lib[req_unit][target_mode].requirements[field] - set(mode)
                                 if not neutral_lib[req_unit][target_mode].requirements[field]:
                                     del neutral_lib[req_unit][target_mode]
                                     if self.logger:
                                         self.logger.add_log(self.generator_id,
                                                             f"Mode: {target_mode} in field: {req_unit}: Was deleted because will never use in generation")
 
-        crop_types(neutral_lib, neutral_types)
+
 
         return neutral_lib
```

### Comparing `combidata-0.2.2/combidata/processes/combine.py` & `combidata-0.2.2.1/combidata/processes/combine.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
             template[field][mode] = copy.deepcopy(
                 lib[field][mode])  # TODO fix_it copy.deepcopy(lib[field][mode]) is tooo dum
             for seed_field, seed_modes in lib.items():
                 if seed_field != field:
                     template[field][mode].requirements[seed_field] = set(seed_modes)
     return template
 
+
 def form_poss(init_lib, neutral_types=None):
     neutral_lib = form_template(init_lib)
 
     for field, modes in init_lib.items():
         for mode in modes:
             if init_lib[field][mode].requirements:
                 for req_unit, req_modes in init_lib[field][mode].requirements.items():
@@ -43,40 +44,42 @@
 
     if neutral_types is not None:
         crop_types(neutral_lib, neutral_types)
 
     return neutral_lib
 
 
-def process_mode(seed, poss_di, chosen_unit, chosen_mode):
-    for pos_unit, pos_modes in poss_di[chosen_unit][chosen_mode].requirements.items():
+def process_mode(seed, poss_di, chosen_case):
+    for pos_unit, pos_modes in chosen_case.requirements.items():
         if poss_di.get(pos_unit):
             modes_for_del = set(poss_di[pos_unit].keys()) - set(pos_modes)
             for mode_for_del in modes_for_del:
                 del poss_di[pos_unit][mode_for_del]
-    seed[chosen_unit] = chosen_mode
-    del poss_di[chosen_unit]
+    seed[chosen_case.field_name] = chosen_case.field_mode
+    del poss_di[chosen_case.field_name]
     return form_poss(poss_di)
 
-def generate_seed(di, main_unit, main_mode):
+
+def generate_seed(di, main_case):
     poss_di = copy.deepcopy(di)
     seed = {}
 
-    poss_di = process_mode(seed, poss_di, main_unit, main_mode)
+    poss_di = process_mode(seed, poss_di, main_case)
 
     while poss_di:
         chosen_unit = random.choice(list(poss_di.keys()))
         chosen_mode = random.choice(list(poss_di[chosen_unit].keys()))
-        poss_di = process_mode(seed, poss_di, chosen_unit, chosen_mode)
+        poss_di = process_mode(seed, poss_di, poss_di[chosen_unit][chosen_mode])
 
     return seed
 
+
 def combine(combination):
     neutral_lib = combination.init_lib
     main_case = combination.main_case
 
-    combination.test_seed = generate_seed(neutral_lib, main_case.field_name, main_case.field_mode)
+    combination.test_seed = generate_seed(neutral_lib, main_case)
 
     combination.other_cases = {field: combination.init_lib[field][mode] for field, mode in combination.test_seed.items()
                                if field != combination.main_case.field_name}
 
     return True
```

### Comparing `combidata-0.2.2/combidata/processes/form.py` & `combidata-0.2.2.1/combidata/processes/form.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2/combidata/processes/genetate.py` & `combidata-0.2.2.1/combidata/processes/genetate.py`

 * *Files identical despite different names*

### Comparing `combidata-0.2.2/combidata.egg-info/PKG-INFO` & `combidata-0.2.2.1/combidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combidata
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Package for random data generation, combination and data prepare for tests
 Home-page: https://github.com/Warrfie/combidata
 Author: Kuklikov Maxim (Warrfie)
 Author-email: "MaximKuklikov(Warrfie)" <warrfie@gmail.com>
 Project-URL: Homepage, https://github.com/Warrfie/combidata
 Keywords: QA,SET,random data generation,testing API,testing,autotesting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `combidata-0.2.2/pyproject.toml` & `combidata-0.2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     "testing API",
     "testing",
     "autotesting"
 ]
 urls = {Homepage = "https://github.com/Warrfie/combidata"}
 authors = [{name = "MaximKuklikov(Warrfie)", email = "warrfie@gmail.com"}]
 requires-python = ">=3.10"
-version="0.2.2"
+version="0.2.2.1"
```

### Comparing `combidata-0.2.2/setup.py` & `combidata-0.2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="combidata",
-    version="0.2.2",
+    version="0.2.2.1",
     description="Package for random data generation and combination different cases",
     long_description=long_description,
     url="https://github.com/Warrfie/combidata",
     author="Kuklikov Maxim (Warrfie)",
     author_email="warrfie@gmail.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `combidata-0.2.2/tests/test_generator.py` & `combidata-0.2.2.1/tests/test_generator.py`

 * *Files identical despite different names*

