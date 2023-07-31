# Comparing `tmp/machinable-4.4.0.tar.gz` & `tmp/machinable-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machinable-4.4.0.tar", max compression
+gzip compressed data, was "machinable-4.5.0.tar", max compression
```

## Comparing `machinable-4.4.0.tar` & `machinable-4.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1245 2023-06-21 04:47:12.751073 machinable-4.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2023-06-21 04:47:12.751073 machinable-4.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1135 2023-06-21 04:47:12.751073 machinable-4.4.0/README.md
--rw-r--r--   0        0        0     2137 2023-06-21 04:47:12.755073 machinable-4.4.0/pyproject.toml
--rw-r--r--   0        0        0     1356 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/__init__.py
--rw-r--r--   0        0        0     3137 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/cli.py
--rw-r--r--   0        0        0    37541 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/collection.py
--rw-r--r--   0        0        0     8576 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/component.py
--rw-r--r--   0        0        0     2933 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/config.py
--rw-r--r--   0        0        0    22767 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/element.py
--rw-r--r--   0        0        0      615 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/errors.py
--rw-r--r--   0        0        0    14141 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/execution.py
--rw-r--r--   0        0        0     1596 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/group.py
--rw-r--r--   0        0        0     8877 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/index.py
--rw-r--r--   0        0        0    13936 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/interface.py
--rw-r--r--   0        0        0     2480 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/mixin.py
--rw-r--r--   0        0        0    10835 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/project.py
--rw-r--r--   0        0        0       10 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/py.typed
--rw-r--r--   0        0        0      630 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/schedule.py
--rw-r--r--   0        0        0     1349 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/schema.py
--rw-r--r--   0        0        0      952 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/settings.py
--rw-r--r--   0        0        0     1041 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/storage.py
--rw-r--r--   0        0        0      359 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/types.py
--rw-r--r--   0        0        0    16651 2023-06-21 04:47:12.755073 machinable-4.4.0/src/machinable/utils.py
--rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 machinable-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1437 2023-07-31 18:16:02.004095 machinable-4.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2023-07-31 18:16:02.004095 machinable-4.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1135 2023-07-31 18:16:02.004095 machinable-4.5.0/README.md
+-rw-r--r--   0        0        0     2133 2023-07-31 18:16:02.008095 machinable-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1357 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/__init__.py
+-rw-r--r--   0        0        0     3137 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/cli.py
+-rw-r--r--   0        0        0    37182 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/collection.py
+-rw-r--r--   0        0        0     8542 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/component.py
+-rw-r--r--   0        0        0     3359 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/config.py
+-rw-r--r--   0        0        0    22416 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/element.py
+-rw-r--r--   0        0        0      615 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/errors.py
+-rw-r--r--   0        0        0    14158 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/execution.py
+-rw-r--r--   0        0        0     9794 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/index.py
+-rw-r--r--   0        0        0    13769 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/interface.py
+-rw-r--r--   0        0        0     2480 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/mixin.py
+-rw-r--r--   0        0        0    10729 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/project.py
+-rw-r--r--   0        0        0       10 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/py.typed
+-rw-r--r--   0        0        0      630 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/schedule.py
+-rw-r--r--   0        0        0     1299 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/schema.py
+-rw-r--r--   0        0        0      740 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/scope.py
+-rw-r--r--   0        0        0     1000 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/settings.py
+-rw-r--r--   0        0        0     1041 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/storage.py
+-rw-r--r--   0        0        0      359 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/types.py
+-rw-r--r--   0        0        0    16651 2023-07-31 18:16:02.008095 machinable-4.5.0/src/machinable/utils.py
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 machinable-4.5.0/PKG-INFO
```

### Comparing `machinable-4.4.0/CHANGELOG.md` & `machinable-4.5.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 <!-- Please add changes under the Unreleased section that reads 'No current changes' otherwise -->
 
 # Unreleased
 
 No current changes
 
+# v4.5.0
+
+- Adds scopes to support context annotations
+- Adds all() and new() interface query modifiers
+- Adds config `to_dict` helper
+- Gracefully end output streaming on keyboard interrupt
+
 # v4.4.0
 
 - Improved tracking of execution meta-data
 - Realiable `.execution` access to make None-checks obsolete
 - Adds `stream_output` to simplify live monitoring of execution logs
 - Allow predicate specification based on the element kind
 - Prevent index errors in multithreaded enviroments
```

### Comparing `machinable-4.4.0/LICENSE.txt` & `machinable-4.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/README.md` & `machinable-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/pyproject.toml` & `machinable-4.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "machinable"
-version = "4.4.0"
+version = "4.5.0"
 description = "A modular configuration system for research projects"
 license = "MIT"
 authors = [
     "Frithjof Gressmann <hello@machinable.org>"
 ]
 maintainers = [
     "Frithjof Gressmann <hello@machinable.org>"
@@ -22,27 +22,27 @@
 ]
 include = ["CHANGELOG.md", "src/machinable/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 flatten-dict = "^0.4"
 jsonlines = "^3.1"
-pydantic = "^1.10.8"
+pydantic = "1.*"
 arrow = "^1.2"
 importlib-metadata = {version = "^6.7", python = "<3.8"}
 omegaconf = "^2.3.0"
-dill = "^0.3.6"
-typing-extensions = {version = "^4.5.0", python = "<3.11"}
+dill = "^0.3.7"
+typing-extensions = {version = "^4.7.0", python = "<3.11"}
 
 
 [tool.poetry.dev-dependencies]
 isort = "^5.11.5"
 pyupgrade = "^3.3"
 black = "^23.3.0"
-pytest = "^7.3"
+pytest = "^7.4"
 pre-commit = "^2.21.0"
 editorconfig-checker = "^2.7.2"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 all = [
   "numpy",
```

### Comparing `machinable-4.4.0/src/machinable/__init__.py` & `machinable-4.5.0/src/machinable/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "Interface",
     "Execution",
     "Component",
     "Project",
     "Storage",
     "Mixin",
     "Index",
+    "Scope",
     "mixin",
     "Schedule",
     "get",
     "get_settings",
 ]
 __doc__ = """A modular system for machinable research code"""
 
@@ -27,26 +28,26 @@
 from machinable.element import Element
 from machinable.execution import Execution
 from machinable.index import Index
 from machinable.interface import Interface
 from machinable.mixin import Mixin, mixin
 from machinable.project import Project
 from machinable.schedule import Schedule
+from machinable.scope import Scope
 from machinable.settings import get_settings
 from machinable.storage import Storage
 from machinable.types import Optional, Union, VersionType
 
 
 def get(
     module: Union[str, Element, None] = None,
     version: VersionType = None,
-    predicate: Optional[str] = "$",
     **kwargs,
 ) -> Interface:
-    return Interface.get(module, version, predicate, **kwargs)
+    return Interface.get(module, version, **kwargs)
 
 
 def get_version() -> str:
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
         return "unknown"
```

### Comparing `machinable-4.4.0/src/machinable/cli.py` & `machinable-4.5.0/src/machinable/cli.py`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/src/machinable/collection.py` & `machinable-4.5.0/src/machinable/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1375,50 +1375,39 @@
         import pandas
 
         return pandas.DataFrame.from_dict(data)
 
     def filter_by_module(self, module):
         return self.filter(lambda x: x.module == module)
 
-    def filter_by_predicate(
+    def filter_by_context(
         self,
         module: str,
         version: VersionType = None,
-        predicate: str = "$",
         **kwargs,
     ):
         from machinable import Element
 
-        try:
-            instance = Element.make(module, version, **kwargs)
-        except ModuleNotFoundError:
-            from machinable.element import equalversion
-
-            # use direct comparison fallback
-            return self.filter(
-                lambda x: bool(
-                    x.module == module and equalversion(x.version(), version)
-                )
-            )
+        instance = Element.make(module, version, **kwargs)
 
-        return self.filter(lambda x: x.matches(instance, predicate))
+        return self.filter(lambda x: x.matches(instance))
 
     def singleton(
         self,
         module: str,
         version: VersionType = None,
-        predicate: str = "$",
         **kwargs,
     ) -> Union[Any, "Component"]:
         from machinable import Element
 
         instance = Element.make(module, version, **kwargs)
+        context = instance.compute_context()
 
         for candidate in self:
-            if candidate.matches(instance, predicate):
+            if candidate.matches(instance, context):
                 return candidate
 
         return instance
 
     def __str__(self):
         return f"Elements <{len(self.items)}>"
```

### Comparing `machinable-4.4.0/src/machinable/component.py` & `machinable-4.5.0/src/machinable/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,14 @@
         related.of(self)
 
         return related
 
     def launch(self) -> Self:
         from machinable.execution import Execution
 
-        self.execution.add(self)
-
         if Execution.is_connected():
             # commit only, defer execution
             Execution.get().add(self)
             self.commit()
         else:
             self.current_execution_context.add(self)
             self.current_execution_context.dispatch()
```

### Comparing `machinable-4.4.0/src/machinable/config.py` & `machinable-4.5.0/src/machinable/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = ["Field", "validator", "RequiredField", "Model"]
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Union
 
 import collections
 import re
 from inspect import isclass
 
+import omegaconf
 from pydantic import BaseModel as Model
 from pydantic import Field
 from pydantic import validator as _validator
 from pydantic.dataclasses import dataclass
 from pydantic.typing import AnyCallable
 
 if TYPE_CHECKING:
@@ -91,7 +92,20 @@
 
     if isinstance(config, str) and match_method(config):
         # todo: take advatage of walrus operator in Python 3.8
         function, args = match_method(config)
         return '${config_method:"' + function + '","' + args + '"}'
 
     return config
+
+
+def to_dict(dict_like):
+    if isinstance(dict_like, (omegaconf.DictConfig, omegaconf.ListConfig)):
+        return omegaconf.OmegaConf.to_container(dict_like)
+
+    if isinstance(dict_like, (list, tuple)):
+        return dict_like.__class__([k for k in dict_like])
+
+    if not isinstance(dict_like, collections.abc.Mapping):
+        return dict_like
+
+    return {k: to_dict(v) for k, v in dict_like.items()}
```

### Comparing `machinable-4.4.0/src/machinable/element.py` & `machinable-4.5.0/src/machinable/element.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,21 @@
 import omegaconf
 from machinable import schema
 from machinable.collection import ElementCollection
 from machinable.config import from_element, match_method, rewrite_config_methods
 from machinable.errors import ConfigurationError, MachinableError
 from machinable.mixin import Mixin
 from machinable.types import DatetimeType, ElementType, VersionType
-from machinable.utils import Jsonable, sentinel, unflatten_dict, update_dict
+from machinable.utils import (
+    Jsonable,
+    sentinel,
+    serialize,
+    unflatten_dict,
+    update_dict,
+)
 from omegaconf import DictConfig, OmegaConf
 
 
 class ConfigMethod:
     def __init__(self, element: "Element", prefix="config") -> None:
         self.element = element
         self.prefix = prefix
@@ -168,37 +174,41 @@
 
     if len(compact_element) == 1:
         return compact_element[0], None
 
     return compact_element[0], normversion(compact_element[1:])
 
 
-def equalversion(a: VersionType, b: VersionType) -> bool:
-    return json.dumps(normversion(a), sort_keys=True) == json.dumps(
-        normversion(b), sort_keys=True
+def equaljson(a: Any, b: Any) -> bool:
+    return json.dumps(a, sort_keys=True, default=serialize) == json.dumps(
+        b, sort_keys=True, default=serialize
     )
 
 
-def _filter_enderscores(m: Any):
+def equalversion(a: VersionType, b: VersionType) -> bool:
+    return equaljson(normversion(a), normversion(b))
+
+
+def filter_enderscores(m: Any):
     if not isinstance(m, collections.abc.Mapping):
         return m
     return {
-        k: _filter_enderscores(v) for k, v in m.items() if not k.endswith("_")
+        k: filter_enderscores(v) for k, v in m.items() if not k.endswith("_")
     }
 
 
-def _idversion_filter(value: Union[str, dict]) -> Union[str, dict, None]:
+def idversion_filter(value: Union[str, dict]) -> Union[str, dict, None]:
     if isinstance(value, str) and value.endswith("_"):
         return None
 
-    return _filter_enderscores(value)
+    return filter_enderscores(value)
 
 
 def idversion(version: VersionType) -> VersionType:
-    return normversion([_idversion_filter(v) for v in normversion(version)])
+    return normversion([idversion_filter(v) for v in normversion(version)])
 
 
 def transfer_to(src: "Element", destination: "Element") -> "Element":
     destination.__model__ = src.__model__
 
     return destination
 
@@ -210,48 +220,14 @@
     result = ""
     for i in range(0, 6 * 2, 2):
         result += alphabet[int(uuid[i : i + 2], 16) % 62]
 
     return result
 
 
-def resolve_custom_predicate(
-    predicate: Optional[str], element: "Element"
-) -> Optional[List[str]]:
-    # predicate may look like this "example,test,*"
-    #  where * represents a placeholder for all the custom predicates
-    #  that are marked with a trailing * (i.e. default predicates)
-    # $ is a shorthand for inferring the predicate from the element
-    if predicate == "$":
-        predicate = element.default_predicate
-
-    if predicate is None:
-        return None
-
-    from machinable.project import Project
-
-    custom = element.on_compute_predicate() or {}
-    if isinstance(element, Project):
-        custom.update(element.global_predicate() or {})
-    else:
-        custom.update(Project.get().provider().global_predicate() or {})
-    custom.update(getattr(element, "_starred_predicates", {}))
-
-    if custom:
-        predicate = predicate.replace(
-            "*",
-            ",".join(
-                [k.replace("*", "") for k in custom.keys() if k.endswith("*")]
-            ),
-        )
-    return [
-        p.strip() for p in predicate.split(",") if p.strip() not in ("*", "")
-    ]
-
-
 def instantiate(
     module: str, class_: "Element", version: VersionType, **constructor_kwargs
 ):
     try:
         Element._module_ = module  # assign project-relative module
         instance = class_(version=version, **constructor_kwargs)
         instance.on_instantiate()
@@ -266,39 +242,45 @@
 
 
 class Element(Mixin, Jsonable):
     """Element baseclass"""
 
     kind: Optional[str] = "Element"
     default: Optional["Element"] = None
-    default_predicate: Optional[str] = "config,*"
     _module_: Optional[str] = None
 
     def __init__(self, version: VersionType = None):
         super().__init__()
         if Element._module_ is None:
             Element._module_ = self.__module__
-        self.__model__ = schema.Element(
+        self.__model__ = getattr(schema, self.kind, schema.Element)(
             kind=self.kind,
             module=Element._module_,
             version=normversion(version),
             lineage=get_lineage(self),
             _dump=pickle.dumps(self.__class__)
             if Element._module_.startswith("__session__")
             else None,
         )
         self.__mixin__ = None
         self.__mixins__ = {}
         self._config: Optional[DictConfig] = None
         self._predicate: Optional[DictConfig] = None
         self._cache = {}
+        self._kwargs = {}
 
         Element._module_ = None
 
     @property
+    def _enderscore_config(self):
+        if "enderscore_config" not in self._cache:
+            self._cache["enderscore_config"] = filter_enderscores(self.config)
+        return self._cache["enderscore_config"]
+
+    @property
     def uuid(self) -> str:
         return self.__model__.uuid
 
     @property
     def id(self) -> str:
         return self.uuid[:6]
 
@@ -351,30 +333,29 @@
         return _CONNECTIONS[cls.kind]
 
     @classmethod
     def get(
         cls,
         module: Union[str, "Element", None] = None,
         version: VersionType = None,
-        predicate: Optional[str] = "$",
         **kwargs,
     ) -> "Element":
         if module is None and version is None:
             if len(_CONNECTIONS[cls.kind]) > 0:
                 return _CONNECTIONS[cls.kind][-1]
 
-        if module is None or predicate is None:
-            return cls.instance(module, version, **kwargs)
+        if module is None:
+            return cls.make(module, version, **kwargs)
 
-        return cls.singleton(module, version, predicate, **kwargs)
+        return cls.singleton(module, version, **kwargs)
 
     @classmethod
     def make(
         cls,
-        module: Optional[str] = None,
+        module: Union[None, str, "Element"] = None,
         version: VersionType = None,
         base_class: "Element" = None,
         **kwargs,
     ) -> "Element":
         if module is None:
             module = cls.__module__
 
@@ -405,15 +386,14 @@
         return cls.make(module, version, base_class=cls, **kwargs)
 
     @classmethod
     def singleton(
         cls,
         module: Union[str, "Element"],
         version: VersionType = None,
-        predicate: Optional[str] = "$",
         **kwargs,
     ) -> "Element":
         # no-op as elements do not have a storage representation
         return cls.make(module, version, **kwargs)
 
     @classmethod
     def from_model(cls, model: schema.Element) -> "Element":
@@ -430,28 +410,50 @@
         else:
             instance = cls()
 
         instance.set_model(model)
 
         return instance
 
-    def on_compute_predicate(self) -> Optional[Dict]:
-        """Event to compute a custom predicate dictionary of the element
-        where each key presents a predicate that can be used
-        during element lookup. Keys marked with a * are automatically
-        matched."""
+    def compute_context(self) -> Optional[Dict]:
+        """Computes the context contraints of the element
+
+        Returns:
+            Optional[Dict]: Maps constraint fields their required JSON-able values.
+                An empty dict means no constraits, i.e. all elements will be matched.
+                Returning None means full constraits, i.e. no element will be matched.
+        """
+        return {
+            "module": self.module,
+            "config": self._enderscore_config,
+            "predicate": self.compute_predicate(),
+        }
+
+    def on_compute_predicate(self) -> Dict:
+        """Event to compute additional predicates that identify this element.
+
+        Returns:
+            Dict: Maps the names used during lookup to their JSON-able value.
+        """
+        return {}
+
+    def compute_predicate(self) -> Dict:
+        predicate = self.on_compute_predicate() or {}
+
+        # apply scopes
+        for scope in _CONNECTIONS["Scope"]:
+            predicate.update(scope())
+
+        return predicate
 
     @property
     def predicate(self) -> DictConfig:
         if self._predicate is None:
-            if self.__model__.predicate is None:
-                self.__model__.predicate = OmegaConf.to_container(
-                    OmegaConf.create(self.compute_predicate())
-                )
-
+            if not self.__model__.predicate:
+                return OmegaConf.create({})
             self._predicate = OmegaConf.create(self.__model__.predicate)
 
         return self._predicate
 
     @property
     def config(self) -> DictConfig:
         """Element configuration"""
@@ -573,22 +575,45 @@
             raise ValueError(f"Invalid {cls.kind.lower()} model: {element}.")
 
         if cls.kind is None:
             return schema.Element
 
         return getattr(schema, cls.kind)
 
-    def matches(self, element: "Element", predicate: str) -> bool:
-        predicate_fields = resolve_custom_predicate(predicate, element)
-        if predicate_fields is None:
+    def matches(
+        self, element: "Element", context: Optional[Dict] = sentinel
+    ) -> bool:
+        if context is sentinel:
+            context = element.compute_context()
+
+        if context is None:
+            # full constraint, match none
             return False
 
-        for p in predicate_fields:
-            if not equalversion(self.predicate[p], element.predicate[p]):
-                return False
+        if not context:
+            # no constraints, match all
+            return True
+
+        for field, value in context.items():
+            if field in (
+                "uuid",
+                "kind",
+                "module",
+            ):
+                if not equaljson(getattr(self, field), value):
+                    return False
+            elif field == "config":
+                if not equaljson(self._enderscore_config, value):
+                    return False
+            elif field == "predicate":
+                for p, v in value.items():
+                    if not equaljson(self.predicate[p], v):
+                        return False
+            else:
+                raise ValueError("Invalid context field: {field}")
 
         return True
 
     def set_model(self, model: schema.Element) -> Self:
         self.__model__ = model
 
         # invalidate cached config
@@ -606,38 +631,14 @@
     def unserialize(cls, serialized):
         return cls.from_model(cls.model()(**serialized))
 
     @classmethod
     def is_connected(cls) -> bool:
         return len(_CONNECTIONS[cls.kind]) > 0
 
-    def compute_predicate(self) -> Dict:
-        from machinable.project import Project
-
-        custom = self.on_compute_predicate() or {}
-        if isinstance(self, Project):
-            custom.update(self.global_predicate() or {})
-        else:
-            custom.update(Project.get().provider().global_predicate() or {})
-
-        config = copy.deepcopy(OmegaConf.to_container(self.config))
-        default = config.pop("_default_")
-        version = config.pop("_version_")
-        update = config.pop("_update_")
-
-        return {
-            "config_update": _filter_enderscores(update),
-            "config_update_": update,
-            "config": _filter_enderscores(config),
-            "config_": config,
-            "version": idversion(version),
-            "version_": version,
-            **{k.replace("*", ""): v for k, v in custom.items()},
-        }
-
     def on_instantiate(self) -> None:
         """Event that is invoked whenever the element is instantiated"""
 
     def on_before_configure(self, config: DictConfig) -> None:
         """Configuration event operating on the raw configuration
         This may be used to apply computed configuration updates
         Do not use to validate the configuration but use validators in the config schema
@@ -687,18 +688,18 @@
     def __repr__(self):
         return f"{self.kind} [{self.id}]"
 
     def __str__(self):
         return self.id
 
     def __eq__(self, other):
-        return self.uuid == other.uuid
+        return self.uuid == getattr(other, "uuid", None)
 
     def __ne__(self, other):
-        return self.uuid != other.uuid
+        return self.uuid != getattr(other, "uuid", None)
 
 
 def get_lineage(element: "Element") -> Tuple[str, ...]:
     return tuple(
         obj.module if isinstance(obj, Element) else obj.__module__
         for obj in element.__class__.__mro__[1:-3]
     )
```

### Comparing `machinable-4.4.0/src/machinable/errors.py` & `machinable-4.5.0/src/machinable/errors.py`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/src/machinable/execution.py` & `machinable-4.5.0/src/machinable/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 StatusType = Literal["started", "heartbeat", "finished", "resumed"]
 
 
 class Execution(Interface):
     kind = "Execution"
     default = get_settings().default_execution
-    default_predicate: Optional[str] = None
 
     def __init__(
         self,
         version: VersionType = None,
         resources: Optional[Dict] = None,
         schedule: Union[
             Schedule, ElementType, None
@@ -68,25 +67,25 @@
             lineage=get_lineage(self),
         )
         self.__model__._dump = get_dump(self)
         if schedule is not None:
             if not isinstance(schedule, Schedule):
                 schedule = Schedule.make(*extract(schedule))
             self.push_related("schedule", schedule)
-        self._starred_predicates = {"resources": None}
         self._executable_ = None
 
     @classmethod
     def collect(cls, executions) -> "ExecutionCollection":
         return ExecutionCollection(executions)
 
-    def compute_predicate(self) -> Dict:
-        predicates = super().compute_predicate()
-        predicates["resources"] = self.__model__.resources
-        return predicates
+    def compute_context(self) -> Optional[Dict]:
+        return None  # do not retrieve existing execution
+
+    def on_compute_predicate(self) -> Dict:
+        return {"resources": self.__model__.resources}
 
     @has_one
     def schedule() -> "Schedule":
         return Schedule
 
     @has_many(key="execution_history")
     def executables() -> ComponentCollection:
@@ -286,19 +285,22 @@
     def stream_output(
         self,
         executable: Optional["Component"] = None,
         refresh_every: Union[int, float] = 1,
         stream=print,
     ):
         executable = self.executable(executable)
-        while not self.is_started(executable) or self.is_active(executable):
-            output = self.output(executable, incremental=True)
-            if output:
-                stream(output)
-            time.sleep(refresh_every)
+        try:
+            while not self.is_started(executable) or self.is_active(executable):
+                output = self.output(executable, incremental=True)
+                if output:
+                    stream(output)
+                time.sleep(refresh_every)
+        except KeyboardInterrupt:
+            pass
 
     def update_status(
         self,
         executable: Optional["Component"] = None,
         status: StatusType = "heartbeat",
         timestamp: Optional[TimestampType] = None,
     ) -> TimestampType:
```

### Comparing `machinable-4.4.0/src/machinable/index.py` & `machinable-4.5.0/src/machinable/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 from typing import Any, Dict, List, Optional, Union
 
+import copy
 import json
 import os
 from contextlib import contextmanager
 from datetime import datetime
 
 try:
     from pysqlite3 import dbapi2 as sqlite3
 except ModuleNotFoundError:
     import sqlite3
 
 from machinable import schema
-from machinable.element import Element, get_lineage
+from machinable.element import filter_enderscores, get_lineage, idversion
 from machinable.interface import Interface
 from machinable.settings import get_settings
 from machinable.types import VersionType
-from machinable.utils import is_directory_version
+from machinable.utils import is_directory_version, serialize
 
 
 def _jn(data: Any) -> str:
-    return json.dumps(data, sort_keys=True, separators=(",", ":"))
+    return json.dumps(
+        data, sort_keys=True, separators=(",", ":"), default=serialize
+    )
 
 
 def interface_row_factory(cursor, row) -> schema.Interface:
     return schema.Interface(
         uuid=row[0],
         kind=row[1],
         module=row[2],
-        config=json.loads(row[3]),
-        version=json.loads(row[4]),
-        predicate=json.loads(row[5]),
-        lineage=json.loads(row[6]),
-        timestamp=float(row[7]),
+        config=None,
+        version=json.loads(row[9]),
+        predicate=json.loads(row[10]),
+        lineage=json.loads(row[11]),
+        timestamp=float(row[12]),
     )
 
 
 def migrate(db: sqlite3.Connection) -> None:
     cur = db.cursor()
     version = cur.execute("PRAGMA user_version;").fetchone()[0]
     if version == 0:
         # initial migration
         cur.execute(
             """CREATE TABLE 'index' (
                 uuid text PRIMARY KEY,
                 kind text,
                 module text,
                 config json,
+                config_ json,
+                config_update json,
+                config_update_ json,
+                config_default json,
                 version json,
+                version_ json,
                 predicate json,
                 lineage json,
                 'timestamp' real
             )"""
         )
         cur.execute(
             """CREATE TABLE 'relations' (
@@ -137,31 +145,46 @@
         with db(self.config.database, create=True) as _db:
             cur = _db.cursor()
             if cur.execute(
                 """SELECT uuid FROM 'index' WHERE uuid=?""", (model.uuid,)
             ).fetchone():
                 # already exists
                 return False
+            config = copy.deepcopy(model.config or {})
+            default = config.pop("_default_", {})
+            version = config.pop("_version_", [])
+            update = config.pop("_update_", {})
+
             cur.execute(
                 """INSERT INTO 'index' (
                     uuid,
                     kind,
                     module,
                     config,
+                    config_,
+                    config_update,
+                    config_update_,
+                    config_default,
                     version,
+                    version_,
                     predicate,
                     lineage,
                     'timestamp'
-                ) VALUES (?,?,?,?,?,?,?,?)""",
+                ) VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?)""",
                 (
                     model.uuid,
                     model.kind,
                     model.module,
-                    _jn(model.config),
-                    _jn(model.version),
+                    _jn(filter_enderscores(config)),
+                    _jn(config),
+                    _jn(filter_enderscores(update)),
+                    _jn(update),
+                    _jn(default),
+                    _jn(idversion(version)),
+                    _jn(version),
                     _jn(model.predicate),
                     _jn(model.lineage),
                     model.timestamp,
                 ),
             )
             _db.commit()
         return True
@@ -208,38 +231,41 @@
             row = cur.execute(
                 """SELECT * FROM 'index' WHERE uuid=?""", (uuid,)
             ).fetchone()
             if row is None:
                 return None
             return interface_row_factory(cur, row)
 
-    def find_by_predicate(
-        self, module: str, predicate: Optional[Dict] = None
-    ) -> List[schema.Interface]:
+    def find_by_context(self, context: Dict) -> List[schema.Interface]:
         with db(self.config.database, create=False) as _db:
             if not _db:
                 return []
             cur = _db.cursor()
-            if predicate:
-                keys = ["module=?"]
-                values = [module]
-                for p, v in predicate.items():
-                    keys.append(f"json_extract(predicate, '$.{p}')=?")
-                    values.append(
-                        v if isinstance(v, (str, int, float)) else _jn(v)
-                    )
+
+            keys = []
+            equals = []
+            for field, value in context.items():
+                if field == "predicate":
+                    for p, v in value.items():
+                        keys.append(f"json_extract(predicate, '$.{p}')=?")
+                        equals.append(v)
+                else:
+                    keys.append(f"{field}=?")
+                    equals.append(value)
+
+            if len(keys) > 0:
                 query = cur.execute(
                     """SELECT * FROM 'index' WHERE """ + (" AND ".join(keys)),
-                    values,
+                    [
+                        v if isinstance(v, (str, int, float)) else _jn(v)
+                        for v in equals
+                    ],
                 )
             else:
-                query = cur.execute(
-                    """SELECT * FROM 'index' WHERE module=?""",
-                    (module,),
-                )
+                query = cur.execute("""SELECT * FROM 'index'""")
 
             return [interface_row_factory(cur, row) for row in query.fetchall()]
 
     def find_related(
         self, relation: str, uuid: str, inverse: bool = False
     ) -> Union[None, List[schema.Interface]]:
         with db(self.config.database, create=False) as _db:
```

### Comparing `machinable-4.4.0/src/machinable/interface.py` & `machinable-4.5.0/src/machinable/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,33 +9,32 @@
     from typing import Self
 else:
     from typing_extensions import Self
 
 from typing import Callable
 
 import os
-from functools import partial, wraps
+from functools import partial
 
 from machinable import errors, schema
 from machinable.collection import Collection, InterfaceCollection
 from machinable.element import (
     Element,
+    filter_enderscores,
     get_dump,
     get_lineage,
-    resolve_custom_predicate,
 )
 from machinable.settings import get_settings
 from machinable.types import VersionType
 from machinable.utils import (
     is_directory_version,
     joinpath,
     load_file,
     save_file,
 )
-from omegaconf import OmegaConf
 
 
 class Relation:
     inverse: bool = False
     multiple: bool = False
 
     def __init__(
@@ -207,24 +206,24 @@
         from machinable.index import Index
 
         return Index.get().find(self.uuid) is not None
 
     def commit(self) -> Self:
         from machinable.index import Index
 
-        # ensure that configuration has been parsed
-        assert self.config is not None
-        assert self.predicate is not None
-
         index = Index.get()
 
         # only commit if not already in index
         if index.find(self.uuid) is not None:
             return self
 
+        # ensure that configuration and predicate has been computed
+        assert self.config is not None
+        self.__model__.predicate = self.compute_predicate()
+
         # commit to index
         self.to_directory(self.local_directory(create=True))
         index.commit(self.__model__)
         for k, v in self.__related__.items():
             if v is None:
                 continue
             r = self.__relations__[k]
@@ -284,57 +283,55 @@
 
         return " ".join(cli)
 
     def derive(
         self,
         module: Union[str, Element, None] = None,
         version: VersionType = None,
-        predicate: Optional[str] = "$",
         **kwargs,
     ) -> Self:
-        if module is None or predicate is None:
+        if module is None:
             return self.make(module, version, derived_from=self, **kwargs)
 
         return self.derived.singleton(
-            module, version, predicate, derived_from=self, **kwargs
+            module, version, derived_from=self, **kwargs
         )
 
     @classmethod
     def singleton(
         cls,
         module: Union[str, "Element"],
         version: VersionType = None,
-        predicate: Optional[str] = "$",
         **kwargs,
     ) -> "Collection":
         if module in [
             "machinable.index",
             "machinable.project",
         ] and is_directory_version(version):
             # interpret as shortcut for directory
             version = {"directory": version}
-        candidates = cls.find_by_predicate(
+        candidates = cls.find_in_context(
             module,
             version,
-            predicate,
             **kwargs,
         )
+
         if candidates:
             return candidates[-1]
 
         return cls.make(module, version, **kwargs)
 
     def is_mounted(self) -> bool:
         if self.__model__ is None:
             return False
 
         return os.path.exists(self.local_directory())
 
     @classmethod
-    def find(cls, uuid: str) -> Optional["Element"]:
+    def find(cls, uuid: str) -> Optional["Interface"]:
         from machinable.index import Index
 
         index = Index.get()
 
         if not index.find(uuid):
             return None
 
@@ -352,57 +349,44 @@
 
             if not available:
                 return None
 
         return cls.from_directory(local_directory)
 
     @classmethod
-    def find_many(cls, uuids: List[str]) -> "Collection":
+    def find_many(cls, uuids: List[str]) -> "InterfaceCollection":
         return cls.collect([cls.find(uuid) for uuid in uuids])
 
     @classmethod
-    def find_by_predicate(
+    def find_in_context(
         cls,
         module: Union[str, "Element"],
         version: VersionType = None,
-        predicate: Optional[str] = "$",
         **kwargs,
-    ) -> "Collection":
+    ) -> "InterfaceCollection":
         from machinable.index import Index
 
         try:
             candidate = cls.make(module, version, **kwargs)
         except ModuleNotFoundError:
             return cls.collect([])
 
-        predicate_fields = resolve_custom_predicate(predicate, candidate)
-
-        if predicate_fields is None:
+        context = candidate.compute_context()
+        if context is None:
             return cls.collect([])
 
-        predicate_data = OmegaConf.to_container(
-            OmegaConf.create(
-                {p: candidate.predicate[p] for p in predicate_fields}
-            )
-        )
-
         return cls.collect(
             [
                 cls.find(interface.uuid)
-                for interface in Index.get().find_by_predicate(
-                    module
-                    if isinstance(module, str)
-                    else f"__session__{module.__name__}",
-                    predicate_data,
-                )
+                for interface in Index.get().find_by_context(context)
             ]
         )
 
     @classmethod
-    def from_directory(cls, directory: str) -> "Element":
+    def from_directory(cls, directory: str) -> Self:
         """Returns an interface from a storage directory
 
         Note that this does not verify the integrity of the directory.
         In particular, the interface may be missing or not be indexed.
         """
         data = load_file([directory, "model.json"])
 
@@ -413,14 +397,27 @@
 
         interface = model(**data)
         if interface.module.startswith("__session__"):
             interface._dump = load_file([directory, "dump.p"], None)
 
         return cls.from_model(interface)
 
+    def all(self) -> "InterfaceCollection":
+        module = (
+            self.module
+            if not self.module.startswith("__session__")
+            else self.__class__
+        )
+        return self.find_in_context(
+            module, self.__model__.version, **self._kwargs
+        )
+
+    def new(self) -> Self:
+        return self.make(self.module, self.__model__.version, **self._kwargs)
+
     def to_directory(self, directory: str, relations=True) -> Self:
         save_file([directory, ".machinable"], self.__model__.uuid)
         save_file([directory, "model.json"], self.__model__)
         if self.__model__._dump is not None:
             save_file([directory, "dump.p"], self.__model__._dump)
         if relations:
             for k, v in self.__related__.items():
```

### Comparing `machinable-4.4.0/src/machinable/mixin.py` & `machinable-4.5.0/src/machinable/mixin.py`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/src/machinable/project.py` & `machinable-4.5.0/src/machinable/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,13 +350,9 @@
     def on_parse_cli(self):
         """Triggered when CLI is invoked.
 
         You may return a list of modified arguments or implement a fully custom CLI here by returning its exit code.
         """
         return sys.argv[1:]
 
-    def global_predicate(self) -> Dict:
-        """Project-wide element predicates."""
-        return {}
-
     def __repr__(self) -> str:
         return f"Project({self.config.directory})"
```

### Comparing `machinable-4.4.0/src/machinable/schedule.py` & `machinable-4.5.0/src/machinable/schedule.py`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/src/machinable/schema.py` & `machinable-4.5.0/src/machinable/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     kind: str = "Storage"
 
 
 class Index(Element):
     kind: str = "Index"
 
 
+class Scope(Element):
+    kind: str = "Scope"
+
+
 class Interface(Element):
     kind: str = "Interface"
     _dump: Optional[bytes] = PrivateAttr(default=None)
 
 
 class Component(Interface):
     kind: str = "Component"
@@ -45,13 +49,7 @@
     kind: str = "Execution"
     seed: int = Field(default_factory=generate_seed)
     resources: Optional[Dict] = None
 
 
 class Schedule(Interface):
     kind: str = "Schedule"
-
-
-class Group(Interface):
-    kind: str = "Group"
-    pattern: str
-    path: Optional[str] = None
```

### Comparing `machinable-4.4.0/src/machinable/settings.py` & `machinable-4.5.0/src/machinable/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     default_execution: Optional[ElementType] = None
     default_component: Optional[ElementType] = None
     default_interface: Optional[ElementType] = None
     default_schedule: Optional[ElementType] = None
     default_group: Optional[str] = "%Y_%U_%a/"
     default_storage: Optional[ElementType] = None
     default_index: Optional[ElementType] = None
+    default_scope: Optional[ElementType] = None
 
 
 def get_settings(file="~/.machinable/settings.json"):
     try:
         with open(os.path.expanduser(file)) as f:
             data = json.load(f)
     except FileNotFoundError:
```

### Comparing `machinable-4.4.0/src/machinable/storage.py` & `machinable-4.5.0/src/machinable/storage.py`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/src/machinable/utils.py` & `machinable-4.5.0/src/machinable/utils.py`

 * *Files identical despite different names*

### Comparing `machinable-4.4.0/PKG-INFO` & `machinable-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: machinable
-Version: 4.4.0
+Version: 4.5.0
 Summary: A modular configuration system for research projects
 Home-page: https://machinable.org
 License: MIT
 Keywords: machine-learning,research
 Author: Frithjof Gressmann
 Author-email: hello@machinable.org
 Maintainer: Frithjof Gressmann
@@ -18,21 +18,21 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Requires-Dist: arrow (>=1.2,<2.0)
-Requires-Dist: dill (>=0.3.6,<0.4.0)
+Requires-Dist: dill (>=0.3.7,<0.4.0)
 Requires-Dist: flatten-dict (>=0.4,<0.5)
 Requires-Dist: importlib-metadata (>=6.7,<7.0) ; python_version < "3.8"
 Requires-Dist: jsonlines (>=3.1,<4.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
+Requires-Dist: pydantic (==1.*)
+Requires-Dist: typing-extensions (>=4.7.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Documentation, https://machinable.org
 Project-URL: Repository, https://github.com/machinable-org/machinable
 Description-Content-Type: text/markdown
 
 # machinable
 
 <div align="center">
```

