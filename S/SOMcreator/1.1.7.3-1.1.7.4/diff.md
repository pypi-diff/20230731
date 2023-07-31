# Comparing `tmp/SOMcreator-1.1.7.3.tar.gz` & `tmp/SOMcreator-1.1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.1.7.3.tar", last modified: Wed Jul 26 11:28:05 2023, max compression
+gzip compressed data, was "SOMcreator-1.1.7.4.tar", last modified: Mon Jul 31 11:01:39 2023, max compression
```

## Comparing `SOMcreator-1.1.7.3.tar` & `SOMcreator-1.1.7.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.253295 SOMcreator-1.1.7.3/
--rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.7.3/LICENSE
--rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1556 2023-07-26 11:28:05.253295 SOMcreator-1.1.7.3/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.7.3/README.md
--rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 11:28:05.253295 SOMcreator-1.1.7.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.030560 SOMcreator-1.1.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.061327 SOMcreator-1.1.7.3/src/SOMcreator/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.128820 SOMcreator-1.1.7.3/src/SOMcreator/Template/
--rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.143583 SOMcreator-1.1.7.3/src/SOMcreator/Template/__pyinstaller/
--rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/bookmark_template.txt
--rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/ifc.json
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.180724 SOMcreator-1.1.7.3/src/SOMcreator/Template/js_templates/
--rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/js_templates/end_ungetestet.js
--rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/mapping_template.txt
--rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/Template/template.txt
--rw-rw-rw-   0        0        0      156 2023-07-26 11:27:35.000000 SOMcreator-1.1.7.3/src/SOMcreator/__init__.py
--rw-rw-rw-   0        0        0    24822 2023-07-26 11:27:19.000000 SOMcreator-1.1.7.3/src/SOMcreator/classes.py
--rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.3/src/SOMcreator/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.252162 SOMcreator-1.1.7.3/src/SOMcreator/external_software/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/external_software/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/external_software/allplan.py
--rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/external_software/card1.py
--rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.3/src/SOMcreator/external_software/desite.py
--rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.7.3/src/SOMcreator/external_software/excel.py
--rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.3/src/SOMcreator/external_software/revit.py
--rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/external_software/vestra.py
--rw-rw-rw-   0        0        0     9363 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.3/src/SOMcreator/filehandling.py
--rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.3/src/SOMcreator/quality_check.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:05.086104 SOMcreator-1.1.7.3/src/SOMcreator.egg-info/
--rw-rw-rw-   0        0        0     1556 2023-07-26 11:28:05.000000 SOMcreator-1.1.7.3/src/SOMcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-07-26 11:28:05.000000 SOMcreator-1.1.7.3/src/SOMcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:28:05.000000 SOMcreator-1.1.7.3/src/SOMcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-07-26 11:28:05.000000 SOMcreator-1.1.7.3/src/SOMcreator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-07-26 11:28:05.000000 SOMcreator-1.1.7.3/src/SOMcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 11:28:05.000000 SOMcreator-1.1.7.3/src/SOMcreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.561345 SOMcreator-1.1.7.4/
+-rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.7.4/LICENSE
+-rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1556 2023-07-31 11:01:39.561345 SOMcreator-1.1.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.7.4/README.md
+-rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.7.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:01:39.562292 SOMcreator-1.1.7.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.325697 SOMcreator-1.1.7.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.355883 SOMcreator-1.1.7.4/src/SOMcreator/
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.446789 SOMcreator-1.1.7.4/src/SOMcreator/Template/
+-rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.457950 SOMcreator-1.1.7.4/src/SOMcreator/Template/__pyinstaller/
+-rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/bookmark_template.txt
+-rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/ifc.json
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.511437 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/
+-rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/end_ungetestet.js
+-rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/mapping_template.txt
+-rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/Template/template.txt
+-rw-rw-rw-   0        0        0      156 2023-07-31 10:59:21.000000 SOMcreator-1.1.7.4/src/SOMcreator/__init__.py
+-rw-rw-rw-   0        0        0    24958 2023-07-26 15:19:58.000000 SOMcreator-1.1.7.4/src/SOMcreator/classes.py
+-rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.4/src/SOMcreator/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.560329 SOMcreator-1.1.7.4/src/SOMcreator/external_software/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/__init__.py
+-rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/allplan.py
+-rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/card1.py
+-rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/desite.py
+-rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/excel.py
+-rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/revit.py
+-rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/external_software/vestra.py
+-rw-rw-rw-   0        0        0     9379 2023-07-31 10:58:59.000000 SOMcreator-1.1.7.4/src/SOMcreator/filehandling.py
+-rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.4/src/SOMcreator/quality_check.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:01:39.398561 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/
+-rw-rw-rw-   0        0        0     1556 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 11:01:39.000000 SOMcreator-1.1.7.4/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.1.7.3/LICENSE` & `SOMcreator-1.1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/PKG-INFO` & `SOMcreator-1.1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7.3
+Version: 1.1.7.4
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7.3/pyproject.toml` & `SOMcreator-1.1.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.1.7.4/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/Template/js_templates/end_ungetestet.js` & `SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/end_ungetestet.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.1.7.4/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.1.7.4/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/Template/template.txt` & `SOMcreator-1.1.7.4/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/classes.py` & `SOMcreator-1.1.7.4/src/SOMcreator/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -624,17 +624,16 @@
     @property
     def aggregation_representations(self) -> set[Aggregation]:  # Todo: add nodes functionality to graphs_window
         return self._aggregations
 
     def add_aggregation_representation(self, node: Aggregation) -> None:
         self._aggregations.add(node)
 
-    def remove_node(self, node: Aggregation) -> None:
+    def remove_aggregation_representation(self, node: Aggregation) -> None:
         self.aggregation_representations.remove(node)
-        node.delete()
 
     @property
     def inherited_property_sets(self) -> dict[Object, list[PropertySet]]:
         def recursion(recursion_property_sets, recursion_obj: Object):
             psets = recursion_obj.property_sets
 
             if psets:
@@ -748,14 +747,18 @@
             self.uuid = str(uuid)
         self.object = obj
         self._parent: Aggregation | None = None
         self.connection_dict: dict[Aggregation, int] = dict()
 
         self.object.add_aggregation_representation(self)
 
+    def delete(self) -> None:
+        super(Aggregation, self).delete()
+        self.object.remove_aggregation_representation(self)
+
     @property
     def parent_connection(self) -> int:
         """
         NO PARENT = 0
         AGGREGATION = 1
         INHERITANCE = 2
         AGGREGATION+INHERITANCE =3
```

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/constants.py` & `SOMcreator-1.1.7.4/src/SOMcreator/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.1.7.4/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.1.7.4/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/external_software/desite.py` & `SOMcreator-1.1.7.4/src/SOMcreator/external_software/desite.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.1.7.4/src/SOMcreator/external_software/excel.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.1.7.4/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.1.7.4/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/filehandling.py` & `SOMcreator-1.1.7.4/src/SOMcreator/filehandling.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         aggregation = classes.Aggregation(obj, identifier, description, optional)
         aggregation_parent_dict[aggregation] = (parent, parent_connection)
 
     def build_aggregation_structure():
         for aggregation, (uuid, connection_type) in aggregation_parent_dict.items():
             parent = project.get_element_by_uuid(uuid)
             if parent is not None:
-                parent.add_child(aggregation)
+                parent.add_child(aggregation,connection_type)
 
     predefined_psets_dict = load_dict(constants.PREDEFINED_PSETS)
 
     for ident, pset_dict in predefined_psets_dict.items():
         load_pset(pset_dict, ident, None)
 
     objects_dict = load_dict(constants.OBJECTS)
```

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator/quality_check.py` & `SOMcreator-1.1.7.4/src/SOMcreator/quality_check.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.1.7.4/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7.3
+Version: 1.1.7.4
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7.3/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.1.7.4/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

