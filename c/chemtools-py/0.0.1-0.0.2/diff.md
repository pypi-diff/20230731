# Comparing `tmp/chemtools-py-0.0.1.tar.gz` & `tmp/chemtools-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemtools-py-0.0.1.tar", last modified: Fri Jul 28 06:39:59 2023, max compression
+gzip compressed data, was "chemtools-py-0.0.2.tar", last modified: Mon Jul 31 15:51:00 2023, max compression
```

## Comparing `chemtools-py-0.0.1.tar` & `chemtools-py-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 06:39:59.942756 chemtools-py-0.0.1/
--rw-rw-rw-   0        0        0      317 2023-07-28 06:39:59.942756 chemtools-py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-07-24 15:38:57.000000 chemtools-py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 06:39:59.931752 chemtools-py-0.0.1/chemtools-py/
--rw-rw-rw-   0        0        0      117 2023-07-28 05:34:11.000000 chemtools-py-0.0.1/chemtools-py/__init__.py
--rw-rw-rw-   0        0        0     3299 2023-07-24 12:01:49.000000 chemtools-py-0.0.1/chemtools-py/funclib.py
-drwxrwxrwx   0        0        0        0 2023-07-28 06:39:59.940754 chemtools-py-0.0.1/chemtools_py.egg-info/
--rw-rw-rw-   0        0        0      317 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-28 06:39:59.000000 chemtools-py-0.0.1/chemtools_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 06:39:59.942756 chemtools-py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      481 2023-07-28 06:39:52.000000 chemtools-py-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:51:00.835300 chemtools-py-0.0.2/
+-rw-rw-rw-   0        0        0      317 2023-07-31 15:51:00.836302 chemtools-py-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-07-29 12:54:10.000000 chemtools-py-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 15:51:00.808308 chemtools-py-0.0.2/chemtools-py/
+-rw-rw-rw-   0        0        0      139 2023-07-31 15:43:36.000000 chemtools-py-0.0.2/chemtools-py/__init__.py
+-rw-rw-rw-   0        0        0     2660 2023-07-31 15:40:13.000000 chemtools-py-0.0.2/chemtools-py/balance_equasion.py
+-rw-rw-rw-   0        0        0     4231 2023-07-31 15:42:51.000000 chemtools-py-0.0.2/chemtools-py/general_purpose_funtions.py
+-rw-rw-rw-   0        0        0      201 2023-07-31 15:40:36.000000 chemtools-py-0.0.2/chemtools-py/test.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:51:00.834313 chemtools-py-0.0.2/chemtools_py.egg-info/
+-rw-rw-rw-   0        0        0      317 2023-07-31 15:51:00.000000 chemtools-py-0.0.2/chemtools_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-31 15:51:00.000000 chemtools-py-0.0.2/chemtools_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 15:51:00.000000 chemtools-py-0.0.2/chemtools_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 15:51:00.000000 chemtools-py-0.0.2/chemtools_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 15:51:00.000000 chemtools-py-0.0.2/chemtools_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 15:51:00.837302 chemtools-py-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      488 2023-07-31 15:45:38.000000 chemtools-py-0.0.2/setup.py
```

### Comparing `chemtools-py-0.0.1/chemtools-py/funclib.py` & `chemtools-py-0.0.2/chemtools-py/general_purpose_funtions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,28 @@
 from requests import get as gt
 from os import listdir
 import json
 from functools import lru_cache
 
 @lru_cache(maxsize=32)
 def get_elements(lower_bound:int = 0,upper_bound: int = 100,raw: bool = False):
+
+    #check if bounds are correct and if not correct them
+    if upper_bound<lower_bound:
+        temp = upper_bound
+        upper_bound = lower_bound
+        lower_bound = temp
+    if upper_bound>118:
+        upper_bound=118
+    if lower_bound<0:
+        lower_bound=0
+        
+    
     #download json containig all info and if it`s already downloaded use it
+
     if not "chem_elements.json" in listdir():
         response = gt("https://raw.githubusercontent.com/Bowserinator/Periodic-Table-JSON/master/PeriodicTableJSON.json")
         #error while accessing
         if response.status_code != 200:
             raise("Error accessing remote json")
         data = response.json()
         #save for later offline uses
@@ -21,28 +34,27 @@
         data = open("chem_elements.json")
         data = json.load(data)
     #return first [lower_bound-upper_bound] ammount of elemnts, default is 100, can be lowered to inscrease speed
     if raw == False:
         return [element['symbol'] for element in data['elements'] if lower_bound <= element['number'] <= upper_bound]
     else:
         return data
-
-
-
+@lru_cache(maxsize=32)
 def molar_mass(formula: str) -> float:
     parsed_formula = parse_chemical_formula(formula)
     molar = 0.0
     data = get_elements(raw=True)
     element_to_mass = {element['symbol']: element['atomic_mass'] for element in data['elements']}
     for element, count in parsed_formula.items():
         molar += float(element_to_mass[element]) * count
     return molar
-
-def parse_chemical_formula(formula:str,error_finding: bool = True):
-    
+@lru_cache(maxsize=32)
+def parse_chemical_formula(formula:str,error_finding: bool = True) -> dict:
+    #delete all spaces cuz they don`t have meaning in them and can make function do wrong outputs
+    formula = formula.replace(" ","")
     # Step 1: Extract and remove the whole molecule coefficient
     coefficient = 1
     for i, char in enumerate(formula):
         if not char.isdigit():
             coefficient = int(formula[:i] or 1)
             formula = formula[i:]
             break
@@ -57,23 +69,43 @@
     for part in formula_parts:
         element, primary_number, _, sub_formula, _, multiplier = part
         if element:
             primary_number = int(primary_number) if primary_number else 1
             primary_number *= coefficient # multiply count by the molecule's coefficient
             result[element] = result.get(element, 0) + primary_number
         else:
-            # when the parentheses has a multiplier (like H2O2),
-            # the coefficient is multiplied by the multiplier
             sub_coefficient = coefficient * (int(multiplier) if multiplier else 1)
             # Process the sub-formula recursively
             sub_result = parse_chemical_formula(sub_formula)
             for sub_element, sub_value in sub_result.items():
                 sub_value *= sub_coefficient
                 result[sub_element] = result.get(sub_element, 0) + sub_value
 
     if error_finding:
         k = get_elements()
         for i, l in result.items():
             if not i in k:
                 raise ValueError(f"Error while parsing formula '{formula}': element '{i}' not found in element list")
             
-    return result
+    return result
+
+
+@lru_cache(maxsize=32)
+def check_equasion(eq:str) -> bool:
+    #taking in mind that eq should have this pattern "a + b => c + d" or "a=>b+c+d+e"
+    first,second = eq.split("=>")
+    def count_half(hf:str) -> dict:
+        res = {}
+        hf = hf.split("+")
+        for l in hf:
+            for k,v in parse_chemical_formula(l).items():
+                if k in res:
+                    res[k] += v
+                else:
+                    res[k] = v
+        return res
+    if count_half(first)==count_half(second):
+        return True
+    return False
+
+
+
```

