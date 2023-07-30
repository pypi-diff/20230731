# Comparing `tmp/electrolytes-0.3.1.tar.gz` & `tmp/electrolytes-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.3.1.tar", last modified: Tue Jul 25 21:50:39 2023, max compression
+gzip compressed data, was "electrolytes-0.3.2.tar", last modified: Sun Jul 30 22:54:56 2023, max compression
```

## Comparing `electrolytes-0.3.1.tar` & `electrolytes-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-25 21:50:28.000000 electrolytes-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-25 21:50:39.964221 electrolytes-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-25 21:50:28.000000 electrolytes-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/db1.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:28.000000 electrolytes-0.3.1/electrolytes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 21:50:39.000000 electrolytes-0.3.1/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-25 21:50:28.000000 electrolytes-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:50:39.964221 electrolytes-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:50:39.964221 electrolytes-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-25 21:50:28.000000 electrolytes-0.3.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-25 21:50:28.000000 electrolytes-0.3.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-30 22:54:43.000000 electrolytes-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-30 22:54:56.430830 electrolytes-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-30 22:54:43.000000 electrolytes-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/db1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-30 22:54:43.000000 electrolytes-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:54:56.430830 electrolytes-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-30 22:54:43.000000 electrolytes-0.3.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-30 22:54:43.000000 electrolytes-0.3.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-30 22:54:43.000000 electrolytes-0.3.2/tests/test_lock.py
```

### Comparing `electrolytes-0.3.1/LICENSE.txt` & `electrolytes-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.1/PKG-INFO` & `electrolytes-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.3.1
+Version: 0.3.2
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -85,34 +85,32 @@
 ```python
 
     def user_defined(self) -> Iterable[str]: ...
 
     def is_user_defined(self, name: str) -> bool: ...
 ```
 
+The `database` object is also usable as a context manager (i.e. `with database:`), which allows multiple operations to be performed with exclusive access to the database (locking out any other processes for the duration).
+
 `Constituent` names are case insensitive and will be automatically converted to all uppercase. Any instances added to (or removed from) the `database` will be saved for the current operating system user. Default components cannot be changed or removed (expect a `ValueError` if you try).
 
-The public stubs of the `Constituent` class are:
+The public interface of the `Constituent` class is:
 
 ```python
 class Constituent:
-    def __init__(self,
-                 *,
-                 name: str,
-                 u_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 u_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
-                 pkas_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 pkas_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = None, # == len(u_neg) == len(pkas_neg)
-                 pos_count: int = None): # == len(u_pos) == len(pkas_pos)
-        ...
+    name: str
+    u_neg: Sequence[float] = []  # mobilities for [..., -3, -2, -1], SI units*1e-9
+    u_pos: Sequence[float] = []  # mobilities for [+1, +2, +3, ...], SI units*1e-9
+    pkas_neg: Sequence[float] = []  # pKas for [..., -3, -2, -1]
+    pkas_pos: Sequence[float] = []  # pKas for [+1, +2, +3, ...]
 
     # Interface for electroMicroTransport
-    def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
-    def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
+    def mobilities(self) -> Sequence[float]: ...  # for [..., +3, +2, +1, -1, -2, -3, ...], SI units
+    def pkas(self) -> Sequence[float]: ...  # for [..., +3, +2, +1, -1, -2, -3, ...]
+    # NOTE: the above are padded if needed so that +3 and -3 are always present (len >= 6)
     def diffusivity(self) -> float: ...  # SI units
 ```
 
 # Data credits
 
 Electrolyte data taken from the Simul 6 application[^simul6] ([homepage](https://simul6.app), [GitHub](https://github.com/hobrasoft/simul6)). The dataset of different electrolytes was originally compiled by Prof. Hirokawa[^Hirokawa].
```

### Comparing `electrolytes-0.3.1/README.md` & `electrolytes-0.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -54,34 +54,32 @@
 ```python
 
     def user_defined(self) -> Iterable[str]: ...
 
     def is_user_defined(self, name: str) -> bool: ...
 ```
 
+The `database` object is also usable as a context manager (i.e. `with database:`), which allows multiple operations to be performed with exclusive access to the database (locking out any other processes for the duration).
+
 `Constituent` names are case insensitive and will be automatically converted to all uppercase. Any instances added to (or removed from) the `database` will be saved for the current operating system user. Default components cannot be changed or removed (expect a `ValueError` if you try).
 
-The public stubs of the `Constituent` class are:
+The public interface of the `Constituent` class is:
 
 ```python
 class Constituent:
-    def __init__(self,
-                 *,
-                 name: str,
-                 u_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 u_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
-                 pkas_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 pkas_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = None, # == len(u_neg) == len(pkas_neg)
-                 pos_count: int = None): # == len(u_pos) == len(pkas_pos)
-        ...
+    name: str
+    u_neg: Sequence[float] = []  # mobilities for [..., -3, -2, -1], SI units*1e-9
+    u_pos: Sequence[float] = []  # mobilities for [+1, +2, +3, ...], SI units*1e-9
+    pkas_neg: Sequence[float] = []  # pKas for [..., -3, -2, -1]
+    pkas_pos: Sequence[float] = []  # pKas for [+1, +2, +3, ...]
 
     # Interface for electroMicroTransport
-    def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
-    def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
+    def mobilities(self) -> Sequence[float]: ...  # for [..., +3, +2, +1, -1, -2, -3, ...], SI units
+    def pkas(self) -> Sequence[float]: ...  # for [..., +3, +2, +1, -1, -2, -3, ...]
+    # NOTE: the above are padded if needed so that +3 and -3 are always present (len >= 6)
     def diffusivity(self) -> float: ...  # SI units
 ```
 
 # Data credits
 
 Electrolyte data taken from the Simul 6 application[^simul6] ([homepage](https://simul6.app), [GitHub](https://github.com/hobrasoft/simul6)). The dataset of different electrolytes was originally compiled by Prof. Hirokawa[^Hirokawa].
```

### Comparing `electrolytes-0.3.1/electrolytes/__init__.py` & `electrolytes-0.3.2/electrolytes/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import sys
 import pkgutil
 from pathlib import Path
-from typing import Iterable, Iterator, List, Sequence, Dict, Optional, Any
+from typing import Collection, Iterator, List, Sequence, Dict, Optional, Any
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 if sys.version_info >= (3, 8):
     from functools import cached_property
 else:
     from backports.cached_property import cached_property
+from contextlib import ContextDecorator
 from warnings import warn
 
 from pydantic import BaseModel, Field, field_validator, FieldValidationInfo, model_validator, TypeAdapter
 from filelock import FileLock
 from typer import get_app_dir
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 
 class Constituent(BaseModel, populate_by_name=True, frozen=True):
     id: Optional[int] = None
     name: str
     u_neg: Annotated[List[float], Field(alias="uNeg")] = [] # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
     u_pos: Annotated[List[float], Field(alias="uPos")] = [] # [+1, +2, +3, ..., +pos_count]
@@ -117,106 +118,117 @@
 def _load_constituents(data: bytes, context: Optional[Dict[str,str]]=None) -> List[Constituent]:
     return _StoredConstituents.validate_json(data, context=context)["constituents"]
 
 def _dump_constituents(constituents: List[Constituent]) -> bytes:
     return  _StoredConstituents.dump_json({"constituents": constituents}, by_alias=True, indent=4)
 
 
-class _FileLock(FileLock):
-    def __enter__(self) -> Any:
-        Path(self.lock_file).parent.mkdir(parents=True, exist_ok=True) # https://github.com/tox-dev/py-filelock/issues/176
-        return super().__enter__()
+class _Database(ContextDecorator):
+    def __init__(self, user_constituents_file: Path) -> None:
+        self._user_constituents_file = user_constituents_file
+        self._user_constituents_lock = FileLock(self._user_constituents_file.with_suffix(".lock"))
+        self._user_constituents_dirty = False
 
-
-class _Database:
     @cached_property
     def _default_constituents(self) -> Dict[str, Constituent]:
         data = pkgutil.get_data(__package__, "db1.json")
         if data is None:
             raise RuntimeError("failed to load default constituents")
         constituents = _load_constituents(data, context={"fix": "db1"})
         return {c.name: c for c in constituents}
 
-    _USER_CONSTITUENTS_FILE = Path(get_app_dir(__package__), "user_constituents.json")
-    _user_constituents_file_lock = _FileLock(_USER_CONSTITUENTS_FILE.with_suffix(".lock"))
-
     @cached_property
     def _user_constituents(self) -> Dict[str, Constituent]:
         try:
-            with self._user_constituents_file_lock, self._USER_CONSTITUENTS_FILE.open("rb") as f:
-                data = f.read()
+            with self:
+                user_data = self._user_constituents_file.read_bytes()
         except OSError:
             return {}
         try:
-            constituents = _load_constituents(data)
+           user_constituents = _load_constituents(user_data)
         except Exception as e:
-            warn(f"failed to load user constituents from {self._USER_CONSTITUENTS_FILE}: {type(e).__name__}", RuntimeWarning)
+            warn(f"failed to load user constituents from {self._user_constituents_file}: {type(e).__name__}", RuntimeWarning)
             return {}
-        return {c.name: c for c in constituents}
-    
+        return {c.name: c for c in user_constituents}
+
     def _invalidate_user_constituents(self) -> None:
+        assert not self._user_constituents_dirty
         try:
             del self._user_constituents
         except AttributeError:
             pass
 
-    @_user_constituents_file_lock
     def _save_user_constituents(self) -> None:
         data = _dump_constituents(list(self._user_constituents.values()))
-        self._USER_CONSTITUENTS_FILE.parent.mkdir(parents=True, exist_ok=True)
-        with self._USER_CONSTITUENTS_FILE.open("wb") as f:
-            f.write(data)
+        self._user_constituents_file.parent.mkdir(parents=True, exist_ok=True)
+        with self:
+            self._user_constituents_file.write_bytes(data)
+        self._user_constituents_dirty = False
+
+    def __enter__(self) -> None:
+        if not self._user_constituents_lock.is_locked:
+            Path(self._user_constituents_lock.lock_file).parent.mkdir(parents=True, exist_ok=True) # https://github.com/tox-dev/py-filelock/issues/176
+            self._invalidate_user_constituents()
+        self._user_constituents_lock.acquire()
+
+    def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
+        try:
+            if self._user_constituents_lock.lock_counter == 1 and self._user_constituents_dirty:
+                self._save_user_constituents()
+        finally:
+            self._user_constituents_lock.release()
 
 
     def __iter__(self) -> Iterator[str]:
         yield from sorted([*self._default_constituents, *self._user_constituents])
 
     def __getitem__(self, name: str) -> Constituent:
         name = name.upper()
         try:
             return self._user_constituents[name]
         except KeyError:
             return self._default_constituents[name]
 
-    @_user_constituents_file_lock
     def add(self, constituent: Constituent) -> None:
-        self._invalidate_user_constituents()
-        if constituent.name not in self:
-            self._user_constituents[constituent.name] = constituent
-            self._save_user_constituents()
-        else:
-            warn(f"{constituent.name}: component was not added (name already exists in database)")
+        with self:
+            if constituent.name not in self:
+                self._user_constituents[constituent.name] = constituent
+                self._user_constituents_dirty = True
+            else:
+                warn(f"{constituent.name}: component was not added (name already exists in database)")
 
-    @_user_constituents_file_lock
     def __delitem__(self, name: str) -> None:
         name = name.upper()
         try:
-            self._invalidate_user_constituents()
-            del self._user_constituents[name]
-            self._save_user_constituents()
+            with self:
+                del self._user_constituents[name]
+                self._user_constituents_dirty = True
         except KeyError:
             if name in self._default_constituents:
                 raise ValueError(f"{name}: cannot remove default component")
             else:
                 raise
 
     def __len__(self) -> int:
         return len(self._default_constituents) + len(self._user_constituents)
 
-    def user_defined(self) -> Iterable[str]:
+    def user_defined(self) -> Collection[str]:
         return sorted(self._user_constituents)
 
     def __contains__(self, obj: Any) -> bool:
         if isinstance(obj, str):
-            obj = obj.upper()
-            return obj in self._default_constituents or obj in self._user_constituents
+            name = obj.upper()
+            return name in self._default_constituents or name in self._user_constituents
         elif isinstance(obj, Constituent):
-            return obj == self[obj.name]
+            try:
+                return obj == self[obj.name]
+            except KeyError:
+                return False
         else:
             return False
 
     def is_user_defined(self, name: str) -> bool:
         name = name.upper()
         return name in self._user_constituents
 
 
-database = _Database()
+database = _Database(Path(get_app_dir(__package__), "user_constituents.json"))
```

### Comparing `electrolytes-0.3.1/electrolytes/__main__.py` & `electrolytes-0.3.2/electrolytes/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,171 +1,204 @@
 import sys
-from typing import Tuple, List
+from typing import Tuple, List, Optional
 if sys.version_info >= (3, 9):
     from typing import Annotated
 else:
     from typing_extensions import Annotated
 
 import typer
-from click import Context, Parameter
 
-from . import database, Constituent
+from . import database, Constituent, __version__
 
 
 app = typer.Typer()
 
 
-def complete_name(ctx: Context, param: Parameter, incomplete: str) -> List[str]:
-    return [name for name in database if name.startswith(incomplete)]
+def complete_name(incomplete: str) -> List[str]:
+    return [name for name in database if name.startswith(incomplete.upper())]
 
-def complete_name_user_defined(ctx: Context, param: Parameter, incomplete: str) -> List[str]:
-    return [name for name in database.user_defined() if name.startswith(incomplete)]
+def complete_name_user_defined(incomplete: str) -> List[str]:
+    return [name for name in database.user_defined() if name.startswith(incomplete.upper())]
 
 
 @app.command()
-def add(name: Annotated[str, typer.Argument(shell_complete=complete_name_user_defined)],
-        p1: Annotated[Tuple[float, float], typer.Option("+1", help="Mobility (*1e-9) and pKa for +1")] = (None, None), # type: ignore
-        p2: Annotated[Tuple[float, float], typer.Option("+2", help="Mobility (*1e-9) and pKa for +2")] = (None, None), # type: ignore
-        p3: Annotated[Tuple[float, float], typer.Option("+3", help="Mobility (*1e-9) and pKa for +3")] = (None, None), # type: ignore
-        p4: Annotated[Tuple[float, float], typer.Option("+4", help="Mobility (*1e-9) and pKa for +4")] = (None, None), # type: ignore
-        p5: Annotated[Tuple[float, float], typer.Option("+5", help="Mobility (*1e-9) and pKa for +5")] = (None, None), # type: ignore
-        p6: Annotated[Tuple[float, float], typer.Option("+6", help="Mobility (*1e-9) and pKa for +6")] = (None, None), # type: ignore
-        m1: Annotated[Tuple[float, float], typer.Option("-1", help="Mobility (*1e-9) and pKa for -1")] = (None, None), # type: ignore
-        m2: Annotated[Tuple[float, float], typer.Option("-2", help="Mobility (*1e-9) and pKa for -2")] = (None, None), # type: ignore
-        m3: Annotated[Tuple[float, float], typer.Option("-3", help="Mobility (*1e-9) and pKa for -3")] = (None, None), # type: ignore
-        m4: Annotated[Tuple[float, float], typer.Option("-4", help="Mobility (*1e-9) and pKa for -4")] = (None, None), # type: ignore
-        m5: Annotated[Tuple[float, float], typer.Option("-5", help="Mobility (*1e-9) and pKa for -5")] = (None, None), # type: ignore
-        m6: Annotated[Tuple[float, float], typer.Option("-6", help="Mobility (*1e-9) and pKa for -6")] = (None, None), # type: ignore
-        force: Annotated[bool, typer.Option("-f", help="Replace any existing user-defined component with the same name")] = False) -> None:
-    """Save a user-defined component"""
+def add(name: Annotated[str, typer.Argument(autocompletion=complete_name_user_defined)],
+        p1: Annotated[Tuple[float, float], typer.Option("+1", help="Mobility (*1e-9) and pKa for +1", show_default=False)] = (None, None), # type: ignore
+        p2: Annotated[Tuple[float, float], typer.Option("+2", help="Mobility (*1e-9) and pKa for +2", show_default=False)] = (None, None), # type: ignore
+        p3: Annotated[Tuple[float, float], typer.Option("+3", help="Mobility (*1e-9) and pKa for +3", show_default=False)] = (None, None), # type: ignore
+        p4: Annotated[Tuple[float, float], typer.Option("+4", help="Mobility (*1e-9) and pKa for +4", show_default=False)] = (None, None), # type: ignore
+        p5: Annotated[Tuple[float, float], typer.Option("+5", help="Mobility (*1e-9) and pKa for +5", show_default=False)] = (None, None), # type: ignore
+        p6: Annotated[Tuple[float, float], typer.Option("+6", help="Mobility (*1e-9) and pKa for +6", show_default=False)] = (None, None), # type: ignore
+        m1: Annotated[Tuple[float, float], typer.Option("-1", help="Mobility (*1e-9) and pKa for -1", show_default=False)] = (None, None), # type: ignore
+        m2: Annotated[Tuple[float, float], typer.Option("-2", help="Mobility (*1e-9) and pKa for -2", show_default=False)] = (None, None), # type: ignore
+        m3: Annotated[Tuple[float, float], typer.Option("-3", help="Mobility (*1e-9) and pKa for -3", show_default=False)] = (None, None), # type: ignore
+        m4: Annotated[Tuple[float, float], typer.Option("-4", help="Mobility (*1e-9) and pKa for -4", show_default=False)] = (None, None), # type: ignore
+        m5: Annotated[Tuple[float, float], typer.Option("-5", help="Mobility (*1e-9) and pKa for -5", show_default=False)] = (None, None), # type: ignore
+        m6: Annotated[Tuple[float, float], typer.Option("-6", help="Mobility (*1e-9) and pKa for -6", show_default=False)] = (None, None), # type: ignore
+        force: Annotated[bool, typer.Option("-f", help="Do not prompt before replacing a user-defined component with the same name")] = False) -> None:
+    """Store a user-defined component in the database."""
     name = name.upper()
 
     if p1[0] is None and m1[0] is None:
         assert p1[1] is None and m1[1] is None
         typer.echo("Error: at least one of the +1 or -1 options is required", err=True)
         raise typer.Exit(code=1)
 
     neg: List[Tuple[float, float]] = []
     any_omitted = False
     for i,m in enumerate([m1, m2, m3, m4, m5, m6]):
         if m[0] is None:
             assert m[1] is None
             any_omitted = True
         elif any_omitted:
-            typer.echo(f"Error: missing charge +{i}", err=True)
+            typer.echo(f"Error: missing charge -{i}", err=True)
             raise typer.Exit(code=1)
         else:
             neg.insert(0, m)
 
     pos: List[Tuple[float, float]] = []
     any_omitted = False
     for i,p in enumerate([p1, p2, p3, p4, p5, p6]):
         if p[0] is None:
             assert p[1] is None
             any_omitted = True
         elif any_omitted:
-            typer.echo(f"Error: missing charge -{i}", err=True)
+            typer.echo(f"Error: missing charge +{i}", err=True)
             raise typer.Exit(code=1)
         else:
             pos.append(p)
 
-    with database._user_constituents_file_lock:
-        if not force and database.is_user_defined(name):
-            typer.echo(f"Error: user-defined component {name} already exists (use -f to replace)", err=True)
-            raise typer.Exit(code=1)
+    constituent = Constituent(name=name,
+                              u_neg=[x[0] for x in neg],
+                              u_pos=[x[0] for x in pos],
+                              pkas_neg=[x[1] for x in neg],
+                              pkas_pos=[x[1] for x in pos])
+
+    with database:
+        if name in database:
+            if not database.is_user_defined(name):
+                typer.echo(f"Error: {name}: is a default component", err=True)
+                raise typer.Exit(code=1)
 
-        try:
-            constituent = Constituent(name=name,
-                                    u_neg=[x[0] for x in neg],
-                                    u_pos=[x[0] for x in pos],
-                                    pkas_neg=[x[1] for x in neg],
-                                    pkas_pos=[x[1] for x in pos])
-            
-            try:
-                del database[name]
-            except KeyError:
-                pass
+            if not force:
+                typer.confirm(f"Replace existing {name}?", abort=True)
 
-            database.add(constituent)
+            del database[name]
 
-        except Exception as e:
-            typer.echo(f"Error: {e}", err=True)
-            raise typer.Exit(code=1)
+        database.add(constituent)
 
 
 @app.command()
-def info(name: Annotated[str, typer.Argument(shell_complete=complete_name)]) -> None:
-    """Show the properties of a component"""
-    name = name.upper()
+def info(names: Annotated[Optional[List[str]], typer.Argument(help="Component names", autocompletion=complete_name)] = None) -> None:
+    """
+    Show the properties of components.
+    
+    If no names are given, print the number of components in the database.
+    """
+    if names:
+        first = True
+        errors_ocurred = False
+        for name in names:
+            name = name.upper()
 
-    try:
-        constituent = database[name]
-    except KeyError:
-        typer.echo(f"Error: {name}: no such component", err=True)
-        raise typer.Exit(code=1)
+            try:
+                constituent = database[name]
+            except KeyError:
+                typer.echo(f"Error: {name}: no such component", err=True)
+                errors_ocurred = True
+                continue
+
+            charges = list(range(constituent.pos_count, 0, -1)) + list(range(-1, -constituent.neg_count - 1, -1))
+            uu = constituent.u_pos[::-1] + constituent.u_neg[::-1]
+            pkas = constituent.pkas_pos[::-1] + constituent.pkas_neg[::-1]
+
+            assert len(charges) == len(uu) == len(pkas)
+
+            if not first:
+                typer.echo()
+            typer.echo(f"Component: {name}")
+            if database.is_user_defined(name):
+                typer.echo("[user-defined]")
+            typer.echo( "                 " + " ".join(f"{c:^+8d}" for c in charges))
+            typer.echo( "Mobilities *1e-9:" + " ".join(f"{u:^8.2f}" for u in uu))
+            typer.echo( "pKas:            " + " ".join(f"{p:^8.2f}" for p in pkas))
+            typer.echo(f"Diffusivity: {constituent.diffusivity():.4e}")
 
-    charges = list(range(constituent.pos_count, 0, -1)) + list(range(-1, -constituent.neg_count - 1, -1))
-    uu = constituent.u_pos[::-1] + constituent.u_neg[::-1]
-    pkas = constituent.pkas_pos[::-1] + constituent.pkas_neg[::-1]
+            first = False
 
-    assert len(charges) == len(uu) == len(pkas)
+        if errors_ocurred:
+            raise typer.Exit(code=1)
     
-    typer.echo(f"Component: {name}")
-    if database.is_user_defined(name):
-        typer.echo("[user-defined]")
-    typer.echo( "                 " + " ".join(f"{c:^+8d}" for c in charges))
-    typer.echo( "Mobilities *1e-9:" + " ".join(f"{u:^8.2f}" for u in uu))
-    typer.echo( "pKas:            " + " ".join(f"{p:^8.2f}" for p in pkas))
-    typer.echo(f"Diffusivity: {constituent.diffusivity():.4e}")
-
+    else:
+        total = len(database)
+        user = len(database.user_defined())
+        typer.echo(f"{total} components stored in the database ({total - user} default, {user} user-defined)")
 
 @app.command()
-def ls(user_only: Annotated[bool, typer.Option("--user", help="Show only user-defined components")] = False) -> None:
-    """List available components"""
-    if user_only:
+def ls(user: Annotated[Optional[bool], typer.Option("--user/--default", help="List only user-defined/default components")] = None) -> None:
+    """List components in the database."""
+
+    if user:
         names = database.user_defined()
+    elif user is not None:
+        names = [name for name in database if not database.is_user_defined(name)]
     else:
         names = database
 
     for name in names:
         typer.echo(name)
 
 
 @app.command()
-def rm(names: Annotated[List[str], typer.Argument(shell_complete=complete_name_user_defined)]) -> None:
-    """Remove user-defined components"""
+def rm(names: Annotated[List[str], typer.Argument(autocompletion=complete_name_user_defined)],
+       force: Annotated[Optional[bool], typer.Option("-f", help="Ignore non-existent components")] = False) -> None:
+    """Remove user-defined components from the database."""
     errors_ocurred = False
     for name in names:
         name = name.upper()
         try:
             del database[name]
         except KeyError:
-            typer.echo(f"Error: {name}: no such component", err=True)
-            errors_ocurred = True
+            if not force:
+                typer.echo(f"Error: {name}: no such component", err=True)
+                errors_ocurred = True
         except ValueError as e:
             typer.echo(f"Error: {e}", err=True)
             errors_ocurred = True
-    
+
     if errors_ocurred:
-        raise typer.Exit(code=-1)
+        raise typer.Exit(code=1)
 
 
 @app.command()
 def search(text: str,
-           user_only: Annotated[bool, typer.Option("--user", help="Search only user-defined components")] = False) -> None:
-    """Search the list of components"""
+           user: Annotated[Optional[bool], typer.Option("--user/--default", help="Search only user-defined/default components")] = None) -> None:
+    """Search for a name in the database."""
     text = text.upper()
 
-    if user_only:
+    if user:
         names = list(database.user_defined())
+    elif user is not None:
+        names = [name for name in database if not database.is_user_defined(name)]
     else:
         names = list(database)
 
     match_indices = [name.find(text) for name in names]
 
     for name, index in zip(names, match_indices):
         if index != -1:
             typer.echo(name[0:index] + typer.style(name[index:index+len(text)], bold=True) + name[index+len(text):])
 
 
+def version_callback(show: bool) -> None:
+    if show:
+        typer.echo(f"{__package__} {__version__}")
+        raise typer.Exit()
+
+@app.callback()
+def common(version: Annotated[bool, typer.Option("--version", help="Show version and exit.", callback=version_callback)] = False) -> None:
+    """Database of electrolytes and their properties."""
+    pass
+
+
 if __name__ == "__main__":
     app(prog_name=__package__)
```

### Comparing `electrolytes-0.3.1/electrolytes/db1.json` & `electrolytes-0.3.2/electrolytes/db1.json`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.1/electrolytes.egg-info/PKG-INFO` & `electrolytes-0.3.2/electrolytes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.3.1
+Version: 0.3.2
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -85,34 +85,32 @@
 ```python
 
     def user_defined(self) -> Iterable[str]: ...
 
     def is_user_defined(self, name: str) -> bool: ...
 ```
 
+The `database` object is also usable as a context manager (i.e. `with database:`), which allows multiple operations to be performed with exclusive access to the database (locking out any other processes for the duration).
+
 `Constituent` names are case insensitive and will be automatically converted to all uppercase. Any instances added to (or removed from) the `database` will be saved for the current operating system user. Default components cannot be changed or removed (expect a `ValueError` if you try).
 
-The public stubs of the `Constituent` class are:
+The public interface of the `Constituent` class is:
 
 ```python
 class Constituent:
-    def __init__(self,
-                 *,
-                 name: str,
-                 u_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 u_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
-                 pkas_neg: Sequence[float] = [],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
-                 pkas_pos: Sequence[float] = [],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = None, # == len(u_neg) == len(pkas_neg)
-                 pos_count: int = None): # == len(u_pos) == len(pkas_pos)
-        ...
+    name: str
+    u_neg: Sequence[float] = []  # mobilities for [..., -3, -2, -1], SI units*1e-9
+    u_pos: Sequence[float] = []  # mobilities for [+1, +2, +3, ...], SI units*1e-9
+    pkas_neg: Sequence[float] = []  # pKas for [..., -3, -2, -1]
+    pkas_pos: Sequence[float] = []  # pKas for [+1, +2, +3, ...]
 
     # Interface for electroMicroTransport
-    def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
-    def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
+    def mobilities(self) -> Sequence[float]: ...  # for [..., +3, +2, +1, -1, -2, -3, ...], SI units
+    def pkas(self) -> Sequence[float]: ...  # for [..., +3, +2, +1, -1, -2, -3, ...]
+    # NOTE: the above are padded if needed so that +3 and -3 are always present (len >= 6)
     def diffusivity(self) -> float: ...  # SI units
 ```
 
 # Data credits
 
 Electrolyte data taken from the Simul 6 application[^simul6] ([homepage](https://simul6.app), [GitHub](https://github.com/hobrasoft/simul6)). The dataset of different electrolytes was originally compiled by Prof. Hirokawa[^Hirokawa].
```

### Comparing `electrolytes-0.3.1/pyproject.toml` & `electrolytes-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.1/tests/test_api.py` & `electrolytes-0.3.2/tests/test_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     assert "CYSTINE" in l
     assert "SILVER" in l
 
 
 def test_get_component() -> None:
     c = database["LYSINE"]
     assert isinstance(c, Constituent)
+    assert c.name == "LYSINE"
+    assert c.name in database
+    assert c in database
+    assert c.name not in database.user_defined()
+    assert c not in database.user_defined()
     assert len(c.mobilities()) == 6
     assert len(c.pkas()) == 6
     print(c.mobilities())
     print(c.diffusivity())
     assert c.diffusivity() == pytest.approx(28.60*1e-9*8.314*300/96485)
```

