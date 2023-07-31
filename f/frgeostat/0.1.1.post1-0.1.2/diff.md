# Comparing `tmp/frgeostat-0.1.1.post1.tar.gz` & `tmp/frgeostat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frgeostat-0.1.1.post1.tar", max compression
+gzip compressed data, was "frgeostat-0.1.2.tar", max compression
```

## Comparing `frgeostat-0.1.1.post1.tar` & `frgeostat-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      892 2023-07-31 05:22:41.212872 frgeostat-0.1.1.post1/README.md
--rw-r--r--   0        0        0        0 2023-07-28 12:51:52.685150 frgeostat-0.1.1.post1/frgeostat/__init__.py
--rw-r--r--   0        0        0     2375 2023-07-31 04:23:17.826154 frgeostat-0.1.1.post1/frgeostat/cli.py
--rw-r--r--   0        0        0     3705 2023-07-28 19:23:04.026154 frgeostat-0.1.1.post1/frgeostat/communes.py
--rw-r--r--   0        0        0      326 2023-07-31 04:13:26.663405 frgeostat-0.1.1.post1/frgeostat/config.toml
--rw-r--r--   0        0        0     7938 2023-07-31 05:16:51.213525 frgeostat-0.1.1.post1/frgeostat/departements.py
--rw-r--r--   0        0        0      697 2023-07-31 04:21:33.051262 frgeostat-0.1.1.post1/frgeostat/utils.py
--rw-r--r--   0        0        0      863 2023-07-31 05:24:41.609608 frgeostat-0.1.1.post1/pyproject.toml
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 frgeostat-0.1.1.post1/PKG-INFO
+-rw-r--r--   0        0        0      964 2023-07-31 05:26:33.631431 frgeostat-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 12:51:52.685150 frgeostat-0.1.2/frgeostat/__init__.py
+-rw-r--r--   0        0        0     2483 2023-07-31 06:25:24.917384 frgeostat-0.1.2/frgeostat/cli.py
+-rw-r--r--   0        0        0     3705 2023-07-28 19:23:04.026154 frgeostat-0.1.2/frgeostat/communes.py
+-rw-r--r--   0        0        0      326 2023-07-31 04:13:26.663405 frgeostat-0.1.2/frgeostat/config.toml
+-rw-r--r--   0        0        0     9048 2023-07-31 06:30:01.824460 frgeostat-0.1.2/frgeostat/departements.py
+-rw-r--r--   0        0        0      697 2023-07-31 04:21:33.051262 frgeostat-0.1.2/frgeostat/utils.py
+-rw-r--r--   0        0        0      857 2023-07-31 06:32:45.790728 frgeostat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 frgeostat-0.1.2/PKG-INFO
```

### Comparing `frgeostat-0.1.1.post1/README.md` & `frgeostat-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# A small package to generate LeafletJS maps of France using `folium`
+[![PyPI version](https://badge.fury.io/py/frgeostat.svg)](https://badge.fury.io/py/frgeostat)
+
+# A package to create LeafletJS maps of France
 
 To install, create a virtualenv using whichever method you want, and either:
 
 ```shell
 pip install frgeostat
 ```
```

### Comparing `frgeostat-0.1.1.post1/frgeostat/cli.py` & `frgeostat-0.1.2/frgeostat/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,16 @@
             p = Path(ot)
             d = p.parent if p.is_file() else ''
             if d:
                 d.mkdir(parents=True, exist_ok=True)
                 cout.log(f"[yellow]Created directory: [dim]{d}[/dim][/yellow]")
             p = p if p.is_file() else d / 'communes.score.map.html' if d else p
             dept.build().save(str(p))
-            
+            for dept, m in dept.buildDepts().items():
+                m.save(p.parent / f"{dept}.zoomed.score.map.html")
         else:
             cout.log("[red]Error:[/red] Incorrect kind of map, exiting..")
             typer.Exit(1)
     
 
 @app.command("ls", help="List the kinds of map this toolbox can build.")
 def list_maps(
```

### Comparing `frgeostat-0.1.1.post1/frgeostat/communes.py` & `frgeostat-0.1.2/frgeostat/communes.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.1.post1/frgeostat/departements.py` & `frgeostat-0.1.2/frgeostat/departements.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 
 import sys
+import json
 import geopandas as gpd
 import pandas as pd
 import plotly.express as px
 import folium as fl
 import numpy as np
+import shapely
 import requests as rq
 from folium.plugins import Search
 from frgeostat.utils import cerr, SITE_ROOT, cout
 from quickbar import Quickbar
 from unidecode import unidecode
 
 from typing import Generator, Any, Dict, Callable        
 
+processString = lambda s : unidecode(s).lower().replace("'", "")
+
 class Departements:
     def __init__(self, save: bool = False) -> None:
         qbar = Quickbar('spin')
         qbar.bar.start()
         starting = qbar.bar.add_task("Downloading Departements Data...", total=None, start=True)
         self.df = pd.read_parquet("https://github.com/volt-france/bureaux-vote/releases/download/v0.0.1/plot.scoring.metadata.table.parquet")
         
@@ -33,14 +37,15 @@
         self.m = fl.Map(
             location=[47, 2.5], zoom_start=6,
             tiles="CartoDB positron", max_bounds=True,
             max_lat=self.latHigh, max_lon=self.lonHigh,
             min_lat=self.latLow, min_lon=self.lonLow, 
             min_zoom=6
             )
+        self.perDeptMaps = {}
         qbar.bar.remove_task(mkmap)
         proctask = qbar.bar.add_task("Processing metadata ...", total=None, start=True)
         dropcols = [
             'id', 'nom', 'insee', 'bureau', 'num_bureau',
             'num_circo', 'name_circo', 'num_commune', 'name_commune',
             'code', 'label'
             ]
@@ -138,17 +143,18 @@
             for i, r in rows.iterrows():
                 columns = []
                 aliases = []
                 for col, lab, val in self.describeRow(r):
                     if col not in columns:
                         columns += [col]
                         aliases += [lab]
+                    
                     georow['properties'][col] = val
                     props = georow['properties']
-                    popup = fl.Popup(f"<a href={SITE_ROOT + f'/map/z/dept/{unidecode(props[geo_on]).lower()}' }><h4>Go to Zone</h4></a>") if popup_on else None
+                    popup = fl.Popup(f"<a href={SITE_ROOT + f'/map/z/dept/{processString(props[geo_on])}'}><h4>Go to Zone</h4></a>") if popup_on else None
                     yield fl.GeoJson(
                         data={"type":"FeatureCollection", "features": [georow]},
                         style_function=lambda x: { 'fillColor' : '#00000000', 'lineColor': '#00000000', 'line_opacity':0.01, "weight": 0.01},
                         tooltip=fl.GeoJsonTooltip(fields=columns, aliases=aliases),
                         popup=popup
                         )
                 idx += 1
@@ -188,8 +194,31 @@
         fg.add_to(self.m)
         self.m.keep_in_front(fg)
         fl.LayerControl().add_to(self.m)
         
     def build(self):
         return self.m
     
+    def buildDepts(self):
+        geodf = gpd.read_file("https://france-geojson.gregoiredavid.fr/repo/departements.geojson")
+        deptMaps = {}
+        for i, row in Quickbar.track(geodf.iterrows()):
+            center = [row.geometry.centroid.x, row.geometry.centroid.y]
+
+            lonLow, latLow, lonHigh, latHigh = row.geometry.bounds
+
+            dm = fl.Map(
+                location=center, zoom_start=10,
+                tiles="CartoDB positron", max_bounds=True,
+                max_lat=latHigh, max_lon=lonHigh,
+                min_lat=latLow, min_lon=lonLow, 
+                min_zoom=10
+                )
+            fl.GeoJson(
+                data={"type":"FeatureCollection", "features": [json.loads(shapely.to_geojson(row.geometry))] },
+                style_function=lambda x: { 'line_opacity':0.01, "weight": 0.01, 'opacity': 0.1},
+                ).add_to(dm)
+            
+            deptMaps[processString(row.nom)] = dm
+
+        return deptMaps
```

### Comparing `frgeostat-0.1.1.post1/frgeostat/utils.py` & `frgeostat-0.1.2/frgeostat/utils.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.1.post1/pyproject.toml` & `frgeostat-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "frgeostat"
-version = "0.1.1-post1"
+version = "0.1.2"
 description = "A small package to help creating maps of france with geo statistical data overlays."
 authors = ["volt-france <arno.veletanlic@volteuropa.org>"]
 readme = "README.md"
 homepage = "https://bureaux-vote.v.olt.sh"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `frgeostat-0.1.1.post1/PKG-INFO` & `frgeostat-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frgeostat
-Version: 0.1.1.post1
+Version: 0.1.2
 Summary: A small package to help creating maps of france with geo statistical data overlays.
 Home-page: https://bureaux-vote.v.olt.sh
 Author: volt-france
 Author-email: arno.veletanlic@volteuropa.org
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -25,15 +25,17 @@
 Requires-Dist: pynsee (>=0.1.4,<0.2.0)
 Requires-Dist: quickbar (>=0.1.1.post0,<0.2.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: unidecode (>=1.3.6,<2.0.0)
 Description-Content-Type: text/markdown
 
-# A small package to generate LeafletJS maps of France using `folium`
+[![PyPI version](https://badge.fury.io/py/frgeostat.svg)](https://badge.fury.io/py/frgeostat)
+
+# A package to create LeafletJS maps of France
 
 To install, create a virtualenv using whichever method you want, and either:
 
 ```shell
 pip install frgeostat
 ```
```

