# Comparing `tmp/ckanext-envidat-validators-0.0.0.tar.gz` & `tmp/ckanext-envidat-validators-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-envidat-validators-0.0.0.tar", last modified: Mon Jul 31 13:33:49 2023, max compression
+gzip compressed data, was "ckanext-envidat-validators-0.0.1.tar", last modified: Mon Jul 31 13:42:38 2023, max compression
```

## Comparing `ckanext-envidat-validators-0.0.0.tar` & `ckanext-envidat-validators-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-31 13:16:57.641018 ckanext-envidat-validators-0.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1060 2023-07-31 13:16:44.311022 ckanext-envidat-validators-0.0.0/LICENSE
--rw-r--r--   0        0        0     1015 2023-07-31 13:26:01.920832 ckanext-envidat-validators-0.0.0/README.md
--rw-r--r--   0        0        0      230 2023-07-31 13:16:44.311022 ckanext-envidat-validators-0.0.0/ckanext/__init__.py
--rw-r--r--   0        0        0      237 2023-07-31 13:17:18.241012 ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/__init__.py
--rw-r--r--   0        0        0       43 2023-07-31 13:23:24.290886 ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/__version__.py
--rw-r--r--   0        0        0     3041 2023-07-31 13:30:11.590730 ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/logic.py
--rw-r--r--   0        0        0     1057 2023-07-31 13:29:29.420768 ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/plugin.py
--rw-r--r--   0        0        0       51 2023-07-31 13:17:18.241012 ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/tests/__init__.py
--rw-r--r--   0        0        0     1436 2023-07-31 13:17:31.721006 ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/tests/test_plugin.py
--rw-r--r--   0        0        0     2137 2023-07-31 13:23:43.440880 ckanext-envidat-validators-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 ckanext-envidat-validators-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1060 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/LICENSE
+-rw-r--r--   0        0        0     1015 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/README.md
+-rw-r--r--   0        0        0      230 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/ckanext/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/__version__.py
+-rw-r--r--   0        0        0     3205 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/logic.py
+-rw-r--r--   0        0        0     1118 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/plugin.py
+-rw-r--r--   0        0        0       51 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/tests/__init__.py
+-rw-r--r--   0        0        0     1436 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/tests/test_plugin.py
+-rw-r--r--   0        0        0     2137 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 ckanext-envidat-validators-0.0.1/PKG-INFO
```

### Comparing `ckanext-envidat-validators-0.0.0/LICENSE` & `ckanext-envidat-validators-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-envidat-validators-0.0.0/README.md` & `ckanext-envidat-validators-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/logic.py` & `ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from ckantoolkit import _
-import json
-from ckanext.scheming.validation import scheming_validator
+"""Validator logic for IValidators."""
 
+import json
 import logging
 
-logger = logging.getLogger(__name__)
-
 import ckan.lib.navl.dictization_functions as df
+from ckantoolkit import _
+
+from ckanext.scheming.validation import scheming_validator
 
+log = logging.getLogger(__name__)
 StopOnError = df.StopOnError
 
 
 def envidat_shortname_validator(key, data, errors, context):
+    """Prevent short package titles <80 char."""
     value = data.get(key)
     if not value or len(value) > 80:
         errors[key].append(_("text should be maximum 80 characters long"))
         raise StopOnError
 
 
 def envidat_string_uppercase(key, data, errors, context):
-    """
-    if the value is a string, make it uppercase, otherwise leave the value as it is.
+    """Make string values uppercase.
+
+    If the value is a string, make it uppercase, otherwise leave the value as it is.
     make all tags uppercase if possible.
     """
     # Plain value to uppercase
     tags = data[key]
     if isinstance(tags, str):
         data[key] = tags.upper()
 
@@ -34,34 +37,30 @@
     while tag:
         data[("tags", num, "name")] = _safe_upper(tag)
         num += 1
         tag = data.get(("tags", num, "name"), "")
 
 
 def envidat_minimum_tag_count(key, data, errors, context):
-    """
-    count tags and raise an error if there are less than 5
-    """
+    """Count tags and raise an error if there are less than 5."""
     min_tags = 5
     # tags to count
     num = 0
     tag = data.get(("tags", num, "name"), "")
     while tag:
         num += 1
         tag = data.get(("tags", num, "name"), "")
 
     if num < min_tags:
         errors[key].append(_("at least " + str(min_tags) + " tags"))
         raise StopOnError
 
 
 def envidat_minimum_description_length(key, data, errors, context):
-    """
-    count description chars and raise an error if there are less than 100
-    """
+    """Count description chars and raise an error if there are less than 100."""
     min_length = 100
     # tags to count
     description = data.get(key, "")
     description_length = len(description)
 
     if description_length < min_length:
         errors[key].append(
@@ -72,47 +71,46 @@
             )
         )
         raise StopOnError
 
 
 @scheming_validator
 def envidat_reorder(field, schema):
-    def validator(key, data, errors, context):
-        """
-        reorder sub elements
-        """
+    """Reorder sub elements."""
 
+    def validator(key, data, errors, context):
+        """Logic for envidat_reorder."""
         try:
             field_data = json.loads(data[key])
             sorted_list = sorted(
                 field_data, key=lambda k: int(k.get("order", len(field_data)))
             )
             for element in sorted_list:
                 element.pop("order", 0)
             data[key] = json.dumps(sorted_list)
 
         except ValueError as e:
-            logger.error(
+            log.error(
                 "Could not reorder field {0}, exception raised {1}".format(key, e)
             )
             return
 
     return validator
 
 
 @scheming_validator
 def envidat_copy_type_general(field, schema):
+    """Copy type general."""
+
     def validator(key, data, errors, context):
-        """
-        copy type general
-        """
+        """Logic for envidat_copy_type_general."""
         data[key] = data.get(("resource_type_general",), data[key])
 
     return validator
 
 
-# upper or same value if it is not a string
 def _safe_upper(value):
+    """Upper or same value if it is not a string."""
     try:
         return value.upper()
-    except:
+    except Exception:
         return value
```

### Comparing `ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/plugin.py` & `ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Init plugin with CKAN interfaces."""
 
 import logging
 
 from ckan.plugins import SingletonPlugin, implements, interfaces
 
 from ckanext.envidat_validators.logic import (
-    envidat_string_uppercase,
-    envidat_shortname_validator,
-    envidat_minimum_tag_count,
-    envidat_reorder,
     envidat_copy_type_general,
     envidat_minimum_description_length,
+    envidat_minimum_tag_count,
+    envidat_reorder,
+    envidat_shortname_validator,
+    envidat_string_uppercase,
 )
 
 log = logging.getLogger(__name__)
 
 
 class EnviDatValidatorsPlugin(SingletonPlugin):
     """EnviDatValidatorsPlugin.
@@ -22,14 +22,15 @@
     Plugin to add additional validation to CKAN.
     """
 
     implements(interfaces.IValidators)
 
     # IValidators
     def get_validators(self):
+        """Assemble validators for IValidators interface."""
         return {
             "envidat_string_uppercase": envidat_string_uppercase,
             "envidat_shortname_validator": envidat_shortname_validator,
             "envidat_minimum_tag_count": envidat_minimum_tag_count,
             "envidat_reorder": envidat_reorder,
             "envidat_copy_type_general": envidat_copy_type_general,
             "envidat_minimum_description_length": envidat_minimum_description_length,
```

### Comparing `ckanext-envidat-validators-0.0.0/ckanext/envidat_validators/tests/test_plugin.py` & `ckanext-envidat-validators-0.0.1/ckanext/envidat_validators/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-envidat-validators-0.0.0/pyproject.toml` & `ckanext-envidat-validators-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-version = "0.0.0"
+version = "0.0.1"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."ckan.plugins"]
 envidat_validators = "ckanext.envidat_validators.plugin:EnviDatValidatorsPlugin"
 
@@ -58,15 +58,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest-ckan>=0.0.12",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.0"
+version = "0.0.1"
 version_files = [
     "pyproject.toml:version",
     "ckanext/envidat_validators/__version__.py",
 ]
 
 [tool.isort]
 profile = "black"
```

### Comparing `ckanext-envidat-validators-0.0.0/PKG-INFO` & `ckanext-envidat-validators-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-envidat_validators
-Version: 0.0.0
+Version: 0.0.1
 Summary: Custom CKAN validators for EnviDat.
 License: MIT
 Keywords: CKAN,validators,schema
 Author-email: Sam Woodcock <sam.woodcock@protonmail.com>
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ckanext-envidat_validators Version: 0.0.0 Summary:
+Metadata-Version: 2.1 Name: ckanext-envidat_validators Version: 0.0.1 Summary:
 Custom CKAN validators for EnviDat. License: MIT Keywords:
 CKAN,validators,schema Author-email: Sam Woodcock
 woodcock@protonmail.com> Requires-Python: >=3.8 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities Project-URL: documentation, https://
```

