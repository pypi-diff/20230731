# Comparing `tmp/sparkql-0.7.0.tar.gz` & `tmp/sparkql-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkql-0.7.0.tar", max compression
+gzip compressed data, was "sparkql-0.8.0.tar", max compression
```

## Comparing `sparkql-0.7.0.tar` & `sparkql-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1087 2023-04-10 20:40:55.925387 sparkql-0.7.0/LICENSE
--rw-r--r--   0        0        0    14716 2023-04-10 20:40:55.925387 sparkql-0.7.0/README.md
--rw-r--r--   0        0        0     1443 2023-04-10 20:41:40.449412 sparkql-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      952 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/__init__.py
--rw-r--r--   0        0        0     1066 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/accessors.py
--rw-r--r--   0        0        0     2387 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/exceptions.py
--rw-r--r--   0        0        0      491 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/__init__.py
--rw-r--r--   0        0        0     5913 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/array.py
--rw-r--r--   0        0        0     4165 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/atomic.py
--rw-r--r--   0        0        0    12199 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/base.py
--rw-r--r--   0        0        0    26425 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/fields/struct.py
--rw-r--r--   0        0        0     3436 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/formatters.py
--rw-r--r--   0        0        0      351 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/schema_builder.py
--rw-r--r--   0        0        0     5762 2023-04-10 20:40:55.929387 sparkql-0.7.0/sparkql/schema_merger.py
--rw-r--r--   0        0        0    16521 1970-01-01 00:00:00.000000 sparkql-0.7.0/setup.py
--rw-r--r--   0        0        0    15434 1970-01-01 00:00:00.000000 sparkql-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-30 22:43:49.078621 sparkql-0.8.0/LICENSE
+-rw-r--r--   0        0        0    15308 2023-07-30 22:43:49.078621 sparkql-0.8.0/README.md
+-rw-r--r--   0        0        0     1443 2023-07-30 22:44:41.414889 sparkql-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/__init__.py
+-rw-r--r--   0        0        0     1218 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/accessors.py
+-rw-r--r--   0        0        0     2387 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/exceptions.py
+-rw-r--r--   0        0        0      491 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/__init__.py
+-rw-r--r--   0        0        0     6065 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/array.py
+-rw-r--r--   0        0        0     4165 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/atomic.py
+-rw-r--r--   0        0        0    13748 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/base.py
+-rw-r--r--   0        0        0    26487 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/fields/struct.py
+-rw-r--r--   0        0        0     3692 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/formatters.py
+-rw-r--r--   0        0        0      351 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/schema_builder.py
+-rw-r--r--   0        0        0     6566 2023-07-30 22:43:49.082621 sparkql-0.8.0/sparkql/schema_merger.py
+-rw-r--r--   0        0        0    17131 1970-01-01 00:00:00.000000 sparkql-0.8.0/setup.py
+-rw-r--r--   0        0        0    16026 1970-01-01 00:00:00.000000 sparkql-0.8.0/PKG-INFO
```

### Comparing `sparkql-0.7.0/LICENSE` & `sparkql-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkql-0.7.0/README.md` & `sparkql-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -234,14 +234,32 @@
 Both give the same result. However, the former (`e`) is more
 type-oriented. The `e` attribute corresponds to the array's element
 field. Although this looks strange at first, it has the advantage of
 being inspectable by IDEs and other tools, allowing goodness such as
 IDE auto-completion, automated refactoring, and identifying errors
 before runtime.
 
+### Field metadata
+
+Field [metadata](https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.types.StructField.html) can be specified with the `metadata` argument to a field, which accepts a dictionary
+of key-value pairs.
+
+```python
+class Article(Struct):
+    title = String(nullable=False,
+                   metadata={"description": "The title of the article", "max_length": 100})
+```
+
+The metadata can be accessed with the `METADATA` property of the field:
+
+```python
+Article.title.METADATA
+{"description": "The title of the article", "max_length": 100}
+```
+
 ### DataFrame validation
 
 Struct method `validate_data_frame` will verify if a given DataFrame's
 schema matches the Struct.
 [For example](https://github.com/mattjw/sparkql/tree/master/examples/validation/test_validation.py),
 if we have our `Article`
 struct and a DataFrame we want to ensure adheres to the `Article`
```

### Comparing `sparkql-0.7.0/pyproject.toml` & `sparkql-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkql"
-version = "0.7.0"  # do not edit manually. kept in sync with `tool.commitizen` config via automation
+version = "0.8.0"  # do not edit manually. kept in sync with `tool.commitizen` config via automation
 description = "sparkql: Apache Spark SQL DataFrame schema management for sensible humans"
 authors = ["Matt J Williams <mattjw@mattjw.net>"]
 repository = "https://github.com/mattjw/sparkql"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
@@ -39,15 +39,15 @@
 debug-auto-git-tag = "tasks:debug_auto_git_tag"
 
 [tool.black]
 line-length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0"  # do not edit manually. kept in sync with `tool.poetry` config via automation
+version = "0.8.0"  # do not edit manually. kept in sync with `tool.poetry` config via automation
 tag_format = "v$version"
 
 [tool.coverage.run]
 branch = true
 
 [build-system]
 requires = ["poetry>=1.3"]
```

### Comparing `sparkql-0.7.0/sparkql/__init__.py` & `sparkql-0.8.0/sparkql/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.7.0/sparkql/accessors.py` & `sparkql-0.8.0/sparkql/accessors.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,10 +24,15 @@
 
 
 def name(field: BaseField) -> str:
     """Return field name of field `field`; an alias of `BaseField.NAME`."""
     return field.NAME
 
 
+def metadata(field: BaseField) -> dict:
+    """Return field metadata of field `field`; an alias of `BaseField.METADATA`."""
+    return field.METADATA
+
+
 def struct_field(field: BaseField) -> StructField:
     """Return the equivalent PySpark StructField of field `field`."""
     return field._spark_struct_field  # pylint: disable=protected-access
```

### Comparing `sparkql-0.7.0/sparkql/exceptions.py` & `sparkql-0.8.0/sparkql/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.7.0/sparkql/fields/array.py` & `sparkql-0.8.0/sparkql/fields/array.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Array field."""
 
 import copy
 from collections.abc import Sequence
-from typing import Optional, Generic, TypeVar, Any
+from typing import Optional, Generic, TypeVar, Any, Dict
 
 from pyspark.sql.types import ArrayType, StructField
 
 from sparkql.exceptions import FieldValueValidationError
 from sparkql.fields.base import BaseField
 
 
@@ -27,16 +27,22 @@
         etype: Data type info for the element of this array. Should be an instance of a `BaseField`.
     """
 
     __hash__ = BaseField.__hash__
 
     e: ArrayElementType  # pytype: disable=not-supported-yet  # pylint: disable=invalid-name
 
-    def __init__(self, element: ArrayElementType, nullable: bool = True, name: Optional[str] = None):
-        super().__init__(nullable=nullable, name=name)
+    def __init__(
+        self,
+        element: ArrayElementType,
+        nullable: bool = True,
+        name: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+    ):
+        super().__init__(nullable=nullable, name=name, metadata=metadata)
 
         if not isinstance(element, BaseField):
             raise ValueError(f"Array element must be a field. Found type: {type(element).__name__}")
 
         if element._resolve_field_name() is not None:
             # we require that the array's element should be a "vanilla" field. it should not have been given
             # any name (explicit nor contextual)
@@ -103,14 +109,15 @@
             name=self._field_name,
             dataType=ArrayType(
                 # Note that we do not care about the element's field name here:
                 elementType=self.e._spark_struct_field.dataType,  # pylint: disable=protected-access
                 containsNull=self.e._is_nullable,  # pylint: disable=protected-access
             ),
             nullable=self._is_nullable,
+            metadata=self._metadata,
         )
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         if value is None:
             # super() will have already validate none vs nullability. if None, then it's safe to be none
             return
```

### Comparing `sparkql-0.7.0/sparkql/fields/atomic.py` & `sparkql-0.8.0/sparkql/fields/atomic.py`

 * *Files identical despite different names*

### Comparing `sparkql-0.7.0/sparkql/fields/base.py` & `sparkql-0.8.0/sparkql/fields/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base field and abstract fields."""
 
 from abc import ABC, abstractmethod
-from typing import Optional, Type, Any, Tuple, Sequence
+from typing import Optional, Type, Any, Tuple, Sequence, Dict
 import copy
 
 from pyspark.sql import types as sql_type, Column
 from pyspark.sql import functions as sql_funcs
 from pyspark.sql.types import StructField, DataType
 
 from sparkql.exceptions import FieldNameError, FieldParentError, FieldValueValidationError
@@ -29,38 +29,52 @@
     # Name management logic:
     # - Explicit name (`__name_explicit`): Set via constructor.
     # - Contextual name (`__name_contextual`): Inferred for the field as it is used in a struct object.
     #   This will always get set, although not immediately. The struct object that will contain this field
     #   is responsible for setting the contextual name.
     # The explicit name, if provided, will override the contextual name.
 
+    # Placeholders for private instance variables received via the constructor. (Represented here
+    # for convenience only; these will be overwritten.)
     __nullable: bool = True
     __name_explicit: Optional[str] = None
     __name_contextual: Optional[str] = None
+    __metadata: Dict[str, Any] = {}  # must be overwritten in constructor
+
+    # Placeholder for "protected" style variables. (Again, represented only for convenience.)
     _parent_struct: Optional["Struct"] = None  # pytype: disable=name-error
 
-    def __init__(self, nullable: bool = True, name: Optional[str] = None):
+    def __init__(self, nullable: bool = True, name: Optional[str] = None, metadata: Optional[Dict[str, Any]] = None):
         """
         Constructor for a base field.
 
         Args:
             nullable: Is this field nullable.
             name: Field name. If None, field name will be identified via ivar context resolution.
+            metadata:
+                Metadata for this field. Metadata is a native feature of Spark and PySpark, allowing a field to be
+                annotated. If None, then metadata will be treated as an empty dictionary.
         """
         self.__nullable = nullable
         self.__name_explicit = name
+        self.__metadata = {} if metadata is None else dict(metadata)
 
     #
     # Nullability
 
     @property
     def _is_nullable(self) -> bool:
         """The nullability status of this field."""
         return self.__nullable
 
+    @property
+    def _metadata(self) -> Optional[Dict[str, Any]]:
+        """The metadata of this field."""
+        return self.__metadata
+
     #
     # Field path chaining
 
     @property
     def _parent(self) -> Optional["Struct"]:  # pytype: disable=name-error
         return self._parent_struct
 
@@ -175,14 +189,19 @@
         return ".".join(self.SEQ)
 
     @property
     def NAME(self) -> str:
         """The name of this field."""
         return self._field_name
 
+    @property
+    def METADATA(self) -> Dict[str, Any]:
+        """The metadata for this field."""
+        return self._metadata
+
     #
     # Spark type management
 
     @property
     @abstractmethod
     def _spark_type_class(self) -> Type[DataType]:
         """The class of the Spark type corresponding to this field."""
@@ -216,14 +235,15 @@
         """True if `self` equals `other`."""
         # Subclasses should call this as part of their equality checks
         return (
             isinstance(other, BaseField)
             and self._is_nullable == other._is_nullable
             and self._resolve_field_name() == other._resolve_field_name()  # may be None == None
             and self._spark_type_class == other._spark_type_class
+            and self._metadata == other._metadata  # may be None == None
         )
 
     def __str__(self):
         """Returns the name of this field."""
         # stringifying a field as its field adds some convenience for cases where we need the field
         # name
         return self._resolve_field_name("")
@@ -232,21 +252,32 @@
         """String formatted object with a more complete summary of this field, primarily for debugging."""
         return (
             f"<{self.__class__.__name__}\n"
             f"  spark type = {self._spark_type_class.__name__}\n"
             f"  nullable = {self._is_nullable}\n"
             f"  name = {self._resolve_field_name()} <- {[self.__name_explicit, self.__name_contextual]}\n"
             f"  parent = {self._parent}\n"
+            f"  metadata = {self._metadata}\n"
             ">"
         )
 
     def _short_info(self):
         """Short info string for use in error messages."""
         nullable = "Nullable " if self._is_nullable else ""
-        return f"<{nullable}{self.__class__.__name__}: {self._resolve_field_name()}>"
+
+        # Good candidate for python pattern matching once <3.10 support no longer required
+        num_metadata_items = len(self.__metadata)
+        if num_metadata_items == 0:
+            metadata = ""
+        elif num_metadata_items == 1:
+            metadata = f" [with {num_metadata_items} metadata item]"
+        else:
+            metadata = f" [with {num_metadata_items} metadata items]"
+
+        return f"<{nullable}{self.__class__.__name__}{metadata}: {self._resolve_field_name()}>"
 
     def __hash__(self):
         return hash((self._is_nullable, self._resolve_field_name(""), self._spark_type_class))
 
     def __repr__(self):
         return self._short_info()
 
@@ -275,15 +306,20 @@
     def _spark_data_type(self) -> sql_type.DataType:
         """Corresponding Spark datatype for this class."""
         return self._spark_type_class()
 
     @property
     def _spark_struct_field(self) -> StructField:
         """The StructField for this object."""
-        return StructField(name=self._field_name, dataType=self._spark_data_type, nullable=self._is_nullable)
+        return StructField(
+            name=self._field_name,
+            dataType=self._spark_data_type,
+            nullable=self._is_nullable,
+            metadata=self._metadata,
+        )
 
     def __eq__(self, other: Any) -> bool:
         """True if `self` equals `other`."""
         return (
             super().__eq__(other) and isinstance(other, AtomicField) and self._spark_data_type == other._spark_data_type
         )
```

### Comparing `sparkql-0.7.0/sparkql/fields/struct.py` & `sparkql-0.8.0/sparkql/fields/struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,18 @@
     def _spark_type_class(self) -> Type[DataType]:
         return sql_types.StructType
 
     @property
     def _spark_struct_field(self) -> StructField:
         """The Spark StructField for this field."""
         return StructField(
-            name=self._field_name, dataType=self._struct_metadata.spark_struct, nullable=self._is_nullable
+            name=self._field_name,
+            dataType=self._struct_metadata.spark_struct,
+            nullable=self._is_nullable,
+            metadata=self._metadata,
         )
 
     def _validate_on_value(self, value: Any) -> None:
         super()._validate_on_value(value)
         if value is None:
             # super() will have already validate none vs nullability. if None, then it's safe to be none
             return
```

### Comparing `sparkql-0.7.0/sparkql/formatters.py` & `sparkql-0.8.0/sparkql/formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,24 @@
         if isinstance(field.dataType, (StructType, ArrayType)):
             formatted += "\n" + cls._indent(depth + 1)
 
         formatted += cls._pretty_data_type(field.dataType, depth + 1) + ", "
 
         if isinstance(field.dataType, (StructType, ArrayType)):
             formatted += "\n" + cls._indent(depth + 1)
-        formatted += f"{cls._boolean_as_str(field.nullable)})"
+
+        formatted += f"{cls._boolean_as_str(field.nullable)}"
+
+        if field.metadata:
+            formatted += ", "
+            if isinstance(field.dataType, (StructType, ArrayType)):
+                formatted += "\n" + cls._indent(depth + 1)
+            formatted += str(field.metadata)
+
+        formatted += ")"
 
         return formatted
 
 
 def pretty_schema(struct: StructType) -> str:
     """
     Returns a pretty stringified `struct`.
```

### Comparing `sparkql-0.7.0/sparkql/schema_merger.py` & `sparkql-0.8.0/sparkql/schema_merger.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,18 +76,32 @@
                     "Fields must have matching nullability constraints. "
                     f"nullable of field A is {field_a.nullable}. "
                     f"nullable of field B is {field_b.nullable}",
                     parent_field_name=field_a.name,
                 )
             )
 
+        shared_metadata_keys = set(field_a.metadata.keys()) & set(field_b.metadata.keys())
+        if shared_metadata_keys:
+            if any(field_a.metadata[key] != field_b.metadata[key] for key in shared_metadata_keys):
+                raise ValueError(
+                    _validation_error_message(
+                        "Cannot merge due to a conflict in field metadata. "
+                        "If both metadata share the same keys, those keys must have the same values. "
+                        f"metadata of field A is {field_a.metadata}. "
+                        f"metadata of field B is {field_b.metadata}. ",
+                        parent_field_name=field_a.name,
+                    )
+                )
+
         return StructField(
             name=field_a.name,
             dataType=cls.merge_types(field_a.dataType, field_b.dataType, parent_field_name=field_a.name),
             nullable=field_a.nullable,
+            metadata={**(field_a.metadata or {}), **(field_b.metadata or {})},
         )
 
     #
     # Merge by type
 
     @classmethod
     def merge_types(
```

### Comparing `sparkql-0.7.0/setup.py` & `sparkql-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
                      'reformat = tasks:reformat',
                      'test = tasks:test',
                      'typecheck = tasks:typecheck',
                      'verify-all = tasks:verify_all']}
 
 setup_kwargs = {
     'name': 'sparkql',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'sparkql: Apache Spark SQL DataFrame schema management for sensible humans',
-    'long_description': '# sparkql ✨\n\n[![PyPI version](https://badge.fury.io/py/sparkql.svg)](https://badge.fury.io/py/sparkql)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/mattjw/sparkql/workflows/CI/badge.svg)](https://github.com/mattjw/sparkql/actions)\n[![codecov](https://codecov.io/gh/mattjw/sparkql/branch/master/graph/badge.svg)](https://codecov.io/gh/mattjw/sparkql)\n\nPython Spark SQL DataFrame schema management for sensible humans.\n\n> _Don\'t sweat it... sparkql it ✨_\n\n## Why use sparkql\n\n`sparkql` takes the pain out of working with DataFrame schemas in PySpark.\nIt makes schema definition more Pythonic. And it\'s\nparticularly useful you\'re dealing with structured data.\n\nIn plain old PySpark, you might find that you write schemas\n[like this](https://github.com/mattjw/sparkql/tree/master/examples/conferences_comparison/plain_schema.py):\n\n```python\nCITY_SCHEMA = StructType()\nCITY_NAME_FIELD = "name"\nCITY_SCHEMA.add(StructField(CITY_NAME_FIELD, StringType(), False))\nCITY_LAT_FIELD = "latitude"\nCITY_SCHEMA.add(StructField(CITY_LAT_FIELD, FloatType()))\nCITY_LONG_FIELD = "longitude"\nCITY_SCHEMA.add(StructField(CITY_LONG_FIELD, FloatType()))\n\nCONFERENCE_SCHEMA = StructType()\nCONF_NAME_FIELD = "name"\nCONFERENCE_SCHEMA.add(StructField(CONF_NAME_FIELD, StringType(), False))\nCONF_CITY_FIELD = "city"\nCONFERENCE_SCHEMA.add(StructField(CONF_CITY_FIELD, CITY_SCHEMA))\n```\n\nAnd then plain old PySpark makes you deal with nested fields like this:\n\n```python\ndframe.withColumn("city_name", df[CONF_CITY_FIELD][CITY_NAME_FIELD])\n```\n\nInstead, with `sparkql`, schemas become a lot\n[more literate](https://github.com/mattjw/sparkql/tree/master/examples/conferences_comparison/sparkql_schema.py):\n\n```python\nclass City(Struct):\n    name = String(nullable=False)\n    latitude = Float()\n    longitude = Float()\n\nclass Conference(Struct):\n    name = String(nullable=False)\n    city = City()\n```\n\nAs does dealing with nested fields:\n\n```python\ndframe.withColumn("city_name", Conference.city.name.COL)\n```\n\nHere\'s a summary of `sparkql`\'s features.\n\n- ORM-like class-based Spark schema definitions.\n- Automated field naming: The attribute name of a field as it appears\n  in its `Struct` is (by default) used as its field name. This name can\n  be optionally overridden.\n- Programatically reference nested fields in your structs with the\n  `PATH` and `COL` special properties. Avoid hand-constructing strings\n  (or `Column`s) to reference your nested fields.\n- Validate that a DataFrame matches a `sparkql` schema.\n- Reuse and build composite schemas with `inheritance`, `includes`, and\n  `implements`.\n- Get a human-readable Spark schema representation with `pretty_schema`.\n- Create an instance of a schema as a dictionary, with validation of\n  the input values.\n\nRead on for documentation on these features.\n\n## Defining a schema\n\nEach Spark atomic type has a counterpart `sparkql` field:\n\n| PySpark type | `sparkql` field |\n|---|---|\n| `ByteType` | `Byte` |\n| `IntegerType` | `Integer` |\n| `LongType` | `Long` |\n| `ShortType` | `Short` |\n| `DecimalType` | `Decimal` |\n| `DoubleType` | `Double` |\n| `FloatType` | `Float` |\n| `StringType` | `String` |\n| `BinaryType` | `Binary` |\n| `BooleanType` | `Boolean` |\n| `DateType` | `Date` |\n| `TimestampType` | `Timestamp` |\n\n`Array` (counterpart to `ArrayType` in PySpark) allows the definition\nof arrays of objects. By creating a subclass of `Struct`, we can\ndefine a custom class that will be converted to a `StructType`.\n\nFor\n[example](https://github.com/mattjw/sparkql/tree/master/examples/arrays/arrays.py),\ngiven the `sparkql` schema definition:\n\n```python\nfrom sparkql import Struct, String, Array\n\nclass Article(Struct):\n    title = String(nullable=False)\n    tags = Array(String(), nullable=False)\n    comments = Array(String(nullable=False))\n```\n\nThen we can build the equivalent PySpark schema (a `StructType`)\nwith:\n\n```python\nfrom sparkql import schema\n\npyspark_struct = schema(Article)\n```\n\nPretty printing the schema with the expression\n`sparkql.pretty_schema(pyspark_struct)` will give the following:\n\n```text\nStructType([\n    StructField(\'title\', StringType(), False),\n    StructField(\'tags\',\n        ArrayType(StringType(), True),\n        False),\n    StructField(\'comments\',\n        ArrayType(StringType(), False),\n        True)])\n```\n\n## Features\n\nMany examples of how to use `sparkql` can be found in\n[`examples`](https://github.com/mattjw/sparkql/tree/master/examples).\n\n### Automated field naming\n\nBy default, field names are inferred from the attribute name in the\nstruct they are declared.\n\nFor example, given the struct\n\n```python\nclass Geolocation(Struct):\n    latitude = Float()\n    longitude = Float()\n```\n\nthe concrete name of the `Geolocation.latitude` field is `latitude`.\n\nNames also be overridden by explicitly specifying the field name as an\nargument to the field\n\n```python\nclass Geolocation(Struct):\n    latitude = Float(name="lat")\n    longitude = Float(name="lon")\n```\n\nwhich would mean the concrete name of the `Geolocation.latitude` field\nis `lat`.\n\n### Field paths and nested objects\n\nReferencing fields in nested data can be a chore. `sparkql` simplifies this\nwith path referencing.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/nested_objects/sparkql_example.py), if we have a\nschema with nested objects:\n\n```python\nclass Address(Struct):\n    post_code = String()\n    city = String()\n\n\nclass User(Struct):\n    username = String(nullable=False)\n    address = Address()\n\n\nclass Comment(Struct):\n    message = String()\n    author = User(nullable=False)\n\n\nclass Article(Struct):\n    title = String(nullable=False)\n    author = User(nullable=False)\n    comments = Array(Comment())\n```\n\nWe can use the special `PATH` property to turn a path into a\nSpark-understandable string:\n\n```python\nauthor_city_str = Article.author.address.city.PATH\n"author.address.city"\n```\n\n`COL` is a counterpart to `PATH` that returns a Spark `Column`\nobject for the path, allowing it to be used in all places where Spark\nrequires a column.\n\nFunction equivalents `path_str`, `path_col`, and `name` are also available.\nThis table demonstrates the equivalence of the property styles and the function\nstyles:\n\n| Property style | Function style | Result (both styles are equivalent) |\n| --- | --- | --- |\n| `Article.author.address.city.PATH` | `sparkql.path_str(Article.author.address.city)` | `"author.address.city"` |\n| `Article.author.address.city.COL` | `sparkql.path_col(Article.author.address.city)` | `Column` pointing to `author.address.city` |\n| `Article.author.address.city.NAME` | `sparkql.name(Article.author.address.city)` | `"city"` |\n\nFor paths that include an array, two approaches are provided:\n\n```python\ncomment_usernames_str = Article.comments.e.author.username.PATH\n"comments.author.username"\n\ncomment_usernames_str = Article.comments.author.username.PATH\n"comments.author.username"\n```\n\nBoth give the same result. However, the former (`e`) is more\ntype-oriented. The `e` attribute corresponds to the array\'s element\nfield. Although this looks strange at first, it has the advantage of\nbeing inspectable by IDEs and other tools, allowing goodness such as\nIDE auto-completion, automated refactoring, and identifying errors\nbefore runtime.\n\n### DataFrame validation\n\nStruct method `validate_data_frame` will verify if a given DataFrame\'s\nschema matches the Struct.\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/validation/test_validation.py),\nif we have our `Article`\nstruct and a DataFrame we want to ensure adheres to the `Article`\nschema:\n\n```python\ndframe = spark_session.createDataFrame([{"title": "abc"}])\n\nclass Article(Struct):\n    title = String()\n    body = String()\n```\n\nThen we can can validate with:\n\n```python\nvalidation_result = Article.validate_data_frame(dframe)\n```\n\n`validation_result.is_valid` indicates whether the DataFrame is valid\n(`False` in this case), and `validation_result.report` is a\nhuman-readable string describing the differences:\n\n```text\nStruct schema...\n\nStructType([\n    StructField(\'title\', StringType(), True),\n    StructField(\'body\', StringType(), True)])\n\nDataFrame schema...\n\nStructType([\n    StructField(\'title\', StringType(), True)])\n\nDiff of struct -> data frame...\n\n  StructType([\n-     StructField(\'title\', StringType(), True)])\n+     StructField(\'title\', StringType(), True),\n+     StructField(\'body\', StringType(), True)])\n```\n\nFor convenience,\n\n```python\nArticle.validate_data_frame(dframe).raise_on_invalid()\n```\n\nwill raise a `InvalidDataFrameError` (see `sparkql.exceptions`) if the  \nDataFrame is not valid.\n\n### Creating an instance of a schema\n\n`sparkql` simplifies the process of creating an instance of a struct.\nYou might need to do this, for example, when creating test data, or\nwhen creating an object (a dict or a row) to return from a UDF.\n\nUse `Struct.make_dict(...)` to instantiate a struct as a dictionary.\nThis has the advantage that the input values will be correctly\nvalidated, and it will convert schema property names into their\nunderlying field names.\n\nFor\n[example](https://github.com/mattjw/sparkql/tree/master/examples/struct_instantiation/instantiate_as_dict.py),\ngiven some simple Structs:\n\n```python\nclass User(Struct):\n    id = Integer(name="user_id", nullable=False)\n    username = String()\n\nclass Article(Struct):\n    id = Integer(name="article_id", nullable=False)\n    title = String()\n    author = User()\n    text = String(name="body")\n```\n\nHere are a few examples of creating dicts from `Article`:\n\n```python\nArticle.make_dict(\n    id=1001,\n    title="The article title",\n    author=User.make_dict(\n        id=440,\n        username="user"\n    ),\n    text="Lorem ipsum article text lorem ipsum."\n)\n\n# generates...\n{\n    "article_id": 1001,\n    "author": {\n        "user_id": 440,\n        "username": "user"},\n    "body": "Lorem ipsum article text lorem ipsum.",\n    "title": "The article title"\n}\n```\n\n```python\nArticle.make_dict(\n    id=1002\n)\n\n# generates...\n{\n    "article_id": 1002,\n    "author": None,\n    "body": None,\n    "title": None\n}\n```\n\nSee\n[this example](https://github.com/mattjw/sparkql/tree/master/examples/conferences_extended/conferences.py)\nfor an extended example of using `make_dict`.\n\n### Composite schemas\n\nIt is sometimes useful to be able to re-use the fields of one struct\nin another struct. `sparkql` provides a few features to enable this:\n\n- _inheritance_: A subclass inherits the fields of a base struct class.\n- _includes_: Incorporate fields from another struct.\n- _implements_: Enforce that a struct must implement the fields of\n  another struct.\n\nSee the following examples for a better explanation.\n\n#### Using inheritance\n\nFor [example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/inheritance.py), the following:\n\n```python\nclass BaseEvent(Struct):\n    correlation_id = String(nullable=False)\n    event_time = Timestamp(nullable=False)\n\nclass RegistrationEvent(BaseEvent):\n    user_id = String(nullable=False)\n```\n\nwill produce the following `RegistrationEvent` schema:\n\n```text\nStructType([\n    StructField(\'correlation_id\', StringType(), False),\n    StructField(\'event_time\', TimestampType(), False),\n    StructField(\'user_id\', StringType(), False)])\n```\n\n#### Using an `includes` declaration\n\nFor [example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/includes.py), the following:\n\n```python\nclass EventMetadata(Struct):\n    correlation_id = String(nullable=False)\n    event_time = Timestamp(nullable=False)\n\nclass RegistrationEvent(Struct):\n    class Meta:\n        includes = [EventMetadata]\n    user_id = String(nullable=False)\n```\n\nwill produce the `RegistrationEvent` schema:\n\n```text\nStructType(List(\n    StructField(\'user_id\', StringType(), False),\n    StructField(\'correlation_id\', StringType(), False),\n    StructField(\'event_time\', TimestampType(), False)))\n```\n\n#### Using an `implements` declaration\n\n`implements` is similar to `includes`, but does not automatically\nincorporate the fields of specified structs. Instead, it is up to\nthe implementor to ensure that the required fields are declared in\nthe struct.\n\nFailing to implement a field from an `implements` struct will result in\na `StructImplementationError` error.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/implements.py):\n\n```\nclass LogEntryMetadata(Struct):\n    logged_at = Timestamp(nullable=False)\n\nclass PageViewLogEntry(Struct):\n    class Meta:\n        implements = [LogEntryMetadata]\n    page_id = String(nullable=False)\n\n# the above class declaration will fail with the following StructImplementationError error:\n#   Struct \'PageViewLogEntry\' does not implement field \'logged_at\' required by struct \'LogEntryMetadata\'\n```\n\n\n### Prettified Spark schema strings\n\nSpark\'s stringified schema representation isn\'t very user-friendly, particularly for large schemas:\n\n\n```text\nStructType([StructField(\'name\', StringType(), False), StructField(\'city\', StructType([StructField(\'name\', StringType(), False), StructField(\'latitude\', FloatType(), True), StructField(\'longitude\', FloatType(), True)]), True)])\n```\n\nThe function `pretty_schema` will return something more useful:\n\n```text\nStructType([\n    StructField(\'name\', StringType(), False),\n    StructField(\'city\',\n        StructType([\n            StructField(\'name\', StringType(), False),\n            StructField(\'latitude\', FloatType(), True),\n            StructField(\'longitude\', FloatType(), True)]),\n        True)])\n```\n\n### Merge two Spark `StructType` types\n\nIt can be useful to build a composite schema from two `StructType`s. sparkql provides a\n`merge_schemas` function to do this.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/merge_struct_types/merge_struct_types.py):\n\n```python\nschema_a = StructType([\n    StructField("message", StringType()),\n    StructField("author", ArrayType(\n        StructType([\n            StructField("name", StringType())\n        ])\n    ))\n])\n\nschema_b = StructType([\n    StructField("author", ArrayType(\n        StructType([\n            StructField("address", StringType())\n        ])\n    ))\n])\n\nmerged_schema = merge_schemas(schema_a, schema_b) \n```\n\nresults in a `merged_schema` that looks like:\n\n```text\nStructType([\n    StructField(\'message\', StringType(), True),\n    StructField(\'author\',\n        ArrayType(StructType([\n            StructField(\'name\', StringType(), True),\n            StructField(\'address\', StringType(), True)]), True),\n        True)])\n```\n\n## Contributing\n\nContributions are very welcome. Developers who\'d like to contribute to\nthis project should refer to [CONTRIBUTING.md](./CONTRIBUTING.md).\n',
+    'long_description': '# sparkql ✨\n\n[![PyPI version](https://badge.fury.io/py/sparkql.svg)](https://badge.fury.io/py/sparkql)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/mattjw/sparkql/workflows/CI/badge.svg)](https://github.com/mattjw/sparkql/actions)\n[![codecov](https://codecov.io/gh/mattjw/sparkql/branch/master/graph/badge.svg)](https://codecov.io/gh/mattjw/sparkql)\n\nPython Spark SQL DataFrame schema management for sensible humans.\n\n> _Don\'t sweat it... sparkql it ✨_\n\n## Why use sparkql\n\n`sparkql` takes the pain out of working with DataFrame schemas in PySpark.\nIt makes schema definition more Pythonic. And it\'s\nparticularly useful you\'re dealing with structured data.\n\nIn plain old PySpark, you might find that you write schemas\n[like this](https://github.com/mattjw/sparkql/tree/master/examples/conferences_comparison/plain_schema.py):\n\n```python\nCITY_SCHEMA = StructType()\nCITY_NAME_FIELD = "name"\nCITY_SCHEMA.add(StructField(CITY_NAME_FIELD, StringType(), False))\nCITY_LAT_FIELD = "latitude"\nCITY_SCHEMA.add(StructField(CITY_LAT_FIELD, FloatType()))\nCITY_LONG_FIELD = "longitude"\nCITY_SCHEMA.add(StructField(CITY_LONG_FIELD, FloatType()))\n\nCONFERENCE_SCHEMA = StructType()\nCONF_NAME_FIELD = "name"\nCONFERENCE_SCHEMA.add(StructField(CONF_NAME_FIELD, StringType(), False))\nCONF_CITY_FIELD = "city"\nCONFERENCE_SCHEMA.add(StructField(CONF_CITY_FIELD, CITY_SCHEMA))\n```\n\nAnd then plain old PySpark makes you deal with nested fields like this:\n\n```python\ndframe.withColumn("city_name", df[CONF_CITY_FIELD][CITY_NAME_FIELD])\n```\n\nInstead, with `sparkql`, schemas become a lot\n[more literate](https://github.com/mattjw/sparkql/tree/master/examples/conferences_comparison/sparkql_schema.py):\n\n```python\nclass City(Struct):\n    name = String(nullable=False)\n    latitude = Float()\n    longitude = Float()\n\nclass Conference(Struct):\n    name = String(nullable=False)\n    city = City()\n```\n\nAs does dealing with nested fields:\n\n```python\ndframe.withColumn("city_name", Conference.city.name.COL)\n```\n\nHere\'s a summary of `sparkql`\'s features.\n\n- ORM-like class-based Spark schema definitions.\n- Automated field naming: The attribute name of a field as it appears\n  in its `Struct` is (by default) used as its field name. This name can\n  be optionally overridden.\n- Programatically reference nested fields in your structs with the\n  `PATH` and `COL` special properties. Avoid hand-constructing strings\n  (or `Column`s) to reference your nested fields.\n- Validate that a DataFrame matches a `sparkql` schema.\n- Reuse and build composite schemas with `inheritance`, `includes`, and\n  `implements`.\n- Get a human-readable Spark schema representation with `pretty_schema`.\n- Create an instance of a schema as a dictionary, with validation of\n  the input values.\n\nRead on for documentation on these features.\n\n## Defining a schema\n\nEach Spark atomic type has a counterpart `sparkql` field:\n\n| PySpark type | `sparkql` field |\n|---|---|\n| `ByteType` | `Byte` |\n| `IntegerType` | `Integer` |\n| `LongType` | `Long` |\n| `ShortType` | `Short` |\n| `DecimalType` | `Decimal` |\n| `DoubleType` | `Double` |\n| `FloatType` | `Float` |\n| `StringType` | `String` |\n| `BinaryType` | `Binary` |\n| `BooleanType` | `Boolean` |\n| `DateType` | `Date` |\n| `TimestampType` | `Timestamp` |\n\n`Array` (counterpart to `ArrayType` in PySpark) allows the definition\nof arrays of objects. By creating a subclass of `Struct`, we can\ndefine a custom class that will be converted to a `StructType`.\n\nFor\n[example](https://github.com/mattjw/sparkql/tree/master/examples/arrays/arrays.py),\ngiven the `sparkql` schema definition:\n\n```python\nfrom sparkql import Struct, String, Array\n\nclass Article(Struct):\n    title = String(nullable=False)\n    tags = Array(String(), nullable=False)\n    comments = Array(String(nullable=False))\n```\n\nThen we can build the equivalent PySpark schema (a `StructType`)\nwith:\n\n```python\nfrom sparkql import schema\n\npyspark_struct = schema(Article)\n```\n\nPretty printing the schema with the expression\n`sparkql.pretty_schema(pyspark_struct)` will give the following:\n\n```text\nStructType([\n    StructField(\'title\', StringType(), False),\n    StructField(\'tags\',\n        ArrayType(StringType(), True),\n        False),\n    StructField(\'comments\',\n        ArrayType(StringType(), False),\n        True)])\n```\n\n## Features\n\nMany examples of how to use `sparkql` can be found in\n[`examples`](https://github.com/mattjw/sparkql/tree/master/examples).\n\n### Automated field naming\n\nBy default, field names are inferred from the attribute name in the\nstruct they are declared.\n\nFor example, given the struct\n\n```python\nclass Geolocation(Struct):\n    latitude = Float()\n    longitude = Float()\n```\n\nthe concrete name of the `Geolocation.latitude` field is `latitude`.\n\nNames also be overridden by explicitly specifying the field name as an\nargument to the field\n\n```python\nclass Geolocation(Struct):\n    latitude = Float(name="lat")\n    longitude = Float(name="lon")\n```\n\nwhich would mean the concrete name of the `Geolocation.latitude` field\nis `lat`.\n\n### Field paths and nested objects\n\nReferencing fields in nested data can be a chore. `sparkql` simplifies this\nwith path referencing.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/nested_objects/sparkql_example.py), if we have a\nschema with nested objects:\n\n```python\nclass Address(Struct):\n    post_code = String()\n    city = String()\n\n\nclass User(Struct):\n    username = String(nullable=False)\n    address = Address()\n\n\nclass Comment(Struct):\n    message = String()\n    author = User(nullable=False)\n\n\nclass Article(Struct):\n    title = String(nullable=False)\n    author = User(nullable=False)\n    comments = Array(Comment())\n```\n\nWe can use the special `PATH` property to turn a path into a\nSpark-understandable string:\n\n```python\nauthor_city_str = Article.author.address.city.PATH\n"author.address.city"\n```\n\n`COL` is a counterpart to `PATH` that returns a Spark `Column`\nobject for the path, allowing it to be used in all places where Spark\nrequires a column.\n\nFunction equivalents `path_str`, `path_col`, and `name` are also available.\nThis table demonstrates the equivalence of the property styles and the function\nstyles:\n\n| Property style | Function style | Result (both styles are equivalent) |\n| --- | --- | --- |\n| `Article.author.address.city.PATH` | `sparkql.path_str(Article.author.address.city)` | `"author.address.city"` |\n| `Article.author.address.city.COL` | `sparkql.path_col(Article.author.address.city)` | `Column` pointing to `author.address.city` |\n| `Article.author.address.city.NAME` | `sparkql.name(Article.author.address.city)` | `"city"` |\n\nFor paths that include an array, two approaches are provided:\n\n```python\ncomment_usernames_str = Article.comments.e.author.username.PATH\n"comments.author.username"\n\ncomment_usernames_str = Article.comments.author.username.PATH\n"comments.author.username"\n```\n\nBoth give the same result. However, the former (`e`) is more\ntype-oriented. The `e` attribute corresponds to the array\'s element\nfield. Although this looks strange at first, it has the advantage of\nbeing inspectable by IDEs and other tools, allowing goodness such as\nIDE auto-completion, automated refactoring, and identifying errors\nbefore runtime.\n\n### Field metadata\n\nField [metadata](https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.types.StructField.html) can be specified with the `metadata` argument to a field, which accepts a dictionary\nof key-value pairs.\n\n```python\nclass Article(Struct):\n    title = String(nullable=False,\n                   metadata={"description": "The title of the article", "max_length": 100})\n```\n\nThe metadata can be accessed with the `METADATA` property of the field:\n\n```python\nArticle.title.METADATA\n{"description": "The title of the article", "max_length": 100}\n```\n\n### DataFrame validation\n\nStruct method `validate_data_frame` will verify if a given DataFrame\'s\nschema matches the Struct.\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/validation/test_validation.py),\nif we have our `Article`\nstruct and a DataFrame we want to ensure adheres to the `Article`\nschema:\n\n```python\ndframe = spark_session.createDataFrame([{"title": "abc"}])\n\nclass Article(Struct):\n    title = String()\n    body = String()\n```\n\nThen we can can validate with:\n\n```python\nvalidation_result = Article.validate_data_frame(dframe)\n```\n\n`validation_result.is_valid` indicates whether the DataFrame is valid\n(`False` in this case), and `validation_result.report` is a\nhuman-readable string describing the differences:\n\n```text\nStruct schema...\n\nStructType([\n    StructField(\'title\', StringType(), True),\n    StructField(\'body\', StringType(), True)])\n\nDataFrame schema...\n\nStructType([\n    StructField(\'title\', StringType(), True)])\n\nDiff of struct -> data frame...\n\n  StructType([\n-     StructField(\'title\', StringType(), True)])\n+     StructField(\'title\', StringType(), True),\n+     StructField(\'body\', StringType(), True)])\n```\n\nFor convenience,\n\n```python\nArticle.validate_data_frame(dframe).raise_on_invalid()\n```\n\nwill raise a `InvalidDataFrameError` (see `sparkql.exceptions`) if the  \nDataFrame is not valid.\n\n### Creating an instance of a schema\n\n`sparkql` simplifies the process of creating an instance of a struct.\nYou might need to do this, for example, when creating test data, or\nwhen creating an object (a dict or a row) to return from a UDF.\n\nUse `Struct.make_dict(...)` to instantiate a struct as a dictionary.\nThis has the advantage that the input values will be correctly\nvalidated, and it will convert schema property names into their\nunderlying field names.\n\nFor\n[example](https://github.com/mattjw/sparkql/tree/master/examples/struct_instantiation/instantiate_as_dict.py),\ngiven some simple Structs:\n\n```python\nclass User(Struct):\n    id = Integer(name="user_id", nullable=False)\n    username = String()\n\nclass Article(Struct):\n    id = Integer(name="article_id", nullable=False)\n    title = String()\n    author = User()\n    text = String(name="body")\n```\n\nHere are a few examples of creating dicts from `Article`:\n\n```python\nArticle.make_dict(\n    id=1001,\n    title="The article title",\n    author=User.make_dict(\n        id=440,\n        username="user"\n    ),\n    text="Lorem ipsum article text lorem ipsum."\n)\n\n# generates...\n{\n    "article_id": 1001,\n    "author": {\n        "user_id": 440,\n        "username": "user"},\n    "body": "Lorem ipsum article text lorem ipsum.",\n    "title": "The article title"\n}\n```\n\n```python\nArticle.make_dict(\n    id=1002\n)\n\n# generates...\n{\n    "article_id": 1002,\n    "author": None,\n    "body": None,\n    "title": None\n}\n```\n\nSee\n[this example](https://github.com/mattjw/sparkql/tree/master/examples/conferences_extended/conferences.py)\nfor an extended example of using `make_dict`.\n\n### Composite schemas\n\nIt is sometimes useful to be able to re-use the fields of one struct\nin another struct. `sparkql` provides a few features to enable this:\n\n- _inheritance_: A subclass inherits the fields of a base struct class.\n- _includes_: Incorporate fields from another struct.\n- _implements_: Enforce that a struct must implement the fields of\n  another struct.\n\nSee the following examples for a better explanation.\n\n#### Using inheritance\n\nFor [example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/inheritance.py), the following:\n\n```python\nclass BaseEvent(Struct):\n    correlation_id = String(nullable=False)\n    event_time = Timestamp(nullable=False)\n\nclass RegistrationEvent(BaseEvent):\n    user_id = String(nullable=False)\n```\n\nwill produce the following `RegistrationEvent` schema:\n\n```text\nStructType([\n    StructField(\'correlation_id\', StringType(), False),\n    StructField(\'event_time\', TimestampType(), False),\n    StructField(\'user_id\', StringType(), False)])\n```\n\n#### Using an `includes` declaration\n\nFor [example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/includes.py), the following:\n\n```python\nclass EventMetadata(Struct):\n    correlation_id = String(nullable=False)\n    event_time = Timestamp(nullable=False)\n\nclass RegistrationEvent(Struct):\n    class Meta:\n        includes = [EventMetadata]\n    user_id = String(nullable=False)\n```\n\nwill produce the `RegistrationEvent` schema:\n\n```text\nStructType(List(\n    StructField(\'user_id\', StringType(), False),\n    StructField(\'correlation_id\', StringType(), False),\n    StructField(\'event_time\', TimestampType(), False)))\n```\n\n#### Using an `implements` declaration\n\n`implements` is similar to `includes`, but does not automatically\nincorporate the fields of specified structs. Instead, it is up to\nthe implementor to ensure that the required fields are declared in\nthe struct.\n\nFailing to implement a field from an `implements` struct will result in\na `StructImplementationError` error.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/composite_schemas/implements.py):\n\n```\nclass LogEntryMetadata(Struct):\n    logged_at = Timestamp(nullable=False)\n\nclass PageViewLogEntry(Struct):\n    class Meta:\n        implements = [LogEntryMetadata]\n    page_id = String(nullable=False)\n\n# the above class declaration will fail with the following StructImplementationError error:\n#   Struct \'PageViewLogEntry\' does not implement field \'logged_at\' required by struct \'LogEntryMetadata\'\n```\n\n\n### Prettified Spark schema strings\n\nSpark\'s stringified schema representation isn\'t very user-friendly, particularly for large schemas:\n\n\n```text\nStructType([StructField(\'name\', StringType(), False), StructField(\'city\', StructType([StructField(\'name\', StringType(), False), StructField(\'latitude\', FloatType(), True), StructField(\'longitude\', FloatType(), True)]), True)])\n```\n\nThe function `pretty_schema` will return something more useful:\n\n```text\nStructType([\n    StructField(\'name\', StringType(), False),\n    StructField(\'city\',\n        StructType([\n            StructField(\'name\', StringType(), False),\n            StructField(\'latitude\', FloatType(), True),\n            StructField(\'longitude\', FloatType(), True)]),\n        True)])\n```\n\n### Merge two Spark `StructType` types\n\nIt can be useful to build a composite schema from two `StructType`s. sparkql provides a\n`merge_schemas` function to do this.\n\n[For example](https://github.com/mattjw/sparkql/tree/master/examples/merge_struct_types/merge_struct_types.py):\n\n```python\nschema_a = StructType([\n    StructField("message", StringType()),\n    StructField("author", ArrayType(\n        StructType([\n            StructField("name", StringType())\n        ])\n    ))\n])\n\nschema_b = StructType([\n    StructField("author", ArrayType(\n        StructType([\n            StructField("address", StringType())\n        ])\n    ))\n])\n\nmerged_schema = merge_schemas(schema_a, schema_b) \n```\n\nresults in a `merged_schema` that looks like:\n\n```text\nStructType([\n    StructField(\'message\', StringType(), True),\n    StructField(\'author\',\n        ArrayType(StructType([\n            StructField(\'name\', StringType(), True),\n            StructField(\'address\', StringType(), True)]), True),\n        True)])\n```\n\n## Contributing\n\nContributions are very welcome. Developers who\'d like to contribute to\nthis project should refer to [CONTRIBUTING.md](./CONTRIBUTING.md).\n',
     'author': 'Matt J Williams',
     'author_email': 'mattjw@mattjw.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mattjw/sparkql',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sparkql-0.7.0/PKG-INFO` & `sparkql-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkql
-Version: 0.7.0
+Version: 0.8.0
 Summary: sparkql: Apache Spark SQL DataFrame schema management for sensible humans
 Home-page: https://github.com/mattjw/sparkql
 License: MIT
 Author: Matt J Williams
 Author-email: mattjw@mattjw.net
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -253,14 +253,32 @@
 Both give the same result. However, the former (`e`) is more
 type-oriented. The `e` attribute corresponds to the array's element
 field. Although this looks strange at first, it has the advantage of
 being inspectable by IDEs and other tools, allowing goodness such as
 IDE auto-completion, automated refactoring, and identifying errors
 before runtime.
 
+### Field metadata
+
+Field [metadata](https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.types.StructField.html) can be specified with the `metadata` argument to a field, which accepts a dictionary
+of key-value pairs.
+
+```python
+class Article(Struct):
+    title = String(nullable=False,
+                   metadata={"description": "The title of the article", "max_length": 100})
+```
+
+The metadata can be accessed with the `METADATA` property of the field:
+
+```python
+Article.title.METADATA
+{"description": "The title of the article", "max_length": 100}
+```
+
 ### DataFrame validation
 
 Struct method `validate_data_frame` will verify if a given DataFrame's
 schema matches the Struct.
 [For example](https://github.com/mattjw/sparkql/tree/master/examples/validation/test_validation.py),
 if we have our `Article`
 struct and a DataFrame we want to ensure adheres to the `Article`
```

