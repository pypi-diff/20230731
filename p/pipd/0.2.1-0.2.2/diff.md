# Comparing `tmp/pipd-0.2.1.tar.gz` & `tmp/pipd-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.2.1.tar", last modified: Thu Jul 20 12:07:00 2023, max compression
+gzip compressed data, was "pipd-0.2.2.tar", last modified: Mon Jul 31 09:41:02 2023, max compression
```

## Comparing `pipd-0.2.1.tar` & `pipd-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.889286 pipd-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 12:07:00.889286 pipd-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-20 12:06:47.000000 pipd-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.885286 pipd-0.2.1/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.889286 pipd-0.2.1/pipd/pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/map_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/mix.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/pipes/write_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.889286 pipd-0.2.1/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-20 12:06:47.000000 pipd-0.2.1/pipd/tests/test_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:07:00.885286 pipd-0.2.1/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 12:07:00.000000 pipd-0.2.1/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:07:00.889286 pipd-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-20 12:06:47.000000 pipd-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:02.179296 pipd-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 09:41:02.179296 pipd-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-31 09:40:50.000000 pipd-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:02.171296 pipd-0.2.2/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:02.175296 pipd-0.2.2/pipd/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/map_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/pipes/write_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:02.179296 pipd-0.2.2/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/tests/test_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 09:40:50.000000 pipd-0.2.2/pipd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:02.171296 pipd-0.2.2/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 09:41:02.000000 pipd-0.2.2/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-31 09:41:02.000000 pipd-0.2.2/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:41:02.000000 pipd-0.2.2/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 09:41:02.000000 pipd-0.2.2/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:41:02.179296 pipd-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-31 09:40:50.000000 pipd-0.2.2/setup.py
```

### Comparing `pipd-0.2.1/README.md` & `pipd-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,22 @@
 ```py
 from pipd import Pipe
 
 pipe = Pipe(range(10)).limit(5).log()
 list(pipe) == [0, 1, 2, 3, 4]
 ```
 
+### `repeat`
+```py
+from pipd import Pipe
+
+pipe = Pipe(1, 2, 3).repeat(2)
+list(pipe) == [1, 2, 3, 1, 2, 3]
+```
+
 ### `sleep`
 Useful for debugging a pipeline that runs too fast.
 ```py
 from pipd import Pipe
 
 pipe = Pipe(range(5)).sleep(0.1).log()
 list(pipe) # runs the pipeline
@@ -327,14 +335,16 @@
 
 ### `read_csv`
 ### `write_csv`
 
 ## Create custom `Pipe` object
 
 ```py
+from pipd import Pipe
+
 class PlusOne(Pipe):
 
     def __call__(self, items):
         for item in items:
             yield item + 1
 
 # Usage
```

### Comparing `pipd-0.2.1/pipd/pipe.py` & `pipd-0.2.2/pipd/pipe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import re
 import traceback
-from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Type, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, Type, TypeVar
 
 T = TypeVar("T")
 
 
 def is_iterable(obj):
     try:
         iter(obj)
@@ -23,85 +23,54 @@
     print(message)
 
 
 def camelcase_to_snakecase(name):
     return re.sub(r"([a-z])([A-Z])", r"\1_\2", name).lower()
 
 
-def identity(x: Any) -> Any:
-    return x
-
-
-def compose(source: Callable, target: Callable):
-    def composed(*args):
-        return target(source(*args))
-
-    return composed
-
-
-class Chain:
-    def __init__(self, *iterables):
-        self.iterables = iterables
-
-    def __iter__(self):
-        for iterable in self.iterables:
-            yield from iterable
-
-
 def unpack_iterable(*iterable: Any) -> Iterable[T]:
     if len(iterable) == 1 and is_iterable(iterable[0]):
         iterable = iterable[0]
     return iterable
 
 
 class PipeMeta(type):
     def __init__(cls, name, bases, attrs):
         super().__init__(name, bases, attrs)
         if name != "Pipe":
             cls.register()
 
     def __getattr__(cls, name):
-        """Allows to use meta pipe with no iterable: e.g. Pipe.map"""
+        """Allows to use meta  pipe with no iterable: e.g. Pipe.map"""
 
         def method(*args, **kwargs):
             return cls().__getattr__(name)(*args, **kwargs)
 
         return method
 
 
 class Pipe(metaclass=PipeMeta):
-    _iterable: Iterable = []
-    _function: Callable = identity
-    _handler: Callable = log_traceback_and_continue
     _pipes: Dict[str, Type[Pipe]] = {}
 
-    def __init__(self, *iterable, handler: Optional[Callable] = None):
-        self._iterable = unpack_iterable(*iterable)
-        self._handler = handler or self._handler  # type: ignore
-        self._function = identity  # type: ignore
+    def __init__(self, *iterable, handler: Callable = log_traceback_and_continue):
+        self.iter: Iterable = unpack_iterable(*iterable)
+        self.handler = handler
 
-    def __call__(self, iterable: Iterable[Any]) -> Iterator[Any]:
-        return self._function(iterable)
+    def __call__(self, *iterable: Iterable[Any]) -> Iterable[Any]:
+        yield from unpack_iterable(*iterable)
 
     def __iter__(self):
-        for item in self(self._iterable):
+        for item in self.iter:
             try:
                 yield item
             except Exception as e:
-                self._handler(e)
-
-    def new(self):
-        return Pipe()
+                self.handler(e)
 
     def __or__(self, other: Pipe):
-        new = other.new()
-        new._function = compose(self, other)
-        new._iterable = Chain(self._iterable, other._iterable)
-        new._handler = self._handler
-        return new
+        return Chain(self, other)
 
     def __getattr__(self, name):
         def method(*args, **kwargs):
             other = self._pipes[name](*args, **kwargs)
             return self | other
 
         return method
@@ -111,7 +80,19 @@
         pass
 
     @classmethod
     def register(cls, target: Optional[Type] = None, name: Optional[str] = None):
         pipe_name = name or camelcase_to_snakecase(cls.__name__)
         target = target or Pipe
         target._pipes[pipe_name] = cls
+
+
+class Chain(Pipe):
+    def __init__(self, pipe0: Pipe, pipe1: Pipe) -> None:
+        self.pipe0 = pipe0
+        self.pipe1 = pipe1
+
+    def __iter__(self):
+        return self.pipe1(self.pipe0)
+
+    def __call__(self, *items):
+        return self.pipe1(self.pipe0(*items))
```

### Comparing `pipd-0.2.1/pipd/pipes/__init__.py` & `pipd-0.2.2/pipd/pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `pipd-0.2.1/pipd/pipes/batch.py` & `pipd-0.2.2/pipd/pipes/batch.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class Batch(Pipe):
     def __init__(self, size: int, partial: bool = True) -> None:
         self.size = size
         self.partial = partial
 
-    def __call__(self, items: Iterable[T]) -> Iterator[List[T]]:
+    def __call__(self, items: Iterable[T]) -> Iterator[List[T]]:  # type: ignore
         batch = []
         for item in items:
             batch.append(item)
             if len(batch) == self.size:
                 yield batch
                 batch = []
         if batch and self.partial:
```

### Comparing `pipd-0.2.1/pipd/pipes/filter.py` & `pipd-0.2.2/pipd/pipes/filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 class Filter(Pipe):
     def __init__(self, fn: Callable[[T], bool], *args, **kwargs) -> None:
         self.fn = lambda x: (x, fn(x))
         self.args = args
         self.kwargs = kwargs
 
-    def __call__(self, items: Iterable[T]) -> Iterator[T]:
+    def __call__(self, items: Iterable[T]) -> Iterator[T]:  # type: ignore
         for item, keep in Map(self.fn, *self.args, **self.kwargs)(items):  # type: ignore
             if keep:  # type: ignore
                 yield item  # type: ignore
```

### Comparing `pipd-0.2.1/pipd/pipes/filter_cached.py` & `pipd-0.2.2/pipd/pipes/filter_cached.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class FilterCached(Pipe):
     def __init__(self, filepath: str, key: Optional[Callable] = None) -> None:
         self.filepath = filepath
         self.key = key
 
-    def __call__(self, items: Iterable[T]) -> Iterator[T]:
+    def __call__(self, items: Iterable[T]) -> Iterator[T]:  # type: ignore
         cache = (
             set(read_lines(self.filepath)) if os.path.exists(self.filepath) else set()
         )
         with open(self.filepath, "a") as file:
             for item in items:
                 value = str(self.key(item) if self.key is not None else item)
                 if value not in cache:
```

### Comparing `pipd-0.2.1/pipd/pipes/map.py` & `pipd-0.2.2/pipd/pipes/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         assert mode in ["multithread", "multiprocess"]
         self.fn = fn
         self.num_workers = num_workers
         self.buffer = buffer
         self.mode = mode
         self.handler = handler
 
-    def __call__(self, items: Iterable[T]) -> Iterator[U]:
+    def __call__(self, items: Iterable[T]) -> Iterator[U]:  # type: ignore
         if self.num_workers == 0:
             for item in items:
                 try:
                     yield self.fn(item)
                 except Exception as e:
                     self.handler(e)
             return
```

### Comparing `pipd-0.2.1/pipd/pipes/mix.py` & `pipd-0.2.2/pipd/pipes/mix.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,62 +2,54 @@
 from typing import Callable, Iterable, Iterator, Optional, Sequence, TypeVar
 
 from pipd import Pipe
 
 T = TypeVar("T")
 
 
-def mix_iters(
-    *iterators: Iterable[T],
-    repeat: bool = False,
-    repeat_callback: Optional[Callable] = None,
-    random: bool = False,
-    weights: Optional[Sequence[float]] = None,
-) -> Iterator[T]:
-    assert weights is None or random, "weights only works with random=True"
-
-    iters = [iter(it) for it in iterators]
-    ids = list(range(len(iterators)))
-
-    while True:
-        # Choose random iter ids if random=True
-        ids_curr = (
-            choices(ids, k=len(iterators), weights=weights or [1] * len(iterators))
-            if random
-            else ids
-        )
-
-        for i in ids_curr:
-            try:
-                yield next(iters[i])
-            except StopIteration:
-                if repeat:
-                    # Reset iterator and add item
-                    iters[i] = iter(iterators[i])
-                    yield next(iters[i])
-                    # Notify callback with pipe index
-                    if repeat_callback is not None:
-                        repeat_callback(i)
-                else:
-                    return
-
-
 class Mix(Pipe):
     def __init__(
         self,
         *iters,
         repeat: bool = False,
         repeat_callback: Optional[Callable] = None,
         random: bool = False,
         weights: Optional[Sequence[float]] = None,
         **kwargs,
     ):
-        super().__init__(
-            mix_iters(
-                *iters,
-                repeat=repeat,
-                repeat_callback=repeat_callback,
-                random=random,
-                weights=weights,
-            ),
-            **kwargs,
-        )
+        assert weights is None or random, "weights only works with random=True"
+        self.iters = iters
+        self.repeat = repeat
+        self.repeat_callback = repeat_callback
+        self.random = random
+        self.weights = weights
+
+    def __iter__(self):
+        return self(*self.iters)
+
+    def __call__(self, *iterators: Iterable[T]) -> Iterator[T]:  # type: ignore
+        iters = [iter(it) for it in iterators]
+        ids = list(range(len(iterators)))
+
+        while True:
+            # Choose random iter ids if random=True
+            ids_curr = (
+                choices(
+                    ids, k=len(iterators), weights=self.weights or [1] * len(iterators)
+                )
+                if self.random
+                else ids
+            )
+
+            for i in ids_curr:
+                try:
+                    yield next(iters[i])
+                except StopIteration:
+                    if self.repeat:
+                        # Reset iterator and add item
+                        iters[i] = iter(iterators[i])
+                        yield next(iters[i])
+                        # Notify callback with pipe index
+                        if self.repeat_callback is not None:
+                            self.repeat_callback(i)
+                    else:
+                        return
```

### Comparing `pipd-0.2.1/pipd/pipes/read_csv.py` & `pipd-0.2.2/pipd/pipes/read_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.2.1/pipd/pipes/read_files.py` & `pipd-0.2.2/pipd/pipes/read_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         watch: bool = False,
         shuffle: bool = False,
     ) -> None:
         self.cache_filepath = cache_filepath
         self.watch = watch
         self.shuffle = shuffle
 
-    def __call__(self, items: Iterable[str]) -> Iterator[str]:
+    def __call__(self, items: Iterable[str]) -> Iterator[str]:  # type: ignore
         for filepath in items:
             files = []
             if self.cache_filepath is not None:
                 if os.path.exists(self.cache_filepath):
                     files = list(read_lines(filepath=self.cache_filepath))
                 else:
                     files = glob.glob(filepath)
```

### Comparing `pipd-0.2.1/pipd/pipes/read_lines.py` & `pipd-0.2.2/pipd/pipes/read_lines.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,10 +20,10 @@
                 yield line.strip()
 
 
 class ReadLines(Pipe):
     def __init__(self, watch: bool = False) -> None:
         self.watch = watch
 
-    def __call__(self, items: Iterable[str]) -> Iterator[str]:
+    def __call__(self, items: Iterable[str]) -> Iterator[str]:  # type: ignore
         for filepath in items:
             yield from read_lines(filepath=filepath, watch=self.watch)
```

### Comparing `pipd-0.2.1/pipd/pipes/shuffle.py` & `pipd-0.2.2/pipd/pipes/shuffle.py`

 * *Files identical despite different names*

### Comparing `pipd-0.2.1/pipd/pipes/side.py` & `pipd-0.2.2/pipd/pipes/side.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ) -> None:
         assert mode in ["multithread", "multiprocess"]
         self.fn = fn
         self.num_workers = num_workers
         self.mode = mode
         self.handler = handler
 
-    def __call__(self, items: Iterable[T]) -> Iterator[T]:
+    def __call__(self, items: Iterable[T]) -> Iterator[T]:  # type: ignore
         if self.num_workers == 0:
             for item in items:
                 try:
                     self.fn(item)
                 except Exception as e:
                     self.handler(e)
                 yield item
```

### Comparing `pipd-0.2.1/pipd/pipes/write_csv.py` & `pipd-0.2.2/pipd/pipes/write_csv.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from pipd import Pipe
 
 
 class WriteCSV(Pipe):
     def __init__(self, filepath: str) -> None:
         self.filepath = filepath
 
-    def __call__(
+    def __call__(  # type: ignore
         self, items: Iterable[Union[Dict[str, Any], Sequence[Any]]]
-    ) -> Iterator[Union[Dict[str, Any], Sequence[Any]]]:
+    ) -> Iterator[Union[Dict[str, Any], Sequence[Any]]]:  # type: ignore
         import csv
 
         with open(self.filepath, "w", newline="") as f:
             writer = csv.writer(f)
             for i, item in enumerate(items):
                 if isinstance(item, dict):
                     if i == 0:  # Write headers only for the first dictionary item
```

### Comparing `pipd-0.2.1/pipd/tests/test_pipe.py` & `pipd-0.2.2/pipd/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `pipd-0.2.1/pipd/tests/test_pipes.py` & `pipd-0.2.2/pipd/tests/test_pipes.py`

 * *Files 10% similar despite different names*

```diff
@@ -181,14 +181,22 @@
         os.remove(f1.name)
         os.remove(f2.name)
 
 
 def test_mix_pipe():
     from pipd import Mix
 
+    pipe = Mix([0, 0, 0], [1, 1, 1], [2, 2, 2])
+    assert list(pipe) == [0, 1, 2, 0, 1, 2, 0, 1, 2]
+    assert list(pipe) == [0, 1, 2, 0, 1, 2, 0, 1, 2]
+
+    pipe = Mix(Pipe([0, 0, 0]), Pipe([1, 1, 1]), Pipe([2, 2, 2]))
+    assert list(pipe) == [0, 1, 2, 0, 1, 2, 0, 1, 2]
+    assert list(pipe) == [0, 1, 2, 0, 1, 2, 0, 1, 2]
+
     pipe = Pipe([0, 1, 2, 3])
     pipe1 = Pipe(["a", "b", "c", "d", "e"])
     merged = Mix(pipe, pipe1)
 
     it = iter(merged)
     assert next(it) == 0
     assert next(it) == "a"
@@ -213,10 +221,7 @@
     assert next(it) == "c"
     assert next(it) == 3
     assert next(it) == "d"
     assert next(it) == 0
     assert next(it) == "e"
     assert next(it) == 1
     assert next(it) == "a"
-
-    items = list(Pipe.mix(Pipe([0, 1, 2, 3]), Pipe(["a", "b", "c", "d", "e"])))
-    assert items == [0, "a", 1, "b", 2, "c", 3, "d"]
```

### Comparing `pipd-0.2.1/pipd.egg-info/SOURCES.txt` & `pipd-0.2.2/pipd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 pipd/__init__.py
 pipd/pipe.py
+pipd/utils.py
 pipd.egg-info/PKG-INFO
 pipd.egg-info/SOURCES.txt
 pipd.egg-info/dependency_links.txt
 pipd.egg-info/top_level.txt
 pipd/pipes/__init__.py
 pipd/pipes/batch.py
 pipd/pipes/filter.py
```

