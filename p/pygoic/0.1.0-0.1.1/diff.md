# Comparing `tmp/pygoic-0.1.0.tar.gz` & `tmp/pygoic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoic-0.1.0.tar", max compression
+gzip compressed data, was "pygoic-0.1.1.tar", max compression
```

## Comparing `pygoic-0.1.0.tar` & `pygoic-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-18 04:57:47.642522 pygoic-0.1.0/LICENSE
--rw-r--r--   0        0        0     5277 2023-07-18 15:05:16.921605 pygoic-0.1.0/README.md
--rw-r--r--   0        0        0      331 2023-07-18 15:05:16.921605 pygoic-0.1.0/pygoic/__init__.py
--rw-r--r--   0        0        0     7784 2023-07-18 15:05:16.921605 pygoic-0.1.0/pygoic/channel.py
--rw-r--r--   0        0        0     8196 2023-07-18 15:05:16.921605 pygoic-0.1.0/pygoic/context.py
--rw-r--r--   0        0        0     4198 2023-07-18 15:05:16.921605 pygoic-0.1.0/pygoic/executor.py
--rw-r--r--   0        0        0     1339 2023-07-18 15:05:16.921605 pygoic-0.1.0/pygoic/sync.py
--rw-r--r--   0        0        0     2332 2023-07-18 15:05:16.921605 pygoic-0.1.0/pygoic/time.py
--rw-r--r--   0        0        0      340 2023-07-18 04:57:47.642522 pygoic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 pygoic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-18 04:57:47.642522 pygoic-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5137 2023-07-31 10:03:55.998753 pygoic-0.1.1/README.md
+-rw-r--r--   0        0        0      321 2023-07-31 10:03:55.998753 pygoic-0.1.1/pygoic/__init__.py
+-rw-r--r--   0        0        0     8341 2023-07-31 10:03:55.998753 pygoic-0.1.1/pygoic/channel.py
+-rw-r--r--   0        0        0     8196 2023-07-18 15:05:16.921605 pygoic-0.1.1/pygoic/context.py
+-rw-r--r--   0        0        0     2982 2023-07-31 10:03:55.998753 pygoic-0.1.1/pygoic/executor.py
+-rw-r--r--   0        0        0     2609 2023-07-31 10:03:55.998753 pygoic-0.1.1/pygoic/linked.py
+-rw-r--r--   0        0        0     1339 2023-07-18 15:05:16.921605 pygoic-0.1.1/pygoic/sync.py
+-rw-r--r--   0        0        0     2332 2023-07-18 15:05:16.921605 pygoic-0.1.1/pygoic/time.py
+-rw-r--r--   0        0        0      383 2023-07-31 10:11:19.628743 pygoic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5682 1970-01-01 00:00:00.000000 pygoic-0.1.1/PKG-INFO
```

### Comparing `pygoic-0.1.0/LICENSE` & `pygoic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygoic-0.1.0/README.md` & `pygoic-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,64 @@
 # pygoic
 
-**pygoic** is a simple, golang style, concurrency python library on asyncio.
+**pygoic** is a Go-like asynchronous concurrency library for python based on asyncio.
+
+[![Python](https://img.shields.io/pypi/pyversions/pygoic.svg)](https://pypi.org/project/pygoic)
+[![PyPI](https://badge.fury.io/py/pygoic.svg)](https://pypi.org/project/pygoic)
+
 
 ```python
 import asyncio
-from pygoic import go, do, Chan, select
-from pygoic import Background, WithCancel
+from pygoic import go, do, Chan, select, After
 
-ctx, cancel = WithCancel(Background())
 ch = Chan()
 
 async def foo1():
-    await ch.send('hi')
-    print('foo1')
-    cancel()
-    
+    await asyncio.sleep(0.02)
+    await ch.send('a')
+    await ch.send('b')
+    ch.close()
+
 async def foo2():
-    await asyncio.sleep(0.01)
-    print('foo2: 0')
-    id, x, ok = await select(ch, ctx.done())
-    if id == 0:
-        print('foo2: ch')
-    elif id == 1:
-        print('foo2: ctx')
-    
+    id, x, ok = await select(ch, After(0.01))   # gives (1, time(), True)
+    print(id, x, ok)
+
 async def foo3():
-    await ctx.done().recv()
-    print('foo3')
-    
-go(foo1())
-go(foo2())
-go(foo3())
-do(ctx.done().recv())
+    async for x in ch:    # loop until chan is closed and empty
+        print(x)
 
-### Output:
-# foo2: 0
-# foo2: ch
-# foo1
-# foo3
+go(foo1())
+go(foo2())                      
+do(foo3())                # block until foo3 done
 
 ```
 
-pygoic allows you to levarage coroutine in python extremely easily. There's no need to manually deal with a lot of trival and error-prone details, especially about event loop, which is designed to be so anti-human. This library will try its best to help you forgot those unpleasant things.
+pygoic allows you to levarage coroutine in python extremely easily. There's no need to manually deal with trival and error-prone details, especially about event loop, which is designed to be so anti-human. This library will try its best to help you forgot those unpleasant things.
 
-Follow a few simple principles, and you will get a golang-like concurrent programming experience. 
+Follow a few simple principles, and you will get a Go-like concurrent programming experience. 
 
 
 ## Principles
-1. Do not call any **blocking** operation inside coroutines. If you can't avoid it, use `delegate`.  
-    *Common blocking operations include but are not limited to:*
-    * `requests.post`
-    * `time.sleep`
-    * `queue.Queue.get`
-    * `threading.Lock.acquire`
-2. `do` can only be called out of coroutines, while `go` is for anywhere.
 
+1. Don't call any **blocking** operation inside coroutines. If not avoidable, please use `delegate`.
+2. Function `do` can only be called out of coroutines, while `go` is for anywhere.
 
 
 ## Installation
 
 ```console
-$ python -m pip install pygoic
+$ pip install pygoic
 ```
 
-pygoic officially supports Python 3.8+.
 
+## Quick Tutorial
 
-## Tutorial
+### go and do
 
-### **go** and **do**
-
-`go` accepts a coroutine object (call of async funcion) as parameter, and start executing it concurrently (not accurate). You can expect `go` to behave the same as in golang. Except it will return an `awaitable`, which can be used with `await` or `do` when need to wait.
+`go` accepts a coroutine object (call of async funcion) as parameter, and start executing it concurrently (not accurate). You can expect `go` to behave the same as in Golang. Except it will return an `awaitable`, which can be consumed by `await` or `do` if needed.
 
 `do` also accepts a coroutine object as parameter. The difference is that it will **block** until coroutine object is finished, and will return the result.
 
 ```python
 import asyncio
 from pygoic import go, do
 
@@ -88,24 +72,24 @@
     print('foo2')
     print(await x)
     return 'world'
     
 go(foo1(1))
 print(do(foo2()))
 
-### Output:
+### Output ###
 # foo2
 # foo1: 1
 # foo1: 2
 # hello
 # world
 
 ```
 
-### **delegate**
+### delegate
 
 `delegate` accepts a function and the args to call this function. It will execute this funcion in a thread pool, and return an `awaitable`. Looks like it is an asynchronous operation.
 
 ```python
 import time
 from pygoic import  go, do, delegate
 
@@ -117,65 +101,66 @@
     await delegate(time.sleep, 0.01) 
     print('foo2')
     
 x = go(foo1())
 go(foo2())
 do(x)
 
-### Output:
+### Output ###
 # foo2
 # foo1
 
 ```
 
-### **Chan** and **select**
+### Chan and select
+
+Behavior of `Chan` is similar to that in Golang. 
 
-Behavior of `Chan` is similar to that in golang. `select` accepts `Chan`s as parameters, and returns when one of the `Chan`s can be read.
+`select` accepts `Chan`s as parameters, and returns when any of the `Chan` operations is unblocked. 
 
 ```python
 from pygoic import Chan, select, go, do
 
 ch1 = Chan()
 ch2 = Chan()
-done = Chan()
 
 async def foo1():
-    await ch1.send('world')
-    print('foo1')
+    await ch1.send('hi')
+    print('foo1: 0')
+    await ch2.send('a')
+    await ch2.send('b')
     ch2.close()
 
 async def foo2():
-    id, x, ok = await select(ch1, ch2)
+    id, item, ok = await select(ch1, ch2)
     if id == 0:
-        print(f'foo2: ch1')
+        print(f'foo2: 0, ch1')
     elif id == 1:
-        print(f'foo2: ch2')
+        print(f'foo2: 0, ch2')
 
-    id, x, ok = await select(ch1, ch2)
-    if id == 0:
-        print(f'foo2: ch1')
-    elif id == 1:
-        print(f'foo2: ch2')
+    async for item in ch2:
+        print(f'foo2: 1, {item}')
 
-    done.close()
+    print('foo2: 2')
     
 go(foo1())
-go(foo2())
-do(done.recv())
+do(foo2())
 
-### Output:
-# foo2: ch1
-# foo1
-# foo2: ch2
+### Output ###
+# foo2: 0, ch1
+# foo1: 0
+# foo2: 1, a
+# foo2: 1, b
+# foo2: 2
 
 ```
 
-### **Context**
+### Context
 
-You can expect `Context` to behave the same as in golang.
+You can expect `Context` to behave the same as in Golang.
 
 ```python
 import asyncio
 from pygoic import select, go, do
 from pygoic import Background, WithCancel, WithTimeout, WithValue
 
 ctx1 = WithValue(Background(), 'k', 'v')
@@ -186,68 +171,68 @@
     await asyncio.sleep(0.02)
     cancel()
     
 async def foo2():
     print(ctx3.value('k'))
     go(foo1())
     
-    id, x, ok = await select(ctx2.done(), ctx3.done())
+    id, item, ok = await select(ctx2.done(), ctx3.done())
     if id == 0:
         print('foo2: ctx2')
     elif id == 1:
         print('foo2: ctx3')
     
 go(foo1())
 go(foo2())
 do(ctx3.done().recv())
 
-### Output:
+### Output ###
 # v
 # foo2: ctx2
 
 ```
 
-### **After**, **AfterFunc** and **Timer**
+### After, AfterFunc and Timer
 
-Behave similar to golang.
+Behave the same as in Golang.
 
 ```python
 from pygoic import go, do, select, Chan
 from pygoic import After, AfterFunc
 
 ch = Chan()
 
 async def foo1():
     ch.close()
     
 async def foo2():
     AfterFunc(0.015, foo1)
-    id, x, ok = await select(After(0.01), ch)
+    id, item, ok = await select(After(0.01), ch)
     if id == 0:
         print('foo2: after')
     elif id == 1:
         print('foo2: ch')
 
-    id, x, ok = await select(After(0.01), ch)
+    id, item, ok = await select(After(0.01), ch)
     if id == 0:
         print('foo2: after')
     elif id == 1:
         print('foo2: ch')
 
 do(foo2())
 
-### Output:
+### Output ###
 # foo2: after
 # foo2: ch
 
 ```
 
-### **WaitGroup**
+### WaitGroup
 
-Behave similar to golang.
+Behave the same as in Golang.
 
 ```python
 import asyncio
 from pygoic import go, do, WaitGroup
 
 wg = WaitGroup(2)
 
@@ -263,14 +248,14 @@
     print('foo2: 0')
     await wg.wait()
     print('foo2: 1')
 
 go(foo2())
 do(foo1())
 
-### Output:
+### Output ###
 # foo2: 0
 # foo1: 0
 # foo2: 1
 # foo1: 1
 
 ```
```

### Comparing `pygoic-0.1.0/pygoic/context.py` & `pygoic-0.1.1/pygoic/context.py`

 * *Files identical despite different names*

### Comparing `pygoic-0.1.0/pygoic/executor.py` & `pygoic-0.1.1/pygoic/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,18 @@
 
 from __future__ import annotations
 import asyncio
 import threading
 from asyncio import AbstractEventLoop, Future as AsyncFuture
 from concurrent.futures import Future as ConcurrentFuture, ThreadPoolExecutor
-from typing import Any, Awaitable, Callable, Generic, Optional, TypeVar
+from typing import Any, Awaitable, Callable, Optional, TypeVar
 
 
 T = TypeVar('T')
 
-# TODO: only awaitable is enought
-
-class CoFuture(Generic[T]):
-    def __init__(self, future: ConcurrentFuture[T], loop: AbstractEventLoop):
-        self._future = future
-        self._loop = loop
-
-    def cancelled(self) -> bool:
-        return self._future.cancelled()
-    
-    def running(self) -> bool:
-        return self._future.running()
-    
-    def done(self) -> bool:
-        return self._future.done()
-    
-    def result(self, timeout: Optional[float] = None) -> T:
-        if asyncio._get_running_loop() is not None:
-            raise RuntimeError(f"Not allow to call `CoFuture.result` inside a event loop.")
-        else:
-            return self._future.result(timeout)
-        
-    def exception(self, timeout: Optional[float] = None) -> Optional[BaseException]:
-        if asyncio._get_running_loop() is not None:
-            raise RuntimeError(f"Not allow to call `CoFuture.exception` inside a event loop.")
-        else:
-            return self._future.exception(timeout)
-
-    def __await__(self):
-        afut = asyncio.wrap_future(self._future, loop=self._loop)
-        return afut.__await__()
-
-    __iter__ = __await__
-
-
 
 class GoroutineExecutor:
     def __init__(self):
         self._lock = threading.Lock()
         self._loop = asyncio.new_event_loop()
         self._worker: Optional[threading.Thread] = None
         self._pool: Optional[ThreadPoolExecutor] = None
@@ -105,20 +70,19 @@
         with self._lock:
             if self._worker and self._worker.is_alive():
                 self._loop.call_soon_threadsafe(self._loop.stop)
             if self._pool:
                 self._pool.shutdown(wait=False)
     
     
-    def go(self, coro: Awaitable[T]) -> CoFuture[T]:
+    def go(self, coro: Awaitable[T]) -> Awaitable[T]:
         loop = self._get_event_loop()
-        afut = asyncio.ensure_future(coro, loop=loop)
-        cfut = ConcurrentFuture()
-        loop.call_soon_threadsafe(self._future_callback, afut, cfut)
-        return CoFuture(cfut, loop)
+        future = asyncio.ensure_future(coro, loop=loop)
+        loop.call_soon_threadsafe(lambda: None)
+        return future
 
     
     def do(self, coro: Awaitable[T]) -> T:
         if asyncio._get_running_loop() is not None:
             raise RuntimeError(f"Not allow to call `do` inside a event loop.")
         else:
             self._init_worker()
@@ -136,7 +100,8 @@
 
 
 _executor = GoroutineExecutor()
 _get_event_loop = _executor._get_event_loop
 go = _executor.go
 do = _executor.do
 delegate = _executor.delegate
+
```

### Comparing `pygoic-0.1.0/pygoic/sync.py` & `pygoic-0.1.1/pygoic/sync.py`

 * *Files identical despite different names*

### Comparing `pygoic-0.1.0/pygoic/time.py` & `pygoic-0.1.1/pygoic/time.py`

 * *Files identical despite different names*

### Comparing `pygoic-0.1.0/PKG-INFO` & `pygoic-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,80 @@
 Metadata-Version: 2.1
 Name: pygoic
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: A Go-like asynchronous concurrency library.
 License: MIT
 Author: Xiaodong Yang
 Author-email: yxdong.cc@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # pygoic
 
-**pygoic** is a simple, golang style, concurrency python library on asyncio.
+**pygoic** is a Go-like asynchronous concurrency library for python based on asyncio.
+
+[![Python](https://img.shields.io/pypi/pyversions/pygoic.svg)](https://pypi.org/project/pygoic)
+[![PyPI](https://badge.fury.io/py/pygoic.svg)](https://pypi.org/project/pygoic)
+
 
 ```python
 import asyncio
-from pygoic import go, do, Chan, select
-from pygoic import Background, WithCancel
+from pygoic import go, do, Chan, select, After
 
-ctx, cancel = WithCancel(Background())
 ch = Chan()
 
 async def foo1():
-    await ch.send('hi')
-    print('foo1')
-    cancel()
-    
+    await asyncio.sleep(0.02)
+    await ch.send('a')
+    await ch.send('b')
+    ch.close()
+
 async def foo2():
-    await asyncio.sleep(0.01)
-    print('foo2: 0')
-    id, x, ok = await select(ch, ctx.done())
-    if id == 0:
-        print('foo2: ch')
-    elif id == 1:
-        print('foo2: ctx')
-    
+    id, x, ok = await select(ch, After(0.01))   # gives (1, time(), True)
+    print(id, x, ok)
+
 async def foo3():
-    await ctx.done().recv()
-    print('foo3')
-    
-go(foo1())
-go(foo2())
-go(foo3())
-do(ctx.done().recv())
+    async for x in ch:    # loop until chan is closed and empty
+        print(x)
 
-### Output:
-# foo2: 0
-# foo2: ch
-# foo1
-# foo3
+go(foo1())
+go(foo2())                      
+do(foo3())                # block until foo3 done
 
 ```
 
-pygoic allows you to levarage coroutine in python extremely easily. There's no need to manually deal with a lot of trival and error-prone details, especially about event loop, which is designed to be so anti-human. This library will try its best to help you forgot those unpleasant things.
+pygoic allows you to levarage coroutine in python extremely easily. There's no need to manually deal with trival and error-prone details, especially about event loop, which is designed to be so anti-human. This library will try its best to help you forgot those unpleasant things.
 
-Follow a few simple principles, and you will get a golang-like concurrent programming experience. 
+Follow a few simple principles, and you will get a Go-like concurrent programming experience. 
 
 
 ## Principles
-1. Do not call any **blocking** operation inside coroutines. If you can't avoid it, use `delegate`.  
-    *Common blocking operations include but are not limited to:*
-    * `requests.post`
-    * `time.sleep`
-    * `queue.Queue.get`
-    * `threading.Lock.acquire`
-2. `do` can only be called out of coroutines, while `go` is for anywhere.
 
+1. Don't call any **blocking** operation inside coroutines. If not avoidable, please use `delegate`.
+2. Function `do` can only be called out of coroutines, while `go` is for anywhere.
 
 
 ## Installation
 
 ```console
-$ python -m pip install pygoic
+$ pip install pygoic
 ```
 
-pygoic officially supports Python 3.8+.
 
+## Quick Tutorial
 
-## Tutorial
+### go and do
 
-### **go** and **do**
-
-`go` accepts a coroutine object (call of async funcion) as parameter, and start executing it concurrently (not accurate). You can expect `go` to behave the same as in golang. Except it will return an `awaitable`, which can be used with `await` or `do` when need to wait.
+`go` accepts a coroutine object (call of async funcion) as parameter, and start executing it concurrently (not accurate). You can expect `go` to behave the same as in Golang. Except it will return an `awaitable`, which can be consumed by `await` or `do` if needed.
 
 `do` also accepts a coroutine object as parameter. The difference is that it will **block** until coroutine object is finished, and will return the result.
 
 ```python
 import asyncio
 from pygoic import go, do
 
@@ -104,24 +88,24 @@
     print('foo2')
     print(await x)
     return 'world'
     
 go(foo1(1))
 print(do(foo2()))
 
-### Output:
+### Output ###
 # foo2
 # foo1: 1
 # foo1: 2
 # hello
 # world
 
 ```
 
-### **delegate**
+### delegate
 
 `delegate` accepts a function and the args to call this function. It will execute this funcion in a thread pool, and return an `awaitable`. Looks like it is an asynchronous operation.
 
 ```python
 import time
 from pygoic import  go, do, delegate
 
@@ -133,65 +117,66 @@
     await delegate(time.sleep, 0.01) 
     print('foo2')
     
 x = go(foo1())
 go(foo2())
 do(x)
 
-### Output:
+### Output ###
 # foo2
 # foo1
 
 ```
 
-### **Chan** and **select**
+### Chan and select
+
+Behavior of `Chan` is similar to that in Golang. 
 
-Behavior of `Chan` is similar to that in golang. `select` accepts `Chan`s as parameters, and returns when one of the `Chan`s can be read.
+`select` accepts `Chan`s as parameters, and returns when any of the `Chan` operations is unblocked. 
 
 ```python
 from pygoic import Chan, select, go, do
 
 ch1 = Chan()
 ch2 = Chan()
-done = Chan()
 
 async def foo1():
-    await ch1.send('world')
-    print('foo1')
+    await ch1.send('hi')
+    print('foo1: 0')
+    await ch2.send('a')
+    await ch2.send('b')
     ch2.close()
 
 async def foo2():
-    id, x, ok = await select(ch1, ch2)
+    id, item, ok = await select(ch1, ch2)
     if id == 0:
-        print(f'foo2: ch1')
+        print(f'foo2: 0, ch1')
     elif id == 1:
-        print(f'foo2: ch2')
+        print(f'foo2: 0, ch2')
 
-    id, x, ok = await select(ch1, ch2)
-    if id == 0:
-        print(f'foo2: ch1')
-    elif id == 1:
-        print(f'foo2: ch2')
+    async for item in ch2:
+        print(f'foo2: 1, {item}')
 
-    done.close()
+    print('foo2: 2')
     
 go(foo1())
-go(foo2())
-do(done.recv())
+do(foo2())
 
-### Output:
-# foo2: ch1
-# foo1
-# foo2: ch2
+### Output ###
+# foo2: 0, ch1
+# foo1: 0
+# foo2: 1, a
+# foo2: 1, b
+# foo2: 2
 
 ```
 
-### **Context**
+### Context
 
-You can expect `Context` to behave the same as in golang.
+You can expect `Context` to behave the same as in Golang.
 
 ```python
 import asyncio
 from pygoic import select, go, do
 from pygoic import Background, WithCancel, WithTimeout, WithValue
 
 ctx1 = WithValue(Background(), 'k', 'v')
@@ -202,68 +187,68 @@
     await asyncio.sleep(0.02)
     cancel()
     
 async def foo2():
     print(ctx3.value('k'))
     go(foo1())
     
-    id, x, ok = await select(ctx2.done(), ctx3.done())
+    id, item, ok = await select(ctx2.done(), ctx3.done())
     if id == 0:
         print('foo2: ctx2')
     elif id == 1:
         print('foo2: ctx3')
     
 go(foo1())
 go(foo2())
 do(ctx3.done().recv())
 
-### Output:
+### Output ###
 # v
 # foo2: ctx2
 
 ```
 
-### **After**, **AfterFunc** and **Timer**
+### After, AfterFunc and Timer
 
-Behave similar to golang.
+Behave the same as in Golang.
 
 ```python
 from pygoic import go, do, select, Chan
 from pygoic import After, AfterFunc
 
 ch = Chan()
 
 async def foo1():
     ch.close()
     
 async def foo2():
     AfterFunc(0.015, foo1)
-    id, x, ok = await select(After(0.01), ch)
+    id, item, ok = await select(After(0.01), ch)
     if id == 0:
         print('foo2: after')
     elif id == 1:
         print('foo2: ch')
 
-    id, x, ok = await select(After(0.01), ch)
+    id, item, ok = await select(After(0.01), ch)
     if id == 0:
         print('foo2: after')
     elif id == 1:
         print('foo2: ch')
 
 do(foo2())
 
-### Output:
+### Output ###
 # foo2: after
 # foo2: ch
 
 ```
 
-### **WaitGroup**
+### WaitGroup
 
-Behave similar to golang.
+Behave the same as in Golang.
 
 ```python
 import asyncio
 from pygoic import go, do, WaitGroup
 
 wg = WaitGroup(2)
 
@@ -279,15 +264,15 @@
     print('foo2: 0')
     await wg.wait()
     print('foo2: 1')
 
 go(foo2())
 do(foo1())
 
-### Output:
+### Output ###
 # foo2: 0
 # foo1: 0
 # foo2: 1
 # foo1: 1
 
 ```
```

