# Comparing `tmp/map_with_stats-0.1.1.tar.gz` & `tmp/map_with_stats-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_with_stats-0.1.1.tar", last modified: Sat Jul 29 13:45:39 2023, max compression
+gzip compressed data, was "map_with_stats-0.1.2.tar", last modified: Mon Jul 31 17:32:22 2023, max compression
```

## Comparing `map_with_stats-0.1.1.tar` & `map_with_stats-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.190817 map_with_stats-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.194817 map_with_stats-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/publish_prod.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/publish_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/assets/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/assets/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (123)  1021823 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/figs/map_screenshot.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/docs/quick_start.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.198818 map_with_stats-0.1.1/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/linux.env
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/environment/windows.env
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.194817 map_with_stats-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/src/map_with_stats/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/map.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/src/map_with_stats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/src/map_with_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 13:45:39.000000 map_with_stats-0.1.1/src/map_with_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:45:39.202818 map_with_stats-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-29 13:45:28.000000 map_with_stats-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.124651 map_with_stats-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/publish_prod.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/publish_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/assets/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/assets/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1021823 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/figs/map_screenshot.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/docs/quick_start.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.128651 map_with_stats-0.1.2/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/linux.env
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/requirements_lib.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/environment/windows.env
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.124651 map_with_stats-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/src/map_with_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 17:32:21.000000 map_with_stats-0.1.2/src/map_with_stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/src/map_with_stats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/src/map_with_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 17:32:22.000000 map_with_stats-0.1.2/src/map_with_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:32:22.132650 map_with_stats-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-31 17:32:10.000000 map_with_stats-0.1.2/tests/test_utils.py
```

### Comparing `map_with_stats-0.1.1/.github/workflows/docs.yml` & `map_with_stats-0.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/.github/workflows/publish_template.yml` & `map_with_stats-0.1.2/.github/workflows/publish_template.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/.github/workflows/test.yml` & `map_with_stats-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/.gitignore` & `map_with_stats-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/.pre-commit-config.yaml` & `map_with_stats-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/.vscode/settings.json` & `map_with_stats-0.1.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/LICENSE` & `map_with_stats-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/PKG-INFO` & `map_with_stats-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: map_with_stats
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactive map with a choropleth displaying some statistics as color per hectare
 Author: Mischa Lisovyi
 License: MIT License
         
         Copyright (c) 2023 Mischa Lisovyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `map_with_stats-0.1.1/README.md` & `map_with_stats-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/docs/assets/favicon-16x16.png` & `map_with_stats-0.1.2/docs/assets/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/docs/assets/favicon-32x32.png` & `map_with_stats-0.1.2/docs/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/docs/faq.md` & `map_with_stats-0.1.2/docs/faq.md`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/docs/figs/map_screenshot.jpeg` & `map_with_stats-0.1.2/docs/figs/map_screenshot.jpeg`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/docs/index.md` & `map_with_stats-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/docs/quick_start.md` & `map_with_stats-0.1.2/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/mkdocs.yml` & `map_with_stats-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/pyproject.toml` & `map_with_stats-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/src/map_with_stats/data.py` & `map_with_stats-0.1.2/src/map_with_stats/data.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/src/map_with_stats/map.py` & `map_with_stats-0.1.2/src/map_with_stats/map.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     n_bins: int = 5,
     clip_quantile: Optional[float] = 0.01,
     map_tiles_provider: str = "OpenStreetMap",
     optimise_choropleth_size: bool = True,
     coordinates_start: Tuple[float, float] = (47.39, 8.53),
     zoom_start: int = 15,
     max_n_hectares_to_display: Optional[int] = None,
+    plot_boundaries: bool = False,
 ) -> folium.Map:
     """Generate a folium map with the some statistics per hectare added as a choropleth alayer on top.
 
     See [FAQ](faq) for detailed explanation and typical use-cases of more complex attributes.
 
     Args:
         gdf_stats (gpd.GeoDataFrame): input table with the hectare polygons and statistics values.
@@ -41,22 +42,26 @@
             coordinates to a pre-defined optimised value that will keep hectare boundary precision.
             This allows to reduce the size of the map HTML dump on disk. Defaults to True.
         coordinates_start (Tuple[float, float], optional): starting coordinated in longiotude and latitude.
             Defaults to (47.39, 8.53) [Zürich].
         zoom_start (int, optional): starting zoom. Defaults to 15.
         max_n_hectares_to_display (Optional[int], optional): the top-N hectares to display.
             Defaults to None.
+        plot_boundaries (bool, optional): set to True to display boundaries between choroplet elements.
+            This is useful if you visualise not hectares but some administrative entities.
+            Defaults to False.
 
     Raises:
         ValueError: unsupported `bins_type` provided.
 
     Returns:
         folium.Map: the map with cholopleth layer
     """
-    _check_cols_in_df(gdf_stats, ["geometry", "value", "X", "Y"])
+
+    _check_cols_in_df(gdf_stats, ["geometry", "value"])
 
     # make a copy to avoid modifying input data in-place
     gdf = gdf_stats.copy(deep=True)
 
     ch_map = folium.Map(
         location=coordinates_start, zoom_start=zoom_start, tiles=map_tiles_provider
     )
@@ -85,34 +90,47 @@
         quantiles = [i / (n_bins) for i in range(n_bins + 1)]
         bins = list(cliped_values.quantile(quantiles))
     elif bins_type == "equidistant":
         bins = n_bins
     else:
         raise ValueError(f"Unexpected type of bins: {bins_type}")
 
-    # coloured square with the colour reflecting the statistics value
+    if plot_boundaries:
+        # thin gray line
+        line_weight = 0.5
+        line_color = "gray"
+    else:
+        # no line, for example around hectares
+        line_weight = 0
+        line_color = "black"
+    # coloured choropleth with the colour reflecting the statistics value
+    # for example squares in the case of hectares
     choropleth = folium.Choropleth(
         geo_data=gdf,
         data=cliped_values,
         key_on="feature.id",  # index of the geodataframe is transformed into `id` field
         fill_color="YlOrBr",
         fill_opacity=0.6,
         bins=bins,
-        line_weight=0,  # no line around hectare
+        line_weight=line_weight,
+        line_color=line_color,
         nan_fill_opacity=1,  # fully transparent hectares if the valueis mising
         legend_name=title,  # title under the color scale
         name=title,  # name of thew layer, e.g. in the layer control
     ).add_to(ch_map)
 
+    # optional X and Y coordinates that would appear for hectares, but not for administrative regions
+    cols_xy = [c for c in ["X", "Y"] if c in gdf]
+    labels_xy = ["LV03 X:", "LV03 Y:"] if cols_xy else []
     # add tooltip to appear, when pointing at a hectar
     tooltip = folium.GeoJsonTooltip(
         # column names with values to be displayed
-        fields=["X", "Y", "value"],
+        fields=cols_xy + ["value"],
         # text to be shown explaining each value
-        aliases=["LV03 X:", "LV03 Y:", f"{title}:"],
+        aliases=labels_xy + [f"{title}:"],
         localize=True,
         max_width=800,
     )
     tooltip.add_to(choropleth.geojson)
 
     folium.LayerControl().add_to(ch_map)
     return ch_map
```

### Comparing `map_with_stats-0.1.1/src/map_with_stats/utils.py` & `map_with_stats-0.1.2/src/map_with_stats/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,13 @@
         geom (shapely.Geometry): input geometries
         n_digits_after_comma (int): rounding precision
 
     Returns:
         shapely.Geometry: output geometries with reduced precision
     """
 
-    def _round_coords(x: float, y: float) -> Tuple[float, float]:
-        x = round(x, n_digits_after_comma)
-        y = round(y, n_digits_after_comma)
-        return (x, y)
+    def _round_coords(*arg: float) -> Tuple[float, ...]:
+        out = [round(x, n_digits_after_comma) for x in arg]
+        return tuple(out)
 
     geom_transformed = shapely.ops.transform(_round_coords, geom)
     return geom_transformed
```

### Comparing `map_with_stats-0.1.1/src/map_with_stats.egg-info/PKG-INFO` & `map_with_stats-0.1.2/src/map_with_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: map-with-stats
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactive map with a choropleth displaying some statistics as color per hectare
 Author: Mischa Lisovyi
 License: MIT License
         
         Copyright (c) 2023 Mischa Lisovyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `map_with_stats-0.1.1/src/map_with_stats.egg-info/SOURCES.txt` & `map_with_stats-0.1.2/src/map_with_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/tests/test_data.py` & `map_with_stats-0.1.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `map_with_stats-0.1.1/tests/test_utils.py` & `map_with_stats-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

