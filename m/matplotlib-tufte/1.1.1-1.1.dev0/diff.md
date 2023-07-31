# Comparing `tmp/matplotlib_tufte-1.1.1.tar.gz` & `tmp/matplotlib_tufte-1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_tufte-1.1.1.tar", max compression
+gzip compressed data, was "matplotlib_tufte-1.1.dev0.tar", max compression
```

## Comparing `matplotlib_tufte-1.1.1.tar` & `matplotlib_tufte-1.1.dev0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1953 2023-07-31 08:46:22.049741 matplotlib_tufte-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-07-31 08:46:22.049741 matplotlib_tufte-1.1.1/LICENSE
-drwxr-xr-x   0        0        0        0 2023-07-31 08:46:22.049741 matplotlib_tufte-1.1.1/LICENSES/
--rw-r--r--   0        0        0     1250 2023-07-31 08:46:22.049741 matplotlib_tufte-1.1.1/README.md
--rw-r--r--   0        0        0     1215 2023-07-31 08:46:22.051741 matplotlib_tufte-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     7093 2023-07-31 08:46:22.051741 matplotlib_tufte-1.1.1/tuftelike/__init__.py
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 matplotlib_tufte-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1781 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/LICENSES/
+-rw-r--r--   0        0        0     1250 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/README.md
+-rw-r--r--   0        0        0     1218 2023-06-29 19:28:35.199576 matplotlib_tufte-1.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7088 2023-06-29 19:28:35.199576 matplotlib_tufte-1.1.dev0/tuftelike/__init__.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 matplotlib_tufte-1.1.dev0/PKG-INFO
```

### Comparing `matplotlib_tufte-1.1.1/CHANGELOG.md` & `matplotlib_tufte-1.1.dev0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [1.1.1]
-
-Fixed:
-
-- tuftelike creates correct bars again, after a bug in 1.1 broke the adjustment.
-
 ## [1.1]
 
 Added:
 
 - Method `tuftelike.adjust` now has parameters `xpadding` and `ypadding`:
 
       xpadding: padding to add in the front of the x axis.
@@ -49,11 +43,10 @@
 Added:
 
 - Method `tuftelike.adjust` allows to turn existing Matplotlib plots into tufte-like plots
   with less chart-junk and more expressive axis boundaries. 
 
 
 
-[Unreleased]: https://gitlab.com/lemberger/matplotlib-tufte/-/compare/1.1.1...main
+[Unreleased]: https://gitlab.com/lemberger/matplotlib-tufte/-/compare/1.1...main
 [1.0]: https://gitlab.com/lemberger/matplotlib-tufte/-/tree/1.0
 [1.1]: https://gitlab.com/lemberger/matplotlib-tufte/-/tree/1.1
-[1.1.1]: https://gitlab.com/lemberger/matplotlib-tufte/-/tree/1.1.1
```

### Comparing `matplotlib_tufte-1.1.1/LICENSE` & `matplotlib_tufte-1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_tufte-1.1.1/README.md` & `matplotlib_tufte-1.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib_tufte-1.1.1/pyproject.toml` & `matplotlib_tufte-1.1.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-FileCopyrightText: 2022 Thomas Lemberger <https://thomaslemberger.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "matplotlib-tufte"
-version = "1.1.1"
+version = "1.1.dev0"
 description = "Tufte-style plots for matplotlib"
 readme = "README.md"
 authors = ["Thomas Lemberger <lembergerth@gmail.com>"]
 repository = "https://gitlab.com/lemberger/matplotlib-tufte"
 keywords = ["plotting", "matplotlib"]
 classifiers = [
   "Framework :: Matplotlib",
```

### Comparing `matplotlib_tufte-1.1.1/tuftelike/__init__.py` & `matplotlib_tufte-1.1.dev0/tuftelike/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 
 import logging
 import math
 import matplotlib.pyplot as plt  # type: ignore
 from matplotlib.ticker import FixedFormatter, FixedLocator, NullLocator  # type: ignore
 
-__version__ = "1.1.1"
+__version__ = "1.1.dev0"
 
 logger = logging.getLogger(__name__)
 
 
 def _pad_xlabel(ax):
     label = ax.get_xlabel()
     if not label:
@@ -159,21 +159,21 @@
             amplitude = int(math.log(distance, 10))
         axis.set_major_locator(FixedLocator(ticks))
         axis.set_major_formatter(
             FixedFormatter([ticks_format(t, amplitude) for t in ticks])
         )
 
     # we keep ticks for categories (string values) as they are, so we only change ticks for x/y if it has numeric values.
-    if not isinstance(xs[0], str):
+    if isinstance(xs[0], str):
         xticks = get_ticks(xs)
         set_ticks_labels(xs, xticks, ax.xaxis)
         ax.set_xticks(xticks)
         if xaxis_inverted:
             ax.invert_xaxis()
-    if not isinstance(ys[0], str):
+    if isinstance(ys[0], str):
         yticks = get_ticks(ys)
         set_ticks_labels(ys, yticks, ax.yaxis)
         ax.set_yticks(yticks)
         if yaxis_inverted:
             ax.invert_yaxis()
```

### Comparing `matplotlib_tufte-1.1.1/PKG-INFO` & `matplotlib_tufte-1.1.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib-tufte
-Version: 1.1.1
+Version: 1.1.dev0
 Summary: Tufte-style plots for matplotlib
 Home-page: https://gitlab.com/lemberger/matplotlib-tufte
 License: Apache-2.0
 Keywords: plotting,matplotlib
 Author: Thomas Lemberger
 Author-email: lembergerth@gmail.com
 Requires-Python: >=3.7,<4.0
```

