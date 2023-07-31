# Comparing `tmp/rsplan-1.0.4.tar.gz` & `tmp/rsplan-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsplan-1.0.4.tar", last modified: Tue Jul 25 19:48:43 2023, max compression
+gzip compressed data, was "rsplan-1.0.5.tar", last modified: Mon Jul 31 17:37:07 2023, max compression
```

## Comparing `rsplan-1.0.4.tar` & `rsplan-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 19:48:43.930349 rsplan-1.0.4/
--rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.4/LICENSE
--rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 19:48:43.930349 rsplan-1.0.4/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)     3833 2023-07-25 02:06:53.000000 rsplan-1.0.4/README.md
--rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-25 19:48:33.000000 rsplan-1.0.4/pyproject.toml
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 19:48:43.930349 rsplan-1.0.4/rsplan/
--rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-19 03:21:47.000000 rsplan-1.0.4/rsplan/__init__.py
--rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-24 00:19:10.000000 rsplan-1.0.4/rsplan/curves.py
--rw-rw-r--   0 built     (1000) built     (1000)     2582 2023-07-25 01:59:29.000000 rsplan-1.0.4/rsplan/demo.py
--rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.4/rsplan/helpers.py
--rw-rw-r--   0 built     (1000) built     (1000)     6597 2023-07-25 02:48:24.000000 rsplan-1.0.4/rsplan/planner.py
--rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.4/rsplan/primitives.py
--rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-25 19:46:23.000000 rsplan-1.0.4/rsplan/py.typed
--rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.4/rsplan/unit_tests.py
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-25 19:48:43.930349 rsplan-1.0.4/rsplan.egg-info/
--rw-rw-r--   0 built     (1000) built     (1000)     5490 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)      335 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/SOURCES.txt
--rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/dependency_links.txt
--rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/requires.txt
--rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-25 19:48:43.000000 rsplan-1.0.4/rsplan.egg-info/top_level.txt
--rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-25 19:48:43.930349 rsplan-1.0.4/setup.cfg
--rw-rw-r--   0 built     (1000) built     (1000)      686 2023-07-25 19:48:23.000000 rsplan-1.0.4/setup.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-31 17:37:07.410989 rsplan-1.0.5/
+-rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.5/LICENSE
+-rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-07-31 17:37:07.410989 rsplan-1.0.5/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)     4083 2023-07-25 20:27:37.000000 rsplan-1.0.5/README.md
+-rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-07-31 17:37:00.000000 rsplan-1.0.5/pyproject.toml
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-31 17:37:07.410989 rsplan-1.0.5/rsplan/
+-rw-rw-r--   0 built     (1000) built     (1000)      113 2023-07-31 17:32:15.000000 rsplan-1.0.5/rsplan/__init__.py
+-rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-25 20:19:49.000000 rsplan-1.0.5/rsplan/curves.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2650 2023-07-31 17:34:37.000000 rsplan-1.0.5/rsplan/demo.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.5/rsplan/helpers.py
+-rw-rw-r--   0 built     (1000) built     (1000)     6597 2023-07-25 20:19:52.000000 rsplan-1.0.5/rsplan/planner.py
+-rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.5/rsplan/primitives.py
+-rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-25 19:46:23.000000 rsplan-1.0.5/rsplan/py.typed
+-rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.5/rsplan/unit_tests.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-07-31 17:37:07.410989 rsplan-1.0.5/rsplan.egg-info/
+-rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)      335 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/SOURCES.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        1 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/dependency_links.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       39 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/requires.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        7 2023-07-31 17:37:07.000000 rsplan-1.0.5/rsplan.egg-info/top_level.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       38 2023-07-31 17:37:07.410989 rsplan-1.0.5/setup.cfg
+-rw-rw-r--   0 built     (1000) built     (1000)      686 2023-07-31 17:36:44.000000 rsplan-1.0.5/setup.py
```

### Comparing `rsplan-1.0.4/LICENSE` & `rsplan-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.4/PKG-INFO` & `rsplan-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.4
+Version: 1.0.5
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
@@ -23,17 +23,16 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 ## README
 
 - [Overview](#overview)
 - [Usage](#usage)
-  - [Initial setup](#installation)
+  - [Installation](#installation)
   - [Running](#running)
-  - [Demo](#demo)
 - [FAQ](#faq)
 - [Exhibits](#exhibits)
 - [References](#references)
 
 ## Overview
 This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions >= 3.9, including 3.11.
 
@@ -50,20 +49,20 @@
 
 
 ## Usage
 
 ### Installation
 You can install this software using pip:
 
-`pip install -U rsplan`
+`$ pip3 install -U rsplan`
 
 
 ### Running
 
-See demo.py for example usage
+See demo.py for example usage 
 
 path(start_pose, end_pose, turn_radius, runway_length, step_size, length_tolerance (optional))
 - return a Reeds-Shepp path from start_pose to end_pose with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
 - start_pose and end_pose are in the format `Tuple[float, float, float]` of x, y, yaw values.
 
 
 ## FAQ
@@ -75,17 +74,26 @@
   - t, u, u, v for cccc paths (2nd and 3rd segments have same angular distance)
   - t, pi/2, u, v for ccsc paths (2nd segment has angle pi/2)
   - t, u, pi/2, v for cscc paths (3rd segment has angle pi/2)
   - t, pi/2, u, pi/2, v for ccscc paths (2nd and 4th segments have angle pi/2)
 - These are represented generally in the Segment class in the "distance" parameter, which we pass in t, u, v, or pi/2 for depending on the segment.
 
 
-### Exhibits
+## Exhibits
 
-From demo.py:
+### How to run the demo
+
+- Clone this repository
+
+- Update `_END_POSES` path coordinates in demo.py to the paths you would like to visualize
+
+- In terminal in the rsplan subfolder of this rsplan repository, run:
+  `$ python3 demo.py`
+
+### Example paths visualized from demo.py:
 
 Paths start from origin
 
 Format: (end x, end y, yaw, turn radius, runway length)
 1. (5, 6, np.pi, 1, 0)
 2. (15, 3, np.pi / 2.0, 2, 6)
 3. (-2, -4, np.pi, 4, 3)
@@ -95,14 +103,16 @@
 7. (-5, 6, np.pi / 3.0, 2, 1)
 8. (7, 2, 0.0, 6, 3)
 9. (-4, -1, -np.pi / 2.0, 1, 3)
 
 ![Screenshot from 2023-07-18 11-50-32](https://github.com/builtrobotics/mariana/assets/44348827/eed5e06c-059e-48cb-9dc3-e56346f84476)
 
 
+
+
 ## References
 Paper providing more information on the algorithm:
 Reeds, J., & Shepp, L. (1990). Optimal paths for a car that goes both forwards and backwards. https://msp.org/pjm/1990/145-2/pjm-v145-n2-p06-s.pdf
 
 Curve formulas can be found on page 390-391.
 Inspiration for this Python implementation of the Reeds-Shepp algorithm:
 https://github.com/boyali/reeds_and_shepp_curves/tree/master
```

### Comparing `rsplan-1.0.4/README.md` & `rsplan-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ## README
 
 - [Overview](#overview)
 - [Usage](#usage)
-  - [Initial setup](#installation)
+  - [Installation](#installation)
   - [Running](#running)
-  - [Demo](#demo)
 - [FAQ](#faq)
 - [Exhibits](#exhibits)
 - [References](#references)
 
 ## Overview
 This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions >= 3.9, including 3.11.
 
@@ -25,20 +24,20 @@
 
 
 ## Usage
 
 ### Installation
 You can install this software using pip:
 
-`pip install -U rsplan`
+`$ pip3 install -U rsplan`
 
 
 ### Running
 
-See demo.py for example usage
+See demo.py for example usage 
 
 path(start_pose, end_pose, turn_radius, runway_length, step_size, length_tolerance (optional))
 - return a Reeds-Shepp path from start_pose to end_pose with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
 - start_pose and end_pose are in the format `Tuple[float, float, float]` of x, y, yaw values.
 
 
 ## FAQ
@@ -50,17 +49,26 @@
   - t, u, u, v for cccc paths (2nd and 3rd segments have same angular distance)
   - t, pi/2, u, v for ccsc paths (2nd segment has angle pi/2)
   - t, u, pi/2, v for cscc paths (3rd segment has angle pi/2)
   - t, pi/2, u, pi/2, v for ccscc paths (2nd and 4th segments have angle pi/2)
 - These are represented generally in the Segment class in the "distance" parameter, which we pass in t, u, v, or pi/2 for depending on the segment.
 
 
-### Exhibits
+## Exhibits
 
-From demo.py:
+### How to run the demo
+
+- Clone this repository
+
+- Update `_END_POSES` path coordinates in demo.py to the paths you would like to visualize
+
+- In terminal in the rsplan subfolder of this rsplan repository, run:
+  `$ python3 demo.py`
+
+### Example paths visualized from demo.py:
 
 Paths start from origin
 
 Format: (end x, end y, yaw, turn radius, runway length)
 1. (5, 6, np.pi, 1, 0)
 2. (15, 3, np.pi / 2.0, 2, 6)
 3. (-2, -4, np.pi, 4, 3)
@@ -70,14 +78,16 @@
 7. (-5, 6, np.pi / 3.0, 2, 1)
 8. (7, 2, 0.0, 6, 3)
 9. (-4, -1, -np.pi / 2.0, 1, 3)
 
 ![Screenshot from 2023-07-18 11-50-32](https://github.com/builtrobotics/mariana/assets/44348827/eed5e06c-059e-48cb-9dc3-e56346f84476)
 
 
+
+
 ## References
 Paper providing more information on the algorithm:
 Reeds, J., & Shepp, L. (1990). Optimal paths for a car that goes both forwards and backwards. https://msp.org/pjm/1990/145-2/pjm-v145-n2-p06-s.pdf
 
 Curve formulas can be found on page 390-391.
 Inspiration for this Python implementation of the Reeds-Shepp algorithm:
 https://github.com/boyali/reeds_and_shepp_curves/tree/master
```

### Comparing `rsplan-1.0.4/pyproject.toml` & `rsplan-1.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsplan"
-version = "1.0.4"
+version = "1.0.5"
 description = "Reeds-Shepp algorithm implementation in Python"
 readme = "README.md"
 authors = [{ name = "Built Robotics", email = "tarakapoor9@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rsplan-1.0.4/rsplan/curves.py` & `rsplan-1.0.5/rsplan/curves.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.4/rsplan/demo.py` & `rsplan-1.0.5/rsplan/demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from typing import List, Tuple
 
 import matplotlib.pyplot as plt  # type: ignore[import]
 import numpy as np
 
-from rsplan import planner, primitives
+# from rsplan import planner, primitives
+import rsplan
 
 # List of path end poses to visualize Reeds-Shepp paths for with matplotlib.
 # Format: (end x, end y, end yaw, turn radius, runway length)
 _END_POSES: List[Tuple[float, float, float, int, float]] = [
     (5, 6, np.pi, 1, 0),
     (15, 3, np.pi / 2.0, 2, 6),
     (-2, -4, np.pi, 4, 3),
@@ -42,15 +43,15 @@
         length * np.sin(yaw),
         head_width=width,
         head_length=width,
     )
     plt.plot(x, y, marker="s", label=label)
 
 
-def _viz_path(rs_path: primitives.Path, path_num: int) -> None:
+def _viz_path(rs_path: rsplan.Path, path_num: int) -> None: #primitives.Path, path_num: int) -> None:
     """Visualizes the given path in the plot."""
     x_coords, y_coords, _ = rs_path.coordinates_tuple()
 
     path_plt = plt.subplot(111)
     path_plt.plot(x_coords, y_coords, label=(f"Path ix: {path_num}"))
 
     # Shrink current axis's height by 10% on the bottom
@@ -78,15 +79,15 @@
         end_coords = _END_POSES[i]
         x, y, yaw, turn_radius, runway_length = end_coords
         step_size = 0.05
 
         _plot_arrow(*start)  # Start arrow same for all paths starting at origin
 
         # Passing in yaw angles in radians
-        rs_path = planner.path(
+        rs_path = rsplan.path( #planner.path(
             start, (x, y, yaw), turn_radius, runway_length, step_size
         )
         _viz_path(rs_path, i + 1)
         _plot_arrow(x, y, yaw)  # End of path arrow to show direction
 
     plt.show()
```

### Comparing `rsplan-1.0.4/rsplan/helpers.py` & `rsplan-1.0.5/rsplan/helpers.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.4/rsplan/planner.py` & `rsplan-1.0.5/rsplan/planner.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.4/rsplan/primitives.py` & `rsplan-1.0.5/rsplan/primitives.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.4/rsplan/unit_tests.py` & `rsplan-1.0.5/rsplan/unit_tests.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.4/rsplan.egg-info/PKG-INFO` & `rsplan-1.0.5/rsplan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.4
+Version: 1.0.5
 Summary: Reeds-Shepp algorithm implementation in Python
 Home-page: https://github.com/builtrobotics/rs
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
@@ -23,17 +23,16 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 ## README
 
 - [Overview](#overview)
 - [Usage](#usage)
-  - [Initial setup](#installation)
+  - [Installation](#installation)
   - [Running](#running)
-  - [Demo](#demo)
 - [FAQ](#faq)
 - [Exhibits](#exhibits)
 - [References](#references)
 
 ## Overview
 This package is a Reeds-Shepp library implementation with Python that is compatible with Python versions >= 3.9, including 3.11.
 
@@ -50,20 +49,20 @@
 
 
 ## Usage
 
 ### Installation
 You can install this software using pip:
 
-`pip install -U rsplan`
+`$ pip3 install -U rsplan`
 
 
 ### Running
 
-See demo.py for example usage
+See demo.py for example usage 
 
 path(start_pose, end_pose, turn_radius, runway_length, step_size, length_tolerance (optional))
 - return a Reeds-Shepp path from start_pose to end_pose with specified turning radius and step_size between points. The length_tolerance default is 2 meters but can be set to user preference — if paths’ total lengths are within length tolerance of each other, the path function will choose the one with fewer segments as the optimal path. The runway_length is for the runway at the end of the path that helps improve accuracy in reaching the final position — this can be set to 0, or a positive or negative number for a forwards or backwards driving runway.
 - start_pose and end_pose are in the format `Tuple[float, float, float]` of x, y, yaw values.
 
 
 ## FAQ
@@ -75,17 +74,26 @@
   - t, u, u, v for cccc paths (2nd and 3rd segments have same angular distance)
   - t, pi/2, u, v for ccsc paths (2nd segment has angle pi/2)
   - t, u, pi/2, v for cscc paths (3rd segment has angle pi/2)
   - t, pi/2, u, pi/2, v for ccscc paths (2nd and 4th segments have angle pi/2)
 - These are represented generally in the Segment class in the "distance" parameter, which we pass in t, u, v, or pi/2 for depending on the segment.
 
 
-### Exhibits
+## Exhibits
 
-From demo.py:
+### How to run the demo
+
+- Clone this repository
+
+- Update `_END_POSES` path coordinates in demo.py to the paths you would like to visualize
+
+- In terminal in the rsplan subfolder of this rsplan repository, run:
+  `$ python3 demo.py`
+
+### Example paths visualized from demo.py:
 
 Paths start from origin
 
 Format: (end x, end y, yaw, turn radius, runway length)
 1. (5, 6, np.pi, 1, 0)
 2. (15, 3, np.pi / 2.0, 2, 6)
 3. (-2, -4, np.pi, 4, 3)
@@ -95,14 +103,16 @@
 7. (-5, 6, np.pi / 3.0, 2, 1)
 8. (7, 2, 0.0, 6, 3)
 9. (-4, -1, -np.pi / 2.0, 1, 3)
 
 ![Screenshot from 2023-07-18 11-50-32](https://github.com/builtrobotics/mariana/assets/44348827/eed5e06c-059e-48cb-9dc3-e56346f84476)
 
 
+
+
 ## References
 Paper providing more information on the algorithm:
 Reeds, J., & Shepp, L. (1990). Optimal paths for a car that goes both forwards and backwards. https://msp.org/pjm/1990/145-2/pjm-v145-n2-p06-s.pdf
 
 Curve formulas can be found on page 390-391.
 Inspiration for this Python implementation of the Reeds-Shepp algorithm:
 https://github.com/boyali/reeds_and_shepp_curves/tree/master
```

### Comparing `rsplan-1.0.4/setup.py` & `rsplan-1.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "rsplan",
-    version = "1.0.4",
+    version = "1.0.5",
     author = "Built Robotics",
     author_email = "tarakapoor9@gmail.com",
     description = ("Reeds-Shepp algorithm implementation in Python."),
     license = "MIT",
     keywords = "reeds-shepp path planning",
     url = "https://github.com/builtrobotics/rs",
     packages=['rsplan'],
```

