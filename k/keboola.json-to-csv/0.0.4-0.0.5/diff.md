# Comparing `tmp/keboola.json-to-csv-0.0.4.tar.gz` & `tmp/keboola.json-to-csv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keboola.json-to-csv-0.0.4.tar", last modified: Mon Jul 31 11:48:03 2023, max compression
+gzip compressed data, was "keboola.json-to-csv-0.0.5.tar", last modified: Mon Jul 31 12:25:02 2023, max compression
```

## Comparing `keboola.json-to-csv-0.0.4.tar` & `keboola.json-to-csv-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.413680 keboola.json-to-csv-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 11:48:03.413680 keboola.json-to-csv-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.405680 keboola.json-to-csv-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.405680 keboola.json-to-csv-0.0.4/src/keboola/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/csv_row.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/tests/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:25:02.177895 keboola.json-to-csv-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-31 12:25:02.177895 keboola.json-to-csv-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:25:02.177895 keboola.json-to-csv-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:25:02.173895 keboola.json-to-csv-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:25:02.173895 keboola.json-to-csv-0.0.5/src/keboola/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:25:02.177895 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22514 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/csv_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:25:02.173895 keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-31 12:25:02.000000 keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 12:25:02.000000 keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:25:02.000000 keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:25:02.000000 keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 12:25:02.000000 keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:25:02.177895 keboola.json-to-csv-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 12:24:42.000000 keboola.json-to-csv-0.0.5/tests/test_functional.py
```

### Comparing `keboola.json-to-csv-0.0.4/LICENSE` & `keboola.json-to-csv-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.4/PKG-INFO` & `keboola.json-to-csv-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keboola.json-to-csv
-Version: 0.0.4
+Version: 0.0.5
 Summary: General utility library for Python applications running in Keboola Connection environment
 Home-page: https://github.com/keboola/python-utils
 Author: Keboola KDS Team
 Author-email: support@keboola.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `keboola.json-to-csv-0.0.4/README.md` & `keboola.json-to-csv-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.4/setup.py` & `keboola.json-to-csv-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="keboola.json-to-csv",
-    version="0.0.4",
+    version="0.0.5",
     author="Keboola KDS Team",
     setup_requires=['flake8'],
     tests_require=[],
     install_requires=[],
     author_email="support@keboola.com",
     description="General utility library for Python applications running in Keboola Connection environment",
     long_description=long_description,
```

### Comparing `keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/analyzer.py` & `keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,15 @@
             child_columns, child_child_tables, child_primary_keys, child_force_types = self._analyze_child_node_mapping(
                 node_hierarchy, child)
             columns.update(child_columns)
             child_tables.update(child_child_tables)
             force_types.extend(child_force_types)
             primary_keys.extend(child_primary_keys)
         return {"table_name": table_name,
-                "columns": columns,
+                "column_mappings": columns,
                 "primary_keys": primary_keys,
                 "force_types": force_types,
                 "child_tables": child_tables}
 
     def _analyze_child_node_mapping(self, node_hierarchy, child_name):
         primary_keys = []
         force_types = []
@@ -430,24 +430,24 @@
 
     def get_column_mappings_at_path(self, node_path: List[str]) -> Dict[str, str]:
         headers = {}
         node_data = self.get_node_dict(node_path) or {}
         if "node" in node_data:
             node_type = node_data.get("node").data_type
             if node_type == NodeType.SCALAR:
-                headers[".".join(node_data.get("node").path)] = node_data.get("node").header_name
+                headers[".".join(node_data.get("node").path)] = node_data.get("node").header_name.replace(".", "_")
 
         for node_name, data in node_data.get("children").items():
             if data.get("node").data_type == NodeType.DICT:
                 ch = self.get_column_mappings_at_path(self.create_path_to_child_object(node_path, node_name))
                 headers.update(ch)
             elif data.get("node").data_type == NodeType.LIST:
                 continue
             else:
-                headers[".".join(data.get("node").path)] = data.get("node").header_name
+                headers[".".join(data.get("node").path)] = data.get("node").header_name.replace(".", "_")
 
         return headers
 
     @staticmethod
     def add_prefix_to_list_items(input_list, prefix):
         return [prefix + item for item in input_list]
```

### Comparing `keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/csv_row.py` & `keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/csv_row.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/mapping.py` & `keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/mapping.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/node.py` & `keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/node.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/parser.py` & `keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,11 +315,11 @@
 
     def _get_primary_key_values(self, data_row: Dict[str, Any], node_path: List[Union[Any, str]]) -> Dict[str, str]:
         current_table_primary_keys = {}
         children_nodes = self.analyzer.get_node_dict(path_to_object=node_path).get("children")
         for child_node in children_nodes:
             if children_nodes.get(child_node).get("node").is_primary_key:
                 # TODO FIX WHEN ID IS NESTED e.g. some_dict.id
-                name = "_".join([self.main_table_name] + node_path + [child_node])
+                name = ".".join([self.main_table_name] + node_path + [child_node])
                 current_table_primary_keys[name] = data_row.get(child_node)
 
         return current_table_primary_keys
```

### Comparing `keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/table.py` & `keboola.json-to-csv-0.0.5/src/keboola/json_to_csv/table.py`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/PKG-INFO` & `keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keboola.json-to-csv
-Version: 0.0.4
+Version: 0.0.5
 Summary: General utility library for Python applications running in Keboola Connection environment
 Home-page: https://github.com/keboola/python-utils
 Author: Keboola KDS Team
 Author-email: support@keboola.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/SOURCES.txt` & `keboola.json-to-csv-0.0.5/src/keboola.json_to_csv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.4/tests/test_functional.py` & `keboola.json-to-csv-0.0.5/tests/test_functional.py`

 * *Files identical despite different names*

