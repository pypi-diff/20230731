# Comparing `tmp/strawberry_resources-0.8.0.tar.gz` & `tmp/strawberry_resources-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_resources-0.8.0.tar", max compression
+gzip compressed data, was "strawberry_resources-0.8.1.tar", max compression
```

## Comparing `strawberry_resources-0.8.0.tar` & `strawberry_resources-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/LICENSE
--rw-r--r--   0        0        0     9125 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/README.md
--rw-r--r--   0        0        0     3851 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1174 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/__init__.py
--rw-r--r--   0        0        0       59 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/__main__.py
--rw-r--r--   0        0        0      123 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/cli/__init__.py
--rw-r--r--   0        0        0     1268 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/cli/export.py
--rw-r--r--   0        0        0     2811 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/exporter.py
--rw-r--r--   0        0        0      124 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/integrations/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/integrations/base.py
--rw-r--r--   0        0        0     9607 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/integrations/django.py
--rw-r--r--   0        0        0        0 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/py.typed
--rw-r--r--   0        0        0      628 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/queries.py
--rw-r--r--   0        0        0     7943 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/resolver.py
--rw-r--r--   0        0        0     7169 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/types.py
--rw-r--r--   0        0        0        0 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/utils/__init__.py
--rw-r--r--   0        0        0     2021 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/utils/inspect.py
--rw-r--r--   0        0        0      662 2023-07-29 13:56:47.382921 strawberry_resources-0.8.0/strawberry_resources/utils/pyutils.py
--rw-r--r--   0        0        0    10547 1970-01-01 00:00:00.000000 strawberry_resources-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-31 20:00:36.803022 strawberry_resources-0.8.1/LICENSE
+-rw-r--r--   0        0        0     9125 2023-07-31 20:00:36.803022 strawberry_resources-0.8.1/README.md
+-rw-r--r--   0        0        0     3851 2023-07-31 20:00:36.803022 strawberry_resources-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-07-31 20:00:36.803022 strawberry_resources-0.8.1/strawberry_resources/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-31 20:00:36.803022 strawberry_resources-0.8.1/strawberry_resources/__main__.py
+-rw-r--r--   0        0        0      123 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/cli/__init__.py
+-rw-r--r--   0        0        0     1268 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/cli/export.py
+-rw-r--r--   0        0        0     2811 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/exporter.py
+-rw-r--r--   0        0        0      124 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/integrations/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/integrations/base.py
+-rw-r--r--   0        0        0     9607 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/integrations/django.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/py.typed
+-rw-r--r--   0        0        0      628 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/queries.py
+-rw-r--r--   0        0        0     8995 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/resolver.py
+-rw-r--r--   0        0        0     7169 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/types.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/utils/__init__.py
+-rw-r--r--   0        0        0     2021 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/utils/inspect.py
+-rw-r--r--   0        0        0      662 2023-07-31 20:00:36.807022 strawberry_resources-0.8.1/strawberry_resources/utils/pyutils.py
+-rw-r--r--   0        0        0    10547 1970-01-01 00:00:00.000000 strawberry_resources-0.8.1/PKG-INFO
```

### Comparing `strawberry_resources-0.8.0/LICENSE` & `strawberry_resources-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/README.md` & `strawberry_resources-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/pyproject.toml` & `strawberry_resources-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-resources"
-version = "0.8.0"
+version = "0.8.1"
 description = "Introspection utilities to extract data from strawberry graphql"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-resources"
 repository = "https://github.com/blb-ventures/strawberry-resources"
 documentation = "https://github.com/blb-ventures/strawberry-resources"
```

### Comparing `strawberry_resources-0.8.0/strawberry_resources/__init__.py` & `strawberry_resources-0.8.1/strawberry_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/cli/export.py` & `strawberry_resources-0.8.1/strawberry_resources/cli/export.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/exporter.py` & `strawberry_resources-0.8.1/strawberry_resources/exporter.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/integrations/base.py` & `strawberry_resources-0.8.1/strawberry_resources/integrations/base.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/integrations/django.py` & `strawberry_resources-0.8.1/strawberry_resources/integrations/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/queries.py` & `strawberry_resources-0.8.1/strawberry_resources/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/resolver.py` & `strawberry_resources-0.8.1/strawberry_resources/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
+import contextlib
 import datetime
 import decimal
 import uuid
+import weakref
 from typing import (
+    Any,
     Dict,
     Optional,
     Tuple,
     Type,
     TypeVar,
+    _GenericAlias,  # type: ignore
     cast,
 )
 
 import strawberry
 from django.db import models
-from strawberry import Schema, relay
+from strawberry import Schema, object_type, relay
 from strawberry.custom_scalar import ScalarWrapper
 from strawberry.enum import EnumDefinition
 from strawberry.file_uploads import Upload
 from strawberry.lazy_type import LazyType
 from strawberry.scalars import JSON
 from strawberry.type import (
     StrawberryContainer,
     StrawberryList,
     StrawberryOptional,
     WithStrawberryObjectDefinition,
     get_object_definition,
+    has_object_definition,
 )
-from strawberry.types.types import TypeDefinition
 from strawberry.utils.str_converters import to_camel_case
 from typing_extensions import Annotated, TypeAlias, get_args, get_origin
 
 from .integrations.base import get_all
 from .types import (
     BaseFieldValidation,
     Field,
@@ -48,15 +52,15 @@
 from .utils.pyutils import dict_merge
 
 _R = TypeVar("_R")
 _T = TypeVar("_T", bound=type)
 _M = TypeVar("_M", bound=models.Model)
 _TypeMap: TypeAlias = Dict[str, Resource]
 
-MAX_DEPTH = 5
+DEFAULT_MAX_DEPTH = 2
 type_name_map: Dict[Schema, Optional[_TypeMap]] = {}
 field_type_map: Dict[type, FieldKind] = {
     bool: FieldKind.BOOLEAN,
     str: FieldKind.STRING,
     int: FieldKind.INT,
     float: FieldKind.FLOAT,
     datetime.date: FieldKind.DATE,
@@ -66,14 +70,28 @@
     decimal.Decimal: FieldKind.DECIMAL,
     uuid.UUID: FieldKind.UUID,
     strawberry.ID: FieldKind.ID,
     relay.GlobalID: FieldKind.ID,
     Upload.wrap: FieldKind.FILE,  # type: ignore
 }
 
+_original_annotations: Dict[type, Any] = cast(Dict[type, Any], weakref.WeakKeyDictionary())
+_original_wrap_dataclass = object_type._wrap_dataclass
+
+
+def _wrap_dataclass(cls: type):
+    with contextlib.suppress(AttributeError):
+        _original_annotations[cls] = cls.__annotations__.copy()
+    return _original_wrap_dataclass(cls)
+
+
+# FIXME: We might be able to remove this once we fix an issue on strawberry
+# which overrides annotations when graphql_type is defined.
+object_type._wrap_dataclass = _wrap_dataclass
+
 
 def get_resource_map(schema: "Schema") -> _TypeMap:
     if (type_map := type_name_map.get(schema)) is None:
         type_map = {}
 
         for resource in resolve_all(schema):
             type_map[resource.name] = resource
@@ -96,21 +114,28 @@
                 continue
 
             yield Resource(
                 name=type_def.name,
                 fields=list(
                     resolve_fields_for_type(
                         cast(Type[WithStrawberryObjectDefinition], type_def.origin),
+                        # We are resolving all types, no need to get more deep than 2
+                        max_depth=2,
                     ),
                 ),
             )
             seen.add(type_def.name)
 
 
-def resolve_fields_for_type(type_: Type[WithStrawberryObjectDefinition], *, depth: int = 0):
+def resolve_fields_for_type(
+    type_: Type[WithStrawberryObjectDefinition],
+    *,
+    depth: int = 0,
+    max_depth: int = DEFAULT_MAX_DEPTH,
+):
     integrations = get_all()
 
     type_def = get_object_definition(type_, strict=True)
 
     annotations = {}
     for o in reversed(type_def.origin.__mro__):
         annotations.update(getattr(o, "__annotations__", {}))
@@ -160,14 +185,17 @@
                 )
                 for value in f_type.values
             ]
             f_type = f_type.wrapped_cls
         if isinstance(f_type, ScalarWrapper):
             f_type = f_type.wrap
 
+        if isinstance(f_type, _GenericAlias):
+            continue
+
         type_map = field_type_map.copy()
         for integration in integrations:
             type_map.update(integration.get_extra_mappings())
             try:
                 options = dict_merge(
                     options,
                     integration.get_field_options(
@@ -182,19 +210,25 @@
                 break
 
         if (f_kind := field_type_map.get(cast(type, f_type))) is not None:
             options["kind"] = f_kind  # type: ignore
 
         # Override those options with the field options
         if (
-            (annotation := annotations.get(field.name)) and get_origin(annotation) is Annotated
-        ) or (
-            (resolver := getattr(type_def.origin, field.name, None))
-            and hasattr(resolver, "__annotations__")
-            and get_origin(annotation := resolver.__annotations__.get("return")) is Annotated
+            ((annotation := annotations.get(field.name)) and get_origin(annotation) is Annotated)
+            or (
+                (resolver := getattr(type_def.origin, field.name, None))
+                and hasattr(resolver, "__annotations__")
+                and get_origin(annotation := resolver.__annotations__.get("return")) is Annotated
+            )
+            or (
+                (original_annotations := _original_annotations.get(type_))
+                and (annotation := original_annotations.get(field.name))
+                and get_origin(annotation) is Annotated
+            )
         ):
             for opt in get_args(annotation)[1:]:
                 if isinstance(opt, HiddenField):
                     hidden = True
                     break
 
                 if not isinstance(opt, FieldOptionsConfig):
@@ -202,22 +236,19 @@
 
                 options = dict_merge(options, opt.options)
 
         if hidden:
             continue
 
         # If this is another type, we should return a FieldObject instead
-        if "obj_kind" in options or hasattr(f_type, "_type_definition"):
-            if depth > MAX_DEPTH:
+        if "obj_kind" in options or has_object_definition(f_type):
+            if depth > max_depth:
                 continue
 
-            inner_type_def = cast(
-                TypeDefinition,
-                f_type._type_definition,  # type: ignore
-            )
+            inner_type_def = get_object_definition(f_type, strict=True)
 
             assert isinstance(f_type, type)
             obj_kind = options.get("obj_kind")
             if obj_kind is None:
                 obj_kind_map: Dict[Tuple[bool, bool], FieldObjectKind] = {
                     (False, False): FieldObjectKind.OBJECT,
                     (True, False): FieldObjectKind.OBJECT_LIST,
@@ -232,15 +263,15 @@
                 ]
 
             yield FieldObject(
                 name=cname,
                 label=options.get("label", field.name),
                 obj_kind=obj_kind,
                 obj_type=inner_type_def.name,
-                fields=list(resolve_fields_for_type(f_type, depth=depth + 1)),
+                fields=list(resolve_fields_for_type(f_type, depth=depth + 1, max_depth=max_depth)),
             )
         else:
             options = cast(FieldOptions, options)
 
             # FIXME: How to improve this?
             if "kind" not in options:
                 continue
```

### Comparing `strawberry_resources-0.8.0/strawberry_resources/types.py` & `strawberry_resources-0.8.1/strawberry_resources/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/utils/inspect.py` & `strawberry_resources-0.8.1/strawberry_resources/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/strawberry_resources/utils/pyutils.py` & `strawberry_resources-0.8.1/strawberry_resources/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.8.0/PKG-INFO` & `strawberry_resources-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-resources
-Version: 0.8.0
+Version: 0.8.1
 Summary: Introspection utilities to extract data from strawberry graphql
 Home-page: https://github.com/blb-ventures/strawberry-resources
 License: MIT
 Keywords: strawberry,django,graphql,resources,forms
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

