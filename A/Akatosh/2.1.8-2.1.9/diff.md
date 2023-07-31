# Comparing `tmp/Akatosh-2.1.8.tar.gz` & `tmp/Akatosh-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.8.tar", last modified: Tue Jul 25 01:26:07 2023, max compression
+gzip compressed data, was "Akatosh-2.1.9.tar", last modified: Mon Jul 31 04:42:02 2023, max compression
```

## Comparing `Akatosh-2.1.8.tar` & `Akatosh-2.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 01:26:07.656094 Akatosh-2.1.8/
-drwxrwxrwx   0        0        0        0 2023-07-25 01:26:07.574087 Akatosh-2.1.8/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.8/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    14990 2023-07-25 01:00:44.000000 Akatosh-2.1.8/Akatosh/entity.py
--rw-rw-rw-   0        0        0    14704 2023-07-25 01:21:42.000000 Akatosh-2.1.8/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.8/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-20 06:14:59.000000 Akatosh-2.1.8/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.8/Akatosh/states.py
--rw-rw-rw-   0        0        0     6365 2023-07-20 01:43:52.000000 Akatosh-2.1.8/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:26:07.633136 Akatosh-2.1.8/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-25 01:26:07.647087 Akatosh-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.8/README.md
--rw-rw-rw-   0        0        0      635 2023-07-25 01:24:17.000000 Akatosh-2.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 01:26:07.656094 Akatosh-2.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:02.968763 Akatosh-2.1.9/
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:02.921374 Akatosh-2.1.9/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.9/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    15128 2023-07-31 04:35:52.000000 Akatosh-2.1.9/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    15372 2023-07-31 04:39:50.000000 Akatosh-2.1.9/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.9/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9375 2023-07-31 04:40:30.000000 Akatosh-2.1.9/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.9/Akatosh/states.py
+-rw-rw-rw-   0        0        0     6365 2023-07-20 01:43:52.000000 Akatosh-2.1.9/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:02.954901 Akatosh-2.1.9/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-31 04:42:02.000000 Akatosh-2.1.9/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-31 04:42:02.000000 Akatosh-2.1.9/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:42:02.000000 Akatosh-2.1.9/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 04:42:02.000000 Akatosh-2.1.9/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-31 04:42:02.963513 Akatosh-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.9/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-31 04:41:06.000000 Akatosh-2.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 04:42:02.968763 Akatosh-2.1.9/setup.cfg
```

### Comparing `Akatosh-2.1.8/Akatosh/entity.py` & `Akatosh-2.1.9/Akatosh/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,24 @@
 from .states import State
 
 
 class Entity:
     def __init__(
         self,
         label: str | None = None,
-        create_at: int | float | Callable | None = None,
-        terminate_at: int | float | Callable | None = None,
+        create_at: int
+        | float
+        | Callable[..., int]
+        | Callable[..., float]
+        | None = None,
+        terminate_at: int
+        | float
+        | Callable[..., int]
+        | Callable[..., float]
+        | None = None,
         precursor: Entity | List[Entity] | None = None,
     ) -> None:
         """Create a entity.
 
         Args:
             label (str | None, optional): short description of the entity. Defaults to None.
             create_at (int | float | Callable | None, optional): when the life cycle of this entity should start. Defaults to None, then must call create() method manually.
```

### Comparing `Akatosh-2.1.8/Akatosh/event.py` & `Akatosh-2.1.9/Akatosh/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from .states import State
 from .universe import Mundus
 
 
 class Event:
     def __init__(
         self,
-        at: int | float | Callable,
+        at: int | float | Callable[..., int] | Callable[..., float],
         precursor: Event | List[Event] | None = None,
         action: Callable | None = None,
-        priority: int | float | Callable = 0,
+        priority: int | float | Callable[..., int] | Callable[..., float] = 0,
         label: str | None = None,
         **kwargs,
     ) -> None:
         """Base class for all events.
 
         Args:
-            at (int | float | Callable): the time when the event happens.
+            at (int | float | Callable[...,int] | Callable[...,float]): the time when the event happens.
             precursor (Event | List[Event] | None, optional): the precursor events. Defaults to None.
             action (Callable | None, optional): the actual action of the event, must be defined. Defaults to None.
-            priority (int | float | Callable, optional): the priority of the event. When multiple event happen at the same time, the event with lower priority value will happen first. Defaults to 0.
+            priority (int | float | Callable[...,int] | Callable[...,float], optional): the priority of the event. When multiple event happen at the same time, the event with lower priority value will happen first. Defaults to 0.
             label (str | None, optional): Short descirption of the event. Defaults to None.
         """
         self._id = uuid4().int
         # set the time
         if callable(at):
             self._at = round(at(), Mundus.resolution)
         else:
@@ -82,24 +82,24 @@
                 event.activate()
             except RuntimeError:
                 logger.debug(f"Event {event.label} passed due time.")
         logger.debug(f"Event {self.label} is ended.")
 
     def activate(self, force: bool = False):
         """Activate the event."""
-        
+
         # raise error if the event has already ended
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
 
         # raise warning if the event is cancelled
         if self.cancelled:
             warnings.warn(f"Event {self.label} is cancelled.")
             return
-        
+
         # return if the event is already active
         if self.active:
             return
 
         if force:
             self.state = State.ACTIVE
             self._at = Mundus.now
@@ -115,19 +115,19 @@
 
     def deactivate(self):
         """Deactivate the event.
 
         Raises:
             RuntimeError: raise if the event has already ended.
         """
-        
+
         # raise error if the event has already ended
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
-        
+
         # raise warning if the event is cancelled
         if self.cancelled:
             warnings.warn(f"Event {self.label} is cancelled.")
             return
 
         # return if the event is already inactive
         if self.inactive:
@@ -137,15 +137,15 @@
 
     def cancel(self):
         """Cancel the event. Will not set the follower events to active.
 
         Raises:
             RuntimeError: raise if the event has already ended.
         """
-        
+
         # raise error if the event has already ended
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
 
         # return if the event is already cancelled
         if self.cancelled:
             return
@@ -234,28 +234,28 @@
 
 
 class InstantEvent(Event):
     """Instant event is an event that happens at a specific time and only happens once."""
 
     def __init__(
         self,
-        at: int | float | Callable[..., Any],
+        at: int | float | Callable[..., int] | Callable[..., float],
         precursor: Event | List[Event] | None = None,
         action: Callable[..., Any] | None = None,
-        priority: int | float | Callable[..., Any] = 0,
+        priority: int | float | Callable[..., int] | Callable[..., float] = 0,
         label: str | None = None,
         **kwargs,
     ) -> None:
         """Create a instant event.
 
         Args:
-            at (int | float | Callable): the time when the event happens.
+            at (int | float | Callable[...,int] | Callable[...,float]): the time when the event happens.
             precursor (Event | List[Event] | None, optional): the precursor events. Defaults to None.
             action (Callable | None, optional): the actual action of the event, must be defined. Defaults to None.
-            priority (int | float | Callable, optional): the priority of the event. When multiple event happen at the same time, the event with lower priority value will happen first. Defaults to 0.
+            priority (int | float | Callable[...,int] | Callable[...,float], optional): the priority of the event. When multiple event happen at the same time, the event with lower priority value will happen first. Defaults to 0.
             label (str | None, optional): Short descirption of the event. Defaults to None.
         """
         super().__init__(at, precursor, action, priority, label, **kwargs)
 
     async def _perform(self):
         """Perform the action of the event."""
         if self.state == State.ACTIVE:
@@ -266,17 +266,17 @@
                     self.action()
             Mundus.current_events.remove(self)
             Mundus.past_events.append(self)
             self.end()
 
 
 def instant_event(
-    at: int | float | Callable,
+    at: int | float | Callable[..., int] | Callable[..., float],
     precursor: Event | List[Event] | None = None,
-    priority: int | float | Callable = 0,
+    priority: int | float | Callable[..., int] | Callable[..., float] = 0,
     label: str | None = None,
     **kwargs,
 ):
     """Decorator for creating instant event.
 
     Args:
         at (int | float | Callable): When the event happens.
@@ -297,32 +297,32 @@
 
     return _instant_event
 
 
 class ContinuousEvent(Event):
     def __init__(
         self,
-        at: int | float | Callable[..., Any],
-        interval: int | float | Callable[..., Any],
-        duration: int | float | Callable[..., Any],
+        at: int | float | Callable[..., int] | Callable[..., float],
+        interval: int | float | Callable[..., int] | Callable[..., float],
+        duration: int | float | Callable[..., int] | Callable[..., float],
         precursor: Event | List[Event] | None = None,
         action: Callable[..., Any] | None = None,
-        priority: int | float | Callable[..., Any] = 0,
+        priority: int | float | Callable[..., int] | Callable[..., float] = 0,
         label: str | None = None,
         **kwargs,
     ) -> None:
         """Continous event is an event that happens at a specific time and happens multiple times for a specific duration.
 
         Args:
-            at (int | float | Callable[..., Any]): when the event happens.
-            interval (int | float | Callable[..., Any]): the interval between each action repeat.
-            duration (int | float | Callable[..., Any]): the duration of the event.
+            at (int | float | Callable[...,int] | Callable[...,float]): when the event happens.
+            interval (int | float | Callable[...,int] | Callable[...,float]): the interval between each action repeat.
+            duration (int | float | Callable[...,int] | Callable[...,float]): the duration of the event.
             precursor (Event | List[Event] | None, optional): the precursor events, can be both instant events or continous events. Defaults to None.
             action (Callable[..., Any] | None, optional): the actual action of the event. Defaults to None.
-            priority (int | float | Callable[..., Any], optional): the priority of the event. Defaults to 0.
+            priority (int | float | Callable[...,int] | Callable[...,float], optional): the priority of the event. Defaults to 0.
             label (str | None, optional): short description of the event.. Defaults to None.
         """
         super().__init__(
             at=at,
             precursor=precursor,
             action=action,
             priority=priority,
@@ -348,17 +348,16 @@
                 self._at = round(self.interval + Mundus.now, Mundus.resolution)
             if self.at <= self.till:
                 logger.debug(f"Event {self.label} next step is at {self.at}.")
                 Mundus.future_events.append(self)
                 Mundus.current_events.remove(self)
             else:
                 self.end()
-                
+
     def activate(self, force: bool = False):
-        
         if Mundus.now > self.till:
             warnings.warn(f"Event {self.label} has passed due time.")
         else:
             super().activate(force)
 
     @property
     def interval(self) -> int | float | Callable[..., Any]:
@@ -378,30 +377,30 @@
     @property
     def sub_events(self) -> List[InstantEvent]:
         """Return the sub events of the continous event."""
         return self._sub_events
 
 
 def continuous_event(
-    at: int | float | Callable,
-    interval: int | float | Callable,
-    duration: int | float | Callable,
+    at: int | float | Callable[..., int] | Callable[..., float],
+    interval: int | float | Callable[..., int] | Callable[..., float],
+    duration: int | float | Callable[..., int] | Callable[..., float],
     precursor: Event | List[Event] | None = None,
-    priority: int | float | Callable = 0,
+    priority: int | float | Callable[..., int] | Callable[..., float] = 0,
     label: str | None = None,
     **kwargs,
 ):
     """A decorator for creating continous event.
 
     Args:
-        at (int | float | Callable): when the continuous event starts.
-        interval (int | float | Callable): how frequent the event happens.
-        duration (int | float | Callable): the duration of the event.
+        at (int | float | Callable[...,int] | Callable[...,float]): when the continuous event starts.
+        interval (int | float | Callable[...,int] | Callable[...,float]): how frequent the event happens.
+        duration (int | float | Callable[...,int] | Callable[...,float]): the duration of the event.
         precursor (Event | List[Event] | None, optional): the precursors for this event. Defaults to None.
-        priority (int | float | Callable, optional): the priority for this event. Defaults to 0.
+        priority (int | float | Callable[...,int] | Callable[...,float], optional): the priority for this event. Defaults to 0.
         label (str | None, optional): short description of the event. Defaults to None.
     """
 
     def _continous_event(func: Callable):
         return ContinuousEvent(
             at=at,
             interval=interval,
```

### Comparing `Akatosh-2.1.8/Akatosh/resource.py` & `Akatosh-2.1.9/Akatosh/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 from .logger import logger
 from .universe import Mundus
 
 
 class Resource:
     def __init__(
         self,
-        capacity: int | float | Callable,
-        initial_amount: int | float | Callable | None = None,
+        capacity: int | float | Callable[..., int] | Callable[..., float],
+        initial_amount: int
+        | float
+        | Callable[..., int]
+        | Callable[..., float]
+        | None = None,
         label: str | None = None,
     ) -> None:
         """Resource is a class that represents a resource with capacity and amount, any object can use this resource by calling distribute() and return by calling collect() methods.
 
         Args:
-            capacity (int | float | Callable): the capacity of the resource.
-            initial_amount (int | float | Callable | None, optional): the initial amount of the resource. Defaults to capacity.
+            capacity (int | float | Callable[...,int] | Callable[...,float]): the capacity of the resource.
+            initial_amount (int | float | Callable[...,int] | Callable[...,float] | None, optional): the initial amount of the resource. Defaults to capacity.
             label (str | None, optional): short description of the resource. Defaults to None.
 
         Raises:
             ValueError: raise if initial amount is greater than capacity.
         """
         if callable(capacity):
             self._capacity = capacity()
@@ -37,41 +41,45 @@
                 if initial_amount > self.capacity:
                     raise ValueError("Initial amount is greater than capacity.")
                 else:
                     self._amount = initial_amount
         else:
             self._amount = self.capacity
         self._label = label
-        self._user_records: List[Tuple[object, int | float]] = list() # (user, amount) tracking the usage of individual user
-        self._usage_records: List[Tuple[int | float, int | float]] = list() # (time, amount) tracking the usage of the resource over time
+        self._user_records: List[
+            Tuple[object, int | float]
+        ] = list()  # (user, amount) tracking the usage of individual user
+        self._usage_records: List[
+            Tuple[int | float, int | float]
+        ] = list()  # (time, amount) tracking the usage of the resource over time
 
     def get(self, amount: int | float) -> None:
         """Get the amount of resource from the resource.
 
         Args:
             amount (int | float): the amount of resource to get.
 
         Raises:
             ValueError: raise if amount is greater than the current available amount of resource.
-        """        
+        """
         if amount > self.amount:
             raise ValueError(f"Not enough amount in Resource {self.label}.")
         else:
             self._amount -= amount
             self.usage_records.append((Mundus.now, self.amount))
 
     def put(self, amount: int | float) -> None:
         """Put the amount of resource back to the resource.
 
         Args:
             amount (int | float): the amount of resource to put.
 
         Raises:
             ValueError: raise if amount is greater than the current used amount of resource.
-        """        
+        """
         if amount > self.occupied:
             raise ValueError(f"Not enough capacity in Resource {self.label}.")
         else:
             self._amount += amount
             self.usage_records.append((Mundus.now, self.amount))
 
     def distribute(self, user: object, amount: int | float) -> None:
@@ -79,15 +87,15 @@
 
         Args:
             user (object): the user of the resource.
             amount (int | float): the amount of resource to distribute.
 
         Raises:
             ValueError: raise if amount is greater than the current available amount of resource.
-        """        
+        """
         if amount > self.amount:
             raise ValueError(f"Not enough amount in Resource {self.label}.")
         else:
             self._amount -= amount
             if user in self.users:
                 for index, record in enumerate(self.user_records):
                     if record[0] is user:
@@ -103,15 +111,15 @@
 
         Args:
             user (object): the user of the resource.
             amount (int | float | None, optional): the amount of resource to collect. Defaults to None means collecting all resource used by the user.
 
         Raises:
             ValueError: raise if user is not using the resource or amount is greater than the current used amount of resource.
-        """        
+        """
         if user not in self.users:
             raise ValueError(f"User {user} is not using Resource {self.label}.")
         if amount is None:
             for index, record in enumerate(self.user_records):
                 if record[0] is user:
                     self._amount += record[1]
                     self.usage_records.append((Mundus.now, self.amount))
@@ -133,20 +141,23 @@
                         self._amount += amount
                         self.usage_records.append((Mundus.now, self.amount))
                         logger.debug(
                             f"Resource {self.label} collected {amount} from {user}."
                         )
                         break
 
-    def usage(self, duration: int | float | Callable | None = None):
+    def usage(
+        self,
+        duration: int | float | Callable[..., int] | Callable[..., float] | None = None,
+    ):
         """Return the usage of the resource in the duration.
 
         Args:
-            duration (int | float | Callable | None, optional): the duration to trace back in time. Defaults to None.
-        """        
+            duration (int | float | Callable[...,int] | Callable[...,float] | None, optional): the duration to trace back in time. Defaults to None.
+        """
         if duration:
             if callable(duration):
                 after = Mundus.now - duration()
             else:
                 after = Mundus.now - duration
             if after < 0:
                 after = 0
```

### Comparing `Akatosh-2.1.8/Akatosh/universe.py` & `Akatosh-2.1.9/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.8/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.9/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.8
+Version: 2.1.9
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.8/PKG-INFO` & `Akatosh-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.8
+Version: 2.1.9
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.8/README.md` & `Akatosh-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.8/pyproject.toml` & `Akatosh-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.8"
+version = "2.1.9"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

