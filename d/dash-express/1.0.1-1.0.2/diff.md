# Comparing `tmp/dash_express-1.0.1.tar.gz` & `tmp/dash_express-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express-1.0.1.tar", last modified: Fri Jul 28 16:21:52 2023, max compression
+gzip compressed data, was "dash_express-1.0.2.tar", last modified: Mon Jul 31 13:36:37 2023, max compression
```

## Comparing `dash_express-1.0.1.tar` & `dash_express-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.943342 dash_express-1.0.1/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1071 2023-07-26 08:37:30.000000 dash_express-1.0.1/LICENSE
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-28 16:21:52.943342 dash_express-1.0.1/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     5606 2023-07-28 14:45:31.000000 dash_express-1.0.1/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.939342 dash_express-1.0.1/dash_express/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)    33840 2023-07-28 14:08:58.000000 dash_express-1.0.1/dash_express/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)    16493 2023-07-28 08:52:30.000000 dash_express-1.0.1/dash_express/_app_shell.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.943342 dash_express-1.0.1/dash_express/filters/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       88 2023-07-26 08:21:26.000000 dash_express-1.0.1/dash_express/filters/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     3374 2023-07-26 08:21:26.000000 dash_express-1.0.1/dash_express/filters/autofilter.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      612 2023-07-26 08:21:26.000000 dash_express-1.0.1/dash_express/filters/filterfunc.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.943342 dash_express-1.0.1/dash_express/kpi/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1761 2023-07-26 17:26:07.000000 dash_express-1.0.1/dash_express/kpi/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     2360 2023-07-26 08:27:32.000000 dash_express-1.0.1/dash_express/preview_chart.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        7 2023-07-28 02:54:43.000000 dash_express-1.0.1/dash_express/version.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-28 16:21:52.939342 dash_express-1.0.1/dash_express.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      443 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      135 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/requires.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       13 2023-07-28 16:21:52.000000 dash_express-1.0.1/dash_express.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-07-28 16:21:52.943342 dash_express-1.0.1/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1366 2023-07-28 16:21:13.000000 dash_express-1.0.1/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.484001 dash_express-1.0.2/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1071 2023-07-26 08:37:30.000000 dash_express-1.0.2/LICENSE
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-31 13:36:37.484001 dash_express-1.0.2/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     5606 2023-07-28 14:45:31.000000 dash_express-1.0.2/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.480001 dash_express-1.0.2/dash_express/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)    38275 2023-07-31 13:35:07.000000 dash_express-1.0.2/dash_express/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)    16540 2023-07-29 14:46:24.000000 dash_express-1.0.2/dash_express/_app_shell.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.484001 dash_express-1.0.2/dash_express/filters/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       88 2023-07-26 08:21:26.000000 dash_express-1.0.2/dash_express/filters/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     3374 2023-07-26 08:21:26.000000 dash_express-1.0.2/dash_express/filters/autofilter.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      482 2023-07-31 13:29:47.000000 dash_express-1.0.2/dash_express/filters/filterfunc.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.484001 dash_express-1.0.2/dash_express/kpi/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     2086 2023-07-31 13:17:41.000000 dash_express-1.0.2/dash_express/kpi/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     2360 2023-07-26 08:27:32.000000 dash_express-1.0.2/dash_express/preview_chart.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       11 2023-07-31 13:34:49.000000 dash_express-1.0.2/dash_express/version.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-07-31 13:36:37.480001 dash_express-1.0.2/dash_express.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     6089 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      443 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      135 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/requires.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       13 2023-07-31 13:36:37.000000 dash_express-1.0.2/dash_express.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-07-31 13:36:37.484001 dash_express-1.0.2/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1090 2023-07-31 13:35:26.000000 dash_express-1.0.2/setup.py
```

### Comparing `dash_express-1.0.1/LICENSE` & `dash_express-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.1/PKG-INFO` & `dash_express-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_express
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool for faster application development Plotly Dash
 Home-page: https://github.com/stpnvkirill/dash-express
 Author: Kirill Stepanov
 Author-email: stpnv.kirill.o@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dash_express-1.0.1/README.md` & `dash_express-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.1/dash_express/__init__.py` & `dash_express-1.0.2/dash_express/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 import pandas as pd
 import dash_leaflet as dl
 import plotly.graph_objects as go
 import dash_mantine_components as dmc
 
 
+from .version import V
 from .kpi import KPI, FastKPI
 from .filters import autofilter
 from flask_caching import Cache
 from dash_iconify import DashIconify
 from .preview_chart import _render_wrapper
 from dash.exceptions import PreventUpdate
 from dash._jupyter import JupyterDisplayMode
@@ -50,15 +51,29 @@
     multi-page web analytics applications.
 
     DashExpress uses the Mantine framework and supports dark theme out of the box. 
     Additionally on the side of DashExpress dark is applied to the objects of PLotly figures and Leaflet maps.
     
     Dash is a framework for building analytic web applications without 
     the use of JavaScript.
+
+    :param logo: navbar logo, string or dict: {'dark':'path/to/darklogo.svg', 'light':...}
+    :type logo: string or dict
+
+    :param cache: flask_caching.Cache instance, dict or True (default: True)
+    :type cache: flask_caching.Cache instance, dict or True
+
+    :param default_cache_timeout: flask_caching.Cache timeout in seconds (default: 3600)
+    :type default_cache_timeout: int
+
+    :param app_shell: Appshell class for customization UI your app
+    :type app_shell: BaseAppShell instance
     
+    -------------------------------
+
     :param name: The name Flask should use for your app. Even if you provide
         your own ``server``, ``name`` will be used to help find assets.
         Typically ``__name__`` (the magic global var, not a string) is the
         best value to use. Default ``'__main__'``, env: ``DASH_APP_NAME``
     :type name: string
 
     :param server: Sets the Flask server for your app. There are three options:
@@ -239,15 +254,15 @@
             raise ValueError("cache must be a flask_caching.Cache or a boolean")
         
     def _app_shell(self):
         self.layout = self.app_shell._app_provider(self)
 
     def register_page(self, Page):
         self.PAGES[Page.URL] = Page
-    
+
     def register_server_callback(self):
         """Register a function callback on the server side"""
         # Send Page.layout to front
         @self.callback(Output("layout-store", 'data'),
                     Input("layout-store", 'data'))
         def send_layout(d):
             dict1 = {k: v.render()
@@ -426,14 +441,15 @@
                 return [layout['navs']] } """,
             [Output("nav-content", 'children')],
             Input("layout-store", 'data'))
         
         self.app_shell.app_shell_clientside(self)
 
     def compile_layout(self):
+        """Compile layout and callback functions"""
         self._app_shell()
         self.DOWNLOAD_OPPORTUNITY = np.any([page.download_opportunity for page in self.PAGES.values()])
         self.register_clientside_callback()
         self.register_server_callback()
 
     def run(self, host=os.getenv("HOST", "127.0.0.1"), port=os.getenv("PORT", "8050"), proxy=os.getenv("DASH_PROXY", None), debug=None,
             jupyter_mode: JupyterDisplayMode = None, jupyter_width="100%", jupyter_height=650, jupyter_server_url=None,
@@ -446,29 +462,51 @@
                            dev_tools_props_check, dev_tools_serve_dev_bundles, dev_tools_hot_reload, dev_tools_hot_reload_interval, 
                            dev_tools_hot_reload_watch_interval, dev_tools_hot_reload_max_retry, dev_tools_silence_routes_logging, 
                            dev_tools_prune_errors, **flask_run_options)
 
 
 class Page(object):  
     """Page object for quickly creating a web dashboard.
-        The app needs 3 components to work:
+        
+        :param app: DashExpress app
+        :type app: DashExpress instance
+
+        :param url_path: page_url
+        :type url_path: str
+
+        :param name: nav name
+        :type name: string
+
+        :param get_df: DataFrame function
+        :type get_df: function
 
-        1) DataFrame get function
+        :param title: page title
+        :type title: string
 
-        2) Dashboard layout
+        :param description: page description
+        :type description: string
 
-        3) Functions for generating graphs, kpi values ​​and getting geojson
+        :param access_func: function access
+        :type access_func: function
+
+        :param access_mode: 'hide' | 'view'
+        :type access_mode: string
+
+        :param download_opportunity: True | False
+        :type download_opportunity: bool
         """  
     def __repr__(self):
         return f'Page: {self.URL}'
 
     def __init__(self, app, url_path, name=None, get_df=None, title=None, description=None,
                  access_func=None, access_mode='hide', download_opportunity=True,):
+        prefix = app.config.get('url_base_pathname') or '/'
+        
         self.name = name or 'Page'        
-        self.URL = url_path
+        self.URL = prefix[:-1] + url_path
         self.title = title if title else app.config['title']
         self.description = description
         self.access_func = access_func
         self.access_mode = access_mode
         self.download_opportunity = download_opportunity
 
         self.RENDER_FUNC = {}
@@ -562,20 +600,84 @@
         def get_df_func():
             df = get_df()
             return df  
                 
         self.get_df_func = get_df_func
            
     def add_kpi(self, kpi):
+        """Add kpi_cards to the layout.
+        
+        The KPI rendering system is based on the use of the KPI class, which contains a container representation and the logic for calculating the indicator. The simplest implementation of KPI, with automatic generation of the calculation function, is presented in the FastKPI class:
+
+        ```python
+        from dash_express import FastKPI
+        app.add_kpi(FastKPI(columns, agg_func=np.sum)
+        ```
+
+        FastKPI Initialization Parameters:
+   
+        ```
+        col = DataFrame Column
+        agg_func = pivot func for calculate kpi
+        pretty_func = pretty func for result calculate, for example: lambda x: f'{x:.1%}'
+        title = title of cards? default automatic generation
+        ```
+        -----
+
+        An advanced way to add KPI is to create your own card by inheriting from the base class of KPI:
+
+        ```python
+        from dash_express import KPI
+
+        class MyKPI(KPI):
+            def __init__(self, ...):
+                ...
+
+            def render_layout(self, id):
+                '''Render Container'''
+                return dmc.Card(...)
+
+            def render_func(self,df):
+                '''Compute & Render value'''
+                return ...
+
+        app.add_kpi(MyKPI())
+        ```
+        """
         id = str(uuid.uuid4())
         self.RENDER_FUNC_KPI[id] = kpi.render_func
         self.RENDER_FUNC_KPI['default'] = self.render_kpi_wrapper
         return kpi.render_layout(dict(type='kpifilter-store', id=id))
 
     def add_graph(self, id=None, render_func=None, **kwargs):
+        """Add plotly figure to the layout
+        
+        The Plotly graphing library has more than 50 chart types to choose from. For Dash Express to work, you need to answer 2 questions:
+
+        1. Where is the graph located
+        2. How to build a graph
+
+        The answer to the first question is laid when developing the layout, by calling the page.add_graph(...) method in the location of the graph, a simple example:
+
+        ```python
+        dmc.SimpleGrid(
+            [
+                page.add_graph(h='100%',render_func=bar_func),
+                page.add_graph(h='100%',render_func=line_func),
+            ],
+            cols=2
+            )
+        ```
+
+        Through .add_graph is a function containing the logic of plotting to which the Dash Express application will pass the filtered DataFrame.
+        ```python
+        def bar_func(df):
+            return px.bar(df, x="nation", y="count", color="medal", title="Long-Form Input")
+        ```
+"""
         CONFIG = {
             'modeBarButtonsToRemove': ['pan2d', 'lasso2d',
                                     'logo', 
                                     'zoom',
                                     'box', 'select',
                                     # 'zoomin', 'zoomout', 
                                     'reset',
@@ -605,14 +707,30 @@
                 dcc.Store(id=dict(type='contentfilter-store', id=id))
             ],
             withBorder=True,
             **kwargs
         ))
 
     def add_map(self, geojson_func=None, p=0, dl_geojson_kwargs={'zoomToBounds': True}, **kwargs):
+        """Add a map to the layout
+        
+        If you use GeoPandas, you can add maps to your dashboard, it's as simple as adding a graph.:
+
+        ```python
+        page.add_map(geojson_func=None)
+        ```
+
+        geojson_func - should return GeoDataFrame.__get_interface__, if you do not need any additional transformations, do not specify this parameter, DashExpress will do everything for you.
+
+        ```python
+        def geojson_func(gdf):
+            gdf = gdf[gdf.geometry.geom_type == 'Polygon']
+            return gdf.__geo_interface__
+        ```
+        """
         id = str(uuid.uuid4())
         geojson_func = geojson_func or self.geojson_wrapper
         self.GEOJSON_FUNC[id] = geojson_func
         self.GEOJSON_FUNC['default'] = self.geojson_wrapper
         return dmc.LoadingOverlay(dmc.Card(
             [
                 html.Div(
@@ -630,15 +748,23 @@
             ],
             withBorder=True,
             p=p,
             **kwargs
         ))
 
     def add_autofilter(self, col,  multi=False, type='auto', label='auto', **kwargs):
+        """Add filter to the layout with automatic generation.
+        
+        Specify the column by which filtering will take place and say the type of filtering multi = True|False
+
+        ```python
+        page.add_autofilter('continent', multi=True)
+        ```
 
+        You can also specify additional parameters of the Dash Mantine component."""
         filter_func, f = self._add_autofilter(
             col, multi, type, label, **kwargs)
         self.FILTERS_FUNC[col] = filter_func
         self.FILTERS.append(f)
 
     def _add_autofilter(self, col, multi=False, type='auto', label='auto', **kwargs):
         with self.app.server.app_context():
@@ -654,14 +780,15 @@
                     if dtype in data_type:
                         type = 'slider' if dtype in [
                             'int', 'float'] else 'select'
                         return autofilter(type, serias, col, multi, label=label, **kwargs)
             return autofilter(type, serias, col, multi, label=label, **kwargs)
 
     def filtered(self, filters):
+        """Filter data by received constraints"""
         df = self.get_df_func()
         for k, v in filters.items():
             if v == None or (type(v) == type(list()) and len(v) == 0):
                 continue
             df = df[self.FILTERS_FUNC[k](df[k], v)]
         return df
```

### Comparing `dash_express-1.0.1/dash_express/_app_shell.py` & `dash_express-1.0.2/dash_express/_app_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,20 +90,20 @@
                 return True
             else:
                 return False
 
         out_filter = list(filter(filters, navs))
         return out_filter
 
-    def logo_container(self):
+    def logo_container(self, app):
         return dmc.Anchor(
             dmc.Image(height=45, id='logo-img') if isinstance(self.LOGO, dict) else self.LOGO,
             weight=550,
             size=30,
-            href="/",
+            href=app.config.get('url_base_pathname') or '/',
             underline=False,
             pr='xl',
         ) if self.LOGO else html.Div()
 
     def color_scheme_toggle(self, icon, **kwargs):
         action_icon = dmc.ActionIcon(icon, **kwargs)
         action_icon.id = "color-scheme-toggle"
@@ -177,15 +177,15 @@
     def nav_content(self, app):
         nav_cont = dmc.Grid(
             justify="center",
             style={"height": 60},
             children=[
                 dmc.Col(
                     dmc.Group([
-                        self.logo_container(),
+                        self.logo_container(app),
                         dmc.MediaQuery(dmc.Group(
                             id='nav-content',
                             spacing=3,
                         ), smallerThan="lg", styles={"display": "none"}, ),
                     ]),
                     pt=7,
                     span="content",
```

### Comparing `dash_express-1.0.1/dash_express/filters/autofilter.py` & `dash_express-1.0.2/dash_express/filters/autofilter.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.1/dash_express/kpi/__init__.py` & `dash_express-1.0.2/dash_express/kpi/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dash_mantine_components as dmc
 from dash_iconify import DashIconify
 from dash import html, dcc
 import numpy as np
 
 
 class KPI(object):
+    """KPI class contains a container representation and the logic for calculating the indicator"""
     def __init__(self, title, func, icon="flat-ui:settings", **kwargs) -> None:
         self.title = title
         self.func = func
         self.icon = icon
         self.kwargs = kwargs
 
     def render_layout(self, id):
@@ -31,14 +32,19 @@
             **self.kwargs)
 
     def render_func(self,df):
         return self.func(df)
     
 
 class FastKPI(KPI):
+    """
+    col = DataFrame Column
+    agg_func = pivot func for calculate kpi
+    pretty_func = pretty func for result calculate, for example: lambda x: f'{x:.1%}'
+    title = title of cards? default automatic generation"""
     def __init__(self, col, agg_func=np.mean, pretty_func=lambda x: f'{x:.1%}', title='auto', 
                  icon="flat-ui:settings", **kwargs) -> None:
         if title == 'auto':
             title = col.capitalize()
         func = self.render_fastkpi_wrapper(col, agg_func, pretty_func=pretty_func)
         super().__init__(title, func, icon=icon, **kwargs)
```

### Comparing `dash_express-1.0.1/dash_express/preview_chart.py` & `dash_express-1.0.2/dash_express/preview_chart.py`

 * *Files identical despite different names*

### Comparing `dash_express-1.0.1/dash_express.egg-info/PKG-INFO` & `dash_express-1.0.2/dash_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-express
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool for faster application development Plotly Dash
 Home-page: https://github.com/stpnvkirill/dash-express
 Author: Kirill Stepanov
 Author-email: stpnv.kirill.o@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dash_express-1.0.1/setup.py` & `dash_express-1.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dash_express",
-    version="1.0.1",                        # Обновляйте это для каждой новой версии
+    version="1.0.2",                     
     author="Kirill Stepanov",
     author_email="stpnv.kirill.o@gmail.com",
     description="A tool for faster application development Plotly Dash",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[                      
         "dash>=2.11.1",
@@ -20,13 +20,13 @@
         "dash_iconify>=0.1.2",
         "dash_leaflet>=0.1.28",
         "flask_caching>=2.0.2",
         "dash_mantine_components>=0.12.1"                                        
     ],                                             
     url="https://github.com/stpnvkirill/dash-express",
     packages=setuptools.find_packages(),
-    classifiers=(                                 # Классификаторы помогают людям находить 
-        "Programming Language :: Python :: 3",    # ваши проекты. См. все возможные классификаторы 
-        "License :: OSI Approved :: MIT License", # на https://pypi.org/classifiers/
+    classifiers=(                                 
+        "Programming Language :: Python :: 3",    
+        "License :: OSI Approved :: MIT License", 
         "Operating System :: OS Independent",   
     ),
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

