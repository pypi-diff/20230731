# Comparing `tmp/pynimate-1.2.0.tar.gz` & `tmp/pynimate-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynimate-1.2.0.tar", last modified: Sat Apr 15 21:10:53 2023, max compression
+gzip compressed data, was "pynimate-1.3.0.tar", last modified: Mon Jul 31 17:01:15 2023, max compression
```

## Comparing `pynimate-1.2.0.tar` & `pynimate-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:10:53.685072 pynimate-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 21:10:42.000000 pynimate-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 21:10:42.000000 pynimate-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-15 21:10:53.685072 pynimate-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-15 21:10:42.000000 pynimate-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-15 21:10:42.000000 pynimate-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 21:10:53.685072 pynimate-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 21:10:42.000000 pynimate-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:10:53.681072 pynimate-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:10:53.681072 pynimate-1.2.0/src/pynimate/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-15 21:10:42.000000 pynimate-1.2.0/src/pynimate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23908 2023-04-15 21:10:42.000000 pynimate-1.2.0/src/pynimate/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-15 21:10:42.000000 pynimate-1.2.0/src/pynimate/barhplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-04-15 21:10:42.000000 pynimate-1.2.0/src/pynimate/baseplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-15 21:10:42.000000 pynimate-1.2.0/src/pynimate/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-04-15 21:10:42.000000 pynimate-1.2.0/src/pynimate/datafier.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-15 21:10:42.000000 pynimate-1.2.0/src/pynimate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:10:53.685072 pynimate-1.2.0/src/pynimate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-15 21:10:53.000000 pynimate-1.2.0/src/pynimate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-15 21:10:53.000000 pynimate-1.2.0/src/pynimate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:10:53.000000 pynimate-1.2.0/src/pynimate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-15 21:10:53.000000 pynimate-1.2.0/src/pynimate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 21:10:53.000000 pynimate-1.2.0/src/pynimate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:10:53.685072 pynimate-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-15 21:10:42.000000 pynimate-1.2.0/tests/test_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-15 21:10:42.000000 pynimate-1.2.0/tests/test_barhplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-15 21:10:42.000000 pynimate-1.2.0/tests/test_baseplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-04-15 21:10:42.000000 pynimate-1.2.0/tests/test_datafier.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-15 21:10:42.000000 pynimate-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:01:15.734602 pynimate-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 17:01:01.000000 pynimate-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 17:01:01.000000 pynimate-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-31 17:01:15.734602 pynimate-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-31 17:01:01.000000 pynimate-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-31 17:01:01.000000 pynimate-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:01:15.734602 pynimate-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 17:01:01.000000 pynimate-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:01:15.726602 pynimate-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:01:15.730602 pynimate-1.3.0/src/pynimate/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/barhplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/baseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/datafier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 17:01:01.000000 pynimate-1.3.0/src/pynimate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:01:15.730602 pynimate-1.3.0/src/pynimate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-31 17:01:15.000000 pynimate-1.3.0/src/pynimate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-31 17:01:15.000000 pynimate-1.3.0/src/pynimate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:01:15.000000 pynimate-1.3.0/src/pynimate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 17:01:15.000000 pynimate-1.3.0/src/pynimate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 17:01:15.000000 pynimate-1.3.0/src/pynimate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:01:15.730602 pynimate-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-31 17:01:01.000000 pynimate-1.3.0/tests/test_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-31 17:01:01.000000 pynimate-1.3.0/tests/test_barhplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-31 17:01:01.000000 pynimate-1.3.0/tests/test_baseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-31 17:01:01.000000 pynimate-1.3.0/tests/test_datafier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-31 17:01:01.000000 pynimate-1.3.0/tests/test_lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-31 17:01:01.000000 pynimate-1.3.0/tests/test_utils.py
```

### Comparing `pynimate-1.2.0/LICENSE` & `pynimate-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynimate-1.2.0/PKG-INFO` & `pynimate-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynimate
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for statistical data animations
 Author-email: julkar9 <julkar9dev@gmail.com>
 License: MIT License (MIT)
 Project-URL: Homepage, https://github.com/julkaar9/pynimate
 Project-URL: Documentation, https://julkaar9.github.io/pynimate/
 Keywords: animations,framework,data,plots
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,15 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/pynimate?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/pynimate) 
 ![Tests](https://github.com/julkaar9/pynimate/actions/workflows/tests.yml/badge.svg)
 [![License](https://img.shields.io/pypi/l/pynimate?color=green)](https://github.com/julkaar9/pynimate/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)  
 
 Python package for statistical data animations.
 ![](https://github.com/julkaar9/pynimate/blob/main/docs/assets/example3.gif)
+![](https://github.com/julkaar9/pynimate/blob/main/docs/assets/lineplot_dark2.gif)
 
 ## Installation
 ### with pip
 Pynimate is avaialbe at [pypi](https://pypi.org/project/pynimate/)
 ``` sh
 pip install pynimate
 ```
```

### Comparing `pynimate-1.2.0/README.md` & `pynimate-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/pynimate?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/pynimate) 
 ![Tests](https://github.com/julkaar9/pynimate/actions/workflows/tests.yml/badge.svg)
 [![License](https://img.shields.io/pypi/l/pynimate?color=green)](https://github.com/julkaar9/pynimate/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)  
 
 Python package for statistical data animations.
 ![](https://github.com/julkaar9/pynimate/blob/main/docs/assets/example3.gif)
+![](https://github.com/julkaar9/pynimate/blob/main/docs/assets/lineplot_dark2.gif)
 
 ## Installation
 ### with pip
 Pynimate is avaialbe at [pypi](https://pypi.org/project/pynimate/)
 ``` sh
 pip install pynimate
 ```
```

### Comparing `pynimate-1.2.0/pyproject.toml` & `pynimate-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "pynimate"
-version = "1.2.0"
+version = "1.3.0"
 description = "Python package for statistical data animations"
 readme = "README.md"
 authors = [{ name = "julkar9", email = "julkar9dev@gmail.com" }]
 license = { text = "MIT License (MIT)" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pynimate-1.2.0/src/pynimate/__init__.py` & `pynimate-1.3.0/src/pynimate/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 =====
 Python package for statistical data animations.
 
 Available Plots
 ---------------
 Barhplot
     Horizontal Bar Chart Race module
-    
+Lineplot
+    Module for Lineplot animations
+
 Barhplot Example
 ---------------
 
 It is assumed `pynimate` is imported as `nim`.
 >>> import pynimate as nim 
 >>> import pandas as pd
 >>> df = pd.read_csv("sample.csv").set_index("time")
@@ -20,14 +22,15 @@
 >>> bar.set_time(callback=lambda i, datafier: datafier.data.index[i].year)
 >>> bar.set_bar_annots(text_callback=human_readable)
 >>> cnv.add_plot(bar)
 >>> cnv.animate()
 >>> cnv.save('sample', fps=24)
 """
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 from .bar import Barplot
 from .barhplot import Barhplot
 from .baseplot import Baseplot
 from .canvas import Canvas
-from .datafier import BarDatafier, BaseDatafier, Datafier
+from .datafier import BarDatafier, BaseDatafier, Datafier, LineDatafier
+from .lineplot import Lineplot
```

### Comparing `pynimate-1.2.0/src/pynimate/bar.py` & `pynimate-1.3.0/src/pynimate/bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,18 @@
         annot_bars: bool = True,
         fixed_xlim: bool = True,
         xticks: bool = True,
         yticks: bool = True,
         grid: bool = True,
         rounded_edges: bool = False,
     ) -> None:
-        """BarChartRace module that requires a valid time index.The data
+        """
+        Barplot is deprecated, use Barhplot instead
+
+        BarChartRace module that requires a valid time index.The data
         should be in this format where time is set to index
             ```
                 Example:
                 >>> time  col1 col2 col3 ...
                 >>> 2012   1    0    2
                 >>> 2013   2    3    1
             ```
```

### Comparing `pynimate-1.2.0/src/pynimate/barhplot.py` & `pynimate-1.3.0/src/pynimate/barhplot.py`

 * *Files identical despite different names*

### Comparing `pynimate-1.2.0/src/pynimate/baseplot.py` & `pynimate-1.3.0/src/pynimate/baseplot.py`

 * *Files identical despite different names*

### Comparing `pynimate-1.2.0/src/pynimate/canvas.py` & `pynimate-1.3.0/src/pynimate/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class Canvas:
     def __init__(
         self,
         nrows: int = 1,
         ncols: int = 1,
-        figsize: tuple[int, int] = (16, 9),
+        figsize: tuple[int, int] = (12.8, 7.2),
         post_update: Callable[[plt.Figure, list[list[plt.Axes]]], None] = None,
         **kwargs,
     ) -> None:
         """Creates the matplotlib figure, subplots and additional figure properties.
         Also creates and saves the animation.
 
         Parameters
```

### Comparing `pynimate-1.2.0/src/pynimate/datafier.py` & `pynimate-1.3.0/src/pynimate/datafier.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,18 @@
         data: pd.DataFrame,
         time_format: str,
         ip_freq: str,
         ip_frac: float = 0.5,
         n_bars: int = 10,
         palettes: list[str] = ["viridis"],
     ) -> None:
-        """Contains data preparation modules, which includes interpolation, rank generation, color_generation.
+        """
+        Datafier is deprecated, use plot specific datafiers instead.
+
+        Contains data preparation modules, which includes interpolation, rank generation, color_generation.
         data should be in this format where time is set to index
         ```
             Example:
             >>> time  col1 col2 col3 ...
             >>> 2012   1    0    2
             >>> 2013   2    3    1
         ```
@@ -488,7 +491,42 @@
         -------
         list[str]
             List of columns that will appear in the animation at least once
         """
         top_cols = self.df_ranks.max(axis=0)
         top_cols = top_cols[top_cols >= 1]
         return list(top_cols.index)
+
+
+class LineDatafier(BaseDatafier):
+    def __init__(
+        self, data, time_format: str, ip_freq: str, ip_method: str = "linear"
+    ) -> None:
+        """Contains data preparation modules, which includes interpolation.
+        data should be in this format where time is set to index
+        ```
+            Example:
+            >>> time  col1 col2 col3 ...
+            >>> 2012   1    0    2
+            >>> 2013   2    3    1
+        ```
+        Parameters
+        ----------
+        data : pd.DataFrame
+            The data to be prepared, should be in this format where time is set to index
+        time_format : str
+            Index datetime format
+        ip_freq : str
+            Interpolation frequency
+        """
+        super().__init__(data, time_format, ip_freq, ip_method)
+        self.data = self.prepare_data()
+
+    def prepare_data(self) -> pd.DataFrame:
+        """Creates interpolated data
+
+        Returns
+        -------
+        pd.DataFrame
+            Interpolated data values
+        """
+        return self.interpolate_even(self.raw_data, self.ip_freq, self.ip_method)
```

### Comparing `pynimate-1.2.0/src/pynimate/utils.py` & `pynimate-1.3.0/src/pynimate/utils.py`

 * *Files identical despite different names*

### Comparing `pynimate-1.2.0/src/pynimate.egg-info/PKG-INFO` & `pynimate-1.3.0/src/pynimate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynimate
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for statistical data animations
 Author-email: julkar9 <julkar9dev@gmail.com>
 License: MIT License (MIT)
 Project-URL: Homepage, https://github.com/julkaar9/pynimate
 Project-URL: Documentation, https://julkaar9.github.io/pynimate/
 Keywords: animations,framework,data,plots
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,15 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/pynimate?period=total&units=international_system&left_color=grey&right_color=red&left_text=Downloads)](https://pepy.tech/project/pynimate) 
 ![Tests](https://github.com/julkaar9/pynimate/actions/workflows/tests.yml/badge.svg)
 [![License](https://img.shields.io/pypi/l/pynimate?color=green)](https://github.com/julkaar9/pynimate/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)  
 
 Python package for statistical data animations.
 ![](https://github.com/julkaar9/pynimate/blob/main/docs/assets/example3.gif)
+![](https://github.com/julkaar9/pynimate/blob/main/docs/assets/lineplot_dark2.gif)
 
 ## Installation
 ### with pip
 Pynimate is avaialbe at [pypi](https://pypi.org/project/pynimate/)
 ``` sh
 pip install pynimate
 ```
```

### Comparing `pynimate-1.2.0/tests/test_bar.py` & `pynimate-1.3.0/tests/test_bar.py`

 * *Files identical despite different names*

### Comparing `pynimate-1.2.0/tests/test_barhplot.py` & `pynimate-1.3.0/tests/test_barhplot.py`

 * *Files identical despite different names*

### Comparing `pynimate-1.2.0/tests/test_baseplot.py` & `pynimate-1.3.0/tests/test_baseplot.py`

 * *Files identical despite different names*

### Comparing `pynimate-1.2.0/tests/test_datafier.py` & `pynimate-1.3.0/tests/test_datafier.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,17 @@
             "Argentina": [1.0, 1.75, 2.5, 3.25, 4.0, 4.25, 4.5, 4.75, 5.0],
         }
     ).set_index("time")
     assert dfr.df_ranks.equals(df_ranks)
     assert dfr.data.equals(data)
 
 
+# 1.2.0 >=
+
+
 def test_basedatafier_interpolate_even(sample_data2):
     dfr = BaseDatafier(sample_data2, "%Y", "3MS")
     interpolated_data = pd.DataFrame(
         {
             "time": pd.to_datetime(
                 [
                     "2012-01-01",
```

