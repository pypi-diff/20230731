# Comparing `tmp/synth_mapping_helper-1.2.4.tar.gz` & `tmp/synth_mapping_helper-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.2.4.tar", last modified: Wed Jul 26 17:48:12 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.3.0.tar", last modified: Mon Jul 31 18:49:19 2023, max compression
```

## Comparing `synth_mapping_helper-1.2.4.tar` & `synth_mapping_helper-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 17:48:12.181260 synth_mapping_helper-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.173260 synth_mapping_helper-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28834 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 17:48:12.000000 synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:48:12.177260 synth_mapping_helper-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 17:48:00.000000 synth_mapping_helper-1.2.4/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:49:19.694785 synth_mapping_helper-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-31 18:49:19.694785 synth_mapping_helper-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 18:49:19.694785 synth_mapping_helper-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:49:19.690785 synth_mapping_helper-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:49:19.694785 synth_mapping_helper-1.3.0/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29082 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:49:19.694785 synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-31 18:49:19.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-31 18:49:19.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:49:19.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 18:49:19.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 18:49:19.000000 synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:49:19.694785 synth_mapping_helper-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 18:49:03.000000 synth_mapping_helper-1.3.0/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.2.4/LICENSE` & `synth_mapping_helper-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/PKG-INFO` & `synth_mapping_helper-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.2.4
+Version: 1.3.0
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
@@ -47,14 +47,15 @@
     * Spike/Buzz-Rails
     * Stack along rails
 * Rail manipulation
     * Merging
     * Splitting
     * Interpolation
     * Convert between single notes and rails
+    * Snapping single notes to rails
 * Cross-Platform (Windows, Linux)
     * For Windows, supports drag and drop actions (fully usable without command prompt)
 * Imports directly from clipboard, and export to it
 * Uses an internal format that is easy to work with ([wiki page](https://github.com/adosikas/synth_mapping_helper/wiki/Glossary#measurement-system)):
     * Position in editor grid coordinates (+x=right, +y=up)
     * Time in measures (starting from start of selection)
     * Angles in degrees (positive=counterclockwise)
```

### Comparing `synth_mapping_helper-1.2.4/README.md` & `synth_mapping_helper-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     * Spike/Buzz-Rails
     * Stack along rails
 * Rail manipulation
     * Merging
     * Splitting
     * Interpolation
     * Convert between single notes and rails
+    * Snapping single notes to rails
 * Cross-Platform (Windows, Linux)
     * For Windows, supports drag and drop actions (fully usable without command prompt)
 * Imports directly from clipboard, and export to it
 * Uses an internal format that is easy to work with ([wiki page](https://github.com/adosikas/synth_mapping_helper/wiki/Glossary#measurement-system)):
     * Position in editor grid coordinates (+x=right, +y=up)
     * Time in measures (starting from start of selection)
     * Angles in degrees (positive=counterclockwise)
```

### Comparing `synth_mapping_helper-1.2.4/setup.py` & `synth_mapping_helper-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     preproc_group.add_argument("-n", "--change-notes", metavar="NEW_NOTE_TYPE", nargs="+", choices=synth_format.NOTE_TYPES, help=f"Change the type/color of notes. Specify multiple to loop over them.")
     preproc_group.add_argument("-w", "--change-walls", metavar="NEW_WALL_TYPE", nargs="+", choices=synth_format.WALL_TYPES, help=f"Change the type of walls. Specify multiple to loop over them.")
     preproc_group.add_argument("--spawn", metavar="OBJECT_TYPE", choices=synth_format.ALL_TYPES, help="Spawn an objects of the given type. Can only spawn one object per call.")
     preproc_group.add_argument("--spawn-location", type=utils.parse_position, help="Location for the spawned object (defaults to 0,0,0)")
 
     rail_pattern_group = parser.add_argument_group("rail patterns")
     interp_group = rail_pattern_group.add_mutually_exclusive_group()
-    interp_group.add_argument("--interpolate", type=utils.parse_time, metavar="INTERVAL", help="Subdivide rail into segments of this length in beats, interpolating using splines (similar to the game). Supports fractions. When used with --spiral or --spikes, this is the distance between each nodes")
+    interp_group.add_argument("--interpolate", type=utils.parse_time, metavar="INTERVAL", help="Subdivide rail into segments of this length in beats, interpolating using splines close to the editor. Supports fractions. When used with --spiral or --spikes, this is the distance between each nodes")
     interp_group.add_argument("--interpolate-linear", type=utils.parse_time, metavar="INTERVAL", help="Subdivide rail into segments of this length in beats, interpolating linearly. Supports fractions. When used with --spiral or --spikes, this is the distance between each nodes")
     rail_pattern_group.add_argument("--shorten-rails", type=utils.parse_time, metavar="DISTANCE", help="Cut some distance from every rail. Supports fractions. When negative, cuts from the start instead of the end")
     rail_pattern_group.add_argument("--start-angle", type=utils.parse_number, default=0.0, metavar="DEGREES", help="Angle of the first node of the spiral in degrees. Default: 0/right")
     rail_pattern_group.add_argument("--radius", type=utils.parse_number, default=1.0, help="Radius of spiral or length of spikes")
     rail_op_group = rail_pattern_group.add_mutually_exclusive_group()
     rail_op_group.add_argument("--spiral", type=utils.parse_number, metavar="NODES_PER_ROT", help="Generate counterclockwise spiral around rails with this number of nodes per full rotation. Supports fractions. 2=zigzag, negative=clockwise")
     rail_op_group.add_argument("--spikes", type=utils.parse_number, metavar="NODES_PER_ROT", help="Generate spikes from rail, either spiraling (see --spiral) or random (when set to 0)")
@@ -131,14 +131,15 @@
     movement_group.add_argument("--stack-duration", type=utils.parse_time, help="Like --stack-count, but you can give it during in beats ('4') or seconds ('2s').")
     movement_group.add_argument("--autostack", nargs="?", choices=("OFFSET", "SPIRAL", "OUTSET", "SCALE"), action="append", metavar="OFFSET/SPIRAL/OUTSET/SCALE", help="Find the first pair of matching objects and continue the pattern. For continuing the positions, the following modes are supported: OFFSET (default, absolute xy), SPIRAL (rotate around implied pivot), OUTSET (distance from pivot) and SCALE (xy ratio).")
 
     postproc_group = parser.add_argument_group("post-processing")
     postproc_group.add_argument("--parallels", type=utils.parse_number, metavar="DISTANCE", help="Create parallel left/right handed patterns with given spacing from input. Negative numbers result in crossovers.")
     postproc_group.add_argument("--split-rails", action="store_true", help="Split rails at single notes")
     postproc_group.add_argument("--rails-to-singles", type=int, nargs="?", action="append", metavar="KEEP_RAIL", help="Replace rails with single notes at all nodes. KEEP_RAIL is optional and can be '1' if you want to keep the rail instead of replacing it")
+    postproc_group.add_argument("--snap-singles-to-rail", action="store_true", help="Snap single notes to rail of the same color")
     postproc_group.add_argument("--keep-alignment", action="store_true", help="Do NOT shift the start of selection to first element")
 
     return parser
 
 def abort(reason: str):
     print("ERROR: " + reason)
     exit(1)
@@ -414,11 +415,13 @@
         # wipe single & both
         data.single = {}
         data.both = {}
     if options.split_rails:
         data.apply_for_note_types(rails.split_rails, types=filter_types)
     if options.rails_to_singles:
         data.apply_for_note_types(rails.rails_to_singles, keep_rail=bool(options.rails_to_singles[0]), types=filter_types)
+    if options.snap_singles_to_rail:
+        data.apply_for_note_types(rails.snap_singles_to_rail, types=filter_types)
     synth_format.export_clipboard(data, not options.keep_alignment)
 
 if __name__ == "__main__":
     main(get_parser().parse_args())
```

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/companion.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/rails.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from scipy.interpolate import pchip_interpolate
+from scipy.interpolate import CubicHermiteSpline
 
 from .synth_format import DataContainer, SINGLE_COLOR_NOTES
 from .utils import bounded_arange
 
 # How far last node and start note can be spaced for two rails to be merged
 MERGE_ACCURACY_GRID = 1 / 8
 MERGE_ACCURACY_BEAT = 1 / 64
@@ -11,24 +11,40 @@
 def interpolate_linear(data: "numpy array (n, m)", new_z: "numpy array (x)", *, direction: bool = 1) -> "numpy array (x, 3)":
     return np.stack((
         np.interp(new_z, data[:, 2], data[:, 0]),
         np.interp(new_z, data[:, 2], data[:, 1]),
         new_z,
     ), axis=-1)
 
-def interpolate_spline(data: "numpy array (n, m)", new_z: "numpy array (x)", *, direction: bool = 1) -> "numpy array (x, 3)":
+def synth_curve(data: "numpy array (n, m)", *, direction: bool = 1):
+    # based on https://github.com/LittleAsi/synth-riders-editor,
+    # which uses LineSmoother.cs from https://forum.unity.com/threads/easy-curved-line-renderer-free-utility.391219
     if data.shape[0] == 1:
         return data
-    # add points in straight line from start and end to match shape more closely
-    padded_data = np.concatenate(([2*data[0]-data[1]], data, [2*data[-1]-data[-2]]))
-    return np.stack((
-        pchip_interpolate(padded_data[:, 2], padded_data[:, 0], new_z),
-        pchip_interpolate(padded_data[:, 2], padded_data[:, 1], new_z),
-        new_z,
-    ), axis=-1)
+
+    # equivalent of Unity's AnimationCurve when doing smoothTangents(0)
+    tangents = np.diff(data, axis=0, prepend=data[0][np.newaxis], append=data[-1][np.newaxis])
+    smoothed_tangents = (tangents[:-1] + tangents[1:]) / 2
+
+    # this interpolates not only x and y, but also time
+    curve = CubicHermiteSpline(range(data.shape[0]), data, smoothed_tangents)
+    curve_points = []
+    for i in range(data.shape[0]-1):
+        curve_points.append(data[i])
+        # interpolate a number of points which is based on distance between nodes
+        # intermediates = int(np.linalg.norm(coord_to_synth(240, data[i+1]-data[i])) / 0.15)
+
+        # we use a different formula, which doesn't rely on BPM but produces very similar results
+        intermediates = int(np.linalg.norm((data[i+1]-data[i])*(0.1,0.1,8)))
+        curve_points.extend(curve(i + np.arange(1, intermediates)/intermediates))
+    curve_points.append(data[-1])
+    return np.array(curve_points)
+
+def interpolate_spline(data: "numpy array (n, m)", new_z: "numpy array (x)", *, direction: bool = 1) -> "numpy array (x, 3)":
+    return interpolate_linear(synth_curve(data), new_z, direction=direction)
 
 def get_position_at(notes: SINGLE_COLOR_NOTES, beat: float, interpolate_gaps: bool = True) -> "numpy array (2)":
     # single note
     if beat in notes:
         return notes[beat][0, 0:2].copy()
     last_before = None
     # on rail, or between notes: interpolate
@@ -84,14 +100,34 @@
                 out[current_rail_start] = previous_nodes[: last_index + 2]
 
             current_rail_start = remainder[0, 2]
             current_rail_end = remainder[-1, 2]
 
     return out
 
+def snap_singles_to_rail(notes: SINGLE_COLOR_NOTES, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
+    """snap single notes to rail"""
+    current_rail_start = None
+    current_rail_end = None
+    out: SINGLE_COLOR_NOTES = {}
+
+    for time in sorted(notes):
+        if current_rail_start is not None and time >= current_rail_end:  # current time is past end of stored rail -> forget stored rail
+            current_rail_start = None
+            current_rail_end = None
+        nodes = notes[time]
+        if nodes.shape[0] > 1:  # rail: store start/end and keep as-is
+            current_rail_start = nodes[0, 2]
+            current_rail_end = nodes[-1, 2]
+            out[time] = nodes
+        elif current_rail_start is not None:  # single next to rail -> snap to it
+            out[time] = interpolate_spline(out[current_rail_start], [time])
+        else:  # single without rail next to it: keep as-is
+            out[time] = nodes
+    return out
 
 def merge_sequential_rails(notes: SINGLE_COLOR_NOTES, *, direction: bool = 1) -> SINGLE_COLOR_NOTES:
     """merges rails where end and start a very close"""
     current_rail_start = None
     current_rail_end = None
     out: SINGLE_COLOR_NOTES = {}
```

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/synth_format.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.2.4
+Version: 1.3.0
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
@@ -47,14 +47,15 @@
     * Spike/Buzz-Rails
     * Stack along rails
 * Rail manipulation
     * Merging
     * Splitting
     * Interpolation
     * Convert between single notes and rails
+    * Snapping single notes to rails
 * Cross-Platform (Windows, Linux)
     * For Windows, supports drag and drop actions (fully usable without command prompt)
 * Imports directly from clipboard, and export to it
 * Uses an internal format that is easy to work with ([wiki page](https://github.com/adosikas/synth_mapping_helper/wiki/Glossary#measurement-system)):
     * Position in editor grid coordinates (+x=right, +y=up)
     * Time in measures (starting from start of selection)
     * Angles in degrees (positive=counterclockwise)
```

### Comparing `synth_mapping_helper-1.2.4/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.3.0/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

