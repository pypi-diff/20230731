# Comparing `tmp/pyfeyn2-2.3.5.tar.gz` & `tmp/pyfeyn2-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.3.5.tar", max compression
+gzip compressed data, was "pyfeyn2-2.3.6.tar", max compression
```

## Comparing `pyfeyn2-2.3.5.tar` & `pyfeyn2-2.3.6.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0    35149 2023-07-24 07:08:04.637394 pyfeyn2-2.3.5/LICENSE
--rw-r--r--   0        0        0     3115 2023-07-24 07:08:04.641394 pyfeyn2-2.3.5/README.md
--rw-r--r--   0        0        0      154 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2838 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      647 2023-07-24 07:08:04.757394 pyfeyn2-2.3.5/pyfeyn2/auto/diagram.py
--rw-r--r--   0        0        0      768 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0    10564 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/auto/reshuffle.py
--rw-r--r--   0        0        0     3279 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2734 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0      279 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0      238 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0     2924 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     3626 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3596 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     5926 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     1617 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2407 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     7120 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     7036 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0        0 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13245 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41394 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12740 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     9146 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2914 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     8914 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      863 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2364 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1701 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     2114 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      527 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3850 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1401 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1976 2023-07-24 07:08:04.761394 pyfeyn2-2.3.5/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2630 2023-07-24 07:08:07.933416 pyfeyn2-2.3.5/pyproject.toml
--rw-r--r--   0        0        0     4904 1970-01-01 00:00:00.000000 pyfeyn2-2.3.5/setup.py
--rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 pyfeyn2-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-31 06:40:27.208997 pyfeyn2-2.3.6/LICENSE
+-rw-r--r--   0        0        0     3115 2023-07-31 06:40:27.208997 pyfeyn2-2.3.6/README.md
+-rw-r--r--   0        0        0      154 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2838 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      647 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/auto/diagram.py
+-rw-r--r--   0        0        0      798 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0    16833 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0     3279 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2734 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0      279 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0      238 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0     2256 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     4370 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3596 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     5926 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     1617 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2407 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     7120 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     7036 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13245 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41394 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12740 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     9146 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2914 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     8914 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      863 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2364 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1701 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     2114 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      527 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3850 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1401 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1976 2023-07-31 06:40:27.288999 pyfeyn2-2.3.6/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2645 2023-07-31 06:40:29.369035 pyfeyn2-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4944 1970-01-01 00:00:00.000000 pyfeyn2-2.3.6/setup.py
+-rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 pyfeyn2-2.3.6/PKG-INFO
```

### Comparing `pyfeyn2-2.3.5/LICENSE` & `pyfeyn2-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/README.md` & `pyfeyn2-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/auto/bend.py` & `pyfeyn2-2.3.6/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/auto/diagram.py` & `pyfeyn2-2.3.6/pyfeyn2/auto/diagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/auto/label.py` & `pyfeyn2-2.3.6/pyfeyn2/auto/label.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,25 @@
     for p in objs:
         if (p.label is None or replace) and p.particle is not None:
             p.label = "$" + p.particle.latex_name + "$"
 
 
 def auto_label_propagators(ifd, replace=False):
     """Automatically label propagators."""
-    fd = copy.deepcopy(ifd)
+    # fd = copy.deepcopy(ifd)
+    fd = ifd
     objs = fd.propagators
     for p in objs:
         if p.label is None or replace:
             p.label = "$" + p.particle.latex_name + "$"
     return fd
 
 
 def auto_label_legs(ifd, replace=False):
     """Automatically label legs."""
-    fd = copy.deepcopy(ifd)
+    # fd = copy.deepcopy(ifd)
+    fd = ifd
     objs = fd.legs
     for p in objs:
         if p.particle is None or replace:
             p.particle = "$" + p.particle.latex_name + "$"
     return fd
```

### Comparing `pyfeyn2-2.3.5/pyfeyn2/auto/position.py` & `pyfeyn2-2.3.6/pyfeyn2/auto/position.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import itertools
 import logging
 from itertools import permutations
 
+import iminuit
 import numpy as np
-from feynml import Point, Propagator
+from feynml import Leg, Point, Propagator
 
 from pyfeyn2.interface.dot import dot_to_positions, feynman_to_dot
 
 
 # from https://stackoverflow.com/a/9997374
 def ccw(A, B, C):
     """
@@ -56,14 +57,22 @@
     if B.x == C.x and B.y == C.y:
         return False
     if B.x == D.x and B.y == D.y:
         return False
     return ccw(A, C, D) != ccw(B, C, D) and ccw(A, B, C) != ccw(A, B, D)
 
 
+def set_none_xy_to_zero(points):
+    for p in points:
+        if p.x is None:
+            p.x = 0
+        if p.y is None:
+            p.y = 0
+
+
 def require_xy(points):
     # check if a vertex or leg is missing a x or y position
     for v in points:
         if v.x is None:
             raise Exception(f"Vertex or leg {v} is missing x position.")
         if v.y is None:
             raise Exception(f"Vertex or leg {v} is missing y position.")
@@ -146,40 +155,46 @@
     return fd
 
 
 def auto_align_legs(fd, incoming=None, outgoing=None):
     """
     Automatically reshuffle the legs of a Feynman diagram.
     """
-    f_min_x, f_min_y, f_max_x, f_max_y = fd.get_bounding_box()
+    set_none_xy_to_zero(fd.legs)
     inc = [l for l in fd.legs if l.is_incoming()]
     outc = [l for l in fd.legs if l.is_outgoing()]
-    if incoming is None:
-        incoming = [[f_min_x, y] for y in np.linspace(f_min_y, f_max_y, len(inc))]
-    if outgoing is None:
-        outgoing = [[f_max_x, y] for y in np.linspace(f_min_y, f_max_y, len(outc))]
+    if incoming is None or outgoing is None:
+        f_min_x, f_min_y, f_max_x, f_max_y = fd.get_bounding_box()
+        if incoming is None:
+            incoming = [[f_min_x, y] for y in np.linspace(f_min_y, f_max_y, len(inc))]
+        if outgoing is None:
+            outgoing = [[f_max_x, y] for y in np.linspace(f_min_y, f_max_y, len(outc))]
     _auto_align(inc, incoming)
     _auto_align(outc, outgoing)
     return fd
 
 
+def _get_dist(points, positions):
+    dist = np.ones((len(points), len(positions))) * np.inf
+    for i, v in enumerate(points):
+        for j, p in enumerate(positions):
+            dist[i][j] = np.sqrt((v.x - p[0]) ** 2 + (v.y - p[1]) ** 2)
+    return dist
+
+
 def _auto_align(points, positions):
     """
     Automatically position the vertices and legs on a list of positions.
     """
     logging.debug(f"_auto_align: positions {positions}")
     # check if a vertex or leg is missing a x or y position
     require_xy(points)
-    vpl = len(points)
     # table of distances between vertices v and points p
-    dist = np.ones((vpl, len(positions))) * np.inf
-    for i, v in enumerate(points):
-        for j, p in enumerate(positions):
-            dist[i][j] = np.sqrt((v.x - p[0]) ** 2 + (v.y - p[1]) ** 2)
-    for i in range(vpl):
+    dist = _get_dist(points, positions)
+    for i in range(len(points)):
         min_i, min_j = np.unravel_index(dist.argmin(), dist.shape)
         v = points[min_i]
         v.x = positions[min_j][0]
         v.y = positions[min_j][1]
         # remove min_i and min_j from dist
         dist[min_i, :] = np.inf
         dist[:, min_j] = np.inf
@@ -208,34 +223,39 @@
 def auto_grid(fd, n_x=None, n_y=None, min_x=None, min_y=None, max_x=None, max_y=None):
     """
     Automatically position the vertices and legs on a grid, with the given
     minimum and maximum values for x and y, and the number of grid points, but
     avoid placing vertices or legs on the same position.
     """
     # get the bounding box and construct grid from that
+    positions = _get_grid(fd, n_x, n_y, min_x, min_y, max_x, max_y)
+    return auto_align(fd, positions)
+
+
+def _get_grid(fd, n_x=None, n_y=None, min_x=None, min_y=None, max_x=None, max_y=None):
+    logging.debug(f"_get_grid {n_x}, {n_y}, {min_x}, {min_y}, {max_x}, {max_y}")
     f_min_x, f_min_y, f_max_x, f_max_y = fd.get_bounding_box()
     if n_x is None:
         n_x = len(fd.vertices) + len(fd.legs)
     if n_y is None:
         n_y = len(fd.vertices) + len(fd.legs)
     if min_x is None:
         min_x = f_min_x
     if max_x is None:
         max_x = f_max_x
     if min_y is None:
         min_y = f_min_y
     if max_y is None:
         max_y = f_max_y
-    logging.debug(f"auto_grid {n_x}, {n_y}, {min_x}, {min_y}, {max_x}, {max_y}")
-
+    # print(min_x, max_x, min_y, max_y, n_x, n_y)
     xvalues = np.linspace(min_x, max_x, n_x)
     yvalues = np.linspace(min_y, max_y, n_y)
     xx, yy = np.meshgrid(xvalues, yvalues)
     positions = [[x, y] for x, y in zip(xx.flatten(), yy.flatten())]
-    return auto_align(fd, positions)
+    return positions
 
 
 def auto_position(fd, layout="neato", clear_vertices=True):
     """Automatically position the vertices and legs."""
     # fd = scale_positions(fd, 10)
     fd = fd.with_style(f"layout : {layout}")
     fd = incoming_to_left(fd)
@@ -332,7 +352,165 @@
                 raise Exception(
                     f"Unknown case, source == source or target == target, {v} {ps[0]} {ps[1]}"
                 )
             continue
         vertices.append(v)
     fd.vertices = vertices
     return fd
+
+
+def auto_vdw(fd, points=None, LJ=1.0, y_symmetry=0.0, x_symmetry=0.0, intersection=0.0):
+    """
+    Minimizes Lennard-Jones potential between vertices and legs (scaled by LJ).
+    Further the function to be minimized gets punished by the number of intersections scaled by intersection.
+    The function to be minimized gets punished by the asymmetry in x and y direction scaled by x_symmetry and y_symmetry.
+
+    Parameters
+    ----------
+    fd : FeynmanDiagram
+        The Feynman diagram to be positioned.
+    points : list of Point, optional
+        The points (leg or vertex) to be positioned. Recommended values are fd.vertices or [*fd.vertices, *fd.legs]
+    LJ : float, optional
+        The strength of the Lennard-Jones potential, by default 1.0
+    y_symmetry : float, optional
+        The strength of the punishment for asymmetry in y direction, by default 0.0
+    x_symmetry : float, optional
+        The strength of the punishment for asymmetry in x direction, by default 0.0
+    intersection : float, optional
+        The strength of the punishment for intersections, by default 0.0
+
+    Returns
+    -------
+    FeynmanDiagram
+        The Feynman diagram with the vertices and legs positioned.
+
+
+
+    """
+    if points is None:
+        points = fd.vertices
+    r = LJ
+    all_points = [*fd.vertices, *fd.legs]
+    set_none_xy_to_zero(points)
+    # get distance to connected points
+    cons = []
+    # dist = []
+    for p in points:
+        n = []
+        # dd = []
+        for c in fd.get_neighbours(p):
+            for j, pp in enumerate(all_points):
+                if pp.x is None or pp.y is None:
+                    continue
+                if pp.id == c.id:
+                    n.append(j)
+                    # dd.append(np.sqrt((p.x - pp.x) ** 2 + (p.y - pp.y) ** 2))
+        cons.append(n)
+        # dist.append(dd)
+
+    def fun(*args):
+        for i, p in enumerate(points):
+            p.x = args[2 * i]
+            p.y = args[2 * i + 1]
+        LenJ = 0
+        if LJ != 0.0:
+            for i, p in enumerate(points):
+                for j in cons[i]:
+                    if all_points[j].x is not None and all_points[j].y is not None:
+                        LenJ = (
+                            LenJ
+                            - (
+                                (
+                                    (
+                                        (
+                                            (p.x - all_points[j].x) ** 2
+                                            + (p.y - all_points[j].y) ** 2
+                                        )
+                                        ** 0.5
+                                    )
+                                    / r
+                                )
+                                ** 6
+                            )
+                            + (
+                                (
+                                    (
+                                        (p.x - all_points[j].x) ** 2
+                                        + (p.y - all_points[j].y) ** 2
+                                    )
+                                    ** 0.5
+                                )
+                                / r
+                            )
+                            ** 12
+                        )
+        inter = 0
+        if intersection != 0.0:
+            inter += intersection * _compute_number_of_intersects(fd)
+        pun_x = 0
+        if x_symmetry != 0.0:
+            min_x, min_y, max_x, max_y = fd.get_bounding_box()
+            # get averate x and y
+            avg_x = (min_x + max_x) / 2
+            avg_y = (min_y + max_y) / 2
+            pun = 0
+            for p in points:
+                nx = p.x - 2 * (p.x - avg_x)
+                # find nearest point to (nx, p.y)
+                min_dist = np.inf
+                for pp in all_points:
+                    if pp.id == p.id or pp.x is None or pp.y is None:
+                        continue
+                    dist = np.sqrt((nx - pp.x) ** 2 + (p.y - pp.y) ** 2)
+                    if dist < min_dist:
+                        min_dist = dist
+                pun += min_dist
+            pun_x = pun
+        pun_y = 0
+        if y_symmetry != 0.0:
+            min_x, min_y, max_x, max_y = fd.get_bounding_box()
+            # get averate x and y
+            avg_x = (min_x + max_x) / 2
+            avg_y = (min_y + max_y) / 2
+            pun = 0
+            for p in points:
+                ny = p.y - 2 * (p.y - avg_y)
+                # find nearest point to (p.x, ny)
+                min_dist = np.inf
+                for pp in all_points:
+                    if pp.id == p.id or pp.x is None or pp.y is None:
+                        continue
+                    dist = np.sqrt((p.x - pp.x) ** 2 + (ny - pp.y) ** 2)
+                    if dist < min_dist:
+                        min_dist = dist
+                pun += min_dist
+            pun_y = pun
+        # TODO add punishment for intersections
+        # TODO add punishment for asymmetry
+        return LenJ + inter + pun_x * x_symmetry + pun_y * y_symmetry
+
+    m = iminuit.Minuit(fun, *[0 for _ in range(len(points) * 2)])
+    v = m.migrad()
+    args = list(v.values.to_dict().values())
+    for i, p in enumerate(points):
+        p.x = args[2 * i]
+        p.y = args[2 * i + 1]
+    return fd
+
+
+def auto_gridded_springs(
+    fd,
+    points=None,
+    n_x=None,
+    n_y=None,
+    min_x=None,
+    min_y=None,
+    max_x=None,
+    max_y=None,
+    **kwargs,
+):  # TODO replace kwargs by actual arguments (i.e. for documentation)
+    fd = auto_vdw(fd, points, **kwargs)
+    fd = auto_grid(
+        fd, n_x=n_x, n_y=n_y, min_x=min_x, min_y=min_y, max_x=max_x, max_y=max_y
+    )
+    return fd
```

### Comparing `pyfeyn2-2.3.5/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.3.6/pyfeyn2/feynmandiagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/interface/dot.py` & `pyfeyn2-2.3.6/pyfeyn2/interface/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/mkfeyndiag.py` & `pyfeyn2-2.3.6/pyfeyn2/mkfeyndiag.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,14 @@
 from xsdata.formats.dataclass.parsers import XmlParser
 
 import pyfeyn2.render.all as renderall
 from pyfeyn2.render.text.ascii import ASCIIRender
 from pyfeyn2.render.text.unicode import UnicodeRender
 
 
-def class_for_name(module_name, class_name):
-    # load the module, will raise ImportError if module cannot be loaded
-    m = importlib.import_module(module_name)
-    # get the class, will raise AttributeError if class cannot be found
-    c = getattr(m, class_name)
-    return c
-
-
-def renderer_from_string(s):
-    return class_for_name(".".join(s.split(".")[0:-1]), s.split(".")[-1])
-
-
 def main(argv=None):
     # parse command line options with argparse
     parser = argparse.ArgumentParser(
         prog="pyfeyn2.mkfeyndiag",
         description="Draw FeynML diagrams with pyfeyn2.",
     )
     parser.add_argument(
@@ -72,32 +60,23 @@
         help="Diagram id to render.",
     )
 
     args = parser.parse_args(argv)
 
     arenderer = args.renderer
     renderer = None
-    if arenderer is None:
-        pass
-    elif arenderer.lower() == "ascii":
-        renderer = ASCIIRender
-    elif arenderer.lower() == "unicode":
-        renderer = UnicodeRender
-    elif arenderer.lower() in renderall.renders:
-        renderer = renderall.renders[arenderer.lower()]
-    else:
-        renderer = renderer_from_string(arenderer)
+    renderer = renderall.renderer_from_string(arenderer)
 
     xml_string = Path(args.input).read_text()
     parser = XmlParser()
     fml = parser.from_string(xml_string, FeynML)
 
     if renderer is None:
         arenderer = fml.head.get_meta_dict()["renderer"]
-        renderer = renderer_from_string(arenderer)
+        renderer = renderall.renderer_from_string(arenderer)
     if args.style is not None:
         style_string = Path(args.style).read_text()
         for diagram in fml.diagrams:
             diagram.external_sheet = cssutils.parseString(style_string)
 
     for i, d in enumerate(fml.diagrams):
         if args.diagram is None or args.diagram == d.id:
```

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/all.py` & `pyfeyn2-2.3.6/pyfeyn2/render/all.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import importlib
 import shutil
 import tempfile
 import traceback
 from typing import List
 
 from feynml.shape import get_shapes
 from feynml.type import get_types
@@ -10,28 +11,51 @@
 
 from pyfeyn2.render.latex.dot import DotRender
 from pyfeyn2.render.latex.feynmp import FeynmpRender
 from pyfeyn2.render.latex.latex import LatexRender
 from pyfeyn2.render.latex.tikzfeynman import TikzFeynmanRender
 from pyfeyn2.render.mpl.feynmanrender import FeynmanRender
 from pyfeyn2.render.pyx.pyxrender import PyxRender
+from pyfeyn2.render.text.ascii import ASCIIRender
 from pyfeyn2.render.text.asciipdf import ASCIIPDFRender
+from pyfeyn2.render.text.unicode import UnicodeRender
 from pyfeyn2.render.text.unicodepdf import UnicodePDFRender
 
 renders = {
     "tikz": TikzFeynmanRender,
     "pyx": PyxRender,
     "feynmp": FeynmpRender,
     "feynman": FeynmanRender,
     "dot": DotRender,
     "asciipdf": ASCIIPDFRender,
     "unicodepdf": UnicodePDFRender,
 }
 
 
+def class_for_name(module_name, class_name):
+    # load the module, will raise ImportError if module cannot be loaded
+    m = importlib.import_module(module_name)
+    # get the class, will raise AttributeError if class cannot be found
+    c = getattr(m, class_name)
+    return c
+
+
+def renderer_from_string(s):
+    if s is None:
+        return None
+    elif s.lower() == "ascii":
+        return ASCIIRender
+    elif s.lower() == "unicode":
+        return UnicodeRender
+    elif s.lower() in renders:
+        return renders[s.lower()]
+    else:
+        return class_for_name(".".join(s.split(".")[0:-1]), s.split(".")[-1])
+
+
 class AllRender(LatexRender):
     """Render all diagrams to PDF."""
 
     def __init__(
         self,
         fd=None,
         documentclass="standalone",
```

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.3.6/pyfeyn2/render/latex/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.3.6/pyfeyn2/render/latex/feynmp.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.3.6/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.3.6/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.3.6/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.3.6/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/lines.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/pyxrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.3.6/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/render.py` & `pyfeyn2-2.3.6/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/ascii.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/label.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/line.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/plainpdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/point.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/point.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/style.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.3.6/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.3.5/pyproject.toml` & `pyfeyn2-2.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.3.5"
+version = "2.3.6"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 particle = "*"
 xsdata = {version = "*", extras = ["cli","lxml","soap"]}
 pylatex = "*"
 dot2tex = "*"
 matplotlib = ">=1.4.0,<4.0.0"
 Wand = "*"
-numpy = ">=1.6,<1.24" # Upper limit due to feynman using np.complex
+numpy = ">=1.6,<1.25" # Upper limit due to feynman using np.complex
 pyx = ">=0.12,<1.0.0"
 pydot = "*"
 feynman="^2.0"
 cssutils= "*"
 pylatexenc = "*"
 pygments = "*"
 graphviz = "*"
 ipyparallel = "*"
 deprecated = "*"
 deprecation = "*"
 cssselect ="*"
 smpl_io = "*"
 smpl_doc = "*"
 smpl_util= "*"
-feynml = {version = ">=0.2.8", extras = ["interfaces"]}
+iminuit = "*"
+colorama = "*"
+termcolor = "*"
+feynml = {version = ">=0.2.10", extras = ["interfaces"]}
 #feynml= {path= "../feynml", develop = true, extras = ["interfaces"]}
 
 [tool.poetry.scripts]
 mkfeyndiag = "pyfeyn2.mkfeyndiag:main"
 
 [tool.poetry.group.docs]
 optional = true
@@ -44,16 +47,14 @@
 sphinxcontrib-napoleon = "*"
 nbsphinx = "*"
 jupyter-sphinx = "*"
 sphinx_autobuild = "*"
 sphinx_math_dollar = "*"
 myst-parser  = "*"
 toml = "*"
-colorama = "*"
-termcolor = "*"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov =  "*"
```

### Comparing `pyfeyn2-2.3.5/setup.py` & `pyfeyn2-2.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,42 +12,45 @@
  'pyfeyn2.render.text']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Wand',
+ 'colorama',
  'cssselect',
  'cssutils',
  'deprecated',
  'deprecation',
  'dot2tex',
  'feynman>=2.0,<3.0',
- 'feynml[interfaces]>=0.2.8',
+ 'feynml[interfaces]>=0.2.10',
  'graphviz',
+ 'iminuit',
  'ipyparallel',
  'matplotlib>=1.4.0,<4.0.0',
- 'numpy>=1.6,<1.24',
+ 'numpy>=1.6,<1.25',
  'particle',
  'pydot',
  'pygments',
  'pylatex',
  'pylatexenc',
  'pyx>=0.12,<1.0.0',
  'smpl_doc',
  'smpl_io',
  'smpl_util',
+ 'termcolor',
  'xsdata[cli,lxml,soap]']
 
 entry_points = \
 {'console_scripts': ['mkfeyndiag = pyfeyn2.mkfeyndiag:main']}
 
 setup_kwargs = {
     'name': 'pyfeyn2',
-    'version': '2.3.5',
+    'version': '2.3.6',
     'description': 'PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around',
     'long_description': "# PyFeyn2\n\nForked from <https://pyfeyn.hepforge.org/> \n\nPyFeyn is a Python-language based system for drawing Feynman diagrams. It was inspired by the C++ FeynDiagram system, and aims to provide the same functionality and quality of output as that, with the added benefits of a modern interpreted language, an improved interface and output direct to both EPS and PDF. Behind the scenes, PyFeyn uses the excellent PyX system - you can use PyX constructs in PyFeyn diagrams if you want, too.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link]  ![downloads](https://img.shields.io/pypi/dm/pyfeyn2.svg)\n\n[![test][a t image]][a t link]      [![Coverage Status][c t i]][c t l]  [![Codacy Badge][cc c i]][cc c l]   [![Codacy Badge][cc q i]][cc q l]  [![Documentation][rtd t i]][rtd t l]\n\n## Dependencies\n\n*   libmagickwand-dev (to display pdfs in a jupyter-notebook, might require a policy change of the imagemagick config for PDFs, see Troubleshooting)\n*   ghostscript\n*   latexmk\n*   (graphviz)\n*   (feynmp-auto/feynmf)\n\n## Installation\n\n```sh\npoerty install --with docs --with dev\npoetry shell\n```\n\n## Documentation\n\n*   <https://pyfeyn2.readthedocs.io/en/stable/>\n*   <https://apn-pucky.github.io/pyfeyn2/index.html>\n\n## Similar Feynman diagram rendering project:\n\n*   <https://github.com/ndeutschmann/qgraf-xml-drawer>\n*   <https://github.com/GkAntonius/feynman>\n*   <https://github.com/JP-Ellis/tikz-feynman>\n*   <https://pyfeyn.hepforge.org/> \n*   <https://feynml.hepforge.org/>\n*   <http://www.feyndiagram.com/>\n\nSeveral of these are integrated into pyfeyn2.\n\n## Troubleshooting\n\n*   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )\n\n## Development\n\n\n### package/python structure:\n\n*   <https://mathspp.com/blog/how-to-create-a-python-package-in-2022>\n*   <https://www.brainsorting.com/posts/publish-a-package-on-pypi-using-poetry/>\n\n[pypi image]: https://badge.fury.io/py/pyfeyn2.svg\n[pypi link]: https://pypi.org/project/pyfeyn2/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyfeyn2.svg\n\n[a t link]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyfeyn2/actions/workflows/test.yml/badge.svg\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/135bae47c6344ab0bfb180135ea1db44\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/pyfeyn2&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/135bae47c6344ab0bfb180135ea1db44\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyfeyn2/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/pyfeyn2&utm_campaign=Badge_Coverage\n\n[c t l]: https://coveralls.io/github/APN-Pucky/pyfeyn2?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyfeyn2/badge.svg?branch=master\n\n[rtd t i]: https://readthedocs.org/projects/pyfeyn2/badge/?version=latest\n[rtd t l]: https://pyfeyn2.readthedocs.io/en/latest/?badge=latest\n",
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyfeyn2',
```

### Comparing `pyfeyn2-2.3.5/PKG-INFO` & `pyfeyn2-2.3.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.3.5
+Version: 2.3.6
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Wand
+Requires-Dist: colorama
 Requires-Dist: cssselect
 Requires-Dist: cssutils
 Requires-Dist: deprecated
 Requires-Dist: deprecation
 Requires-Dist: dot2tex
 Requires-Dist: feynman (>=2.0,<3.0)
-Requires-Dist: feynml[interfaces] (>=0.2.8)
+Requires-Dist: feynml[interfaces] (>=0.2.10)
 Requires-Dist: graphviz
+Requires-Dist: iminuit
 Requires-Dist: ipyparallel
 Requires-Dist: matplotlib (>=1.4.0,<4.0.0)
-Requires-Dist: numpy (>=1.6,<1.24)
+Requires-Dist: numpy (>=1.6,<1.25)
 Requires-Dist: particle
 Requires-Dist: pydot
 Requires-Dist: pygments
 Requires-Dist: pylatex
 Requires-Dist: pylatexenc
 Requires-Dist: pyx (>=0.12,<1.0.0)
 Requires-Dist: smpl_doc
 Requires-Dist: smpl_io
 Requires-Dist: smpl_util
+Requires-Dist: termcolor
 Requires-Dist: xsdata[cli,lxml,soap]
 Project-URL: Repository, https://github.com/APN-Pucky/pyfeyn2
 Description-Content-Type: text/markdown
 
 # PyFeyn2
 
 Forked from <https://pyfeyn.hepforge.org/>
```

