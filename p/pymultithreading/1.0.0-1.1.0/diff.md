# Comparing `tmp/pymultithreading-1.0.0.tar.gz` & `tmp/pymultithreading-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-1.0.0.tar", last modified: Sat Jul  8 21:11:13 2023, max compression
+gzip compressed data, was "pymultithreading-1.1.0.tar", last modified: Mon Jul 31 15:58:12 2023, max compression
```

## Comparing `pymultithreading-1.0.0.tar` & `pymultithreading-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 21:11:13.758590 pymultithreading-1.0.0/
--rw-rw-rw-   0        0        0       98 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2019 2023-07-08 21:11:13.758590 pymultithreading-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1217 2023-07-01 08:57:20.000000 pymultithreading-1.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-1.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-08 21:11:13.743572 pymultithreading-1.0.0/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-1.0.0/multithreading/__init__.py
--rw-rw-rw-   0        0        0    11589 2023-07-08 21:10:47.000000 pymultithreading-1.0.0/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-07-08 21:11:13.757598 pymultithreading-1.0.0/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2019 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-07-08 21:11:13.000000 pymultithreading-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       29 2023-07-08 21:08:12.000000 pymultithreading-1.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       20 2023-07-08 21:08:06.000000 pymultithreading-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 21:11:13.758590 pymultithreading-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-07-08 21:11:08.000000 pymultithreading-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:58:12.129175 pymultithreading-1.1.0/
+-rw-rw-rw-   0        0        0       98 2023-07-31 15:58:10.000000 pymultithreading-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2019 2023-07-31 15:58:12.128167 pymultithreading-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1217 2023-07-01 08:57:20.000000 pymultithreading-1.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-1.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:58:12.114489 pymultithreading-1.1.0/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-1.1.0/multithreading/__init__.py
+-rw-rw-rw-   0        0        0    13792 2023-07-31 15:57:14.000000 pymultithreading-1.1.0/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:58:12.128167 pymultithreading-1.1.0/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2019 2023-07-31 15:58:12.000000 pymultithreading-1.1.0/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-31 15:58:12.000000 pymultithreading-1.1.0/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 15:58:12.000000 pymultithreading-1.1.0/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-31 15:58:12.000000 pymultithreading-1.1.0/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-31 15:58:12.000000 pymultithreading-1.1.0/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-07-31 15:58:10.000000 pymultithreading-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       29 2023-07-08 21:08:12.000000 pymultithreading-1.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       20 2023-07-08 21:08:06.000000 pymultithreading-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 15:58:12.129175 pymultithreading-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-07-31 15:58:00.000000 pymultithreading-1.1.0/setup.py
```

### Comparing `pymultithreading-1.0.0/PKG-INFO` & `pymultithreading-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 1.0.0
+Version: 1.1.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-1.0.0/README.md` & `pymultithreading-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pymultithreading-1.0.0/build.py` & `pymultithreading-1.1.0/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-1.0.0/multithreading/process.py` & `pymultithreading-1.1.0/multithreading/process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # process.py
 
 import datetime as dt
 import threading
 import time
-from abc import ABCMeta
 from typing import (
     Any, Optional, Dict, Callable, ClassVar,
     Iterable, Union, TypeVar, Generic
 )
 
 from attrs import define
 
@@ -15,25 +14,24 @@
 
 __all__ = [
     "Caller",
     "CallDefinition",
     "CallsResults",
     "multi_threaded_call",
     "multi_threaded_defined_call",
-    "wait_call_completion",
+    "await_completion",
     "ProcessTime",
-    "ProcessInfo",
     "find_caller",
-    "CallResults"
+    "CallResult"
 ]
 
-@define(repr=False)
+@define(repr=False, frozen=True)
 @represent
-class ProcessInfo(metaclass=ABCMeta):
-    """A class to contain the info of a call to the callers."""
+class ProcessTime:
+    """A class to contain the info of a call to the results."""
 
     start: dt.datetime
     end: dt.datetime
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(properties=['time'])
 
     @property
@@ -42,51 +40,44 @@
         Returns the time duration of the call.
 
         :return: The call time.
         """
 
         return self.end - self.start
     # end time
-# end CallInfo
-
-class ProcessTime(ProcessInfo):
-    """A class to contain the info of a call to the callers."""
 # end ProcessTime
 
-_ReturnType = TypeVar("_ReturnType")
+_RT = TypeVar("_RT")
 
-@define(repr=False)
+@define(repr=False, frozen=True)
 @represent
-class CallResults(Generic[_ReturnType]):
-    """A class to represent a container for the call results."""
+class CallResult(Generic[_RT]):
+    """A class to represent a container for the call result."""
 
-    returns: Optional[_ReturnType] = None
+    returns: Optional[_RT] = None
     thread: Optional[threading.Thread] = None
-    start: Optional[dt.datetime] = None
-    end: Optional[dt.datetime] = None
+    time: Optional[ProcessTime] = None
 
-    __modifiers__: ClassVar[Modifiers] = Modifiers(
-        excluded=["thread"], force=True
-    )
-# end CallResults
+    __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=['thread'])
+# end CallResult
 
 @represent
-class Caller(Generic[_ReturnType]):
+class Caller(Generic[_RT]):
     """A class to represent a function caller object."""
 
-    __modifiers__ = Modifiers(excluded=["thread", "results"])
+    __modifiers__ = Modifiers(properties=['result'])
 
     __slots__ = (
         "target", "identifier", "args", "kwargs",
-        "thread", "results", "complete", "called"
+        "_thread", "_result", "complete", "called"
     )
 
     def __init__(
             self,
-            target: Callable[..., _ReturnType],
+            target: Callable[..., _RT],
             identifier: Optional[Any] = None,
             args: Optional[Iterable[Any]] = None,
             kwargs: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         Defines the class attributes.
 
@@ -100,19 +91,19 @@
         self.args = args or ()
         self.kwargs = kwargs or {}
         self.identifier = identifier or self.target
 
         self.complete = False
         self.called = False
 
-        self.thread: Optional[threading.Thread] = None
-        self.results: Optional[CallResults[_ReturnType]] = None
+        self._thread: Optional[threading.Thread] = None
+        self._result: Optional[CallResult[_RT]] = None
     # end __init__
 
-    def __call__(self, *args: Any, **kwargs: Any) -> CallResults[_ReturnType]:
+    def __call__(self, *args: Any, **kwargs: Any) -> CallResult[_RT]:
         """
         Calls the function and saves the response.
 
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
 
         :return: The returned response.
@@ -121,43 +112,78 @@
         start = dt.datetime.now()
 
         self.args = args or self.args
         self.kwargs = kwargs or self.kwargs
 
         self.called = True
 
-        returns: _ReturnType = self.target(
-            *self.args, **self.kwargs
-        )
+        returns: _RT = self.target(*self.args, **self.kwargs)
 
         self.complete = True
 
         end = dt.datetime.now()
 
-        self.results = CallResults[_ReturnType](
-            start=start, end=end,
+        self._result = CallResult[_RT](
+            time=ProcessTime(start=start, end=end),
             thread=self.thread, returns=returns
         )
 
-        return self.results
+        return self.result
     # end __call__
 
+    @property
+    def thread(self) -> Optional[threading.Thread]:
+        """
+        Returns the thread object.
+
+        :return: The thread of the caller.
+        """
+
+        return self._thread
+    # end thread
+
+    @property
+    def result(self) -> Optional[CallResult[_RT]]:
+        """
+        Returns the result object.
+
+        :return: The result of the caller.
+        """
+
+        return self._result
+    # end result
+
+    def start(self) -> None:
+        """Starts the process."""
+
+        self._thread = threading.Thread(target=self)
+
+        self.thread.start()
+    # end start
+
     def reset(self) -> None:
         """Rests the values from the calls."""
 
         self.called = False
         self.complete = False
     # end reset
+
+    def clean(self) -> None:
+        """Cleans the caller."""
+
+        self._thread = None
+        self._result = None
+    # end clean
 # end Caller
 
 def find_caller(callers: Iterable[Caller], identifier: Any) -> Caller:
     """
     Finds the caller object by its identifier
 
-    :param callers: The callers in which to search.
+    :param callers: The results in which to search.
     :param identifier: The identifier of the caller to return.
 
     :return: The matching caller object.
     """
 
     for caller in callers:
         if caller.identifier == identifier:
@@ -172,15 +198,15 @@
     )
 # end find_caller
 
 def find_results(callers: Iterable[Caller], identifier: Any) -> Caller:
     """
     Finds the caller object by its identifier
 
-    :param callers: The callers in which to search.
+    :param callers: The results in which to search.
     :param identifier: The identifier of the caller to return.
 
     :return: The matching caller object.
     """
 
     for caller in callers:
         if caller.identifier == identifier:
@@ -198,120 +224,149 @@
 @represent
 class CallDefinition:
     """A class to represent the call definition."""
 
     WAIT = True
     RESET_BEFORE = True
     RESET_AFTER = False
+    CLEAN_BEFORE = True
+    CLEAN_AFTER = False
+    DYNAMIC = False
 
-    SLEEP = 0.005
+    SLEEP = 0.0001
 
-    __slots__ = "wait", "reset_before", "reset_after", "sleep"
+    __slots__ = (
+        "wait", "reset_before", "reset_after", "sleep",
+        "clean_before", "clean_after", "dynamic"
+    )
 
     def __init__(
             self,
             wait: Optional[bool] = None,
             reset_before: Optional[bool] = None,
             reset_after: Optional[bool] = None,
+            clean_before: Optional[bool] = None,
+            clean_after: Optional[bool] = None,
+            dynamic: Optional[bool] = None,
             sleep: Optional[Union[int, float, dt.timedelta]] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param wait: The value to wait.
         :param reset_before: The value to reset before running.
         :param reset_after: The value to reset after running.
+        :param clean_before: The value to clean before running.
+        :param clean_after: The value to clean after running.
+        :param dynamic: The value to enable dynamic sleep time.
         :param sleep: The time for sleeping.
         """
 
         if wait is None:
             wait = self.WAIT
         # end if
 
         if sleep is None:
             sleep = self.SLEEP
         # end if
 
+        if dynamic is None:
+            dynamic = self.DYNAMIC
+        # end if
+
         if reset_before is None:
             reset_before = self.RESET_BEFORE
         # end if
 
         if reset_after is None:
             reset_after = self.RESET_AFTER
         # end if
 
+        if clean_after is None:
+            clean_after = self.CLEAN_AFTER
+        # end if
+
+        if clean_before is None:
+            clean_before = self.CLEAN_BEFORE
+        # end if
+
         self.wait = wait
         self.reset_before = reset_before
         self.reset_after = reset_after
+        self.clean_after = clean_after
+        self.clean_before = clean_before
+        self.dynamic = dynamic
         self.sleep = sleep
     # end __init__
 # end CallDefinition
 
-@define(repr=False)
+@define(repr=False, frozen=True)
 @represent
 class CallsResults:
-    """A class to contain the info of a call to the callers."""
+    """A class to contain the info of a call to the results."""
 
-    callers: Dict[Caller, CallResults]
-    total: ProcessTime
+    results: Dict[Caller, CallResult]
+    time: ProcessTime
     waiting: ProcessTime
     definition: CallDefinition
 
+    __modifiers__ = Modifiers(excluded=['waiting'])
+
     def caller(self, identifier: Any) -> Caller:
         """
         Finds the caller object by its identifier
 
         :param identifier: The identifier of the caller to return.
 
         :return: The matching caller object.
         """
 
-        for caller in self.callers:
+        for caller in self.results:
             if caller.identifier == identifier:
                 return caller
             # end if
         # end for
 
         raise ValueError(
             f"Cannot find a caller object with the identifier: "
             f"{identifier}. valid identifiers are: "
-            f"{', '.join(str(caller.identifier) for caller in self.callers)}"
+            f"{', '.join(str(caller.identifier) for caller in self.results)}"
         )
     # end caller
 
-    def results(self, identifier: Any) -> CallResults:
+    def result(self, identifier: Any) -> CallResult:
         """
         Finds the caller object by its identifier
 
         :param identifier: The identifier of the caller to return.
 
         :return: The matching caller object.
         """
 
-        for caller, results in self.callers.items():
+        for caller, result in self.results.items():
             if caller.identifier == identifier:
-                return results
+                return result
             # end if
         # end for
 
         raise ValueError(
             f"Cannot find a caller object with the identifier: "
             f"{identifier}. valid identifiers are: "
-            f"{', '.join(str(caller.identifier) for caller in self.callers)}"
+            f"{', '.join(str(caller.identifier) for caller in self.results)}"
         )
-    # end results
+    # end result
 # end CallsResults
 
 def validate_callers(data: Any) -> Iterable[Caller]:
     """
-    Validates the data as callers.
+    Validates the data as results.
 
     :param data: The data to validate.
 
-    :return: The valid callers data.
+    :return: The valid results data.
     """
 
     try:
         if not all(isinstance(value, Caller) for value in data):
             raise ValueError
         # end if
 
@@ -321,120 +376,145 @@
         raise type(e)(
             f"Callers must be an iterable of "
             f"{Caller} objects, not: {data}."
         ) from e
     # end try
 # end validate_callers
 
-def wait_call_completion(
+def await_completion(
         callers: Iterable[Caller], definition: CallDefinition
 ) -> ProcessTime:
     """
     Waits for the calls to complete.
 
     :param callers: The call objects for the functions.
     :param definition: The call definition object.
 
-    :return: The waiting results.
+    :return: The waiting result.
     """
 
     start = dt.datetime.now()
 
-    while (
-        definition.wait and
-        not all(caller.complete for caller in callers)
-    ):
-        if isinstance(definition.sleep, dt.timedelta):
-            sleep = definition.sleep.total_seconds()
+    if isinstance(definition.sleep, dt.timedelta):
+        sleep = definition.sleep.total_seconds()
+
+    else:
+        sleep = definition.sleep
+    # end if
+
+    while True:
+        current = time.time()
+
+        if not (
+            definition.wait and
+            not all(caller.complete for caller in callers)
+        ):
+            break
+        # end if
+
+        if definition.dynamic:
+            if isinstance(definition.sleep, dt.timedelta):
+                sleep = definition.sleep.total_seconds()
 
-        else:
-            sleep = definition.sleep
+            else:
+                sleep = definition.sleep
+            # end if
         # end if
 
-        time.sleep(sleep)
+        time.sleep(max((0, sleep - (time.time() - current))))
     # end while
 
     end = dt.datetime.now()
 
     return ProcessTime(start=start, end=end)
-# end wait_call_completion
+# end await_completion
 
 def multi_threaded_defined_call(
         callers: Iterable[Caller],
         definition: Optional[CallDefinition] = None
 ) -> CallsResults:
     """
-    Calls the functions with the callers.
+    Calls the functions with the results.
 
     :param callers: The call objects for the functions.
     :param definition: The call definition object.
 
-    :return: The call results.
+    :return: The call result.
     """
 
     start = dt.datetime.now()
 
     callers = validate_callers(data=callers)
 
     if definition is None:
         definition = CallDefinition()
     # end if
 
-    if definition.reset_before:
-        for caller in callers:
-            caller.reset()
-        # end for
+    if definition.clean_before:
+        [caller.clean() for caller in callers]
     # end if
 
-    for caller in callers:
-        caller.thread = threading.Thread(target=caller)
+    if definition.reset_before:
+        [caller.reset() for caller in callers]
+    # end if
 
-        caller.thread.start()
-    # end for
+    [caller.start() for caller in callers]
 
-    waiting = wait_call_completion(
+    waiting = await_completion(
         callers=callers, definition=definition
     )
 
-    results = {caller: caller.results for caller in callers}
+    results = {caller: caller.result for caller in callers}
 
     if definition.reset_after:
-        for caller in callers:
-            caller.reset()
-        # end for
+        [caller.reset() for caller in callers]
+    # end if
+
+    if definition.clean_after:
+        [caller.clean() for caller in callers]
     # end if
 
     end = dt.datetime.now()
 
     return CallsResults(
-        callers=results, total=ProcessTime(start=start, end=end),
-        definition=definition, waiting=waiting
+        results=results,
+        time=ProcessTime(start=start, end=end),
+        definition=definition,
+        waiting=waiting
     )
 # end multi_threaded_defined_call
 
 def multi_threaded_call(
         callers: Iterable[Caller],
         wait: Optional[bool] = None,
         reset_before: Optional[bool] = None,
         reset_after: Optional[bool] = None,
+        clean_before: Optional[bool] = None,
+        clean_after: Optional[bool] = None,
+        dynamic: Optional[bool] = None,
         sleep: Optional[Union[int, float, dt.timedelta]] = None
 ) -> CallsResults:
     """
-    Calls the functions with the callers.
+    Calls the functions with the results.
 
     :param callers: The call objects for the functions.
     :param wait: The value to wait.
     :param reset_before: The value to reset before running.
     :param reset_after: The value to reset after running.
+    :param clean_before: The value to clean before running.
+    :param clean_after: The value to clean after running.
+    :param dynamic: The value to enable dynamic sleep time.
     :param sleep: The time for sleeping.
 
-    :return: The call results.
+    :return: The call result.
     """
 
     return multi_threaded_defined_call(
         callers=callers,
         definition=CallDefinition(
             wait=wait, reset_after=reset_after,
-            reset_before=reset_before, sleep=sleep
+            reset_before=reset_before, sleep=sleep,
+            clean_before=clean_before, dynamic=dynamic,
+            clean_after=clean_after
         )
     )
 # end multi_threaded_call
```

### Comparing `pymultithreading-1.0.0/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-1.1.0/pymultithreading.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 1.0.0
+Version: 1.1.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-1.0.0/pyproject.toml` & `pymultithreading-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '1.0.0'
+version = '1.1.0'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-1.0.0/setup.py` & `pymultithreading-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='1.0.0',
+        version='1.1.0',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

