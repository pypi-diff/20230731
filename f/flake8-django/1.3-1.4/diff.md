# Comparing `tmp/flake8_django-1.3.tar.gz` & `tmp/flake8_django-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_django-1.3.tar", max compression
+gzip compressed data, was "flake8_django-1.4.tar", max compression
```

## Comparing `flake8_django-1.3.tar` & `flake8_django-1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3393 2022-08-10 20:12:15.744827 flake8_django-1.3/README.md
--rw-r--r--   0        0        0       67 2022-08-10 20:12:15.744919 flake8_django-1.3/flake8_django/__init__.py
--rw-r--r--   0        0        0     3361 2023-05-22 09:49:06.622640 flake8_django-1.3/flake8_django/checker.py
--rw-r--r--   0        0        0      501 2022-08-10 20:12:15.745093 flake8_django-1.3/flake8_django/checkers/__init__.py
--rw-r--r--   0        0        0     1235 2023-05-22 09:49:06.622822 flake8_django-1.3/flake8_django/checkers/base_model_checker.py
--rw-r--r--   0        0        0      708 2023-05-22 09:49:06.622980 flake8_django-1.3/flake8_django/checkers/checker.py
--rw-r--r--   0        0        0      828 2022-08-10 20:12:15.745299 flake8_django-1.3/flake8_django/checkers/decorator.py
--rw-r--r--   0        0        0      504 2022-08-10 20:12:15.745364 flake8_django-1.3/flake8_django/checkers/issue.py
--rw-r--r--   0        0        0     3973 2023-05-22 09:49:06.623142 flake8_django-1.3/flake8_django/checkers/model_content_order.py
--rw-r--r--   0        0        0      906 2023-05-22 09:49:06.623288 flake8_django-1.3/flake8_django/checkers/model_dunder_str.py
--rw-r--r--   0        0        0     1438 2022-08-10 20:12:15.745587 flake8_django-1.3/flake8_django/checkers/model_fields.py
--rw-r--r--   0        0        0     2182 2023-05-22 09:49:06.623441 flake8_django-1.3/flake8_django/checkers/model_form.py
--rw-r--r--   0        0        0     2047 2023-05-22 09:49:06.623597 flake8_django-1.3/flake8_django/checkers/model_meta.py
--rw-r--r--   0        0        0      731 2022-08-10 20:12:15.745787 flake8_django-1.3/flake8_django/checkers/render.py
--rw-r--r--   0        0        0      680 2023-05-22 09:49:06.623716 flake8_django-1.3/flake8_django/checkers/utils.py
--rw-r--r--   0        0        0      979 2023-05-22 09:52:23.605895 flake8_django-1.3/pyproject.toml
--rw-r--r--   0        0        0     4414 1970-01-01 00:00:00.000000 flake8_django-1.3/PKG-INFO
+-rw-r--r--   0        0        0     3393 2022-08-10 20:12:15.744827 flake8_django-1.4/README.md
+-rw-r--r--   0        0        0       67 2022-08-10 20:12:15.744919 flake8_django-1.4/flake8_django/__init__.py
+-rw-r--r--   0        0        0     3361 2023-05-22 09:49:06.622640 flake8_django-1.4/flake8_django/checker.py
+-rw-r--r--   0        0        0      501 2022-08-10 20:12:15.745093 flake8_django-1.4/flake8_django/checkers/__init__.py
+-rw-r--r--   0        0        0     1235 2023-05-22 09:49:06.622822 flake8_django-1.4/flake8_django/checkers/base_model_checker.py
+-rw-r--r--   0        0        0      708 2023-05-22 09:49:06.622980 flake8_django-1.4/flake8_django/checkers/checker.py
+-rw-r--r--   0        0        0      828 2022-08-10 20:12:15.745299 flake8_django-1.4/flake8_django/checkers/decorator.py
+-rw-r--r--   0        0        0      504 2022-08-10 20:12:15.745364 flake8_django-1.4/flake8_django/checkers/issue.py
+-rw-r--r--   0        0        0     4037 2023-07-31 08:55:45.572062 flake8_django-1.4/flake8_django/checkers/model_content_order.py
+-rw-r--r--   0        0        0      906 2023-05-22 09:49:06.623288 flake8_django-1.4/flake8_django/checkers/model_dunder_str.py
+-rw-r--r--   0        0        0     1438 2022-08-10 20:12:15.745587 flake8_django-1.4/flake8_django/checkers/model_fields.py
+-rw-r--r--   0        0        0     2363 2023-07-31 08:55:45.572262 flake8_django-1.4/flake8_django/checkers/model_form.py
+-rw-r--r--   0        0        0     2047 2023-05-22 09:49:06.623597 flake8_django-1.4/flake8_django/checkers/model_meta.py
+-rw-r--r--   0        0        0      731 2022-08-10 20:12:15.745787 flake8_django-1.4/flake8_django/checkers/render.py
+-rw-r--r--   0        0        0      680 2023-05-22 09:49:06.623716 flake8_django-1.4/flake8_django/checkers/utils.py
+-rw-r--r--   0        0        0      980 2023-07-31 09:01:07.009273 flake8_django-1.4/pyproject.toml
+-rw-r--r--   0        0        0     4414 1970-01-01 00:00:00.000000 flake8_django-1.4/PKG-INFO
```

### Comparing `flake8_django-1.3/README.md` & `flake8_django-1.4/README.md`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checker.py` & `flake8_django-1.4/flake8_django/checker.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/base_model_checker.py` & `flake8_django-1.4/flake8_django/checkers/base_model_checker.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/checker.py` & `flake8_django-1.4/flake8_django/checkers/checker.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/decorator.py` & `flake8_django-1.4/flake8_django/checkers/decorator.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/model_content_order.py` & `flake8_django-1.4/flake8_django/checkers/model_content_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import astroid
+from astroid.exceptions import InferenceError
 from functools import partial
 
 from .base_model_checker import BaseModelChecker
 from .issue import Issue
 from .utils import node_is_subclass
 
 
@@ -29,15 +30,15 @@
         for inferred_value in node.value.func.inferred():
             if node_is_subclass(
                 inferred_value,
                 [".Field", "django.db.models.fields.Field"],
             ):
                 return True
         return False
-    except AttributeError:
+    except (AttributeError, InferenceError):
         return False
 
 
 def is_manager_declaration(node):
     return (
         isinstance(node, astroid.Assign)
         and getattr(node.targets[0], 'name', None) == 'objects'
```

### Comparing `flake8_django-1.3/flake8_django/checkers/model_dunder_str.py` & `flake8_django-1.4/flake8_django/checkers/model_dunder_str.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/model_fields.py` & `flake8_django-1.4/flake8_django/checkers/model_fields.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/model_form.py` & `flake8_django-1.4/flake8_django/checkers/model_form.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,21 +20,27 @@
     def checker_applies(self, node):
         return self.is_model(node)
 
     def is_string_dunder_all(self, element):
         """
         Return True if element is astroid.Const, astroid.List or astroid.Tuple  and equals "__all__"
         """
-        if isinstance(element.value, (astroid.List, astroid.Tuple)):
+        assign_value = element.value
+        if not isinstance(
+            assign_value,
+            (astroid.List, astroid.Tuple, astroid.Const),
+        ):
+            return False
+        if isinstance(assign_value, (astroid.List, astroid.Tuple)):
             return any(
                 iter_item.value == '__all__'
-                for iter_item in element.value.itered()
+                for iter_item in assign_value.itered()
             )
         else:
-            node_value = element.value.value
+            node_value = assign_value.value
             if isinstance(node_value, bytes):
                 node_value = node_value.decode()
             return node_value == '__all__'
 
     def run(self, node):
         """
         Captures the use of exclude in ModelForm Meta
```

### Comparing `flake8_django-1.3/flake8_django/checkers/model_meta.py` & `flake8_django-1.4/flake8_django/checkers/model_meta.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/render.py` & `flake8_django-1.4/flake8_django/checkers/render.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/flake8_django/checkers/utils.py` & `flake8_django-1.4/flake8_django/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.3/pyproject.toml` & `flake8_django-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-django"
-version = "1.3"
+version = "1.4"
 license = "GPL-3.0-or-later"
 description = "Plugin to catch bad style specific to Django Projects."
 authors = ["Rocio Aramberri Schegel <rocio.aramberri@schegel.net>"]
 readme = "README.md"
 keywords = ["flake8", "django", "lint"]
 repository = "https://github.com/rocioar/flake8-django"
 classifiers=[
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.plugins]
 [tool.poetry.plugins."flake8.extension"]
-DJ = "flake8_django:DjangoStyleChecker"
+DJ0 = "flake8_django:DjangoStyleChecker"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 astroid = "^2.15.2"
```

### Comparing `flake8_django-1.3/PKG-INFO` & `flake8_django-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-django
-Version: 1.3
+Version: 1.4
 Summary: Plugin to catch bad style specific to Django Projects.
 Home-page: https://github.com/rocioar/flake8-django
 License: GPL-3.0-or-later
 Keywords: flake8,django,lint
 Author: Rocio Aramberri Schegel
 Author-email: rocio.aramberri@schegel.net
 Requires-Python: >=3.7.2,<4.0.0
```

