# Comparing `tmp/eo_styleguide-0.0.1a6.tar.gz` & `tmp/eo_styleguide-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eo_styleguide-0.0.1a6.tar", max compression
+gzip compressed data, was "eo_styleguide-0.0.1a7.tar", max compression
```

## Comparing `eo_styleguide-0.0.1a6.tar` & `eo_styleguide-0.0.1a7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3421 2023-07-29 14:37:37.987684 eo_styleguide-0.0.1a6/README.md
--rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a6/pyeo/__init__.py
--rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a6/pyeo/features/__init__.py
--rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a6/pyeo/features/feature.py
--rw-r--r--   0        0        0     1620 2023-07-29 22:13:02.772938 eo_styleguide-0.0.1a6/pyeo/features/final_object.py
--rw-r--r--   0        0        0     2810 2023-07-29 22:13:02.773315 eo_styleguide-0.0.1a6/pyeo/features/method_has_protocol.py
--rw-r--r--   0        0        0     2881 2023-07-29 22:13:02.773905 eo_styleguide-0.0.1a6/pyeo/features/no_code_in_ctors.py
--rw-r--r--   0        0        0     2046 2023-07-30 18:28:11.179784 eo_styleguide-0.0.1a6/pyeo/features/no_er_names.py
--rw-r--r--   0        0        0     1715 2023-07-29 22:13:02.774156 eo_styleguide-0.0.1a6/pyeo/features/no_property_methods.py
--rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a6/pyeo/features/no_reflection.py
--rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a6/pyeo/features/no_setters.py
--rw-r--r--   0        0        0     1794 2023-07-29 22:13:02.774412 eo_styleguide-0.0.1a6/pyeo/features/no_staticmethods.py
--rw-r--r--   0        0        0     1768 2023-07-23 13:29:32.046560 eo_styleguide-0.0.1a6/pyeo/features/object_has_protocol.py
--rw-r--r--   0        0        0     2128 2023-07-29 22:13:02.774645 eo_styleguide-0.0.1a6/pyeo/features/protocol_method_code_free.py
--rw-r--r--   0        0        0     3508 2023-07-29 22:13:02.774877 eo_styleguide-0.0.1a6/pyeo/main.py
--rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a6/pyeo/py.typed
--rw-r--r--   0        0        0        0 2023-07-29 22:13:02.774933 eo_styleguide-0.0.1a6/pyeo/utils/__init__.py
--rw-r--r--   0        0        0      268 2023-07-29 22:13:02.775282 eo_styleguide-0.0.1a6/pyeo/utils/decorator_name.py
--rw-r--r--   0        0        0      813 2023-07-30 18:28:25.131841 eo_styleguide-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0     3421 2023-07-29 14:37:37.987684 eo_styleguide-0.0.1a7/README.md
+-rw-r--r--   0        0        0     1291 2023-07-29 05:28:56.221950 eo_styleguide-0.0.1a7/pyeo/__init__.py
+-rw-r--r--   0        0        0     1118 2023-07-23 13:29:32.046205 eo_styleguide-0.0.1a7/pyeo/features/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-23 13:29:32.046339 eo_styleguide-0.0.1a7/pyeo/features/feature.py
+-rw-r--r--   0        0        0     1620 2023-07-29 22:13:02.772938 eo_styleguide-0.0.1a7/pyeo/features/final_object.py
+-rw-r--r--   0        0        0     2811 2023-07-31 18:09:02.876772 eo_styleguide-0.0.1a7/pyeo/features/method_has_protocol.py
+-rw-r--r--   0        0        0     2881 2023-07-29 22:13:02.773905 eo_styleguide-0.0.1a7/pyeo/features/no_code_in_ctors.py
+-rw-r--r--   0        0        0     2046 2023-07-30 18:28:11.179784 eo_styleguide-0.0.1a7/pyeo/features/no_er_names.py
+-rw-r--r--   0        0        0     1715 2023-07-29 22:13:02.774156 eo_styleguide-0.0.1a7/pyeo/features/no_property_methods.py
+-rw-r--r--   0        0        0     2495 2023-07-29 13:16:52.754226 eo_styleguide-0.0.1a7/pyeo/features/no_reflection.py
+-rw-r--r--   0        0        0     1977 2023-07-29 05:28:56.222831 eo_styleguide-0.0.1a7/pyeo/features/no_setters.py
+-rw-r--r--   0        0        0     1794 2023-07-29 22:13:02.774412 eo_styleguide-0.0.1a7/pyeo/features/no_staticmethods.py
+-rw-r--r--   0        0        0     1768 2023-07-31 18:09:17.461854 eo_styleguide-0.0.1a7/pyeo/features/object_has_protocol.py
+-rw-r--r--   0        0        0     2128 2023-07-29 22:13:02.774645 eo_styleguide-0.0.1a7/pyeo/features/protocol_method_code_free.py
+-rw-r--r--   0        0        0     3344 2023-07-31 18:09:39.535138 eo_styleguide-0.0.1a7/pyeo/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:17:44.927051 eo_styleguide-0.0.1a7/pyeo/py.typed
+-rw-r--r--   0        0        0        0 2023-07-29 22:13:02.774933 eo_styleguide-0.0.1a7/pyeo/utils/__init__.py
+-rw-r--r--   0        0        0      268 2023-07-29 22:13:02.775282 eo_styleguide-0.0.1a7/pyeo/utils/decorator_name.py
+-rw-r--r--   0        0        0      813 2023-07-31 18:10:25.678006 eo_styleguide-0.0.1a7/pyproject.toml
+-rw-r--r--   0        0        0     4312 1970-01-01 00:00:00.000000 eo_styleguide-0.0.1a7/PKG-INFO
```

### Comparing `eo_styleguide-0.0.1a6/README.md` & `eo_styleguide-0.0.1a7/README.md`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/__init__.py` & `eo_styleguide-0.0.1a7/pyeo/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/__init__.py` & `eo_styleguide-0.0.1a7/pyeo/features/__init__.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/feature.py` & `eo_styleguide-0.0.1a7/pyeo/features/feature.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/final_object.py` & `eo_styleguide-0.0.1a7/pyeo/features/final_object.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/method_has_protocol.py` & `eo_styleguide-0.0.1a7/pyeo/features/method_has_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,19 @@
             def_body.name: def_body
             for def_body in ctx.cls.defs.body
             if isinstance(def_body, FuncDef) and not def_body.name.startswith('_') and not self._method_is_ctor(def_body)
         }
         if not ctx.cls.base_type_exprs:
             return False
         extra_method_names = set(object_methods.keys()) - {  # noqa: WPS224 need a refactor
-            method.name
+            method
             for base_type in ctx.cls.base_type_exprs
             for node in base_type.node.mro
-            for method in node.defn.defs.body
-            if isinstance(method, FuncDef)
+            if hasattr(node.defn.info, 'names')
+            for method in node.defn.info.names
         }
         if extra_method_names:
             failed_methods = [
                 method
                 for method_name, method in object_methods.items()
                 if method_name in extra_method_names
             ]
```

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/no_code_in_ctors.py` & `eo_styleguide-0.0.1a7/pyeo/features/no_code_in_ctors.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/no_er_names.py` & `eo_styleguide-0.0.1a7/pyeo/features/no_er_names.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/no_property_methods.py` & `eo_styleguide-0.0.1a7/pyeo/features/no_property_methods.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/no_reflection.py` & `eo_styleguide-0.0.1a7/pyeo/features/no_reflection.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/no_setters.py` & `eo_styleguide-0.0.1a7/pyeo/features/no_setters.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/no_staticmethods.py` & `eo_styleguide-0.0.1a7/pyeo/features/no_staticmethods.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/object_has_protocol.py` & `eo_styleguide-0.0.1a7/pyeo/features/object_has_protocol.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/features/protocol_method_code_free.py` & `eo_styleguide-0.0.1a7/pyeo/features/protocol_method_code_free.py`

 * *Files identical despite different names*

### Comparing `eo_styleguide-0.0.1a6/pyeo/main.py` & `eo_styleguide-0.0.1a7/pyeo/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,34 +31,29 @@
 from pyeo.features.no_reflection import NoReflectionFeature
 from pyeo.features.no_setters import NoSettersFeature
 from pyeo.features.no_staticmethods import NoStaticmethodsFeature
 from pyeo.features.object_has_protocol import ObjectHasProtocolFeature
 from pyeo.features.protocol_method_code_free import ProtocolMethodCodeFreeFeature
 
 
-def _is_protocl(cls):
+def _is_protocol(cls):
     if not cls.removed_base_type_exprs:
         return False
     if isinstance(cls.removed_base_type_exprs[0], IndexExpr):
         return cls.removed_base_type_exprs[0].base.fullname == 'typing.Protocol'
     return cls.removed_base_type_exprs[0].fullname == 'typing.Protocol'
 
 
 def analyze(ctx):
     """Features controller.
 
     :param ctx: mypy context
     :return: bool
     """
-    # print(ctx.cls.fullname)
-    # # print(ctx.cls.removed_base_type_exprs)
-    # for x in ctx.cls.removed_base_type_exprs:
-    #     print(x)
-    # print('\n' * 3)
-    if _is_protocl(ctx.cls):
+    if _is_protocol(ctx.cls):
         NoPropertyMethodsFeature().analyze(ctx)
         ProtocolMethodCodeFreeFeature().analyze(ctx)
         NoSettersFeature().analyze(ctx)
         NoStaticmethodsFeature().analyze(ctx)
         return True
     if not ObjectHasProtocolFeature().analyze(ctx):
         return True
```

### Comparing `eo_styleguide-0.0.1a6/pyproject.toml` & `eo_styleguide-0.0.1a7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "eo-styleguide"
 packages = [
     {include = "pyeo"}
 ]
-version = "0.0.1-alpha6"
+version = "0.0.1-alpha7"
 description = "Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability."
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `eo_styleguide-0.0.1a6/PKG-INFO` & `eo_styleguide-0.0.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eo-styleguide
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: Pyeo is an advanced static analysis tool tailored specifically to enforce the principles advocated by Elegant Objects (elegantobjects.org) in Python projects. It serves as a quality control instrument to ensure that your Python code adheres to the core tenets of elegance, simplicity, and maintainability.
 License: MIT
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

