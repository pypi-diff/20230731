# Comparing `tmp/frgeostat-0.1.0.tar.gz` & `tmp/frgeostat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frgeostat-0.1.0.tar", max compression
+gzip compressed data, was "frgeostat-0.1.1.tar", max compression
```

## Comparing `frgeostat-0.1.0.tar` & `frgeostat-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-28 12:51:52.685150 frgeostat-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-28 12:51:52.685150 frgeostat-0.1.0/frgeostat/__init__.py
--rw-r--r--   0        0        0     2375 2023-07-31 04:23:17.826154 frgeostat-0.1.0/frgeostat/cli.py
--rw-r--r--   0        0        0     3705 2023-07-28 19:23:04.026154 frgeostat-0.1.0/frgeostat/communes.py
--rw-r--r--   0        0        0      326 2023-07-31 04:13:26.663405 frgeostat-0.1.0/frgeostat/config.toml
--rw-r--r--   0        0        0     7844 2023-07-31 04:31:26.712993 frgeostat-0.1.0/frgeostat/departements.py
--rw-r--r--   0        0        0      697 2023-07-31 04:21:33.051262 frgeostat-0.1.0/frgeostat/utils.py
--rw-r--r--   0        0        0      710 2023-07-31 04:33:33.904651 frgeostat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 frgeostat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      896 2023-07-31 05:06:12.146110 frgeostat-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 12:51:52.685150 frgeostat-0.1.1/frgeostat/__init__.py
+-rw-r--r--   0        0        0     2375 2023-07-31 04:23:17.826154 frgeostat-0.1.1/frgeostat/cli.py
+-rw-r--r--   0        0        0     3705 2023-07-28 19:23:04.026154 frgeostat-0.1.1/frgeostat/communes.py
+-rw-r--r--   0        0        0      326 2023-07-31 04:13:26.663405 frgeostat-0.1.1/frgeostat/config.toml
+-rw-r--r--   0        0        0     7938 2023-07-31 05:16:51.213525 frgeostat-0.1.1/frgeostat/departements.py
+-rw-r--r--   0        0        0      697 2023-07-31 04:21:33.051262 frgeostat-0.1.1/frgeostat/utils.py
+-rw-r--r--   0        0        0      731 2023-07-31 05:19:06.826124 frgeostat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 frgeostat-0.1.1/PKG-INFO
```

### Comparing `frgeostat-0.1.0/frgeostat/cli.py` & `frgeostat-0.1.1/frgeostat/cli.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.0/frgeostat/communes.py` & `frgeostat-0.1.1/frgeostat/communes.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.0/frgeostat/departements.py` & `frgeostat-0.1.1/frgeostat/departements.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import geopandas as gpd
 import pandas as pd
 import plotly.express as px
 import folium as fl
 import numpy as np
 import requests as rq
 from folium.plugins import Search
-from frgeostat.utils import cerr, SITE_ROOT
+from frgeostat.utils import cerr, SITE_ROOT, cout
 from quickbar import Quickbar
+from unidecode import unidecode
 
 from typing import Generator, Any, Dict, Callable        
 
 class Departements:
     def __init__(self, save: bool = False) -> None:
         qbar = Quickbar('spin')
         qbar.bar.start()
@@ -105,15 +106,14 @@
                 }
             }
             
             for metric, opts in metrics.items():
                 values = [row[opts[key]] for key in opts if key != 'template']
                 templated = opts['template'](*values)
                 yield code, label, templated
-                    
         
     def propSetterGeoJSON(
         self,
         on: str = None,
         data_on: str = None,
         geo_on: str = None,
         popup_on: str = None
@@ -129,26 +129,28 @@
         
         is_collection = 'features' in geometries
         if not is_collection:
             geometries = {"type":"FeatureCollection", "features": [geometries]}
             
         idx = 0
         for georow in Quickbar.track(geometries['features'], message="Processing geometries.."):
-            rows = data[data[data_on] == georow['properties'][geo_on]].copy()
+            
+            rows = data[data[data_on].astype(str).str.lower().str.contains(str(georow['properties'][geo_on]).lower())].copy()
             for i, r in rows.iterrows():
                 columns = []
                 aliases = []
                 for col, lab, val in self.describeRow(r):
                     if col not in columns:
                         columns += [col]
                         aliases += [lab]
-                    geometries['features'][idx]['properties'][col] = val
-                    popup = fl.Popup(f"<a href={SITE_ROOT + f'/map/z/dept/{str(r[popup_on]).lower()}'}><h4>Go to Zone</h4></a>") if popup_on else None
+                    georow['properties'][col] = val
+                    props = georow['properties']
+                    popup = fl.Popup(f"<a href={SITE_ROOT + f'/map/z/dept/{unidecode(props[geo_on]).lower()}' }><h4>Go to Zone</h4></a>") if popup_on else None
                     yield fl.GeoJson(
-                        data={"type":"FeatureCollection", "features": [geometries['features'][idx]]},
+                        data={"type":"FeatureCollection", "features": [georow]},
                         style_function=lambda x: { 'fillColor' : '#00000000', 'lineColor': '#00000000', 'line_opacity':0.01, "weight": 0.01},
                         tooltip=fl.GeoJsonTooltip(fields=columns, aliases=aliases),
                         popup=popup
                         )
                 idx += 1
         return columns, aliases, geometries
         
@@ -174,15 +176,15 @@
             line_opacity=0.2,
             legend_name="Probability to vote Volt (%)",
         )
 
         fg = fl.FeatureGroup(name="tooltips")
 
 
-        for geolayer in self.propSetterGeoJSON(data_on='num_dept', geo_on='code', popup_on='name_dept'):
+        for geolayer in self.propSetterGeoJSON(data_on='name_dept', geo_on='nom', popup_on='name_dept'):
             fg.add_child(geolayer)
         
         
         chloro.add_to(self.m)
         fg.add_to(self.m)
         self.m.keep_in_front(fg)
         fl.LayerControl().add_to(self.m)
```

### Comparing `frgeostat-0.1.0/frgeostat/utils.py` & `frgeostat-0.1.1/frgeostat/utils.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.0/pyproject.toml` & `frgeostat-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "frgeostat"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["volt-france <arno.veletanlic@volteuropa.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 geopandas = "^0.13.2"
@@ -20,14 +20,15 @@
 fastparquet = "^2023.7.0"
 pyarrow = "^12.0.1"
 pynsee = "^0.1.4"
 ipywidgets = "^8.0.7"
 jinja2 = "^3.1.2"
 addict = "^2.4.0"
 quickbar = "^0.1.1.post0"
+unidecode = "^1.3.6"
 
 [tool.poetry.scripts]
 fr-geo-stats = "frgeostat.cli:app"
 frgeo = "frgeostat.cli:app"
 
 [build-system]
 requires = ["poetry-core"]
```

