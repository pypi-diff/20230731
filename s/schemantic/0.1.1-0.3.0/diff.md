# Comparing `tmp/schemantic-0.1.1.tar.gz` & `tmp/schemantic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemantic-0.1.1.tar", max compression
+gzip compressed data, was "schemantic-0.3.0.tar", max compression
```

## Comparing `schemantic-0.1.1.tar` & `schemantic-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1658 2023-04-22 06:37:56.957876 schemantic-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     4006 2023-07-21 16:08:39.683555 schemantic-0.1.1/README.md
--rw-r--r--   0        0        0      812 2023-07-26 05:47:30.908141 schemantic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      149 2023-07-20 13:49:23.765353 schemantic-0.1.1/schemantic/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 12:09:04.396978 schemantic-0.1.1/schemantic/model/__init__.py
--rw-r--r--   0        0        0     6273 2023-07-21 10:18:13.332261 schemantic-0.1.1/schemantic/model/field_info.py
--rw-r--r--   0        0        0     3263 2023-07-21 10:08:08.425583 schemantic-0.1.1/schemantic/model/schematic.py
--rw-r--r--   0        0        0     1599 2023-07-20 15:11:31.740543 schemantic-0.1.1/schemantic/project.py
--rw-r--r--   0        0        0       74 2023-07-20 13:48:44.549590 schemantic-0.1.1/schemantic/schema/__init__.py
--rw-r--r--   0        0        0     4095 2023-07-21 10:11:56.538350 schemantic-0.1.1/schemantic/schema/abstract.py
--rw-r--r--   0        0        0    20160 2023-07-21 10:10:18.734882 schemantic-0.1.1/schemantic/schema/main.py
--rw-r--r--   0        0        0        0 2023-07-18 13:10:43.500286 schemantic-0.1.1/schemantic/utils/__init__.py
--rw-r--r--   0        0        0      185 2023-07-19 09:35:47.546132 schemantic-0.1.1/schemantic/utils/constant.py
--rw-r--r--   0        0        0      870 2023-07-21 10:03:29.885030 schemantic-0.1.1/schemantic/utils/misc.py
--rw-r--r--   0        0        0      351 2023-07-21 10:10:18.725883 schemantic-0.1.1/schemantic/utils/typing.py
--rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 schemantic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1658 2023-04-22 06:37:56.957876 schemantic-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     4006 2023-07-21 16:08:39.683555 schemantic-0.3.0/README.md
+-rw-r--r--   0        0        0      812 2023-07-31 07:37:35.359527 schemantic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-07-20 13:49:23.765353 schemantic-0.3.0/schemantic/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:09:04.396978 schemantic-0.3.0/schemantic/model/__init__.py
+-rw-r--r--   0        0        0     6273 2023-07-21 10:18:13.332261 schemantic-0.3.0/schemantic/model/field_info.py
+-rw-r--r--   0        0        0     3256 2023-07-31 07:37:35.353528 schemantic-0.3.0/schemantic/model/schematic.py
+-rw-r--r--   0        0        0     1599 2023-07-20 15:11:31.740543 schemantic-0.3.0/schemantic/project.py
+-rw-r--r--   0        0        0       74 2023-07-20 13:48:44.549590 schemantic-0.3.0/schemantic/schema/__init__.py
+-rw-r--r--   0        0        0     4236 2023-07-31 07:37:35.356527 schemantic-0.3.0/schemantic/schema/abstract.py
+-rw-r--r--   0        0        0    21482 2023-07-31 07:37:35.356527 schemantic-0.3.0/schemantic/schema/main.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:10:43.500286 schemantic-0.3.0/schemantic/utils/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-19 09:35:47.546132 schemantic-0.3.0/schemantic/utils/constant.py
+-rw-r--r--   0        0        0      870 2023-07-21 10:03:29.885030 schemantic-0.3.0/schemantic/utils/misc.py
+-rw-r--r--   0        0        0      344 2023-07-31 07:37:35.353528 schemantic-0.3.0/schemantic/utils/typing.py
+-rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 schemantic-0.3.0/PKG-INFO
```

### Comparing `schemantic-0.1.1/LICENSE.md` & `schemantic-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.1/README.md` & `schemantic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.1/pyproject.toml` & `schemantic-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemantic"
-version = "0.1.1"
+version = "0.3.0"
 description = "Manipulate model schemas utilizing homologous, grouped, or cultured paradigms"
 authors = ["caniko <python@rotas.mozmail.com>"]
 license = "BSD-4"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `schemantic-0.1.1/schemantic/model/field_info.py` & `schemantic-0.3.0/schemantic/model/field_info.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.1/schemantic/model/schematic.py` & `schemantic-0.3.0/schemantic/model/schematic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import cached_property
-from typing import Optional, Union
+from typing import Optional
 
 from pydantic import BaseModel, computed_field, model_validator
 
 from schemantic.model.field_info import FieldMetadata
 from schemantic.utils.constant import (
     SCHEMA_DEFINED_MAPPING_KEY,
     SCHEMA_FIELD_INFO_MAPPING_KEY,
```

### Comparing `schemantic-0.1.1/schemantic/project.py` & `schemantic-0.3.0/schemantic/project.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.1/schemantic/schema/abstract.py` & `schemantic-0.3.0/schemantic/schema/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,16 @@
             # no self.mapping_name resolution needed.
             result = source
 
         return result[SCHEMA_DEFINED_MAPPING_KEY] if stored_in_defined else result
 
 
 class NotCultureSchema(BaseSchema, ABC):
+    pre_definitions: dict | None
+
     @abstractmethod
     def parse_schema(
         self,
         defined_schema: DefinedSchema,
         *,
         _inferior_config_kwargs: Optional[dict[str, Any]] = None,
     ) -> dict[str, dict[str, Any]]:
@@ -137,7 +139,11 @@
         Returns
         -------
 
         """
         return {
             name: self.origin(**instance_kwargs) for name, instance_kwargs in self.parse_schema(defined_schema).items()
         }
+
+
+class HomologousGroupMixin(BaseModel, ABC):
+    pre_definitions: dict[str, dict[str, Any]] | None = None
```

### Comparing `schemantic-0.1.1/schemantic/schema/main.py` & `schemantic-0.3.0/schemantic/schema/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from collections.abc import Mapping, Set
 from functools import cached_property
-from typing import Any, Callable, Generic, Iterable, Optional, Type, TypeVar, Union
+from typing import Any, Callable, Generic, Iterable, Optional, Type, TypeVar
 
 from ordered_set import OrderedSet
 from pydantic import BaseModel, computed_field, field_validator, model_validator, validate_call
 
 from schemantic.model.field_info import FieldMetadata, class_field_alias_to_type_string, model_field_alias_to_field_info
 from schemantic.model.schematic import Schematic
 from schemantic.project import SchemanticProjectMixin
-from schemantic.schema.abstract import BaseSchema, NotCultureSchema, SingleHomologousSchema
+from schemantic.schema.abstract import BaseSchema, HomologousGroupMixin, NotCultureSchema, SingleHomologousSchema
 from schemantic.utils.constant import (
     SCHEMA_DEFINED_MAPPING_KEY,
     SCHEMA_FIELD_INFO_MAPPING_KEY,
     SCHEMA_OPTIONAL_MAPPING_KEY,
     SCHEMA_REQUIRED_MAPPING_KEY,
 )
 from schemantic.utils.misc import update_assert_disjoint
@@ -32,14 +32,15 @@
     Used to define the schema of a single class or model.
 
     origin: Type
         The class or model of interest
     """
 
     origin: Type[T]
+    pre_definitions: dict[str, Any] | None = None
 
     def __hash__(self):
         return hash(self.origin)
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, SingleSchema):
             return False
@@ -62,16 +63,33 @@
             if issubclass(self.origin, BaseModel)
             else class_field_alias_to_type_string(self.origin, **kwargs)
         )
 
         return Schematic(class_name=self.origin.__name__, **required_optional_to_field_to_info)
 
     @validate_call
-    def schema(self, **schematic_dict_kwargs) -> dict[str, str | dict | list[str] | dict[str, str]]:
-        return self.schematic.schema_dict(**schematic_dict_kwargs)
+    def schema(
+        self, with_defined: bool = False, **schematic_dict_kwargs
+    ) -> dict[str, str | dict | list[str] | dict[str, str]]:
+        result = self.schematic.schema_dict(with_defined=with_defined, **schematic_dict_kwargs)
+
+        if self.pre_definitions:
+            if with_defined:
+                result["defined"] = self.pre_definitions
+            else:
+                if SCHEMA_REQUIRED_MAPPING_KEY in result:
+                    for k in result[SCHEMA_REQUIRED_MAPPING_KEY]:
+                        if k in self.pre_definitions:
+                            result[SCHEMA_REQUIRED_MAPPING_KEY][k] = self.pre_definitions[k]
+                if SCHEMA_OPTIONAL_MAPPING_KEY in result:
+                    for k in result[SCHEMA_OPTIONAL_MAPPING_KEY]:
+                        if k in self.pre_definitions:
+                            result[SCHEMA_OPTIONAL_MAPPING_KEY][k] = self.pre_definitions[k]
+
+        return result
 
     @validate_call
     def parse_schema(
         self,
         defined_schema: DefinedSchema,
         *,
         _inferior_config_kwargs: Optional[dict[str, Any]] = None,
@@ -82,15 +100,15 @@
         return {
             self.mapping_name: {**_inferior_config_kwargs, **config_from_file}
             if _inferior_config_kwargs
             else config_from_file
         }
 
 
-class HomologSchema(SingleHomologousSchema, Generic[T]):
+class HomologSchema(HomologousGroupMixin, SingleHomologousSchema, Generic[T]):
     """
     Represents a schema with multiple instances of the same origin, but are uniquely
     identified by their names. This is often useful in situations where you have
     a list of similar objects that each need their own configuration.
 
     single_schema: SingleSchema
         The single schema to use a reference for the single origin
@@ -177,15 +195,15 @@
         self, name_getter_kwargs: Optional[dict[str, Any]] = None, with_common: bool = True
     ) -> dict[str, str | dict | list[str] | NameToFieldMetadata]:
         result = dict(class_name=self.origin.__name__)
         if with_common:
             result["common"] = {}
 
         for name in self.homolog_names(name_getter_kwargs):
-            result[name] = {}
+            result[name] = self.pre_definitions[name] if self.pre_definitions and name in self.pre_definitions else {}
 
         result.update(self.single_schema.schematic.schema_dict_field_info_extracted(with_class_name=False))
 
         return result
 
     @validate_call
     def parse_schema(
@@ -216,15 +234,15 @@
         origin: Type[T],
         instance_names: Optional[OrderedSet[str]] = None,
         name_getter: Optional[Callable[[...], OrderedSet[str]]] = None,
     ) -> "HomologSchema":
         return cls(single_schema=SingleSchema(origin=origin), instance_names=instance_names, name_getter=name_getter)
 
 
-class GroupSchema(NotCultureSchema):
+class GroupSchema(HomologousGroupMixin, NotCultureSchema):
     """
     Represents a group of SingleSchema objects, and is used when you need to handle multiple models at the same time.
     """
 
     single_schemas: OrderedSet[SingleSchema]
     mapping_name: str
 
@@ -293,15 +311,17 @@
         common_field_to_info: dict[str, FieldMetadata] = {}
         field_to_field_info: dict[str, FieldMetadata] = {}
         for single_schema in self.single_schemas:
             name = single_schema.mapping_name
             schema_name_to_sub_schema[name] = dict(class_name=single_schema.origin.__name__)
 
             if with_defined:
-                schema_name_to_sub_schema[name][SCHEMA_DEFINED_MAPPING_KEY] = {}
+                schema_name_to_sub_schema[name][SCHEMA_DEFINED_MAPPING_KEY] = (
+                    self.pre_definitions[name] if self.pre_definitions and name in self.pre_definitions else {}
+                )
 
             if with_required and single_schema.schematic.required:
                 schema_name_to_sub_schema[name][SCHEMA_REQUIRED_MAPPING_KEY] = list(single_schema.schematic.required)
 
             if with_optional and single_schema.schematic.optional:
                 schema_name_to_sub_schema[name][SCHEMA_OPTIONAL_MAPPING_KEY] = list(single_schema.schematic.optional)
 
@@ -323,22 +343,26 @@
 
         result = {}
 
         if common_field_to_info and with_common:
             required: set[str] = set()
             optional: set[str] = set()
             for _schema_name, schema in schema_name_to_sub_schema.items():
-                required.update(schema.get("required", []))
+                required.update(schema.get(SCHEMA_REQUIRED_MAPPING_KEY, []))
                 optional.update(schema.get("optional", []))
 
             common_dict = {}
             if with_defined:
-                common_dict[SCHEMA_DEFINED_MAPPING_KEY] = {}
+                common_dict[SCHEMA_DEFINED_MAPPING_KEY] = (
+                    self.pre_definitions[SCHEMA_DEFINED_MAPPING_KEY]
+                    if self.pre_definitions and SCHEMA_DEFINED_MAPPING_KEY in self.pre_definitions
+                    else {}
+                )
             if required:
-                common_dict["required"] = list(sorted(required))
+                common_dict[SCHEMA_REQUIRED_MAPPING_KEY] = list(sorted(required))
             if optional:
                 common_dict["optional"] = list(sorted(optional))
             result["common"] = common_dict
 
         result.update(schema_name_to_sub_schema)
 
         combined_field_info = field_to_field_info
@@ -401,22 +425,22 @@
     ) -> dict[str, Any]:
         return {
             name: self.member_label_to_origin[name](**instance_kwargs)
             for name, instance_kwargs in self.parse_schema(defined_schema).items()
         }
 
     @classmethod
-    def from_originating_types(cls, origins: Iterable[Type] | Mapping[str, Type], mapping_name: str) -> "GroupSchema":
+    def from_originating_types(cls, origins: Iterable[Type] | Mapping[str, Type], **kwargs) -> "GroupSchema":
         return cls(
             single_schemas=OrderedSet(
                 SingleSchema(origin=origin, schema_alias=alias) for alias, origin in origins.items()
             )
             if isinstance(origins, Mapping)
             else OrderedSet(SingleSchema(origin=source_schema) for source_schema in origins),
-            mapping_name=mapping_name,
+            **kwargs,
         )
 
 
 class CultureSchema(BaseSchema):
     source_schemas: OrderedSet[NotCultureSchema]
 
     @validate_call
```

### Comparing `schemantic-0.1.1/schemantic/utils/misc.py` & `schemantic-0.3.0/schemantic/utils/misc.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.1/PKG-INFO` & `schemantic-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemantic
-Version: 0.1.1
+Version: 0.3.0
 Summary: Manipulate model schemas utilizing homologous, grouped, or cultured paradigms
 License: BSD-4
 Author: caniko
 Author-email: python@rotas.mozmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

