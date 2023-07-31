# Comparing `tmp/valcheck-1.4.tar.gz` & `tmp/valcheck-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valcheck-1.4.tar", last modified: Sun Jul 30 12:25:55 2023, max compression
+gzip compressed data, was "valcheck-1.5.tar", last modified: Mon Jul 31 17:03:14 2023, max compression
```

## Comparing `valcheck-1.4.tar` & `valcheck-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 12:25:55.150120 valcheck-1.4/
--rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-1.4/LICENSE
--rw-rw-rw-   0        0        0      758 2023-07-30 12:25:55.150120 valcheck-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-07-30 12:25:32.000000 valcheck-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-30 12:25:55.150120 valcheck-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1566 2023-07-30 12:25:32.000000 valcheck-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 12:25:55.118125 valcheck-1.4/valcheck/
--rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-1.4/valcheck/__init__.py
--rw-rw-rw-   0        0        0     1736 2023-07-21 18:09:50.000000 valcheck-1.4/valcheck/exceptions.py
--rw-rw-rw-   0        0        0    22468 2023-07-28 17:59:50.000000 valcheck-1.4/valcheck/fields.py
--rw-rw-rw-   0        0        0     2780 2023-07-21 03:21:34.000000 valcheck-1.4/valcheck/models.py
--rw-rw-rw-   0        0        0     3156 2023-07-16 07:09:18.000000 valcheck-1.4/valcheck/utils.py
--rw-rw-rw-   0        0        0     9247 2023-07-30 12:25:32.000000 valcheck-1.4/valcheck/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-30 12:25:55.146119 valcheck-1.4/valcheck.egg-info/
--rw-rw-rw-   0        0        0      758 2023-07-30 12:25:54.000000 valcheck-1.4/valcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-30 12:25:54.000000 valcheck-1.4/valcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 12:25:54.000000 valcheck-1.4/valcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 12:25:54.000000 valcheck-1.4/valcheck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 17:03:14.310953 valcheck-1.5/
+-rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-1.5/LICENSE
+-rw-rw-rw-   0        0        0      758 2023-07-31 17:03:14.306951 valcheck-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-07-31 16:45:40.000000 valcheck-1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 17:03:14.310953 valcheck-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2023-07-31 16:45:40.000000 valcheck-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:03:14.287037 valcheck-1.5/valcheck/
+-rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-1.5/valcheck/__init__.py
+-rw-rw-rw-   0        0        0     1736 2023-07-21 18:09:50.000000 valcheck-1.5/valcheck/exceptions.py
+-rw-rw-rw-   0        0        0    22468 2023-07-28 17:59:50.000000 valcheck-1.5/valcheck/fields.py
+-rw-rw-rw-   0        0        0     2780 2023-07-21 03:21:34.000000 valcheck-1.5/valcheck/models.py
+-rw-rw-rw-   0        0        0     3551 2023-07-31 16:57:02.000000 valcheck-1.5/valcheck/utils.py
+-rw-rw-rw-   0        0        0     9663 2023-07-31 17:00:09.000000 valcheck-1.5/valcheck/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:03:14.306951 valcheck-1.5/valcheck.egg-info/
+-rw-rw-rw-   0        0        0      758 2023-07-31 17:03:14.000000 valcheck-1.5/valcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-31 17:03:14.000000 valcheck-1.5/valcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:03:14.000000 valcheck-1.5/valcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 17:03:14.000000 valcheck-1.5/valcheck.egg-info/top_level.txt
```

### Comparing `valcheck-1.4/LICENSE` & `valcheck-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `valcheck-1.4/PKG-INFO` & `valcheck-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 1.4
+Version: 1.5
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `valcheck-1.4/README.md` & `valcheck-1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```
 
 ## Usage
 - Refer to the `examples/` folder, based on the **valcheck** version you are using
 
 ## Performance benchmarks
 - On comparison of the performance of Django Rest Framework's (version 3.14.0) serializer with Valcheck's
-validator, we found that Valcheck (version 1.4) is ~3.8 times faster for cases where the data is
+validator, we found that Valcheck (version 1.5) is ~3.8 times faster for cases where the data is
 valid, and ~2.7 times faster for cases where the data is invalid.
 - These numbers are averaged over 25,000 iterations.
 
 ```python
 from rest_framework import serializers
 from valcheck import fields, models, validator
```

### Comparing `valcheck-1.4/setup.py` & `valcheck-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import find_packages, setup
 
 # Constants
 PACKAGE_NAME = "valcheck"
-PACKAGE_VERSION = "1.4"
+PACKAGE_VERSION = "1.5"
 AUTHOR_NAME = "Nishant Rao"
 AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
 FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
 REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
 
 # Requirements
```

### Comparing `valcheck-1.4/valcheck/exceptions.py` & `valcheck-1.5/valcheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `valcheck-1.4/valcheck/fields.py` & `valcheck-1.5/valcheck/fields.py`

 * *Files identical despite different names*

### Comparing `valcheck-1.4/valcheck/models.py` & `valcheck-1.5/valcheck/models.py`

 * *Files identical despite different names*

### Comparing `valcheck-1.4/valcheck/utils.py` & `valcheck-1.5/valcheck/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,23 @@
     if not isinstance(obj, list):
         return False
     if not allow_empty and not obj:
         return False
     return all((isinstance(item, type_) for item in obj))
 
 
+def is_list_of_subclasses_of_type(obj: Any, /, *, type_: Type, allow_empty: Optional[bool] = True) -> bool:
+    """Returns True if `obj` is a list of sub-classes of type `type_`"""
+    if not isinstance(obj, list):
+        return False
+    if not allow_empty and not obj:
+        return False
+    return all((bool(isinstance(item, type) and issubclass(item, type_)) for item in obj))
+
+
 def is_valid_object_of_type(obj: Any, /, *, type_: Type, allow_empty: Optional[bool] = True) -> bool:
     if not isinstance(obj, type_):
         return False
     return True if allow_empty else bool(obj)
 
 
 def is_valid_uuid_string(string: str, /) -> bool:
```

### Comparing `valcheck-1.4/valcheck/validator.py` & `valcheck-1.5/valcheck/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -164,19 +164,28 @@
                 value=validated_field.field.field_value,
             )
 
     def _perform_model_validation_checks(self) -> None:
         """Performs model validation checks, and registers errors (if any)"""
         errors: List[Error] = []
         model_validator_classes_to_ignore = self.model_validators_to_ignore()
+        assert utils.is_list_of_subclasses_of_type(
+            model_validator_classes_to_ignore,
+            type_=Validator,
+            allow_empty=True,
+        ), (
+            "The output of the `model_validators_to_ignore()` method must be a list of types, each"
+            " being a sub-class `valcheck.validator.Validator`."
+            " Must be an empty list if there are no classes to ignore."
+        )
         for class_ in self.__class__.__mro__:
             if issubclass(class_, Validator) and class_ not in model_validator_classes_to_ignore:
                 errors += class_.model_validator(self)
         assert utils.is_list_of_instances_of_type(errors, type_=Error, allow_empty=True), (
-            "The output of the model validator method must be a list of errors (each of type `valcheck.models.Error`)."
+            "The output of the `model_validator()` method must be a list of errors (each of type `valcheck.models.Error`)."
             " Must be an empty list if there are no errors."
         )
         INVALID_MODEL_ERROR_MESSAGE = "Invalid model - Validation failed"
         for error in errors:
             error.validator_message = INVALID_MODEL_ERROR_MESSAGE
         self._register_errors(errors=errors)
 
@@ -186,15 +195,15 @@
         method call must be ignored.
         """
         return []
 
     def model_validator(self) -> List[Error]:
         """
         Used to validate the entire model, after all individual fields are validated.
-        The output of the model validator method must be a list of errors (each of type `valcheck.models.Error`).
+        The output of this method must be a list of errors (each of type `valcheck.models.Error`).
         Must be an empty list if there are no errors.
         """
         return []
 
     def run_validations(self, *, raise_exception: Optional[bool] = False) -> List[Error]:
         """
         Runs validations and registers errors/validated-data. Returns list of errors.
```

### Comparing `valcheck-1.4/valcheck.egg-info/PKG-INFO` & `valcheck-1.5/valcheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 1.4
+Version: 1.5
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

