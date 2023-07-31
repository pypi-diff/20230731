# Comparing `tmp/SplatStats-2.3.1.tar.gz` & `tmp/SplatStats-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-2.3.1.tar", last modified: Wed Jul 26 18:20:31 2023, max compression
+gzip compressed data, was "SplatStats-2.3.2.tar", last modified: Mon Jul 31 21:12:27 2023, max compression
```

## Comparing `SplatStats-2.3.1.tar` & `SplatStats-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-26 18:20:31.379848 SplatStats-2.3.1/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.3.1/LICENSE
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-26 18:20:31.379711 SplatStats-2.3.1/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.3.1/README.md
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-26 18:20:31.378609 SplatStats-2.3.1/SplatStats/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/Battle.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10734 2023-07-20 20:13:44.000000 SplatStats-2.3.1/SplatStats/Player.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-07-17 20:54:12.000000 SplatStats-2.3.1/SplatStats/StatInk.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/Team.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14036 2023-07-17 16:23:54.000000 SplatStats-2.3.1/SplatStats/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5905 2023-06-06 02:59:04.000000 SplatStats-2.3.1/SplatStats/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/files.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8968 2023-07-26 17:04:38.000000 SplatStats-2.3.1/SplatStats/parsers.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    59461 2023-07-26 18:06:33.000000 SplatStats-2.3.1/SplatStats/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/plotsAux.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1707 2023-07-26 17:48:54.000000 SplatStats-2.3.1/SplatStats/plotsTeam.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10747 2023-07-17 20:47:10.000000 SplatStats-2.3.1/SplatStats/statInkConstants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10625 2023-06-05 15:55:49.000000 SplatStats-2.3.1/SplatStats/statInkPlots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/statInkStats.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    15022 2023-07-26 17:22:01.000000 SplatStats-2.3.1/SplatStats/stats.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-26 18:20:31.379519 SplatStats-2.3.1/SplatStats.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-26 18:20:31.379900 SplatStats-2.3.1/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.3.1/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-31 21:12:27.142177 SplatStats-2.3.2/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.3.2/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-31 21:12:27.142048 SplatStats-2.3.2/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.3.2/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-31 21:12:27.141079 SplatStats-2.3.2/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.3.2/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10734 2023-07-20 20:13:44.000000 SplatStats-2.3.2/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-07-17 20:54:12.000000 SplatStats-2.3.2/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.3.2/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.3.2/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-31 21:12:27.000000 SplatStats-2.3.2/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.3.2/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14036 2023-07-17 16:23:54.000000 SplatStats-2.3.2/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5905 2023-06-06 02:59:04.000000 SplatStats-2.3.2/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.3.2/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8968 2023-07-26 17:04:38.000000 SplatStats-2.3.2/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    59462 2023-07-31 21:03:57.000000 SplatStats-2.3.2/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.3.2/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1707 2023-07-26 17:48:54.000000 SplatStats-2.3.2/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10747 2023-07-17 20:47:10.000000 SplatStats-2.3.2/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10625 2023-06-05 15:55:49.000000 SplatStats-2.3.2/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.3.2/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    15022 2023-07-26 17:22:01.000000 SplatStats-2.3.2/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-31 21:12:27.141858 SplatStats-2.3.2/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-31 21:12:27.000000 SplatStats-2.3.2/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-07-31 21:12:27.000000 SplatStats-2.3.2/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-31 21:12:27.000000 SplatStats-2.3.2/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-07-31 21:12:27.000000 SplatStats-2.3.2/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-07-31 21:12:27.000000 SplatStats-2.3.2/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-31 21:12:27.142220 SplatStats-2.3.2/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.3.2/setup.py
```

### Comparing `SplatStats-2.3.1/LICENSE` & `SplatStats-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/PKG-INFO` & `SplatStats-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.3.1
+Version: 2.3.2
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.3.1/README.md` & `SplatStats-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/Battle.py` & `SplatStats-2.3.2/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/Player.py` & `SplatStats-2.3.2/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/StatInk.py` & `SplatStats-2.3.2/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/Team.py` & `SplatStats-2.3.2/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/__init__.py` & `SplatStats-2.3.2/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/auxiliary.py` & `SplatStats-2.3.2/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/colors.py` & `SplatStats-2.3.2/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/constants.py` & `SplatStats-2.3.2/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/files.py` & `SplatStats-2.3.2/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/parsers.py` & `SplatStats-2.3.2/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/plots.py` & `SplatStats-2.3.2/SplatStats/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1363,15 +1363,15 @@
         (rowDates, rowMagnitudes) = (
             list(rowValues.index), list(rowValues.values)
         )
         # Convert dates to x coordinates --------------------------------------
         dateTuples = [[int(x) for x in d.split('/')] for d in rowDates]
         weekNumber = [(y%minYear)*52+w-minWeek+1 for (y, w) in dateTuples]
         # Convert values to colors --------------------------------------------
-        rDelta = radians(rRange[1])/weekNumber[-1]
+        rDelta = radians(rRange[1])/len(weekNumber)
         deltas = np.arange(0, radians(rRange[1])+rDelta, rDelta)
         weekBars = [(i*rDelta, rDelta) for i in range(len(deltas)-1)]
         clrsBlocks = [cmapCurrent(norm(value)) for value in rowMagnitudes]
         ax.broken_barh(
             weekBars, (offset+wpix*height, height), lw=edgeWidth,
             facecolors=clrsBlocks, edgecolors=baseColor
         )
```

### Comparing `SplatStats-2.3.1/SplatStats/plotsAux.py` & `SplatStats-2.3.2/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/plotsTeam.py` & `SplatStats-2.3.2/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/statInkConstants.py` & `SplatStats-2.3.2/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/statInkPlots.py` & `SplatStats-2.3.2/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/statInkStats.py` & `SplatStats-2.3.2/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats/stats.py` & `SplatStats-2.3.2/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/SplatStats.egg-info/PKG-INFO` & `SplatStats-2.3.2/SplatStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.3.1
+Version: 2.3.2
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.3.1/SplatStats.egg-info/SOURCES.txt` & `SplatStats-2.3.2/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-2.3.1/setup.py` & `SplatStats-2.3.2/setup.py`

 * *Files identical despite different names*

