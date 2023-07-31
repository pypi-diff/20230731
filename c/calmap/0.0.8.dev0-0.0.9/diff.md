# Comparing `tmp/calmap-0.0.8.dev0.tar.gz` & `tmp/calmap-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calmap-0.0.8.dev0.tar", last modified: Sun Jun 14 22:24:22 2020, max compression
+gzip compressed data, was "dist/calmap-0.0.9.tar", last modified: Wed Mar 24 01:38:56 2021, max compression
```

## Comparing `calmap-0.0.8.dev0.tar` & `calmap-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-14 22:24:22.000000 calmap-0.0.8.dev0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2020-06-14 22:23:43.000000 calmap-0.0.8.dev0/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-06-14 22:23:43.000000 calmap-0.0.8.dev0/LICENSE.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2020-06-14 22:23:43.000000 calmap-0.0.8.dev0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2447 2020-06-14 22:24:22.000000 calmap-0.0.8.dev0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1301 2020-06-14 22:23:43.000000 calmap-0.0.8.dev0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-14 22:24:22.000000 calmap-0.0.8.dev0/calmap/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11151 2020-06-14 22:23:43.000000 calmap-0.0.8.dev0/calmap/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-14 22:24:22.000000 calmap-0.0.8.dev0/calmap.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2447 2020-06-14 22:24:21.000000 calmap-0.0.8.dev0/calmap.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      222 2020-06-14 22:24:21.000000 calmap-0.0.8.dev0/calmap.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-14 22:24:21.000000 calmap-0.0.8.dev0/calmap.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-06-14 22:24:21.000000 calmap-0.0.8.dev0/calmap.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-06-14 22:24:21.000000 calmap-0.0.8.dev0/calmap.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-06-14 22:24:22.000000 calmap-0.0.8.dev0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1898 2020-06-14 22:23:43.000000 calmap-0.0.8.dev0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-24 01:38:56.000000 calmap-0.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2021-03-24 01:38:08.000000 calmap-0.0.9/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2021-03-24 01:38:08.000000 calmap-0.0.9/LICENSE.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       55 2021-03-24 01:38:08.000000 calmap-0.0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2294 2021-03-24 01:38:56.000000 calmap-0.0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1301 2021-03-24 01:38:08.000000 calmap-0.0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-24 01:38:56.000000 calmap-0.0.9/calmap/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12892 2021-03-24 01:38:08.000000 calmap-0.0.9/calmap/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-24 01:38:56.000000 calmap-0.0.9/calmap.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2294 2021-03-24 01:38:55.000000 calmap-0.0.9/calmap.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      222 2021-03-24 01:38:55.000000 calmap-0.0.9/calmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-24 01:38:55.000000 calmap-0.0.9/calmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-03-24 01:38:55.000000 calmap-0.0.9/calmap.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-03-24 01:38:55.000000 calmap-0.0.9/calmap.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-24 01:38:56.000000 calmap-0.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1753 2021-03-24 01:38:08.000000 calmap-0.0.9/setup.py
```

### Comparing `calmap-0.0.8.dev0/LICENSE.rst` & `calmap-0.0.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `calmap-0.0.8.dev0/PKG-INFO` & `calmap-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: calmap
-Version: 0.0.8.dev0
+Version: 0.0.9
 Summary: Calendar heatmaps from Pandas time series data
 Home-page: https://github.com/MarvinT/calmap
 Author: Marvin Thielk; Martijn Vermaat
 Author-email: marvin.thielk@gmail.com, martijn@vermaat.name
 License: MIT License
 Description: # Calendar heatmaps from Pandas time series data
         ------------------------------------------------
@@ -37,15 +37,12 @@
         
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `calmap-0.0.8.dev0/README.md` & `calmap-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `calmap-0.0.8.dev0/calmap/__init__.py` & `calmap-0.0.9/calmap/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 import datetime
 
 from matplotlib.colors import ColorConverter, ListedColormap
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from distutils.version import StrictVersion
+from dateutil.relativedelta import relativedelta
+from matplotlib.patches import Polygon
 
-__version_info__ = ("0", "0", "8", "dev")
+__version_info__ = ("0", "0", "9")
 __date__ = "22 Nov 2018"
 
 
 __version__ = ".".join(__version_info__)
 __author__ = "Marvin Thielk; Martijn Vermaat"
 __contact__ = "marvin.thielk@gmail.com, martijn@vermaat.name"
 __homepage__ = "https://github.com/MarvinT/calmap"
@@ -39,14 +41,15 @@
     fillcolor="whitesmoke",
     linewidth=1,
     linecolor=None,
     daylabels=calendar.day_abbr[:],
     dayticks=True,
     monthlabels=calendar.month_abbr[1:],
     monthticks=True,
+    monthly_border=False,
     ax=None,
     **kwargs
 ):
     """
     Plot one year from a timeseries as a calendar heatmap.
 
     Parameters
@@ -56,16 +59,19 @@
     year : integer
         Only data indexed by this year will be plotted. If `None`, the first
         year for which there is data will be plotted.
     how : string
         Method for resampling data by day. If `None`, assume data is already
         sampled by day and don't resample. Otherwise, this is passed to Pandas
         `Series.resample`.
-    vmin, vmax : floats
-        Values to anchor the colormap. If `None`, min and max are used after
+    vmin : float
+        Min Values to anchor the colormap. If `None`, min and max are used after
+        resampling data by day.
+    vmax : float
+        Max Values to anchor the colormap. If `None`, min and max are used after
         resampling data by day.
     cmap : matplotlib colormap name or object
         The mapping from data values to color space.
     fillcolor : matplotlib color
         Color to use for days without data.
     linewidth : float
         Width of the lines that will divide each day.
@@ -79,14 +85,16 @@
         only label days with these indices. If an integer, label every n day.
     monthlabels : list
         Strings to use as labels for months, must be of length 12.
     monthticks : list or int or bool
         If `True`, label all months. If `False`, don't label months. If a
         list, only label months with these indices. If an integer, label every
         n month.
+    monthly_border : bool
+        Draw black border for each month. Default: False.
     ax : matplotlib Axes
         Axes in which to draw the plot, otherwise use the currently-active
         Axes.
     kwargs : other keyword arguments
         All other keyword arguments are passed to matplotlib `ax.pcolormesh`.
 
     Returns
@@ -174,35 +182,35 @@
 
     # Create data frame we can pivot later.
     by_day = pd.DataFrame(
         {
             "data": by_day,
             "fill": 1,
             "day": by_day.index.dayofweek,
-            "week": by_day.index.week,
+            "week": by_day.index.isocalendar().week,
         }
     )
 
     # There may be some days assigned to previous year's last week or
     # next year's first week. We create new week numbers for them so
     # the ordering stays intact and week/day pairs unique.
     by_day.loc[(by_day.index.month == 1) & (by_day.week > 50), "week"] = 0
     by_day.loc[(by_day.index.month == 12) & (by_day.week < 10), "week"] = (
         by_day.week.max() + 1
     )
 
-    # Pivot data on day and week and mask NaN days.
+    # Pivot data on day and week and mask NaN days. (we can also mask the days with 0 counts)
     plot_data = by_day.pivot("day", "week", "data").values[::-1]
     plot_data = np.ma.masked_where(np.isnan(plot_data), plot_data)
 
     # Do the same for all days of the year, not just those we have data for.
     fill_data = by_day.pivot("day", "week", "fill").values[::-1]
     fill_data = np.ma.masked_where(np.isnan(fill_data), fill_data)
 
-    # Draw heatmap for all days of the year with fill color.
+    # Draw background of heatmap for all days of the year with fillcolor.
     ax.pcolormesh(fill_data, vmin=0, vmax=1, cmap=ListedColormap([fillcolor]))
 
     # Draw heatmap.
     kwargs["linewidth"] = linewidth
     kwargs["edgecolors"] = linecolor
     ax.pcolormesh(plot_data, vmin=vmin, vmax=vmax, cmap=cmap, **kwargs)
 
@@ -231,17 +239,53 @@
         dayticks = range(len(daylabels))
     elif dayticks is False:
         dayticks = []
     elif isinstance(dayticks, int):
         dayticks = range(len(daylabels))[dayticks // 2 :: dayticks]
 
     ax.set_xlabel("")
-    ax.set_xticks([by_day.loc[datetime.date(year, i + 1, 15)].week for i in monthticks])
-    ax.set_xticklabels([monthlabels[i] for i in monthticks], ha="center")
+    timestamps = []
+
+    # Month borders
+    xticks, labels = [], []
+    for month in range(1, 13):
+        first = datetime.datetime(year, month, 1)
+        last = first + relativedelta(months=1, days=-1)
+        # Monday on top
+        y0 = 6 - first.weekday()
+        y1 = 6 - last.weekday()
+        start = datetime.datetime(year, 1, 1).weekday()
+        x0 = (int(first.strftime("%j")) + start - 1) // 7
+        x1 = (int(last.strftime("%j")) + start - 1) // 7
+        P = [
+            (x0, y0 + 1),
+            (x0, 0),
+            (x1, 0),
+            (x1, y1),
+            (x1 + 1, y1),
+            (x1 + 1, 7),
+            (x0 + 1, 7),
+            (x0 + 1, y0 + 1),
+        ]
+
+        xticks.append(x0 + (x1 - x0 + 1) / 2)
+        labels.append(first.strftime("%b"))
+        if monthly_border:
+            poly = Polygon(
+                P,
+                edgecolor="black",
+                facecolor="None",
+                linewidth=1,
+                zorder=20,
+                clip_on=False,
+            )
+            ax.add_artist(poly)
 
+    ax.set_xticks(xticks)
+    ax.set_xticklabels(labels)
     ax.set_ylabel("")
     ax.yaxis.set_ticks_position("right")
     ax.set_yticks([6 - i + 0.5 for i in dayticks])
     ax.set_yticklabels(
         [daylabels[i] for i in dayticks], rotation="horizontal", va="center"
     )
 
@@ -253,14 +297,17 @@
     how="sum",
     yearlabels=True,
     yearascending=True,
     yearlabel_kws=None,
     subplot_kws=None,
     gridspec_kws=None,
     fig_kws=None,
+    fig_suptitle=None,
+    vmin=None,
+    vmax=None,
     **kwargs
 ):
     """
     Plot a timeseries as a calendar heatmap.
 
     Parameters
     ----------
@@ -281,14 +328,22 @@
         Keyword arguments passed to the matplotlib `add_subplot` call used to
         create each subplot.
     gridspec_kws : dict
         Keyword arguments passed to the matplotlib `GridSpec` constructor used
         to create the grid the subplots are placed on.
     fig_kws : dict
         Keyword arguments passed to the matplotlib `figure` call.
+    fig_suptitle : string
+        Title for the entire figure..
+    vmin : float
+        Min Values to anchor the colormap. If `None`, min and max are used after
+        resampling data by day.
+    vmax : float
+        Max Values to anchor the colormap. If `None`, min and max are used after
+        resampling data by day.
     kwargs : other keyword arguments
         All other keyword arguments are passed to `yearplot`.
 
     Returns
     -------
     fig, axes : matplotlib Figure and Axes
         Tuple where `fig` is the matplotlib Figure object `axes` is an array
@@ -319,15 +374,15 @@
         ncols=1,
         squeeze=False,
         subplot_kw=subplot_kws,
         gridspec_kw=gridspec_kws,
         **fig_kws
     )
     axes = axes.T[0]
-
+    plt.suptitle(fig_suptitle)
     # We explicitely resample by day only once. This is an optimization.
     if how is None:
         by_day = data
     else:
         if _pandas_18:
             by_day = data.resample("D").agg(how)
         else:
```

### Comparing `calmap-0.0.8.dev0/calmap.egg-info/PKG-INFO` & `calmap-0.0.9/calmap.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: calmap
-Version: 0.0.8.dev0
+Version: 0.0.9
 Summary: Calendar heatmaps from Pandas time series data
 Home-page: https://github.com/MarvinT/calmap
 Author: Marvin Thielk; Martijn Vermaat
 Author-email: marvin.thielk@gmail.com, martijn@vermaat.name
 License: MIT License
 Description: # Calendar heatmaps from Pandas time series data
         ------------------------------------------------
@@ -37,15 +37,12 @@
         
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `calmap-0.0.8.dev0/setup.py` & `calmap-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,17 +39,14 @@
     install_requires=install_requires,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Scientific/Engineering",
     ],
 )
```

