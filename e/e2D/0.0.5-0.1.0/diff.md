# Comparing `tmp/e2D-0.0.5.tar.gz` & `tmp/e2D-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2D-0.0.5.tar", last modified: Mon Jul 31 16:27:42 2023, max compression
+gzip compressed data, was "e2D-0.1.0.tar", last modified: Mon Jul 31 16:53:51 2023, max compression
```

## Comparing `e2D-0.0.5.tar` & `e2D-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:27:42.485185 e2D-0.0.5/
--rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3085 2023-07-31 16:27:42.485185 e2D-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2492 2023-07-31 14:47:36.000000 e2D-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:27:42.461237 e2D-0.0.5/e2D/
--rw-rw-rw-   0        0        0    49399 2023-07-31 14:52:29.000000 e2D-0.0.5/e2D/__init__.py
--rw-rw-rw-   0        0        0     3899 2023-07-31 14:51:50.000000 e2D-0.0.5/e2D/pg.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:27:42.483183 e2D-0.0.5/e2D.egg-info/
--rw-rw-rw-   0        0        0     3085 2023-07-31 16:27:42.000000 e2D-0.0.5/e2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-31 16:27:42.000000 e2D-0.0.5/e2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:27:42.000000 e2D-0.0.5/e2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 16:27:42.000000 e2D-0.0.5/e2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 16:27:42.000000 e2D-0.0.5/e2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      729 2023-07-31 16:27:42.487186 e2D-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:51.593240 e2D-0.1.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3081 2023-07-31 16:53:51.593240 e2D-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2023-07-31 16:30:45.000000 e2D-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:51.567230 e2D-0.1.0/e2D/
+-rw-rw-rw-   0        0        0    39663 2023-07-31 16:41:56.000000 e2D-0.1.0/e2D/__init__.py
+-rw-rw-rw-   0        0        0    10446 2023-07-31 16:52:35.000000 e2D-0.1.0/e2D/envs.py
+-rw-rw-rw-   0        0        0     3899 2023-07-31 14:51:50.000000 e2D-0.1.0/e2D/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:51.591232 e2D-0.1.0/e2D.egg-info/
+-rw-rw-rw-   0        0        0     3081 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-07-31 16:53:51.595228 e2D-0.1.0/setup.cfg
```

### Comparing `e2D-0.0.5/LICENSE` & `e2D-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `e2D-0.0.5/PKG-INFO` & `e2D-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.0.5
+Version: 0.1.0
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,18 +30,18 @@
 - Simple API for ease of use, suitable for both beginners and experienced developers.
 
 ## Installation
 
 You can install e2D using pip:
 
 ```bash
-pip install e2Dpy
+pip install e2D
 ```
 ```bash
-pip3 install e2Dpy
+pip3 install e2D
 ```
 
 ## Getting Started
 
 To get started with e2D, follow these steps:
 
 1. Create a new Python project or navigate to your existing project directory.
```

### Comparing `e2D-0.0.5/README.md` & `e2D-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 - Simple API for ease of use, suitable for both beginners and experienced developers.
 
 ## Installation
 
 You can install e2D using pip:
 
 ```bash
-pip install e2Dpy
+pip install e2D
 ```
 ```bash
-pip3 install e2Dpy
+pip3 install e2D
 ```
 
 ## Getting Started
 
 To get started with e2D, follow these steps:
 
 1. Create a new Python project or navigate to your existing project directory.
```

### Comparing `e2D-0.0.5/e2D/__init__.py` & `e2D-0.1.0/e2D/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,40 +3,31 @@
 import random as _rnd
 
 PI = _mt.pi
 HALF_PI = PI/2
 QUARTER_PI = PI/4
 DOUBLE_PI = PI*2
 
-DEFAULT_MOUSE_BUTTON_MODE = 0
-OVER_MOUSE_BUTTON_MODE = 1
-CLICKED_MOUSE_BUTTON_MOVE = 2
-
-CALLBACK_MODE_ON_PRESSED = 0
-CALLBACK_MODE_ON_RELEASED = 1
-
-NUM_TYPE = int|float
-ARRAY_TYPE = list|tuple
 
 class Vector2D:
-    def __init__(self, x:NUM_TYPE=0, y:NUM_TYPE=0) -> None:
+    def __init__(self, x:int|float=0, y:int|float=0) -> None:
         self.x = x
         self.y = y
 
-    def distance_to(self, object:"float|int|Vector2D|ARRAY_TYPE", squared:bool=True) -> NUM_TYPE:
+    def distance_to(self, object:"float|int|Vector2D|list|tuple", squared:bool=True) -> int|float:
         """
         # Calculate the distance between the current Vector2D object and another object.
 
         # Parameters:
-            object (float or int or Vector2D or ARRAY_TYPE): The other object to which the distance is calculated.
+            object (float or int or Vector2D or list|tuple): The other object to which the distance is calculated.
             squared (bool, optional): If True, return the squared distance. If False, return the actual distance.
                                       Default is True.
 
         # Returns:
-            NUM_TYPE: The squared distance between the current Vector2D object and the other object if `squared` is True,
+            int|float: The squared distance between the current Vector2D object and the other object if `squared` is True,
                       otherwise the actual distance.
 
         # Example:
             point1 = Vector2D(0, 0)
 
             point2 = Vector2D(3, 4)
 
@@ -56,23 +47,23 @@
 
             The result is returned as the squared distance if `squared` is True, or as the actual distance if `squared` is False.
         """
         object = self.__normalize__(object)
         d = (self.x - object.x)**2 + (self.y - object.y)**2
         return (d**(1/2) if squared else d)
 
-    def angle_to(self, object:"float|int|Vector2D|ARRAY_TYPE") -> NUM_TYPE:
+    def angle_to(self, object:"float|int|Vector2D|list|tuple") -> int|float:
         """
         # Calculate the angle between the current Vector2D object and another object.
 
         # Parameters:
-            object (float or int or Vector2D or ARRAY_TYPE): The other object to which the angle is calculated.
+            object (float or int or Vector2D or list|tuple): The other object to which the angle is calculated.
 
         # Returns:
-            NUM_TYPE: The angle in radians between the current Vector2D object and the other object.
+            int|float: The angle in radians between the current Vector2D object and the other object.
 
         # Example:
             point1 = Vector2D(0, 0)
 
             point2 = Vector2D(1, 1)
 
             angle = point1.angle_to(point2)
@@ -86,21 +77,21 @@
             (object) using the `atan2` function from the `math` module.
 
             The result is returned as the angle in radians.
         """
         object = self.__normalize__(object)
         return _mt.atan2(object.y - self.y, object.x - self.x)
 
-    def point_from_degs(self, rad:NUM_TYPE, radius:NUM_TYPE) -> "Vector2D":
+    def point_from_degs(self, rad:int|float, radius:int|float) -> "Vector2D":
         """
         # Calculate a new Vector2D point from the current point based on an angle in radians and a radius.
 
         # Parameters:
-            rad (NUM_TYPE): The angle in radians.
-            radius (NUM_TYPE): The distance from the current point.
+            rad (int|float): The angle in radians.
+            radius (int|float): The distance from the current point.
 
         # Returns:
             Vector2D: A new Vector2D point calculated from the current point.
 
         # Example:
             point1 = Vector2D(0, 0)
 
@@ -151,15 +142,15 @@
         return Vector2D(self.x, self.y)
 
     def absolute_round(self, n=1) -> "Vector2D":
         """
         # Perform an "absolute round" operation on the Vector2D object.
 
         # Parameters:
-            n (NUM_TYPE, optional): The numeric value to scale the "absolute rounded" vector. Default is 1.
+            n (int|float, optional): The numeric value to scale the "absolute rounded" vector. Default is 1.
 
         # Returns:
             Vector2D: The "absolute rounded" Vector2D object scaled by the provided numeric value.
 
         # Example:
             vector1 = Vector2D(3.3, -4.7)
 
@@ -188,20 +179,20 @@
 
             Note: The "absolute round" operation does not perform standard mathematical rounding; instead, it ensures the resulting
             vector points in the same direction as the original vector but has non-negative components.
         """
         s_abs = abs(self)
         return self.no_zero_div_error(s_abs, "zero") * n
 
-    def floor(self, n:NUM_TYPE=1) -> "Vector2D":
+    def floor(self, n:int|float=1) -> "Vector2D":
         """
         # Round down the components of the Vector2D object to the nearest integer or the specified numeric value.
 
         # Parameters:
-            n (NUM_TYPE, optional): The numeric value to round down the components. Default is 1.
+            n (int|float, optional): The numeric value to round down the components. Default is 1.
 
         # Returns:
             Vector2D: A new Vector2D object with the components rounded down to the nearest integer or the specified numeric value.
 
         # Example:
             vector1 = Vector2D(3.3, 4.7)
 
@@ -228,20 +219,20 @@
             If the provided numeric value (n) is not an integer, it will be converted to an integer before performing the rounding.
 
             Note: The floor operation always moves the components toward negative infinity, regardless of whether the original
             components are positive or negative.
         """
         return self.__floor__(n)
 
-    def ceil(self, n:NUM_TYPE=1) -> "Vector2D":
+    def ceil(self, n:int|float=1) -> "Vector2D":
         """
         # Round up the components of the Vector2D object to the nearest integer or the specified numeric value.
 
         # Parameters:
-            n (NUM_TYPE, optional): The numeric value to round up the components. Default is 1.
+            n (int|float, optional): The numeric value to round up the components. Default is 1.
 
         # Returns:
             Vector2D: A new Vector2D object with the components rounded up to the nearest integer or the specified numeric value.
 
         # Example:
             vector1 = Vector2D(3.3, 4.7)
 
@@ -268,23 +259,23 @@
             If the provided numeric value (n) is not an integer, it will be converted to an integer before performing the rounding.
 
             Note: The ceil operation always moves the components toward positive infinity, regardless of whether the original
             components are positive or negative.
         """
         return self.__ceil__(n)
 
-    def randomize(start:"NUM_TYPE|Vector2D|None"=None, end:"NUM_TYPE|Vector2D|None"=None) -> "Vector2D": #type: ignore
+    def randomize(start:"int|float|Vector2D|None"=None, end:"int|float|Vector2D|None"=None) -> "Vector2D": #type: ignore
         """
         # Generate a random Vector2D point within the specified range.
 
         # Parameters:
-            start (NUM_TYPE or Vector2D or None, optional): The starting point of the range.
+            start (int|float or Vector2D or None, optional): The starting point of the range.
                                                         Default is None, which corresponds to (0, 0).
                                                         If numeric, both x and y will have the same value.
-            end (NUM_TYPE or Vector2D or None, optional): The ending point of the range.
+            end (int|float or Vector2D or None, optional): The ending point of the range.
                                                         Default is None, which corresponds to (1, 1).
                                                         If numeric, both x and y will have the same value.
 
         # Returns:
             Vector2D: A new random Vector2D point within the specified range.
 
         # Example:
@@ -304,19 +295,19 @@
             The function first checks if `start` and `end` are Vector2D objects. If not, it creates new Vector2D objects
             based on the numeric values provided or the default values.
 
             It then generates random x and y coordinates in the range [0, 1) using the `random()` function from the `random` module.
             These random values are then scaled by (end - start) and added to the start point to obtain the final random Vector2D point.
         """
         if not isinstance(start, Vector2D):
-            if type(start) in NUM_TYPE: start = Vector2D(start, start) #type: ignore
+            if type(start) in int|float: start = Vector2D(start, start) #type: ignore
             elif type(start) == None: start = Vector2D(0,0)
             else: raise Exception(f"\nArg start must be in [Vector2D, int, float, tuple, list] not a [{type(start)}]\n")
         if not isinstance(end, Vector2D):
-            if type(end) in NUM_TYPE: end = Vector2D(end, end) #type: ignore
+            if type(end) in int|float: end = Vector2D(end, end) #type: ignore
             elif type(end) == None: end = Vector2D(1,1)
             else: raise Exception(f"\nArg end must be in [Vector2D, int, float, tuple, list] not a [{type(end)}]\n")
         return start + Vector2D(_rnd.random(), _rnd.random()) * (end - start)
 
     def mid_point_to(self, *objects) -> float:
         """
         # Calculate the midpoint between the current Vector2D object and one or more other Vector2D objects.
@@ -387,15 +378,15 @@
             If sort is True, the intersection points are sorted by their distance to the starting point (self).
 
             If return_empty is True, the function includes None in the result for lines without intersection points.
 
             The function returns a list of intersection points as Vector2D objects.
         """
         ray = self() + self_final_point() #type: ignore
-        def lineLineIntersect(P0, P1, Q0, Q1) -> tuple[NUM_TYPE, NUM_TYPE] | None:
+        def lineLineIntersect(P0, P1, Q0, Q1) -> tuple[int|float, int|float] | None:
             d = (P1[0]-P0[0]) * (Q1[1]-Q0[1]) + (P1[1]-P0[1]) * (Q0[0]-Q1[0])
             if d == 0:
                 return None
             t = ((Q0[0]-P0[0]) * (Q1[1]-Q0[1]) +
                  (Q0[1]-P0[1]) * (Q0[0]-Q1[0])) / d
             u = ((Q0[0]-P0[0]) * (P1[1]-P0[1]) +
                  (Q0[1]-P0[1]) * (P0[0]-P1[0])) / d
@@ -403,22 +394,22 @@
                 return P1[0] * t + P0[0] * (1-t), P1[1] * t + P0[1] * (1-t)
             return None
         collisions = [Vector2D(*line) if line else None for line in [lineLineIntersect(line1[1](), line1[0](), ray[:2], ray[2:]) for line1 in lines] if line or return_empty]
         if sort:
             collisions.sort(key=lambda x: self.distance_to(x, False)) #type: ignore
         return collisions
 
-    def normalize(self, max:NUM_TYPE=1, min:NUM_TYPE=0) -> "Vector2D":
+    def normalize(self, max:int|float=1, min:int|float=0) -> "Vector2D":
         """
         # Normalize the Vector2D object to a new magnitude defined by max while preserving its direction.
 
         # Parameters:
-            max (NUM_TYPE, optional): The new magnitude to which the Vector2D object will be scaled.
+            max (int|float, optional): The new magnitude to which the Vector2D object will be scaled.
                                       Default is 1.
-            min (NUM_TYPE, optional): The minimum magnitude. If provided, the Vector2D object will not be scaled
+            min (int|float, optional): The minimum magnitude. If provided, the Vector2D object will not be scaled
                                       below this value. Default is 0.
 
         # Returns:
             Vector2D: A new Vector2D object with the scaled magnitude.
 
         # Example:
             vector = Vector2D(3, 4)
@@ -435,20 +426,20 @@
             If the current magnitude is not zero, it creates a new Vector2D object with magnitude max using
             point_from_degs method and the angle_to method to preserve the direction.
 
             If the current magnitude is zero, it returns a new zero vector (VectorZero.copy()).
         """
         return Vector2D(min, min).point_from_degs(Vector2D(min, min).angle_to(self), max) if Vector2D(min, min).distance_to(self) != 0 else VectorZero.copy()
 
-    def no_zero_div_error(self:"Vector2D", n:"NUM_TYPE|Vector2D", error_mode:str="zero") -> "Vector2D":
+    def no_zero_div_error(self:"Vector2D", n:"int|float|Vector2D", error_mode:str="zero") -> "Vector2D":
         """
         # Handle division between the Vector2D object and a numeric value or another Vector2D object.
 
         # Parameters:
-            n (NUM_TYPE or Vector2D): The numeric value or Vector2D object for division.
+            n (int|float or Vector2D): The numeric value or Vector2D object for division.
             error_mode (str, optional): The mode to handle division by zero scenarios.
                                         - "zero" (default): Return a Vector2D object with zeros for both components.
                                         - "null": Return a Vector2D object with the original x or y component if available,
                                                    otherwise, return NaN (Not a Number) for the component.
 
         # Returns:
             Vector2D: A new Vector2D object after division or handling division by zero scenarios.
@@ -478,109 +469,109 @@
                 - If n's x or y component is zero, the function returns a Vector2D object with zeros for the corresponding component
                   if error_mode is "zero".
                 - If error_mode is "null", the function returns a Vector2D object with the original x or y component if available,
                   otherwise, return NaN (Not a Number) for the component.
 
             If n is neither a numeric value nor a Vector2D object, the function raises an exception.
         """
-        if isinstance(n, NUM_TYPE):
+        if isinstance(n, int|float):
             if n == 0:
                 return Vector2D(0 if error_mode == "zero" else (self.x if error_mode == "null" else _mt.nan), 0 if error_mode == "zero" else (self.y if error_mode == "null" else _mt.nan))
             else:
                 return self / n
         elif isinstance(n, Vector2D):
             return Vector2D((0 if error_mode == "zero" else (self.x if error_mode == "null" else _mt.nan)) if n.x == 0 else self.x / n.x, (0 if error_mode == "zero" else (self.y if error_mode == "null" else _mt.nan)) if n.y == 0 else self.y / n.y)
         else:
             raise Exception(f"\nArg n must be in [Vector2D, int, float, tuple, list] not a [{type(n)}]\n")
 
     def __str__(self) -> str:
         return f"{self.x}, {self.y}"
 
-    def __sub__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __sub__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         object = self.__normalize__(object)
         return Vector2D(self.x - object.x, self.y - object.y)
 
-    def __add__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __add__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         object = self.__normalize__(object)
         return Vector2D(self.x + object.x, self.y + object.y)
 
-    def __mod__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __mod__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         object = self.__normalize__(object)
         return Vector2D(self.x % object.x, self.y % object.y)
 
-    def __radd__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __radd__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         return self.__add__(object)
 
     def __repr__(self) -> str:
         return f"x:{self.x}\ty:{self.y}"
 
     def __call__(self, need_tuple=False) -> list|tuple:
         return (self.x, self.y) if need_tuple else [self.x, self.y]
 
-    def __truediv__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __truediv__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         object = self.__normalize__(object)
         return Vector2D(self.x / object.x, self.y / object.y)
 
-    def __floordiv__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __floordiv__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         object = self.__normalize__(object)
         return Vector2D(self.x // object.x, self.y // object.y)
     
     def __abs__(self) -> "Vector2D":
         return Vector2D(abs(self.x), abs(self.y))
 
-    def __round__(self, n:NUM_TYPE=1) -> "Vector2D":
+    def __round__(self, n:int|float=1) -> "Vector2D":
         return Vector2D(round(self.x / n) * n, round(self.y / n) * n)
 
-    def __floor__(self, n:NUM_TYPE=1) -> "Vector2D":
+    def __floor__(self, n:int|float=1) -> "Vector2D":
         return Vector2D(_mt.floor(self.x / n) * n, _mt.floor(self.y / n) * n)
 
-    def __ceil__(self, n:NUM_TYPE=1) -> "Vector2D":
+    def __ceil__(self, n:int|float=1) -> "Vector2D":
         return Vector2D(_mt.ceil(self.x / n) * n, _mt.ceil(self.y / n) * n)
 
-    def __mul__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __mul__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         object = self.__normalize__(object)
         return Vector2D(self.x * object.x, self.y * object.y)
 
-    def __pow__(self, object:"float|int|Vector2D|ARRAY_TYPE") -> "Vector2D":
+    def __pow__(self, object:"float|int|Vector2D|list|tuple") -> "Vector2D":
         object = self.__normalize__(object)
         return Vector2D(self.x ** object.x, self.y ** object.y)
     
     def __float__(self) -> "Vector2D":
         return Vector2D(float(self.x), float(self.y))
 
-    def __getitem__(self, n) -> NUM_TYPE:
+    def __getitem__(self, n) -> int|float:
         if n in [0, "x"]:
             return self.x
         elif n in [1, "y"]:
             return self.y
         else:
             raise IndexError("V2 has only x,y...")
     
     def __normalize__(self, object) -> "Vector2D":
         if not isinstance(object, Vector2D):
-            if isinstance(object, NUM_TYPE):
+            if isinstance(object, int|float):
                 return Vector2D(object, object)
-            elif isinstance(object, ARRAY_TYPE):
+            elif isinstance(object, list|tuple):
                 return Vector2D(*object[:2])
             else:
-                raise TypeError(f"The value {object} is not a num type: [{NUM_TYPE}] nor an array type: [{ARRAY_TYPE}]")
+                raise TypeError(f"The value {object} is not a num type: [{int|float}] nor an array type: [{list|tuple}]")
         return object
 
 class V2(Vector2D):
-    def  __init__(self, x: NUM_TYPE = 0, y: NUM_TYPE = 0) -> None:
+    def  __init__(self, x: int|float = 0, y: int|float = 0) -> None:
         super().__init__(x, y)
 
 V2inf = Vector2D(float('inf'), float('inf'))
 V2z = VectorZero = Vector2D()
 V2one = Vector2D(1, 1)
 
-def rgb(r:NUM_TYPE, g:NUM_TYPE, b:NUM_TYPE) -> tuple[NUM_TYPE, NUM_TYPE, NUM_TYPE]:
+def rgb(r:int|float, g:int|float, b:int|float) -> tuple[int|float, int|float, int|float]:
     return (r,g,b)
 
-def color_fade(starting_c:ARRAY_TYPE, final_c:ARRAY_TYPE, index:NUM_TYPE, max_index:NUM_TYPE) -> tuple:
+def color_fade(starting_c:list|tuple, final_c:list|tuple, index:int|float, max_index:int|float) -> tuple:
     """
     # Calculate the color at a specific index of a color fade between two given colors.
 
     # Parameters:
         starting_c (tuple or list): The RGB values of the starting color as a tuple or list.
         final_c (tuple or list): The RGB values of the final color as a tuple or list.
         index (int or float): The current index of the color fade, representing a position
@@ -636,15 +627,15 @@
     """
     colors = colors_dict.keys()
     weights = colors_dict.values()
 
     if float("inf") in weights: return list(colors)[list(weights).index(float("inf"))]
     return tuple(sum(n[i]*w for n,w in zip(colors, weights)) / sum(weights) for i in range(3))
 
-def angular_interpolation(starting_angle:NUM_TYPE, final_angle:NUM_TYPE, step:NUM_TYPE=.1) -> float:
+def angular_interpolation(starting_angle:int|float, final_angle:int|float, step:int|float=.1) -> float:
     """
     # Perform angular interpolation between two angles using the shortest distance.
 
     # Parameters:
         starting_angle (int or float): The initial angle in radians.
         final_angle (int or float): The target angle in radians to interpolate towards.
         step (int or float, optional): The step size for interpolation in radians. Default is 0.1.
@@ -678,15 +669,15 @@
 
         The `step` parameter controls the granularity of interpolation. Smaller `step` values
         provide more fine-grained interpolation but may require more iterations.
     """
     distances = (final_angle - starting_angle, final_angle - DOUBLE_PI - starting_angle, final_angle + DOUBLE_PI - starting_angle)
     return min(distances, key=abs) * step
 
-def color_distance(starting_c:ARRAY_TYPE, final_c:ARRAY_TYPE, sqrd:bool=True) -> float:
+def color_distance(starting_c:list|tuple, final_c:list|tuple, sqrd:bool=True) -> float:
     """
     # Calculate the distance between two colors in RGB space.
 
     # Parameters:
         starting_c (list or tuple): The RGB values of the starting color.
         final_c (list or tuple): The RGB values of the final color.
         sqrd (bool, optional): If True, return the squared distance. If False, return
@@ -752,22 +743,22 @@
         It calculates the sum of all the Vector2D objects using the `sum` function and then divides
         it by the total number of objects (length of `objects`) to find the average position.
 
         The result is returned as a new Vector2D object representing the average position.
     """
     return sum(list(objects)) / (len(objects)) # type: ignore
 
-def get_points(position:Vector2D, size:Vector2D, rotation:NUM_TYPE=0, pos_in_middle:bool=True, return_list:bool=False, clockwise_return:bool=False) -> tuple["Vector2D", "Vector2D", "Vector2D", "Vector2D"] | tuple[list[NUM_TYPE]|tuple[NUM_TYPE], list[NUM_TYPE]|tuple[NUM_TYPE], list[NUM_TYPE]|tuple[NUM_TYPE], list[NUM_TYPE]|tuple[NUM_TYPE]]:
+def get_points(position:Vector2D, size:Vector2D, rotation:int|float=0, pos_in_middle:bool=True, return_list:bool=False, clockwise_return:bool=False) -> tuple["Vector2D", "Vector2D", "Vector2D", "Vector2D"] | tuple[list[int|float]|tuple[int|float], list[int|float]|tuple[int|float], list[int|float]|tuple[int|float], list[int|float]|tuple[int|float]]:
     """
     # Generate points for a rectangle based on the given parameters.
 
     # Parameters:
         position (Vector2D): The center position of the rectangle.
         size (Vector2D): The size of the rectangle (width and height).
-        rotation (NUM_TYPE, optional): The rotation angle in degrees. Default is 0.
+        rotation (int|float, optional): The rotation angle in degrees. Default is 0.
         pos_in_middle (bool, optional): If True, the points represent corners of the rectangle.
                                         If False, the points represent the rectangle's edges.
                                         Default is True.
         return_list (bool, optional): If True, return the points as lists instead of Vector2D objects.
                                       Default is False.
         clockwise_return (bool, optional): If True, return the points in clockwise order (A, B, D, C).
                                            If False, return the points in counterclockwise order (A, B, C, D).
@@ -809,22 +800,22 @@
         A, B, C, D = [position.copy(),
                       position.point_from_degs(rotation + V2z.angle_to(Vector2D(size.x, 0)), V2z.distance_to(Vector2D(size.x, 0))),
                       position.point_from_degs(rotation + V2z.angle_to(Vector2D(0, size.y)), V2z.distance_to(Vector2D(0, size.y))),
                       position.point_from_degs(rotation + V2z.angle_to(size),                V2z.distance_to(size))]
     points = (A, B, C, D) if not clockwise_return else (A, B, D, C)
     return points if not return_list else tuple(x() for x in points)
 
-def get_lines(position:Vector2D, size:Vector2D, rotation:NUM_TYPE=0, pos_in_middle:bool=True) -> list[list]:
+def get_lines(position:Vector2D, size:Vector2D, rotation:int|float=0, pos_in_middle:bool=True) -> list[list]:
     """
     # Generate lines representing the sides of a rectangle based on the given parameters.
 
     # Parameters:
         position (Vector2D): The center position of the rectangle.
         size (Vector2D): The size of the rectangle (width and height).
-        rotation (NUM_TYPE, optional): The rotation angle in degrees. Default is 0.
+        rotation (int|float, optional): The rotation angle in degrees. Default is 0.
         pos_in_middle (bool, optional): If True, the points represent corners of the rectangle.
                                         If False, the points represent the rectangle's edges.
                                         Default is True.
 
     # Returns:
         list[list[Vector2D]]: A list of lists, where each sublist contains two Vector2D objects
                               representing the start and end points of a line segment.
@@ -883,247 +874,7 @@
 
         It does this by first computing the cross product of vectors (line_point_b - line_point_a) and (line_point_a - point_c).
         The magnitude of the resulting vector is divided by the magnitude of (line_point_b - line_point_a) to obtain the distance.
 
         The result is returned as a float representing the distance between the line segment and the point.
     """
     return float(_np.linalg.norm(_np.cross((line_point_b-line_point_a)(), (line_point_a-point_c)()))/_np.linalg.norm((line_point_b-line_point_a)()))
-
-
-#  default env
-"""
-import random as rnd
-import numpy as np
-from e2D import *
-
-import pygame as pg
-
-pg.init()
-pg.font.init()
-myfont = pg.font.SysFont("Arial", 32)
-
-class Env:
-    def __init__(self) -> None:
-        self.quit = False
-        self.screen_size = V2(1920, 1080)
-        self.screen = pg.display.set_mode(self.screen_size(), vsync=1)
-        self.clock = pg.time.Clock()
-        self.keyboard = Keyboard(self)
-        self.mouse = Mouse(self)
-    
-    def clear(self) -> None:
-        self.screen.fill((0,0,0))
-    
-    def print(self, text, position, color=(255,255,255)) -> None:
-        text_box = myfont.render(text, True, color)
-        self.screen.blit(text_box, position())
-
-    def draw(self) -> None:
-        self.clock.tick(60)
-        self.clear()
-        self.print(str(self.clock.get_fps()), self.screen_size * .01)
-
-        pg.display.update()
-    
-    def update(self) -> None:
-        self.mouse.update()
-        self.keyboard.update()
-
-    def frame(self) -> None:
-        self.update()
-        self.draw()
-
-        for event in pg.event.get():
-            if event.type == pg.QUIT or (event.type == pg.KEYDOWN and event.key == pg.K_x):
-                self.quit = True
-
-env = Env()
-
-while not env.quit:
-    env.frame()
-"""
-
-
-#############################################################################################################################################################################################################################################################
-# advanced env #TODO
-"""
-from e2D import *
-import keyboard as key
-import time as tm
-import pygame as pg
-import easygui
-import uuid
-
-pg.init()
-pg.font.init()
-myfont = pg.font.SysFont("Arial", 32)
-
-DEFAULT_MOUSE_BUTTON_MODE = 0
-OVER_MOUSE_BUTTON_MODE = 1
-CLICKED_MOUSE_BUTTON_MOVE = 2
-
-CALLBACK_MODE_ON_PRESSED = 0
-CALLBACK_MODE_ON_RELEASED = 1
-
-class Button:
-    def_side_border = .85
-    def __init__(self,
-                 parent,
-                 text,
-                 screen_ratio_position:V2,
-                 screen_ratio_size:V2, 
-                 text_color:tuple[num_type,num_type,num_type],
-                 def_color:tuple[num_type,num_type,num_type],
-                 over_color:tuple[num_type,num_type,num_type],
-                 click_color:tuple[num_type,num_type,num_type],
-                 callback,
-                 border_color:tuple[num_type,num_type,num_type]=(255,255,255),
-                 border_width:num_type=2,
-                 corners:list[num_type]|num_type|None=10,
-                 callback_mode=CALLBACK_MODE_ON_RELEASED,
-                 font="Algerian",
-                 font_downscale:float=1.0,
-                 **callback_kwargs) -> None:
-        self.parent :Env= parent
-        self.text :str= text
-        self.screen_ratio_size = screen_ratio_size  # ratio position is bot right
-        self.screen_ratio_position = screen_ratio_position # ratio position is top left
-        self.text_color = text_color
-        self.callback = callback
-        self.callback_kwargs = callback_kwargs
-        self.def_color = def_color
-        self.over_color = over_color
-        self.click_color = click_color
-        self.mouse_mode = DEFAULT_MOUSE_BUTTON_MODE
-        self.font = font
-        self.font_downscale = font_downscale
-        self.callback_mode = callback_mode
-        self.border_color = border_color
-        self.border_width = border_width
-        self.corners = corners
-        self.update_screen_ratio_position()
-    
-    def update_screen_ratio_position(self) -> None:
-        self.position = self.parent.screen_size * self.screen_ratio_position
-        self.size = self.parent.screen_size * self.screen_ratio_size - self.parent.screen_size * self.screen_ratio_position
-        self.set_box_and_text_size()
-    
-    def set_box_and_text_size(self) -> None:
-        text_box = pg.font.SysFont(self.font, int(self.size.y)).render(self.text, True, self.text_color) #type: ignore
-        text_box_size = V2(*text_box.get_rect()[2:])
-        ratio = text_box_size.x / text_box_size.y
-        self.font_size = min(self.size.x * self.def_side_border / ratio, self.size.y) * self.font_downscale
-        self.text_box = pg.font.SysFont(self.font, int(self.font_size)).render(self.text, True, self.text_color) #type: ignore
-        self.text_box_size = V2(*self.text_box.get_rect()[2:])
-
-    def draw(self) -> None:
-        color = self.def_color
-        if self.mouse_mode == DEFAULT_MOUSE_BUTTON_MODE:
-            color = self.def_color
-        elif self.mouse_mode == OVER_MOUSE_BUTTON_MODE:
-            color = self.over_color
-        elif self.mouse_mode == CLICKED_MOUSE_BUTTON_MOVE:
-            color = self.click_color
-        
-        if self.corners == None:
-            pg.draw.rect(self.parent.screen, color, self.position() + self.size()) #type: ignore
-        elif type(self.corners) in num_type:
-            pg.draw.rect(self.parent.screen, color, self.position() + self.size(), border_radius=self.corners) #type: ignore
-        elif type(self.corners) == list:
-            pg.draw.rect(self.parent.screen, color, self.position() + self.size(), border_top_left_radius=self.corners[0], border_top_right_radius=self.corners[1], border_bottom_left_radius=self.corners[2], border_bottom_right_radius=self.corners[3]) #type: ignore
-        if self.border_width:
-            if self.corners == None:
-                pg.draw.rect(self.parent.screen, self.border_color, self.position() + self.size(), self.border_width) #type: ignore
-            elif type(self.corners) in num_type:
-                pg.draw.rect(self.parent.screen, self.border_color, self.position() + self.size(), self.border_width, border_radius=self.corners) #type: ignore
-            elif type(self.corners) == list:
-                pg.draw.rect(self.parent.screen, self.border_color, self.position() + self.size(), self.border_width, border_top_left_radius=self.corners[0], border_top_right_radius=self.corners[1], border_bottom_left_radius=self.corners[2], border_bottom_right_radius=self.corners[3]) #type: ignore
-        
-        self.parent.screen.blit(self.text_box, (self.position + (self.size - self.text_box_size) / 2)())
-
-    def update(self) -> None:
-        if self.position.x < self.parent.mouse.position.x < self.position.x + self.size.x and self.position.y < self.parent.mouse.position.y < self.position.y + self.size.y:
-            if self.parent.mouse.just_pressed[0] and CALLBACK_MODE_ON_PRESSED or self.parent.mouse.just_released[0] and CALLBACK_MODE_ON_RELEASED:
-                self.mouse_mode = CLICKED_MOUSE_BUTTON_MOVE
-                self.callback(**self.callback_kwargs)
-            elif self.parent.mouse.pressed[0]:
-                self.mouse_mode = CLICKED_MOUSE_BUTTON_MOVE
-            else:
-                self.mouse_mode = OVER_MOUSE_BUTTON_MODE
-        else:
-            self.mouse_mode = DEFAULT_MOUSE_BUTTON_MODE
-
-
-class ButtonCallBacks:
-    def __init__(self, parent) -> None:
-        self.parent :Env= parent
-
-    def on_load_image_callback(self, **kwargs) -> None:
-        path = easygui.fileopenbox(filetypes=["*.png"])
-        if not path: return
-        image = pg.image.load(path) #type: ignore
-        self.parent.reference_images.append({"path": path, "image":image, "id": uuid.uuid4()})
-
-class Env:
-    def __init__(self) -> None:
-        self.quit = False
-        self.screen_size = V2(1920, 1080)
-        self.screen = pg.display.set_mode(self.screen_size(), vsync=1, flags=pg.RESIZABLE)
-        self.clock = pg.time.Clock()
-        self.keyboard = Keyboard(self)
-        self.mouse = Mouse(self)
-        self.buttons_callbacks = ButtonCallBacks(self)
-        self.buttons = [
-            Button(self,
-                   text="add photo path",
-                   screen_ratio_position=V2(.75, .1),
-                   screen_ratio_size=V2(.99, .25),
-                   text_color=rgb(255, 255, 255),
-                   def_color=rgb(194, 87, 0),
-                   over_color=rgb(107, 57, 15),
-                   click_color=rgb(32, 20, 9),
-                   callback=self.buttons_callbacks.on_load_image_callback,
-                   font_downscale=.9)
-                   ]
-        self.reference_images = []
-    
-    def print(self, text, position, color=(255,255,255)) -> None:
-        text_box = myfont.render(text, True, color)
-        self.screen.blit(text_box, position())
-
-    def clear(self) -> None:
-        self.screen.fill((0,0,0))
-    
-    def draw(self) -> None:
-        self.clock.tick(0)
-        self.clear()
-        self.print(str(self.clock.get_fps()), self.screen_size * .01)
-
-        for button in self.buttons: button.draw()
-        self.mouse.draw()
-
-        pg.display.update()
-    
-    def update(self) -> None:
-        last_screen_size = self.screen_size()
-        self.screen_size = V2(*self.screen.get_rect()[2:])
-        if last_screen_size != self.screen_size():
-            for button in self.buttons: button.update_screen_ratio_position()
-        
-        self.keyboard.update()
-        self.mouse.update()
-        for button in self.buttons: button.update()
-    
-    def frame(self) -> None:
-        self.update()
-        self.draw()
-
-        for event in pg.event.get():
-            if event.type == pg.QUIT or (event.type == pg.KEYDOWN and event.key == pg.K_x):
-                self.quit = True
-
-env = Env()
-
-while not env.quit:
-    env.frame()
-"""
-
```

### Comparing `e2D-0.0.5/e2D/pg.py` & `e2D-0.1.0/e2D/utils.py`

 * *Files identical despite different names*

### Comparing `e2D-0.0.5/e2D.egg-info/PKG-INFO` & `e2D-0.1.0/e2D.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.0.5
+Version: 0.1.0
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,18 +30,18 @@
 - Simple API for ease of use, suitable for both beginners and experienced developers.
 
 ## Installation
 
 You can install e2D using pip:
 
 ```bash
-pip install e2Dpy
+pip install e2D
 ```
 ```bash
-pip3 install e2Dpy
+pip3 install e2D
 ```
 
 ## Getting Started
 
 To get started with e2D, follow these steps:
 
 1. Create a new Python project or navigate to your existing project directory.
```

### Comparing `e2D-0.0.5/setup.cfg` & `e2D-0.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 3244 0d0a 7665 7273 696f 6e20   = e2D..version 
-00000020: 3d20 302e 302e 350d 0a61 7574 686f 7220  = 0.0.5..author 
+00000020: 3d20 302e 312e 300d 0a61 7574 686f 7220  = 0.1.0..author 
 00000030: 3d20 5269 6363 6172 646f 204d 6172 6961  = Riccardo Maria
 00000040: 6e69 0d0a 6175 7468 6f72 5f65 6d61 696c  ni..author_email
 00000050: 203d 2072 6963 6f6d 6172 6932 3030 3640   = ricomari2006@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
 00000080: 6c69 6272 6172 7920 666f 7220 3244 2067  library for 2D g
 00000090: 616d 6573 2e20 5374 7265 616d 6c69 6e65  ames. Streamline
```

