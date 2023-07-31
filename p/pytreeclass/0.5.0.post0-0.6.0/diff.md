# Comparing `tmp/pytreeclass-0.5.0.post0.tar.gz` & `tmp/pytreeclass-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.5.0.post0.tar", last modified: Thu Jul 27 21:44:30 2023, max compression
+gzip compressed data, was "pytreeclass-0.6.0.tar", last modified: Mon Jul 31 06:53:53 2023, max compression
```

## Comparing `pytreeclass-0.5.0.post0.tar` & `pytreeclass-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.206432 pytreeclass-0.5.0.post0/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20927 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.206432 pytreeclass-0.5.0.post0/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:53.624274 pytreeclass-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-07-31 06:53:53.624274 pytreeclass-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:53.620274 pytreeclass-0.6.0/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:53.624274 pytreeclass-0.6.0/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/_src/tree_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/_src/tree_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28972 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:53.620274 pytreeclass-0.6.0/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21823 2023-07-31 06:53:53.000000 pytreeclass-0.6.0/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-31 06:53:53.000000 pytreeclass-0.6.0/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:53:53.000000 pytreeclass-0.6.0/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 06:53:53.000000 pytreeclass-0.6.0/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 06:53:53.000000 pytreeclass-0.6.0/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:53:53.624274 pytreeclass-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:53:53.624274 pytreeclass-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-31 06:53:35.000000 pytreeclass-0.6.0/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.5.0.post0/LICENSE` & `pytreeclass-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/README.md` & `pytreeclass-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/pyproject.toml` & `pytreeclass-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dynamic = ["version"]
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 description = "Visualize, create, and operate on JAX PyTree in the most intuitive way possible."
 authors = [{name = "Mahmoud Asem", email = "mahmoudasem00@gmail.com"}]
 keywords = ["jax", "neural-networks", "functional-programming", "machine-learning"]
 dependencies = ["jax>=0.4.7", "typing-extensions"]
+readme = "README.md"
 
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/__init__.py` & `pytreeclass-0.6.0/pytreeclass/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,12 +72,12 @@
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
     "Partial",
     "leafwise",
 )
 
-__version__ = "0.5.0post0"
+__version__ = "0.6.0"
 
 AtIndexer.__module__ = "pytreeclass"
 TreeClass.__module__ = "pytreeclass"
 Partial.__module__ = "pytreeclass"
```

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/_src/__init__.py` & `pytreeclass-0.6.0/pytreeclass/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/_src/code_build.py` & `pytreeclass-0.6.0/pytreeclass/_src/code_build.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,44 +16,59 @@
 
 from __future__ import annotations
 
 import functools as ft
 import sys
 from collections import defaultdict
 from collections.abc import Callable, MutableMapping, MutableSequence, MutableSet
-from types import FunctionType, MappingProxyType
+from types import MappingProxyType
 from typing import Any, Literal, Sequence, TypeVar, get_args
 
+import jax.tree_util as jtu
 from typing_extensions import dataclass_transform
 
 T = TypeVar("T")
 PyTree = Any
 EllipsisType = type(Ellipsis)
 ArgKindType = Literal["POS_ONLY", "POS_OR_KW", "VAR_POS", "KW_ONLY", "VAR_KW"]
 ArgKind = get_args(ArgKindType)
-NULL = type("NULL", (), {"__repr__": lambda _: "NULL"})()
-MUTABLE_TYPES = (MutableSequence, MutableMapping, MutableSet)
-# https://github.com/google/jax/issues/14295
+
+
+class Null:
+    __slots__ = ()
+
+    def __repr__(self) -> str:
+        return "NULL"
+
+
+NULL = Null()
+
+
+def slots(klass) -> tuple[str, ...]:
+    return getattr(klass, "__slots__", ())
 
 
 class Field:
+    """Field placeholder for `autoinit`."""
+
     __slots__ = [
         "name",
         "type",
         "default",
         "init",
         "repr",
         "kind",
         "metadata",
         "callbacks",
         "alias",
     ]
 
     def __init__(
         self,
+        *,
         name: str | None = None,
         type: type | None = None,
         default: Any = NULL,
         init: bool = True,
         repr: bool = True,
         kind: ArgKind = "POS_OR_KW",
         metadata: dict[str, Any] | None = None,
@@ -66,43 +81,50 @@
         self.init = init
         self.repr = repr
         self.kind = kind
         self.metadata = metadata
         self.callbacks = callbacks
         self.alias = alias
 
+    def replace(self, **kwargs) -> Field:
+        """Replace the field attributes."""
+        return type(self)(**{k: kwargs.get(k, getattr(self, k)) for k in slots(Field)})
+
     def __call__(self, value: Any):
-        """Call the callbacks on `value`."""
+        """Apply the callbacks on `value`."""
         for callback in self.callbacks:
             try:
                 value = callback(value)
             except Exception as e:
                 cname = getattr(callback, "__name__", callback)
                 raise type(e)(f"On applying {cname} for field=`{self.name}`:\n{e}")
         return value
 
-    def __repr__(self):
-        """Generate a string representation of the Field instance."""
-        return f"Field({', '.join(f'{k}={getattr(self, k)}' for k in self.__slots__)})"
-
-    def replace(self, **kwargs) -> "Field":
-        """Return a new Field instance with the given fields replaced."""
-        return Field(**{k: kwargs.get(k, getattr(self, k)) for k in self.__slots__})
-
-    def __get__(self, instance, owner):
-        if instance is None:
-            return self
-        return vars(instance)[self.name]
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({', '.join(f'{k}={getattr(self, k)!r}' for k in slots(Field))})"
 
-    def __set_name__(self, owner, name):
+    def __set_name__(self, _, name: str) -> None:
         self.name = name
 
-    def __set__(self, instance, value):
+    def __get__(self: T, instance, _) -> T | Any:
+        return self if instance is None else vars(instance)[self.name]
+
+    def __set__(self: T, instance, value) -> None:
         vars(instance)[self.name] = self(value)
 
+    def __delete__(self: T, instance) -> None:
+        del vars(instance)[self.name]
+
+
+jtu.register_pytree_node(
+    nodetype=Field,
+    flatten_func=lambda field: ((), {k: getattr(field, k) for k in slots(Field)}),
+    unflatten_func=lambda data, _: Field(**data),
+)
+
 
 def field(
     *,
     default: Any = NULL,
     init: bool = True,
     repr: bool = True,
     kind: ArgKindType = "POS_OR_KW",
@@ -112,20 +134,28 @@
 ) -> Field:
     """Field placeholder for type hinted attributes.
 
     Args:
         default: The default value of the field.
         init: Whether the field is included in the object's ``__init__`` function.
         repr: Whether the field is included in the object's ``__repr__`` function.
-        kind: Argument kind, one of: ``POS_ONLY``, ``VAR_POS``, ``POS_OR_KW`` ,
-            ``KW_ONLY``, ``VAR_KW``
+        kind: Argument kind, one of:
+
+            - ``POS_ONLY``: positional only argument (e.g. ``x`` in ``def f(x, /):``)
+            - ``VAR_POS``: variable positional argument (e.g. ``*x`` in ``def f(*x):``)
+            - ``POS_OR_KW``: positional or keyword argument (e.g. ``x`` in ``def f(x):``)
+            - ``KW_ONLY``: keyword only argument (e.g. ``x`` in ``def f(*, x):``)
+            - ``VAR_KW``: variable keyword argument (e.g. ``**x`` in ``def f(**x):``)
+
         metadata: A mapping of user-defined data for the field.
         callbacks: A sequence of functions to called on ``__setattr__`` during
             initialization to modify the field value.
-        alias: An a alias for the field name in the constructor.
+        alias: An a alias for the field name in the constructor. e.g ``name=x``,
+            ``alias=y`` will allow ``obj = Class(y=1)`` to be equivalent to
+            ``obj = Class(x=1)``.
 
     Example:
         >>> import pytreeclass as pytc
         >>> @pytc.autoinit
         ... class IsInstance(pytc.TreeClass):
         ...    klass: type
         ...    def __call__(self, x):
@@ -173,92 +203,101 @@
         metadata=metadata,  # type: ignore
         callbacks=callbacks,
         alias=alias,
     )
 
 
 @ft.lru_cache(maxsize=128)
-def _build_field_map(klass: type) -> MappingProxyType[str, Field]:
+def build_field_map(klass: type) -> MappingProxyType[str, Field]:
     field_map: dict[str, Field] = dict()
 
     if klass is object:
         return MappingProxyType(field_map)
 
     for base in reversed(klass.__mro__[1:]):
-        field_map.update(_build_field_map(base))
+        field_map.update(build_field_map(base))
 
-    # TODO: use inspect to get annotations, once min python version >3.9
-    if "__annotations__" not in vars(klass):
+    if (hint_map := vars(klass).get("__annotations__", NULL)) is NULL:
         return MappingProxyType(field_map)
 
-    for name in (annotation_map := vars(klass)["__annotations__"]):
-        value = vars(klass).get(name, NULL)
-        hint = annotation_map[name]
-
-        if name == "self":
-            # while `dataclasses` allows `self` as a field name, its confusing
-            # and not recommended. so raise an error
-            raise ValueError("Field name cannot be `self`.")
-
-        if isinstance(value, Field):
-            if isinstance(value.default, MUTABLE_TYPES):
-                # example case: `x: Any = field(default=[1, 2, 3])`
-                raise TypeError(f"Mutable {value.default=} is not allowed.")
-            # case: `x: Any = field(default=1)`
-            field_map[name] = value.replace(name=name, type=hint)
-        else:
-            if isinstance(value, MUTABLE_TYPES):
-                # example case: `x: Any = [1, 2, 3]`
-                raise TypeError(f"Mutable {value=} is not allowed")
-            # case: `x: int = 1` or `x: Any`
-            field_map[name] = Field(name=name, type=hint, default=value)
+    if "self" in hint_map:
+        raise ValueError("`Field` name cannot be `self`.")
+
+    for key, hint in hint_map.items():
+        # get the current base key
+        value = vars(klass).get(key, NULL)
+
+        if not isinstance(value, Field):
+            # non-`Field` annotation is ignored
+            # non-autoinit base class type hints are ignored
+            continue
+
+        if isinstance(value.default, (MutableSequence, MutableMapping, MutableSet)):
+            # https://github.com/google/jax/issues/14295
+            # example case: `x: Any = field(default=[1, 2, 3])`
+            raise TypeError(f"Mutable {value.default=} is not allowed.")
+
+        # case: `x: Any = field(default=1)`
+        field_map[key] = value.replace(name=key, type=hint)
+
     return MappingProxyType(field_map)
 
 
-def fields(x: Any) -> Sequence[Field]:
+def fields(x: Any) -> tuple[Field, ...]:
     """Returns a tuple of ``Field`` objects for the given instance or class.
 
     ``Field`` objects are generated from the class type hints and contains
     the information about the field information.if the user uses
     the ``pytreeclass.field`` to annotate.
 
     Note:
         - If the class is not annotated, an empty tuple is returned.
         - The ``Field`` generation is cached for class and its bases.
     """
-    return tuple(_build_field_map(x if isinstance(x, type) else type(x)).values())
+    return tuple(build_field_map(x if isinstance(x, type) else type(x)).values())
 
 
-def _build_init_method(klass: type) -> FunctionType:
+def convert_hints_to_fields(klass: type[T]) -> type[T]:
+    # convert klass hints to `Field` objects for the current decorated class
+    if (hint_map := vars(klass).get("__annotations__", NULL)) is NULL:
+        return klass
+
+    for key, hint in hint_map.items():
+        if not isinstance(value := vars(klass).get(key, NULL), Field):
+            setattr(klass, key, Field(default=value, type=hint, name=key))
+    return klass
+
+
+def build_init_method(klass: type[T]) -> type[T]:
     # generate a code object for the __init__ method and compile it
     # for the given class and return the function object
     body: list[str] = []
     hints: dict[str, str | type | None] = dict()
     head = ["self"]
     heads: dict[str, list[str]] = defaultdict(list)
     has_post = "__post_init__" in vars(klass)
 
     seen = set()
 
-    for field in (field_map := _build_field_map(klass)).values():
-        dref = "" if field.default is NULL else f"=field_map['{field.name}'].default"
+    for field in (field_map := build_field_map(klass)).values():
+        default = "" if field.default is NULL else f"=field_map['{field.name}'].default"
 
         if field.init:
             if field.kind in ("VAR_POS", "VAR_KW"):
                 # disallow multiple `VAR_POS` and `VAR_KW`
                 if field.kind in seen:
                     raise TypeError(f"Duplicate {field.kind=} for {field.name=}")
                 seen.add(field.kind)
 
             alias = field.alias or field.name
             hints[field.name] = field.type
             body += [f"self.{field.name}={alias}"]
-            heads[field.kind] += [f"{alias}{dref}"]
+            heads[field.kind] += [f"{alias}{default}"]
         else:
-            body += [f"self.{field.name}{dref}"]
+            body += [f"self.{field.name}{default}"]
 
     hints["return"] = None
     # add the post init call if the class has it, otherwise add a pass
     # in case all fields are not initialized in the __init__ method
     body += ["self.__post_init__()"] if has_post else ["pass"]
 
     # organize the arguments order:
@@ -276,15 +315,16 @@
     code += f"\tdef __init__({','.join(head)}):"
     code += f"\n\t\t{';'.join(body)}"
     code += f"\n\t__init__.__qualname__ = '{klass.__qualname__}.__init__'"
     code += "\n\treturn __init__"
 
     exec(code, vars(sys.modules[klass.__module__]), namespace := dict())
     setattr(init := namespace["closure"](field_map), "__annotations__", hints)
-    return init
+    setattr(klass, "__init__", init)
+    return klass
 
 
 @dataclass_transform(field_specifiers=(Field, field))
 def autoinit(klass: type[T]) -> type[T]:
     """A class decorator that generates the ``__init__`` method from type hints.
 
     Similar to ``dataclasses.dataclass``, this decorator generates the ``__init__``
@@ -310,16 +350,59 @@
         >>> import pytreeclass as pytc
         >>> @pytc.autoinit
         ... class Tree:
         ...     kw_only_field: int = pytc.field(default=1, kind="KW_ONLY")
         ...     pos_only_field: int = pytc.field(default=2, kind="POS_ONLY")
 
     Example:
-        >>> # define a validator to apply ``abs`` on the field value
+        >>> # define a converter to apply ``abs`` on the field value
         >>> @pytc.autoinit
         ... class Tree:
         ...     a:int = pytc.field(callbacks=[abs])
         >>> Tree(a=-1).a
         1
+
+    .. warning::
+        - The ``autoinit`` decorator will is no-op if the class already has a
+          user-defined ``__init__`` method.
+
+    Note:
+        - In case of inheritance, the ``__init__`` method is generated from the
+          the type hints of the current class and any base classes that
+          are decorated with ``autoinit``.
+
+        >>> import pytreeclass as pytc
+        >>> import inspect
+        >>> @pytc.autoinit
+        ... class Base:
+        ...     x: int
+        >>> @pytc.autoinit
+        ... class Derived(Base):
+        ...     y: int
+        >>> obj = Derived(x=1, y=2)
+        >>> inspect.signature(obj.__init__)
+        <Signature (x: int, y: int) -> None>
+
+        - Base classes that are not decorated with ``autoinit`` are ignored during
+          synthesis of the ``__init__`` method.
+
+        >>> import pytreeclass as pytc
+        >>> import inspect
+        >>> class Base:
+        ...     x: int
+        >>> @pytc.autoinit
+        ... class Derived(Base):
+        ...     y: int
+        >>> obj = Derived(y=2)
+        >>> inspect.signature(obj.__init__)
+        <Signature (y: int) -> None>
     """
-    klass.__init__ = _build_init_method(klass)
-    return klass
+    return (
+        klass
+        # if the class already has a user-defined __init__ method
+        # then return the class as is without any modification
+        if "__init__" in vars(klass)
+        # first convert the current class hints to fields
+        # then build the __init__ method from the fields of the current class
+        # and any base classes that are decorated with `autoinit`
+        else build_init_method(convert_hints_to_fields(klass))
+    )
```

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_base.py` & `pytreeclass-0.6.0/pytreeclass/_src/tree_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 """Define a class that convert a class to a JAX compatible tree structure."""
 
 from __future__ import annotations
 
 import abc
-from contextlib import contextmanager
 from typing import Any, Hashable, TypeVar
 
 import jax
 import jax.tree_util as jtu
 from typing_extensions import Unpack
 
 from pytreeclass._src.code_build import fields
@@ -43,27 +42,32 @@
 
 T = TypeVar("T", bound=Hashable)
 S = TypeVar("S")
 PyTree = Any
 EllipsisType = type(Ellipsis)
 
 
-# allow methods in mutable context to be called without raising `AttributeError`
-# the instances are registered  during initialization and using `at`  property
-# with `__call__` this is done by registering the instance id in a set before
-# entering the mutable context and removing it after exiting the context
+# allow methods in mutable registry to be called without raising `AttributeError`
 _mutable_instance_registry: set[int] = set()
 
 
-@contextmanager
-def _mutable_context(tree, *, kopy: bool = False):
-    tree = tree_copy(tree) if kopy else tree
-    _mutable_instance_registry.add(id(tree))
-    yield tree
-    _mutable_instance_registry.discard(id(tree))
+def add_mutable_entry(node) -> None:
+    _mutable_instance_registry.add(id(node))
+
+
+def discard_mutable_entry(node) -> None:
+    _mutable_instance_registry.discard(id(node))
+
+
+def recursive_getattr(tree: Any, where: tuple[str, ...]):
+    if not isinstance(where[0], str):
+        raise TypeError(f"Expected string, got {type(where[0])!r}.")
+    if len(where) == 1:
+        return getattr(tree, where[0])
+    return recursive_getattr(getattr(tree, where[0]), where[1:])
 
 
 class TreeClassIndexer(AtIndexer):
     def __call__(self, *a, **k) -> tuple[Any, PyTree]:
         """Call a method on the tree instance and return result and new instance.
 
         Returns:
@@ -84,50 +88,46 @@
             >>> tree.at['add'](99)
             (100, Tree(a=100))
 
         Note:
             - `AttributeError` is raised, If the function mutates the instance.
             - Use .at["method_name"](*, **) to call a method that mutates the instance.
         """
-
-        def recursive_getattr(tree: Any, where: tuple[str, ...]):
-            if not isinstance(where[0], str):
-                raise TypeError(f"Expected string, got {type(where[0])!r}.")
-            if len(where) == 1:
-                return getattr(tree, where[0])
-            return recursive_getattr(getattr(tree, where[0]), where[1:])
-
-        with _mutable_context(self.tree, kopy=True) as tree:
-            value = recursive_getattr(tree, self.where)(*a, **k)  # type: ignore
+        tree = tree_copy(self.tree)
+        jtu.tree_map(lambda _: _, tree, is_leaf=add_mutable_entry)
+        value = recursive_getattr(tree, self.where)(*a, **k)  # type: ignore
+        jtu.tree_map(lambda _: _, tree, is_leaf=discard_mutable_entry)
         return value, tree
 
 
 class TreeClassMeta(abc.ABCMeta):
     def __call__(klass: type[T], *a, **k) -> T:
-        with _mutable_context(self := getattr(klass, "__new__")(klass, *a, **k)):
-            getattr(klass, "__init__")(self, *a, **k)
-        return self
+        tree = getattr(klass, "__new__")(klass, *a, **k)
+        add_mutable_entry(tree)
+        getattr(klass, "__init__")(tree, *a, **k)
+        discard_mutable_entry(tree)
+        return tree
 
 
 class TreeClass(metaclass=TreeClassMeta):
-    """Convert a class to a JAX compatible tree structure.
+    """Convert a class to a ``jax``-compatible pytree.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> # Tree leaves are instance attributes
         >>> @pytc.autoinit
         ... class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> jax.tree_util.tree_leaves(tree)
         [1, 2.0]
 
-        >>> # Leaf-wise math operations are supported by setting `leafwise=True`
+        >>> # Leaf-wise math operations are supported  using `leafwise` decorator
         >>> @pytc.leafwise
         ... @pytc.autoinit
         ... class Tree(pytc.TreeClass):
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree + 1
@@ -139,14 +139,47 @@
         ...     a:int = 1
         ...     b:float = 2.0
         >>> tree = Tree()
         >>> tree.at["a"].get()
         Tree(a=1, b=None)
         >>> tree.at[0].get()
         Tree(a=1, b=None)
+
+    Note:
+        - Under ``jax.tree_util.***`` all :class:`.TreeClass` attributes are
+          treated as leaves.
+        - To hide/ignore a specific attribute from the tree leaves, during
+          ``jax.tree_util.***`` operations, freeze the leaf using :func:`.freeze`
+          or :func:`.tree_mask`.
+
+        >>> # freeze(exclude) a leaf from the tree leaves:
+        >>> import jax
+        >>> import pytreeclass as pytc
+        >>> @pytc.autoinit
+        ... class Tree(pytc.TreeClass):
+        ...     a:int = 1
+        ...     b:float = 2.0
+        >>> tree = Tree()
+        >>> tree = tree.at["a"].apply(pytc.freeze)
+        >>> jax.tree_util.tree_leaves(tree)
+        [2.0]
+
+        >>> # undo the freeze
+        >>> tree = tree.at["a"].apply(pytc.unfreeze, is_leaf=pytc.is_frozen)
+        >>> jax.tree_util.tree_leaves(tree)
+        [1, 2.0]
+
+        >>> # using `tree_mask` to exclude a leaf from the tree leaves
+        >>> freeze_mask = Tree(a=True, b=False)
+        >>> jax.tree_util.tree_leaves(pytc.tree_mask(tree, freeze_mask))
+        [2.0]
+
+    Note:
+        - :class:`.TreeClass` inherits from ``abc.ABC`` so ``@abstract...`` decorators
+          can be used to define abstract behavior.
     """
 
     def __init_subclass__(klass: type[T], **k):
         if "__setattr__" in vars(klass):
             raise TypeError(f"Reserved methods: `__setattr__` defined in `{klass}`.")
         if "__delattr__" in vars(klass):
             raise TypeError(f"Reserved methods: `__delattr__` defined in `{klass}`.")
```

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_index.py` & `pytreeclass-0.6.0/pytreeclass/_src/tree_index.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_mask.py` & `pytreeclass-0.6.0/pytreeclass/_src/tree_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,22 +126,22 @@
             return False
         if lhs.dtype != rhs.dtype:
             return False
         return np.all(lhs == rhs)
 
 
 def freeze(value: T) -> _FrozenHashable[T]:
-    """Freeze a value to avoid updating it by `jax` transformations.
+    """Freeze a value to avoid updating it by ``jax`` transformations.
 
     Args:
         value: A value to freeze.
 
     Note:
-        - ``freeze`` is idempotent, i.e. ``freeze(freeze(x)) == freeze(x)``.
-        - ``freeze`` uses single dispatch to support custom types. To define a custom
+        - :func:`.freeze` is idempotent, i.e. ``freeze(freeze(x)) == freeze(x)``.
+        - :func:`.freeze` uses single dispatch to support custom types. To define a custom
           wrapper for a certain type, use ``freeze.def_type(type, func)``.
 
     Example:
         >>> import jax
         >>> import pytreeclass as pytc
         >>> import jax.tree_util as jtu
         >>> # Usage with `jax.tree_util.tree_leaves`
@@ -180,23 +180,23 @@
 
 def is_frozen(value: Any) -> bool:
     """Returns True if the value is a frozen wrapper."""
     return isinstance(value, _FrozenBase)
 
 
 def unfreeze(value: T) -> T:
-    """Unfreeze `frozen` value, otherwise return the value itself.
+    """Unfreeze :func:`.freeze` value, otherwise return the value itself.
 
     Args:
         value: A value to unfreeze.
 
     Note:
-        - use `is_leaf=pytc.is_frozen` with `jax.tree_map` to unfreeze a tree.**
-        - `unfreeze` uses single dispatch to support custom types. To define a custom
-          behavior for a certain type, use `unfreeze.def_type(type, func)`.
+        - use ``is_leaf=pytc.is_frozen`` with ``jax.tree_map`` to unfreeze a tree.**
+        - :func:`.unfreeze` uses single dispatch to support custom types. To define a custom
+          behavior for a certain type, use ``unfreeze.def_type(type, func)``.
 
     Example:
         >>> import pytreeclass as pytc
         >>> import jax
         >>> frozen_value = pytc.freeze(1)
         >>> pytc.unfreeze(frozen_value)
         1
@@ -221,34 +221,34 @@
 def is_nondiff(value: Any) -> bool:
     """Returns True for non-inexact types, False otherwise.
 
     Args:
         value: A value to check.
 
     Note:
-        - `is_nondiff` uses single dispatch to support custom types. To define a custom
-          behavior for a certain type, use `is_nondiff.def_type(type, func)`.
+        - :func:`.is_nondiff` uses single dispatch to support custom types. To define
+          a custom behavior for a certain type, use ``is_nondiff.def_type(type, func)``.
 
     Example:
         >>> import pytreeclass as pytc
         >>> import jax.numpy as jnp
         >>> pytc.is_nondiff(jnp.array(1))  # int array is non-diff type
         True
         >>> pytc.is_nondiff(jnp.array(1.))  # float array is diff type
         False
         >>> pytc.is_nondiff(1)  # int is non-diff type
         True
         >>> pytc.is_nondiff(1.)  # float is diff type
         False
 
     Note:
-        This function is meant to be used with `jax.tree_map` to
+        This function is meant to be used with ``jax.tree_map`` to
         create a mask for non-differentiable nodes in a tree, that can be used
         to freeze the non-differentiable nodes before passing the tree to a
-        `jax` transformation.
+        ``jax`` transformation.
     """
     return is_nondiff.type_dispatcher(value)
 
 
 is_nondiff.type_dispatcher = ft.singledispatch(lambda x: True)
 is_nondiff.def_type = is_nondiff.type_dispatcher.register
 
@@ -296,33 +296,33 @@
         f"`mask` must be a callable that accepts a leaf a returns a boolean "
         f"or a tree with the same structure as tree with boolean values."
         f" Got {mask=} and {tree=}."
     )
 
 
 def tree_mask(tree: T, mask: MaskType = is_nondiff, *, is_leaf: IsLeafType = None):
-    """Mask leaves of a pytree based on `mask` boolean pytree or callable.
+    """Mask leaves of a pytree based on ``mask`` boolean pytree or callable.
 
     Args:
         tree: A pytree of values.
         mask: A pytree of boolean values or a callable that accepts a leaf and
-            returns a boolean. If a leaf is `True` either in the mask or the
+            returns a boolean. If a leaf is ``True`` either in the mask or the
             callable, the leaf is wrapped by with a wrapper that yields no
-            leaves when `jax.tree_util.tree_flatten` is called on it, otherwise
-            it is unchanged. defaults to `is_nondiff` which returns true for
+            leaves when ``jax.tree_util.tree_flatten`` is called on it, otherwise
+            it is unchanged. defaults to :func:`.is_nondiff` which returns true for
             non-differentiable nodes.
         is_leaf: A callable that accepts a leaf and returns a boolean. If
             provided, it is used to determine if a value is a leaf. for example,
-            `is_leaf=lambda x: isinstance(x, list)` will treat lists as leaves
+            ``is_leaf=lambda x: isinstance(x, list)`` will treat lists as leaves
             and will not recurse into them.
 
     Note:
         - Masked leaves are wrapped with a wrapper that yields no leaves when
           ``jax.tree_util.tree_flatten`` is called on it.
-        - Masking is equivalent to applying `freeze` to the masked leaves.
+        - Masking is equivalent to applying :func:`.freeze` to the masked leaves.
 
             >>> import pytreeclass as pytc
             >>> import jax
             >>> tree = [1, 2, {"a": 3, "b": 4.}]
             >>> # mask all non-differentiable nodes by default
             >>> def mask_if_nondiff(x):
             ...     return pytc.freeze(x) if pytc.is_nondiff(x) else x
@@ -355,15 +355,15 @@
         >>> square(pytc.tree_mask(tree))
         (Array(2., dtype=float32, weak_type=True), #2)
     """
     return _tree_mask_map(tree, mask=mask, func=freeze, is_leaf=is_leaf)
 
 
 def tree_unmask(tree: T, mask: MaskType = lambda _: True):
-    """Undo the masking of tree leaves according to `mask`. defaults to unmasking all leaves.
+    """Undo the masking of tree leaves according to ``mask``. defaults to unmasking all leaves.
 
     Args:
         tree: A pytree of values.
         mask: A pytree of boolean values or a callable that accepts a leaf and
             returns a boolean. If a leaf is True either in the mask or the
             callable, the leaf is unfrozen, otherwise it is unchanged. defaults
             unmasking all nodes.
@@ -389,15 +389,15 @@
         ...     tree = pytc.tree_unmask(tree)
         ...     return tree[0]**2
         >>> tree = (1., 2)  # contains a non-differentiable node
         >>> square(pytc.tree_mask(tree))
         (Array(2., dtype=float32, weak_type=True), #2)
 
     Note:
-        - Unmasking is equivalent to applying ``unfreeze`` on the masked leaves.
+        - Unmasking is equivalent to applying :func:`.unfreeze` on the masked leaves.
 
             >>> import pytreeclass as pytc
             >>> import jax
             >>> tree = [1, 2, {"a": 3, "b": 4.}]
             >>> # unmask all nodes
             >>> tree = jax.tree_map(pytc.unfreeze, tree, is_leaf=pytc.is_frozen)
     """
```

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.6.0/pytreeclass/_src/tree_pprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 def tree_repr(
     tree: PyTree,
     *,
     width: int = 80,
     tabwidth: int = 2,
     depth: int | float = float("inf"),
 ) -> str:
-    """Prertty print arbitrary pytrees `__repr__`.
+    """Prertty print arbitrary pytrees ``__repr__``.
 
     Args:
         tree: arbitrary pytree.
         width: max width of the repr string.
         tabwidth: tab width of the repr string.
         depth: max depth of the repr string.
 
@@ -261,15 +261,15 @@
 def tree_str(
     tree: PyTree,
     *,
     width: int = 80,
     tabwidth: int = 2,
     depth: int | float = float("inf"),
 ) -> str:
-    """Prertty print arbitrary pytrees `__str__`.
+    """Prertty print arbitrary pytrees ``__str__``.
 
     Args:
         tree: arbitrary pytree.
         width: max width of the str string.
         tabwidth: tab width of the repr string.
         depth: max depth of the repr string.
 
@@ -316,17 +316,17 @@
         is_leaf: function to determine if a node is a leaf. default is None.
         tabwidth: tab width of the repr string. default is 4.
 
     Example:
         >>> import pytreeclass as pytc
         >>> @pytc.autoinit
         ... class A(pytc.TreeClass):
-        ...        x: int = 10
-        ...        y: int = (20,30)
-        ...        z: int = 40
+        ...     x: int = 10
+        ...     y: int = (20,30)
+        ...     z: int = 40
 
         >>> @pytc.autoinit
         ... class B(pytc.TreeClass):
         ...     a: int = 10
         ...     b: tuple = (20,30, A())
 
         >>> print(pytc.tree_diagram(B(), depth=0))
@@ -600,15 +600,15 @@
 
 def tree_summary(
     tree: PyTree,
     *,
     depth: int | float = float("inf"),
     is_leaf: IsLeafType = None,
 ) -> str:
-    """Print a summary of an arbitrary PyTree.
+    """Print a summary of an arbitrary pytree.
 
     Args:
         tree: a jax registered pytree to summarize.
         depth: max depth to display the tree. defaults to maximum depth.
         is_leaf: function to determine if a node is a leaf. defaults to None
 
     Returns:
```

### Comparing `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_util.py` & `pytreeclass-0.6.0/pytreeclass/_src/tree_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Utility functions for pytrees."""
 
 from __future__ import annotations
 
 import dataclasses as dc
 import functools as ft
 import operator as op
+from copy import copy
 from math import ceil, floor, trunc
 from typing import Any, Callable, Hashable, Iterator, Sequence, Tuple, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from jax._src.tree_util import _registry, _registry_with_keypaths
@@ -53,15 +54,15 @@
 def tree_hash(*trees: PyTree) -> int:
     leaves, treedef = jtu.tree_flatten(trees)
     return hash((*leaves, treedef))
 
 
 def tree_copy(tree: T) -> T:
     """Return a copy of the tree."""
-    return jtu.tree_unflatten(*jtu.tree_flatten(tree)[::-1])
+    return jax.tree_map(lambda x: copy(x), tree)
 
 
 def _is_leaf_rhs_equal(leaf, rhs) -> bool | jax.Array:
     if hasattr(leaf, "shape") and hasattr(leaf, "dtype"):
         if hasattr(rhs, "shape") and hasattr(rhs, "dtype"):
             if leaf.shape != rhs.shape:
                 return False
@@ -93,15 +94,15 @@
         if (treedef != treedef0) or verdict is False:
             return False
         verdict = ft.reduce(op.and_, map(_is_leaf_rhs_equal, leaves0, leaves), verdict)
     return verdict
 
 
 class Partial:
-    """jaxable Partial function with support for positional partial application.
+    """``jax``-able ``Partial`` function with support for positional partial application.
 
     Example:
         >>> import pytreeclass as pytc
         >>> def f(a, b, c):
         ...     print(f"a: {a}, b: {b}, c: {c}")
         ...     return a + b + c
 
@@ -116,22 +117,22 @@
         >>> f_a(1)
         a: 1, b: 2, c: 3
         6
 
     Note:
         - The ``...`` is used to indicate a placeholder for positional arguments.
         - See: https://stackoverflow.com/a/7811270
-        - `Partial` is used internally by `bcmap` which maps a function over pytrees
-          leaves with automatic broadcasting for scalar arguments.
+        - :func:`.Partial` is used internally by :func:`.bcmap` which maps a
+          function over pytrees leaves with automatic broadcasting for scalar arguments.
     """
 
     __slots__ = ["func", "args", "kwargs", "__weakref__"]  # type: ignore
 
     def __init__(self, func: Callable[..., Any], *args: Any, **kwargs: Any):
-        """Initialize a `Partial` function.
+        """Initialize a ``Partial`` function.
 
         Args:
             func: The function to be partially applied.
             args: Positional arguments to be partially applied. use ``...`` as a
                 placeholder for positional arguments.
             kwargs: Keyword arguments to be partially applied.
         """
```

### Comparing `pytreeclass-0.5.0.post0/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.6.0/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/tests/test_indexing.py` & `pytreeclass-0.6.0/tests/test_indexing.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 
 import pytreeclass as pytc
 from pytreeclass import TreeClass
-from pytreeclass._src.tree_base import _mutable_context
+from pytreeclass._src.tree_base import add_mutable_entry, discard_mutable_entry
 from pytreeclass._src.tree_util import construct_tree
 
 
 @pytc.leafwise
 @pytc.autoinit
 class Tree(TreeClass):
     a: float
@@ -730,16 +730,17 @@
         a: int = 1
 
         def delete(self, name):
             del self.a
 
     t = L2()
 
-    with _mutable_context(t) as tx:
-        tx.delete("a")
+    add_mutable_entry(t)
+    t.delete("a")
+    discard_mutable_entry(t)
 
     with pytest.raises(AttributeError):
         t.delete("a")
 
 
 def test_unsupported_indexing_type():
     @pytc.leafwise
@@ -875,7 +876,34 @@
     def func_with_state(x, state):
         return x + 1, state + 1
 
     tree, state = tree.at["a", "b", "d"].scan(func_with_state, state=1)
 
     assert pytc.is_tree_equal(tree, Tree(a=2, b=3, c=3, d=jnp.array([5, 6])))
     assert state == 4
+
+
+def test_dispatch():
+    @jtu.register_pytree_with_keys_class
+    class T:
+        def __init__(self, a, b):
+            self.a = a
+            self.b = b
+
+        def tree_flatten_with_keys(self):
+            ka = ("a", self.a)
+            kb = (2, self.b)
+            return [ka, kb], None
+
+        @classmethod
+        def tree_unflatten(cls, aux_data, children):
+            return cls(*children)
+
+    t = T(1, 2)
+    assert pytc.AtIndexer(t)["a"].get().a == 1
+    assert pytc.AtIndexer(t)["a"].get().b is None
+
+    assert pytc.AtIndexer(t)[2].get().a is None
+    assert pytc.AtIndexer(t)[2].get().b == 2
+
+    assert pytc.AtIndexer(t)[re.compile("a")].get().a == 1
+    assert pytc.AtIndexer(t)[re.compile("a")].get().b is None
```

### Comparing `pytreeclass-0.5.0.post0/tests/test_nn.py` & `pytreeclass-0.6.0/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/tests/test_tree_freeze.py` & `pytreeclass-0.6.0/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/tests/test_tree_operator.py` & `pytreeclass-0.6.0/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/tests/test_tree_pprint.py` & `pytreeclass-0.6.0/tests/test_tree_pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     e: list = None
     f: set = None
     g: dict = None
     h: jnp.ndarray = None
     i: jnp.ndarray = None
     j: jnp.ndarray = None
     k: tuple = pytc.field(repr=False, default=(1, 2, 3))
-    l: namedtuple = namedtuple("a", ["b", "c"])(1, 2)
+    l: tuple = namedtuple("a", ["b", "c"])(1, 2)
     m: jnp.array = jnp.ones((5, 5))
     n: jnp.array = jnp.array(True)
     o: jnp.array = jnp.array([1, 2.0], dtype=jnp.complex64)
 
     def __post_init__(self):
         self.h = jnp.ones((5, 1))
         self.i = jnp.ones((1, 6))
```

### Comparing `pytreeclass-0.5.0.post0/tests/test_tree_viz_util.py` & `pytreeclass-0.6.0/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0.post0/tests/test_treeclass.py` & `pytreeclass-0.6.0/tests/test_treeclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,28 +20,34 @@
 import jax
 import jax.tree_util as jtu
 import numpy.testing as npt
 import pytest
 from jax import numpy as jnp
 
 import pytreeclass as pytc
+from pytreeclass._src.code_build import build_field_map, convert_hints_to_fields
 
 
 def test_fields():
     @pytc.autoinit
     class Test(pytc.TreeClass):
         a: int = pytc.field(default=1, metadata={"meta": 1})
         b: int = 2
 
     assert len(pytc.fields(Test)) == 2
     assert pytc.fields(Test)[0].metadata == {"meta": 1}
 
     with pytest.raises(ValueError):
         pytc.field(kind="WRONG")
 
+    assert (
+        repr(pytc.field(kind="KW_ONLY"))
+        == "Field(name=None, type=None, default=NULL, init=True, repr=True, kind='KW_ONLY', metadata=None, callbacks=(), alias=None)"
+    )
+
 
 def test_field():
     assert pytc.field(default=1).default == 1
 
     with pytest.raises(TypeError):
         pytc.field(metadata=1)
 
@@ -595,7 +601,57 @@
         def __init_subclass__(cls, hello):
             cls.hello = hello
 
     class Test2(pytc.TreeClass, Test, hello=1):
         ...
 
     assert Test2.hello == 1
+
+
+def test_nested_mutation():
+    @pytc.autoinit
+    class InnerModule(pytc.TreeClass):
+        a: int = 1
+
+        def f(self):
+            self.a += 1
+            return self.a
+
+    @pytc.autoinit
+    class OuterModule(pytc.TreeClass):
+        inner: InnerModule = InnerModule()
+
+        def ff(self):
+            return self.inner.f()
+
+        def df(self):
+            del self.inner.a
+
+    _, v = OuterModule().at["ff"]()
+    assert v.inner.a == 2
+
+    _, v = OuterModule().at["df"]()
+    assert "a" not in v.inner.__dict__
+
+
+def test_autoinit_and_user_defined_init():
+    @pytc.autoinit
+    class Tree(pytc.TreeClass):
+        b: int
+
+        def __init__(self, a):
+            self.a = a
+
+    Tree(a=1)
+
+    assert True
+
+
+def test_nohints():
+    assert convert_hints_to_fields(int) is int
+
+
+def non_field_builder():
+    class T:
+        ...
+
+    assert dict(build_field_map(T)) == {}
```

### Comparing `pytreeclass-0.5.0.post0/tests/test_under_jit.py` & `pytreeclass-0.6.0/tests/test_under_jit.py`

 * *Files identical despite different names*

