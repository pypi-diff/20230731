# Comparing `tmp/py_astrolab-0.5.1.tar.gz` & `tmp/py_astrolab-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.5.1.tar", max compression
+gzip compressed data, was "py_astrolab-0.6.0.tar", max compression
```

## Comparing `py_astrolab-0.5.1.tar` & `py_astrolab-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.5.1/README.md
--rwxr-xr-x   0        0        0     4901 2023-07-27 15:11:41.462674 py_astrolab-0.5.1/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    16852 2023-07-27 16:04:29.967031 py_astrolab-0.5.1/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.5.1/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80941 2023-07-21 16:15:50.088586 py_astrolab-0.5.1/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.5.1/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.5.1/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.5.1/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71736 2023-07-25 15:24:19.500166 py_astrolab-0.5.1/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.5.1/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12401 2023-07-25 15:23:51.791751 py_astrolab-0.5.1/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.5.1/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.5.1/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7566 2023-07-25 15:24:01.061996 py_astrolab-0.5.1/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.5.1/py_astrolab/report.py
--rwxr-xr-x   0        0        0     3247 2023-07-27 20:12:31.604054 py_astrolab-0.5.1/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5235 2023-07-27 20:11:43.719226 py_astrolab-0.5.1/py_astrolab/types.py
--rwxr-xr-x   0        0        0     9741 2023-07-26 15:25:12.372813 py_astrolab-0.5.1/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-07-27 20:13:38.665107 py_astrolab-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.6.0/README.md
+-rwxr-xr-x   0        0        0     4910 2023-07-28 14:25:59.099727 py_astrolab-0.6.0/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    15760 2023-07-30 15:40:50.145067 py_astrolab-0.6.0/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.6.0/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80380 2023-07-29 10:08:55.050610 py_astrolab-0.6.0/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.6.0/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.6.0/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.6.0/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71492 2023-07-28 15:58:20.983796 py_astrolab-0.6.0/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.6.0/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-27 22:22:27.571322 py_astrolab-0.6.0/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.6.0/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.6.0/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7533 2023-07-28 15:50:57.383513 py_astrolab-0.6.0/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.6.0/py_astrolab/report.py
+-rwxr-xr-x   0        0        0    17383 2023-07-31 18:16:03.806002 py_astrolab-0.6.0/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5061 2023-07-30 17:36:22.186828 py_astrolab-0.6.0/py_astrolab/types.py
+-rwxr-xr-x   0        0        0    10147 2023-07-28 15:51:20.189316 py_astrolab-0.6.0/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-07-31 18:21:30.538066 py_astrolab-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.6.0/PKG-INFO
```

### Comparing `py_astrolab-0.5.1/py_astrolab/__init__.py` & `py_astrolab-0.6.0/py_astrolab/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,8 +141,8 @@
 from .main import KrInstance
 from .print_all_data import print_all_data
 from .charts.charts_svg import MakeSvgInstance
 from .types import *
 from .relationship_score import RelationshipScore
 from .aspects import NatalAspects, CompositeAspects
 from .report import Report
-from .transits import Transits
+from .transits import Transit, Transits
```

### Comparing `py_astrolab-0.5.1/py_astrolab/aspects.py` & `py_astrolab-0.6.0/py_astrolab/aspects.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,43 +17,29 @@
 class NatalAspects():
     """
     Generates an object with all the aspects of a birthcart.
     """
 
     def __init__(
             self, kr_object: KrInstance,
-            new_settings_file: Union[str, Path, None] = None
+            settings: Union[str, None] = None
     ):
         self.user = kr_object
-        self.new_settings_file = new_settings_file
-        self._parse_json_settings()
-
-        if not hasattr(self.user, "sun"):
-            self.user.__get_all()
-
-        self.init_point_list = self.user.planets_list + self.user.houses_list + self.user.axis_list
-
-    def _parse_json_settings(self):
-        # Load settings file
-        DATADIR = Path(__file__).parent
-
-        if not self.new_settings_file:
-            settings_file = DATADIR / "kr.config.json"
-        else:
-            settings_file = Path(self.new_settings_file)
-
-        with open(settings_file, 'r', encoding="utf-8", errors='ignore') as f:
-            settings = json.load(f)
-
+        self.settings = settings
         self.colors_settings = settings['colors']
         self.planets_settings = settings['planets']
         self.axes_settings = settings['axes']
         self.aspects_settings = settings['aspects']
         self.axes_orbit_settings = settings['axes_orbit']
 
+        if not hasattr(self.user, "sun"):
+            self.user.__get_all()
+
+        self.init_point_list = self.user.planets_list + self.user.houses_list + self.user.axis_list
+
     def asp_calc(self, point_one, point_two):
         """ 
         Utility function.
         It calculates the aspects between the 2 points.
         Args: first point, second point. 
         """
 
@@ -147,29 +133,29 @@
 
     def p_id_decoder(self, name):
         """ 
         Check if the name of the planet is the same in the settings and return
         the correct id for the planet.
         """
         str_name = str(name)
-        settings = self.planets_settings
+        settings = self.planets_settings.copy()
         settings.extend(self.axes_settings)
         for a in settings:
             if a['name'] == str_name:
                 result = a['id']
                 return result
 
     def filter_by_settings(self, init_point_list):
         """
         Creates a list of all the desired
         points filtering by the settings.
         """
 
         set_points_name = []
-        settings = self.planets_settings
+        settings = self.planets_settings.copy()
         settings.extend(self.axes_settings)
         for p in settings:
             if p['visible']:
                 set_points_name.append(p['name'])
 
         point_list = []
         for l in init_point_list:
@@ -210,91 +196,64 @@
                              "p2": self.p_id_decoder(point_list[second]['name'],)
                              }
                     self.all_aspects_list.append(d_asp)
 
         return self.all_aspects_list
 
     def is_fake_aspect(self, aspect: dict) -> bool:
-        is_fake_aspect = False
-        user = json.loads(self.user.json())
         p1_name = aspect['p1_name'].lower().replace(' ', '_')
         p2_name = aspect['p2_name'].lower().replace(' ', '_')
+        p1_attr = getattr(self.user, p1_name)
+        p2_attr = getattr(self.user, p2_name)
         if p1_name == 'true_node' and p2_name == 'south_node':
-            is_fake_aspect = True
-        if user[p1_name]['element'] == user[p2_name]['element'] and aspect['aspect'] == 'square':
-            is_fake_aspect = True
-        if aspect['aspect'] in {'trine', 'conjunction'}:
-            if user[p1_name]['element'] != user[p2_name]['element']:
-                if aspect['orbit'] > 3:
-                    is_fake_aspect = True
-        elif aspect['aspect'] == 'opposition':
-            p1_sign = user[p1_name]['signs'][0]
-            p2_sign = user[p2_name]['signs'][0]
+            return True
+        if p1_attr['element'] == p2_attr['element'] and aspect['aspect'] == 'square':
+            return True
+        if aspect['aspect'] in {'trine', 'conjunction'} and p1_attr['element'] != p2_attr['element'] and aspect['orbit'] > 3:
+            return True
+        if aspect['aspect'] == 'opposition':
+            p1_sign = p1_attr['signs'][0]
+            p2_sign = p2_attr['signs'][0]
             p1_sign_opposite = self.user.signs_dict[p1_sign]['opposite']
-            if not p1_sign_opposite.startswith(p2_sign):
-                is_fake_aspect = True
-        return is_fake_aspect
+            return not p1_sign_opposite.startswith(p2_sign)
+        return False
 
     def get_relevant_aspects(self):
-        """ 
-        Filters the aspects list with the desired points, in this case
-        the most important are hardcoded.
-        Set the list with set_points and creating a list with the names
-        or the numbers of the houses.
-        """
-
         self.get_all_aspects()
-
-        aspects_filtered = []
-        for a in self.all_aspects_list:
-            if self.aspects_settings[a["aid"]]["visible"] == True:
-                aspects_filtered.append(a)
-
-        axes_list = [
+        aspects_filtered = [a for a in self.all_aspects_list if self.aspects_settings[a["aid"]]["visible"] == True]
+        axes_set = {
             "Ascendant",
             "Midheaven",
             "Descendant",
             "Imum Coeli"
-        ]
-        counter = 0
-    
-        aspects_list_subtract = []
-        for a in aspects_filtered:
-            counter += 1
-            name_p1 = str(a['p1_name'])
-            name_p2 = str(a['p2_name'])
-
-            if name_p1 in axes_list:
-                if abs(a['orbit']) >= self.axes_orbit_settings:
-                    aspects_list_subtract.append(a)
-
-            elif name_p2 in axes_list:
-                if abs(a['orbit']) >= self.axes_orbit_settings:
-                    aspects_list_subtract.append(a)
-            
-            if self.is_fake_aspect(a):
-                aspects_list_subtract.append(a)
-
-        self.aspects = [
-            item for item in aspects_filtered if item not in aspects_list_subtract]
-
+        }
+        aspects_filtered = [a for a in aspects_filtered if not (
+            (a['p1_name'] in axes_set and abs(a['orbit']) >= self.axes_orbit_settings) or
+            (a['p2_name'] in axes_set and abs(a['orbit']) >= self.axes_orbit_settings) or
+            self.is_fake_aspect(a)
+        )]
+        self.aspects = aspects_filtered
         return self.aspects
 
 
 class CompositeAspects(NatalAspects):
     """
     Generates an object with all the aspects between two persons.
     """
 
-    def __init__(self, kr_object_one: KrInstance, kr_object_two: KrInstance, new_settings_file: Union[str, Path, None] = None):
+    def __init__(self, kr_object_one: KrInstance, kr_object_two: KrInstance, settings: Union[str, None] = None):
         self.first_user = kr_object_one
         self.second_user = kr_object_two
 
-        self.new_settings_file = new_settings_file
-        self._parse_json_settings()
+        self.settings = settings
+        self.colors_settings = settings['colors']
+        self.planets_settings = settings['planets']
+        self.axes_settings = settings['axes']
+        self.aspects_settings = settings['aspects']
+        self.axes_orbit_settings = settings['axes_orbit']
 
         if not hasattr(self.first_user, "sun"):
             self.first_user.__get_all()
 
         if not hasattr(self.second_user, "sun"):
             self.second_user.__get_all()
```

### Comparing `py_astrolab-0.5.1/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.6.0/py_astrolab/charts/charts_svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # * TODO: Change the label for language in 2 objects, one for IT and one for ENG.
 # * Then change the label for planets like this: planet["label"] => planet[language]
 
-import json
 import math
 from datetime import datetime
-from math import cos, radians, sin
 from pathlib import Path
 from string import Template
 from typing import Union
 
 import pytz
 
 from py_astrolab.aspects import CompositeAspects, NatalAspects
@@ -32,26 +30,26 @@
     Parameters:
         - first_obj: First kerykeion object
         - chart_type: Natal, Transit, Composite (Default: Type="Natal")
         - second_obj: Second kerykeion object (Not required if type is Natal)
         - new_output_directory: Set the output directory (default: output_directory)
         - template_type: set the template type to include or not the aspects grid, default: extended)
         - lang: language settings (default: "EN")
-        - new_settings_file: Set the settings file (default: kr.config.json)
+        - settings: Set the settings
     """
 
     def __init__(
             self,
             first_obj: KrInstance,
             chart_type: ChartType = "Natal",
             second_obj: Union[KrInstance, None] = None,
             new_output_directory: Union[str, None] = None,
             template_type: str = "extended",
             lang: str = "EN",
-            new_settings_file: Union[str, Path, None] = None
+            settings: Union[str, Path, None] = None
     ):
 
         # Directories:
         DATADIR = Path(__file__).parent
         self.homedir = Path.home()
 
         if new_output_directory:
@@ -68,20 +66,21 @@
             self.xml_svg = DATADIR / 'templates/extended.xml'
 
         # SVG Width
         self.natal_width = 772.2
         self.full_width = 1200
 
         # Settings file:
-        if not new_settings_file:
-            self.settings_file = DATADIR.parent / 'kr.config.json'
-        else:
-            self.settings_file = Path(new_settings_file)
-
-        self.parse_json_settings(self.settings_file, lang)
+        self.settings = settings
+        self.language_settings = settings['language_settings'].get(
+            lang, "EN")
+        self.colors_settings = settings['colors']
+        self.planets_settings = settings['planets']
+        self.axes_settings = settings['axes']
+        self.aspects_settings = settings['aspects']
         self.chart_type = chart_type
 
         # Kerykeion instance
         self.user = first_obj
         if not hasattr(self.user, "sun"):
             print(f"Generating kerykeion object for {self.user.name}...")
             self.user.__get_all()
@@ -135,15 +134,15 @@
 
         self.houses_sign_graph = []
         for h in self.user.houses_list:
             self.houses_sign_graph.append(h['sign_num'])
 
         if self.chart_type == "Natal":
             natal_aspects_instance = NatalAspects(
-                self.user, new_settings_file=self.settings_file)
+                self.user, settings=self.settings)
             self.aspects_list = natal_aspects_instance.get_relevant_aspects()
 
         if (self.chart_type == "Transit" or self.chart_type == "Composite"):  # TODO: If not second should exit
 
             if not second_obj:
                 raise KerykeionException(
                     "Second object is required for Transit or Composite charts.")
@@ -1023,15 +1022,15 @@
         """
         conj = {}  # 0
         opp = {}  # 10
         sq = {}  # 5
         tr = {}  # 6
         qc = {}  # 9
         sext = {}  # 3
-        for i in range(len(self.planets_settings)):
+        for i in range(len(self.planets_settings)):            
             a = self.planets_degree_ut[i]
             qc[i] = {}
             sext[i] = {}
             opp[i] = {}
             sq[i] = {}
             tr[i] = {}
             conj[i] = {}
@@ -1219,15 +1218,15 @@
 
     # Aspect and aspect grid functions for transit type charts.
 
     def __makeAspectsTransit(self, r, ar):
         out = ""
 
         self.aspects_list = CompositeAspects(
-            self.user, self.t_user, new_settings_file=self.settings_file
+            self.user, self.t_user, settings=self.settings
         ).get_relevant_aspects()
 
         for aspect_dict in self.aspects_list:
             aspect_id = f"{min(aspect_dict['p1_name'], aspect_dict['p2_name'])}{aspect_dict['aspect'].title()}{max(aspect_dict['p1_name'], aspect_dict['p2_name'])}"
             out += self.__drawAspect(r, ar, aspect_dict, aspect_id)
 
         return out
@@ -1494,28 +1493,14 @@
         """
         Sets the output direcotry and returns it's path.
         """
         self.output_directory = Path(dir_path)
         dir_string = f"Output direcotry set to: {self.output_directory}"
         return (print(dir_string))
 
-    def parse_json_settings(self, settings_file, lang: str):
-        """
-        Parse the settings file.
-        """
-        with open(settings_file, 'r', encoding="utf-8", errors='ignore') as f:
-            settings = json.load(f)
-
-        self.language_settings = settings['language_settings'].get(
-            lang, "EN")
-        self.colors_settings = settings['colors']
-        self.planets_settings = settings['planets']
-        self.axes_settings = settings['axes']
-        self.aspects_settings = settings['aspects']
-
     def makeTemplate(self):
         # self.chart_type = "Transit"
         # empty element points
         self.fire = 0.0
         self.earth = 0.0
         self.air = 0.0
         self.water = 0.0
```

### Comparing `py_astrolab-0.5.1/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.6.0/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.1/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.6.0/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.1/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.6.0/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.1/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.6.0/py_astrolab/charts/wonderful_mistake.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,26 @@
     Parameters:
         - first_obj: First kerykeion object
         - chart_type: Natal, Transit, Composite (Default: Type="Natal")
         - second_obj: Second kerykeion object (Not required if type is Natal)
         - new_output_directory: Set the output directory (default: output_directory)
         - template_type: set the template type to include or not the aspects grid, default: extended)
         - lang: language settings (default: "EN")
-        - new_settings_file: Set the settings file (default: kr.config.json)
+        - settings: Set the settings file (default: kr.config.json)
     """
 
     def __init__(
             self,
             first_obj: KrInstance,
             chart_type: ChartType = "Natal",
             second_obj: Union[KrInstance, None] = None,
             new_output_directory: Union[str, None] = None,
             template_type: str = "extended",
             lang: str = "EN",
-            new_settings_file: Union[str, Path, None] = None
+            settings: Union[str, Path, None] = None
     ):
 
         # Directories:
         DATADIR = Path(__file__).parent
         self.homedir = Path.home()
 
         if new_output_directory:
@@ -66,20 +66,16 @@
             self.xml_svg = DATADIR / 'templates/extended.xml'
 
         # SVG Width
         self.natal_width = 772.2
         self.full_width = 1200
 
         # Settings file:
-        if not new_settings_file:
-            self.settings_file = DATADIR.parent / 'kr.config.json'
-        else:
-            self.settings_file = Path(new_settings_file)
+        self.settings = settings
 
-        self.parse_json_settings(self.settings_file, lang)
         self.chart_type = chart_type
 
         # Kerykeion instance
         self.user = first_obj
         if not hasattr(self.user, "sun"):
             print(f"Generating kerykeion object for {self.user.name}...")
             self.user.__get_all()
@@ -134,15 +130,15 @@
 
         self.houses_sign_graph = []
         for h in self.user.houses_list:
             self.houses_sign_graph.append(h['sign_num'])
 
         if self.chart_type == "Natal":
             natal_aspects_instance = NatalAspects(
-                self.user, new_settings_file=self.settings_file)
+                self.user, settings=self.settings)
             self.aspects_list = natal_aspects_instance.get_relevant_aspects()
 
         if (self.chart_type == "Transit" or self.chart_type == "Composite"):  # TODO: If not second should exit
 
             if not second_obj:
                 raise KerykeionException(
                     "Second object is required for Transit or Composite charts.")
@@ -1109,15 +1105,15 @@
 
     # Aspect and aspect grid functions for transit type charts.
 
     def __makeAspectsTransit(self, r, ar):
         out = ""
 
         self.aspects_list = CompositeAspects(
-            self.user, self.t_user, new_settings_file=self.settings_file
+            self.user, self.t_user, settings=self.settings
         ).get_relevant_aspects()
 
         for element in self.aspects_list:
             out += self.__drawAspect(r, ar, element['p1_abs_pos'], element['p2_abs_pos'],
                                    self.colors_settings[f"aspect_{element['aspect_degrees']}"])
 
         return out
```

### Comparing `py_astrolab-0.5.1/py_astrolab/fetch_geonames.py` & `py_astrolab-0.6.0/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.1/py_astrolab/main.py` & `py_astrolab-0.6.0/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.1/py_astrolab/print_all_data.py` & `py_astrolab-0.6.0/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.1/py_astrolab/relationship_score.py` & `py_astrolab-0.6.0/py_astrolab/relationship_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,27 @@
     first_subject: KrInstance
     second_subject: KrInstance
     score: int
     is_destiny_sign: bool
     relevant_default_aspects: list
     relevant_default_aspects: list
 
-    def __init__(self, first_subject: KrInstance, second_subject: KrInstance, logger: Union[Logger, None] = None, new_settings_file: Union[str, Path, None] = None):
+    def __init__(self, first_subject: KrInstance, second_subject: KrInstance, logger: Union[Logger, None] = None, settings: Union[str, None] = None):
 
         self.first_subject = first_subject
         self.second_subject = second_subject
         self.score = 0
         self.is_destiny_sign = False
         self.relevant_aspects = []
         self.relevant_default_aspects = []
         self.__logger: Logger = logger or getLogger(self.__class__.__name__)
         self.__all_composite_aspects = CompositeAspects(
             first_subject,
             second_subject,
-            new_settings_file=new_settings_file
+            settings=settings
         ).get_all_aspects()
 
         # Calculates all at initialization
         self.__get_all()
 
     def __str__(self) -> str:
         return f'CuppleScoreInstance: {self.first_subject.name} and {self.second_subject.name}, score: {self.score}'
```

### Comparing `py_astrolab-0.5.1/py_astrolab/report.py` & `py_astrolab-0.6.0/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.1/py_astrolab/types.py` & `py_astrolab-0.6.0/py_astrolab/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -233,21 +233,14 @@
     # Lilith
     mean_apog: KerykeionPoint
     oscu_apog: KerykeionPoint
 
     # Lunar Phase
     lunar_phase: LunarPhaseObject
 
-class Transit(BaseModel):
-    transit_aspects: list
-    natal_aspects: list
-    points_in_houses: list
-    phase: Union[LunarPhaseObject, None]
-    new_moon: KerykeionPoint
-
 if __name__ == "__main__":
     sun = KerykeionPoint(
         name='Sun',
         element='Air',
         quality='Fixed',
         sign='Aqu',
         sign_num=1,
```

### Comparing `py_astrolab-0.5.1/py_astrolab/utilities.py` & `py_astrolab-0.6.0/py_astrolab/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,8 +221,22 @@
         planet["house"] = "Eleventh House"
     elif point_between(kr_object.houses_degree_ut[11], kr_object.houses_degree_ut[0],
                         planet_deg) == True:
         planet["house"] = "Twelfth House"
     else:
         planet["house"] = "error!"
 
-    return planet
+    return planet
+
+def parse_json_settings(new_settings_file: Union[str, Path, None] = None):
+    # Load settings file
+    DATADIR = Path(__file__).parent
+
+    if not new_settings_file:
+        settings_file = DATADIR / "kr.config.json"
+    else:
+        settings_file = Path(new_settings_file)
+
+    with open(settings_file, 'r', encoding="utf-8", errors='ignore') as f:
+        settings = json.load(f)
+
+    return settings
```

### Comparing `py_astrolab-0.5.1/pyproject.toml` & `py_astrolab-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.5.1"
+version = "0.6.0"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.5.1/PKG-INFO` & `py_astrolab-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

