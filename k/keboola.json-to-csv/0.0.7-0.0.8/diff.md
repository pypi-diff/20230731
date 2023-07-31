# Comparing `tmp/keboola.json-to-csv-0.0.7.tar.gz` & `tmp/keboola.json-to-csv-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keboola.json-to-csv-0.0.7.tar", last modified: Mon Jul 31 12:35:06 2023, max compression
+gzip compressed data, was "keboola.json-to-csv-0.0.8.tar", last modified: Mon Jul 31 12:38:57 2023, max compression
```

## Comparing `keboola.json-to-csv-0.0.7.tar` & `keboola.json-to-csv-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:35:06.077268 keboola.json-to-csv-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 12:35:06.077268 keboola.json-to-csv-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:35:06.077268 keboola.json-to-csv-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:35:06.073267 keboola.json-to-csv-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:35:06.073267 keboola.json-to-csv-0.0.7/src/keboola/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:35:06.077268 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/csv_row.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:35:06.073267 keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 12:35:06.000000 keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 12:35:06.000000 keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:35:06.000000 keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:35:06.000000 keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 12:35:06.000000 keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:35:06.077268 keboola.json-to-csv-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 12:34:55.000000 keboola.json-to-csv-0.0.7/tests/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:38:57.569854 keboola.json-to-csv-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 12:38:57.569854 keboola.json-to-csv-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:38:57.573854 keboola.json-to-csv-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:38:57.569854 keboola.json-to-csv-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:38:57.569854 keboola.json-to-csv-0.0.8/src/keboola/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:38:57.569854 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/csv_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:38:57.569854 keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 12:38:57.000000 keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 12:38:57.000000 keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:38:57.000000 keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:38:57.000000 keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 12:38:57.000000 keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:38:57.569854 keboola.json-to-csv-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 12:38:46.000000 keboola.json-to-csv-0.0.8/tests/test_functional.py
```

### Comparing `keboola.json-to-csv-0.0.7/LICENSE` & `keboola.json-to-csv-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/PKG-INFO` & `keboola.json-to-csv-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keboola.json-to-csv
-Version: 0.0.7
+Version: 0.0.8
 Summary: General utility library for Python applications running in Keboola Connection environment
 Home-page: https://github.com/keboola/python-utils
 Author: Keboola KDS Team
 Author-email: support@keboola.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `keboola.json-to-csv-0.0.7/README.md` & `keboola.json-to-csv-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/setup.py` & `keboola.json-to-csv-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="keboola.json-to-csv",
-    version="0.0.7",
+    version="0.0.8",
     author="Keboola KDS Team",
     setup_requires=['flake8'],
     tests_require=[],
     install_requires=[],
     author_email="support@keboola.com",
     description="General utility library for Python applications running in Keboola Connection environment",
     long_description=long_description,
```

### Comparing `keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/analyzer.py` & `keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/analyzer.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/csv_row.py` & `keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/csv_row.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/mapping.py` & `keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/mapping.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/node.py` & `keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/node.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/parser.py` & `keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,11 +315,11 @@
 
     def _get_primary_key_values(self, data_row: Dict[str, Any], node_path: List[Union[Any, str]]) -> Dict[str, str]:
         current_table_primary_keys = {}
         children_nodes = self.analyzer.get_node_dict(path_to_object=node_path).get("children")
         for child_node in children_nodes:
             if children_nodes.get(child_node).get("node").is_primary_key:
                 # TODO FIX WHEN ID IS NESTED e.g. some_dict.id
-                name = ".".join([self.main_table_name] + node_path + [child_node])
+                name = "_".join([self.main_table_name] + node_path + [child_node])
                 current_table_primary_keys[name] = data_row.get(child_node)
 
         return current_table_primary_keys
```

### Comparing `keboola.json-to-csv-0.0.7/src/keboola/json_to_csv/table.py` & `keboola.json-to-csv-0.0.8/src/keboola/json_to_csv/table.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/PKG-INFO` & `keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keboola.json-to-csv
-Version: 0.0.7
+Version: 0.0.8
 Summary: General utility library for Python applications running in Keboola Connection environment
 Home-page: https://github.com/keboola/python-utils
 Author: Keboola KDS Team
 Author-email: support@keboola.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `keboola.json-to-csv-0.0.7/src/keboola.json_to_csv.egg-info/SOURCES.txt` & `keboola.json-to-csv-0.0.8/src/keboola.json_to_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.7/tests/test_functional.py` & `keboola.json-to-csv-0.0.8/tests/test_functional.py`

 * *Files identical despite different names*

