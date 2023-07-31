# Comparing `tmp/dtumathtools-1.0.5.tar.gz` & `tmp/dtumathtools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtumathtools-1.0.5.tar", last modified: Sat Apr 15 12:29:47 2023, max compression
+gzip compressed data, was "dtumathtools-1.1.0.tar", last modified: Mon Jul 31 16:26:46 2023, max compression
```

## Comparing `dtumathtools-1.0.5.tar` & `dtumathtools-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.555012 dtumathtools-1.0.5/
--rw-rw-rw-   0        0        0     1471 2023-01-29 21:40:49.000000 dtumathtools-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3648 2023-04-15 12:29:47.553015 dtumathtools-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2635 2023-01-29 21:46:36.000000 dtumathtools-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-15 12:29:47.555012 dtumathtools-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1867 2023-04-15 12:25:48.000000 dtumathtools-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.423995 dtumathtools-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.444996 dtumathtools-1.0.5/src/dtumathtools/
--rw-rw-rw-   0        0        0       84 2023-01-30 09:29:20.000000 dtumathtools-1.0.5/src/dtumathtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.530011 dtumathtools-1.0.5/src/dtumathtools/dtuplot/
--rw-rw-rw-   0        0        0      203 2023-04-14 15:52:31.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/__init__.py
--rw-rw-rw-   0        0        0     2766 2023-04-14 17:21:58.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/boundaryplot.py
--rw-rw-rw-   0        0        0     6322 2022-12-23 22:17:04.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/quiverplot.py
--rw-rw-rw-   0        0        0     2643 2022-12-23 23:07:43.000000 dtumathtools-1.0.5/src/dtumathtools/dtuplot/scatterplot.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.535010 dtumathtools-1.0.5/src/dtumathtools/dtutools/
--rw-rw-rw-   0        0        0       73 2023-04-10 14:03:03.000000 dtumathtools-1.0.5/src/dtumathtools/dtutools/__init__.py
--rw-rw-rw-   0        0        0     3166 2023-04-14 15:52:31.000000 dtumathtools-1.0.5/src/dtumathtools/dtutools/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.517015 dtumathtools-1.0.5/src/dtumathtools.egg-info/
--rw-rw-rw-   0        0        0     3648 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      533 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-15 12:29:47.000000 dtumathtools-1.0.5/src/dtumathtools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:47.551011 dtumathtools-1.0.5/tests/
--rw-rw-rw-   0        0        0     1028 2023-04-14 17:06:37.000000 dtumathtools-1.0.5/tests/test_dtuplot.py
--rw-rw-rw-   0        0        0     1802 2023-03-19 14:08:01.000000 dtumathtools-1.0.5/tests/test_dtutools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:46.898336 dtumathtools-1.1.0/
+-rw-rw-rw-   0        0        0     1471 2023-01-29 21:40:49.000000 dtumathtools-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3731 2023-07-31 16:26:46.890417 dtumathtools-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2635 2023-01-29 21:46:36.000000 dtumathtools-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:26:46.898336 dtumathtools-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2547 2023-07-31 16:26:19.000000 dtumathtools-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:46.746303 dtumathtools-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:46.770550 dtumathtools-1.1.0/src/dtumathtools/
+-rw-rw-rw-   0        0        0       84 2023-01-30 09:29:20.000000 dtumathtools-1.1.0/src/dtumathtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:46.842347 dtumathtools-1.1.0/src/dtumathtools/dtuplot/
+-rw-rw-rw-   0        0        0     1097 2023-07-30 10:17:54.000000 dtumathtools-1.1.0/src/dtumathtools/dtuplot/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-07-30 08:37:31.000000 dtumathtools-1.1.0/src/dtumathtools/dtuplot/asdfasdf.py
+-rw-rw-rw-   0        0        0     2864 2023-07-31 15:09:13.000000 dtumathtools-1.1.0/src/dtumathtools/dtuplot/boundaryplot.py
+-rw-rw-rw-   0        0        0     9383 2023-07-31 15:09:31.000000 dtumathtools-1.1.0/src/dtumathtools/dtuplot/quiverplot.py
+-rw-rw-rw-   0        0        0     5636 2023-07-31 15:09:22.000000 dtumathtools-1.1.0/src/dtumathtools/dtuplot/quiverplot_helpers.py
+-rw-rw-rw-   0        0        0     6164 2023-07-31 15:08:20.000000 dtumathtools-1.1.0/src/dtumathtools/dtuplot/scatterplot.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:46.858350 dtumathtools-1.1.0/src/dtumathtools/dtutools/
+-rw-rw-rw-   0        0        0       73 2023-04-10 14:03:03.000000 dtumathtools-1.1.0/src/dtumathtools/dtutools/__init__.py
+-rw-rw-rw-   0        0        0     6939 2023-07-29 21:58:47.000000 dtumathtools-1.1.0/src/dtumathtools/dtutools/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:46.793763 dtumathtools-1.1.0/src/dtumathtools.egg-info/
+-rw-rw-rw-   0        0        0     3731 2023-07-31 16:26:46.000000 dtumathtools-1.1.0/src/dtumathtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      637 2023-07-31 16:26:46.000000 dtumathtools-1.1.0/src/dtumathtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:26:46.000000 dtumathtools-1.1.0/src/dtumathtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      584 2023-07-31 16:26:46.000000 dtumathtools-1.1.0/src/dtumathtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 16:26:46.000000 dtumathtools-1.1.0/src/dtumathtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:46.890417 dtumathtools-1.1.0/tests/
+-rw-rw-rw-   0        0        0    55910 2023-07-31 15:19:54.000000 dtumathtools-1.1.0/tests/test_F_demos.py
+-rw-rw-rw-   0        0        0    27013 2023-07-31 15:55:30.000000 dtumathtools-1.1.0/tests/test_dtuplot.py
+-rw-rw-rw-   0        0        0     3454 2023-07-28 06:59:35.000000 dtumathtools-1.1.0/tests/test_dtutools.py
```

### Comparing `dtumathtools-1.0.5/LICENSE` & `dtumathtools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.5/PKG-INFO` & `dtumathtools-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: dtumathtools
-Version: 1.0.5
+Version: 1.1.0
 Summary: A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark
 Home-page: https://github.com/Chrillebon/DTUMathTools
 Author: Christian Mikkelstrup and Hans Henrik Hermansen
 Author-email: s194345@student.dtu.dk, s194042@student.dtu.dk
+Maintainer: Christian Mikkelstrup
+Maintainer-email: s194345@student.dtu.dk
 License: BSD License (BSD)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: qt
 Provides-Extra: plotly
 Provides-Extra: ipympl
 Provides-Extra: mayavi
 Provides-Extra: bokeh
 Provides-Extra: k3d
```

### Comparing `dtumathtools-1.0.5/README.md` & `dtumathtools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dtumathtools-1.0.5/src/dtumathtools/dtuplot/boundaryplot.py` & `dtumathtools-1.1.0/src/dtumathtools/dtuplot/boundaryplot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 from spb.functions import plot_parametric
-from sympy import Matrix
+from sympy.matrices import MatrixBase
+from spb.backends.base_backend import Plot
 
-def plot_boundary(param_func: Matrix, *args, **kwargs):
-    """ A function for plotting the boundary of a 2D
-        area
-        
-        ## Input:
-            param_func: A matrix with functions [x(u,v), y(u,v)] determining 
-                        x and y-coordinates of area to be plotted
-            (u, u_min, u_max): A tuple with variable and its limits either as list or two seperate values
-            (v, v_min, v_max): Same as above but for other variable
 
-            rendering_kw: A dictionary forwarded to dtuplot.plot(), see SPB docs for reference
+def plot_boundary(param_func: MatrixBase, *args, **kwargs) -> (Plot):
+    """A function for plotting the boundary of a 2D area
 
-            
-        ### Keyword arguments:
-            color [Optional]: A string to set color boundary with. With no argument color = 'blue'
-            show [Optional]: Boolean, if 'True': show plot, other just return object without plotting
-                            defaults to 'True'
+    Args:
+        param_func (MatrixBase,): A matrix with functions [x(u,v), y(u,v)] determining x and y-coordinates of area to be plotted.
+        U_lim (Tuple[Symbol, float, float]): A tuple with variable and its limits either as list or two seperate values. Example as (u, u_min, u_max).
+        V_lim (Tuple[Symbol, float, float]): A tuple with variable and its limits either as list or two seperate values. Example as (v, v_min, v_max).
+        rendering_kw (dict, optional): A dictionary forwarded to dtuplot.plot(), see SPB docs for reference.
+        color (str, optional): A string to set color boundary with. With no argument color = 'blue'.
+        show (bool, optional): Boolean, if 'True': show plot, other just return object without plotting. Defaults to 'True'.
 
 
-
-        ## Returns:
-            plot: A SPB-plot object
-
-            
+    Returns:
+        Plot: A SPB-plot object
     """
     if len(param_func) == 2:
         bounds = []
         for i, arg in enumerate(args):
             if isinstance(arg, tuple):
                 bounds.append(arg)
                 if isinstance(arg[1], list):
                     bounds[-1] = (arg[0], *arg[1])
             else:
-                rest = args[i+1:]
+                rest = args[i + 1 :]
                 args = rest
                 break
         else:
             args = []
         if len(bounds) != 2:
             raise ValueError("For 2D-areas two variables are needed to plot boundary")
 
-        show = kwargs.pop('show', True)
-        color = kwargs.pop('color', 'blue')
+        show = kwargs.pop("show", True)
+        color = kwargs.pop("color", "blue")
+        adaptive = kwargs.setdefault("adaptive", False)
         plot = plot_parametric(show=False)
         for i in range(2):
-            plot += plot_parametric(*param_func.subs(bounds[i][0], bounds[i][1]),
-                                        (bounds[1-i][0], *bounds[1-i][1:]), 
-                                        {'color': color}, *args, 
-                                        show=False, **kwargs
+            plot += plot_parametric(
+                *param_func.subs(bounds[i][0], bounds[i][1]),
+                (bounds[1 - i][0], *bounds[1 - i][1:]),
+                {"color": color},
+                *args,
+                show=False,
+                **kwargs
             )
-            plot += plot_parametric(*param_func.subs(bounds[i][0], bounds[i][2]),
-                                        (bounds[1-i][0], *bounds[1-i][1:]), 
-                                        {'color': color}, *args, 
-                                        show=False, **kwargs
+            plot += plot_parametric(
+                *param_func.subs(bounds[i][0], bounds[i][2]),
+                (bounds[1 - i][0], *bounds[1 - i][1:]),
+                {"color": color},
+                *args,
+                show=False,
+                **kwargs
             )
     elif len(param_func) == 3:
-        raise NotImplementedError('Volume boundary plots are not yet implemented')
+        raise NotImplementedError("Volume boundary plots are not yet implemented")
 
-    plot.legend = kwargs.pop('legend', False)
-    plot.xlabel = kwargs.pop('xlabel', 'x')
-    plot.ylabel = kwargs.pop('ylabel', 'y')
-    plot.zlabel = kwargs.pop('zlabel', 'z')
-    plot.aspect = kwargs.pop('aspect', 'auto')
+    plot.legend = kwargs.pop("legend", False)
+    plot.xlabel = kwargs.pop("xlabel", "x")
+    plot.ylabel = kwargs.pop("ylabel", "y")
+    plot.zlabel = kwargs.pop("zlabel", "z")
+    plot.aspect = kwargs.pop("aspect", "auto")
 
     if show:
         plot.show()
         return plot
     else:
-        return plot
+        return plot
```

### Comparing `dtumathtools-1.0.5/src/dtumathtools.egg-info/PKG-INFO` & `dtumathtools-1.1.0/src/dtumathtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: dtumathtools
-Version: 1.0.5
+Version: 1.1.0
 Summary: A plotting package for the 01005 Mathematics 1 course at the Technical University of Denmark
 Home-page: https://github.com/Chrillebon/DTUMathTools
 Author: Christian Mikkelstrup and Hans Henrik Hermansen
 Author-email: s194345@student.dtu.dk, s194042@student.dtu.dk
+Maintainer: Christian Mikkelstrup
+Maintainer-email: s194345@student.dtu.dk
 License: BSD License (BSD)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: qt
 Provides-Extra: plotly
 Provides-Extra: ipympl
 Provides-Extra: mayavi
 Provides-Extra: bokeh
 Provides-Extra: k3d
```

### Comparing `dtumathtools-1.0.5/src/dtumathtools.egg-info/SOURCES.txt` & `dtumathtools-1.1.0/src/dtumathtools.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 src/dtumathtools/__init__.py
 src/dtumathtools.egg-info/PKG-INFO
 src/dtumathtools.egg-info/SOURCES.txt
 src/dtumathtools.egg-info/dependency_links.txt
 src/dtumathtools.egg-info/requires.txt
 src/dtumathtools.egg-info/top_level.txt
 src/dtumathtools/dtuplot/__init__.py
+src/dtumathtools/dtuplot/asdfasdf.py
 src/dtumathtools/dtuplot/boundaryplot.py
 src/dtumathtools/dtuplot/quiverplot.py
+src/dtumathtools/dtuplot/quiverplot_helpers.py
 src/dtumathtools/dtuplot/scatterplot.py
 src/dtumathtools/dtutools/__init__.py
 src/dtumathtools/dtutools/helpers.py
+tests/test_F_demos.py
 tests/test_dtuplot.py
 tests/test_dtutools.py
```

