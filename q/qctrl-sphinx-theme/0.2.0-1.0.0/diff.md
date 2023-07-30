# Comparing `tmp/qctrl_sphinx_theme-0.2.0.tar.gz` & `tmp/qctrl_sphinx_theme-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_sphinx_theme-0.2.0.tar", max compression
+gzip compressed data, was "qctrl_sphinx_theme-1.0.0.tar", max compression
```

## Comparing `qctrl_sphinx_theme-0.2.0.tar` & `qctrl_sphinx_theme-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    36653 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/LICENSE
--rw-r--r--   0        0        0      710 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/README.md
--rw-r--r--   0        0        0     2175 2023-05-24 04:57:13.025274 qctrl_sphinx_theme-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      887 2023-05-24 04:57:13.033274 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/__init__.py
--rw-r--r--   0        0        0      467 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/breadcrumbs.html
--rw-r--r--   0        0        0        0 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/footer.html
--rw-r--r--   0        0        0     3084 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/layout.html
--rw-r--r--   0        0        0     1749 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/search.html
--rw-r--r--   0        0        0      359 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/searchbox.html
--rw-r--r--   0        0        0     8557 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css
--rw-r--r--   0        0        0     5430 2023-05-24 04:56:53.808957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/favicon.ico
--rw-r--r--   0        0        0    26880 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png
--rw-r--r--   0        0        0    29759 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png
--rw-r--r--   0        0        0   122791 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png
--rw-r--r--   0        0        0     9545 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg
--rw-r--r--   0        0        0    10694 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg
--rw-r--r--   0        0        0   317604 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/social/image.jpg
--rw-r--r--   0        0        0     1194 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t
--rw-r--r--   0        0        0      609 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/manifest.webmanifest
--rw-r--r--   0        0        0     1985 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/pygments.css
--rw-r--r--   0        0        0      118 2023-05-24 04:56:53.812957 qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/theme.conf
--rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 qctrl_sphinx_theme-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-30 22:36:01.884897 qctrl_sphinx_theme-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1061 2023-07-30 22:36:01.884897 qctrl_sphinx_theme-1.0.0/README.md
+-rw-r--r--   0        0        0     2175 2023-07-30 22:36:23.373118 qctrl_sphinx_theme-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1370 2023-07-30 22:36:23.381118 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/__init__.py
+-rw-r--r--   0        0        0      467 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/breadcrumbs.html
+-rw-r--r--   0        0        0        0 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/footer.html
+-rw-r--r--   0        0        0     3347 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/layout.html
+-rw-r--r--   0        0        0       78 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/searchbox.html
+-rw-r--r--   0        0        0    17409 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/css/docsearch.css
+-rw-r--r--   0        0        0     8860 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css
+-rw-r--r--   0        0        0     5430 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/favicon.ico
+-rw-r--r--   0        0        0    26880 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png
+-rw-r--r--   0        0        0    29759 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png
+-rw-r--r--   0        0        0   122791 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png
+-rw-r--r--   0        0        0     9545 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg
+-rw-r--r--   0        0        0    10694 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg
+-rw-r--r--   0        0        0   317604 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/social/image.jpg
+-rw-r--r--   0        0        0     3209 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/js/qctrlsphinxtheme.js_t
+-rw-r--r--   0        0        0      609 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/manifest.webmanifest
+-rw-r--r--   0        0        0     1985 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/pygments.css
+-rw-r--r--   0        0        0      251 2023-07-30 22:36:01.888897 qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/theme.conf
+-rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 qctrl_sphinx_theme-1.0.0/PKG-INFO
```

### Comparing `qctrl_sphinx_theme-0.2.0/LICENSE` & `qctrl_sphinx_theme-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/README.md` & `qctrl_sphinx_theme-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 ```shell
 pip install qctrl-sphinx-theme
 ```
 
 ## Usage
 
 1. Add `qctrl-sphinx-theme` as a dev dependency in `pyproject.toml`.
-2. Set the `html_theme` config value in `docs/conf.py`.
+```toml
+[tool.poetry.dev-dependencies]
+qctrl-sphinx-theme = "~1.0.0"
+```
+1. Add the following to `docs/conf.py` (this sets the Q-CTRL Sphinx Theme as the theme for your documentation):
   ```python
   html_theme = "qctrl_sphinx_theme"
   ```
-3. Set the `html_theme_options` config value in `docs/conf.py`.
+1. Update (or create) the `html_theme_options` dictionary in `docs/conf.py` using `qctrlsphinxtheme.get_environment_options` (this checks each DocSearch and Segment theme option for an available environment variable and, if one exists, sets it). For example:
   ```python
-  html_theme_options = {
-      "segment_write_key": "<YOUR_SEGMENT_WRITE_KEY>"
-  }
+  from qctrlsphinxtheme import get_environment_options
+  html_theme_options.update(get_environment_options())
   ```
```

### Comparing `qctrl_sphinx_theme-0.2.0/pyproject.toml` & `qctrl_sphinx_theme-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-sphinx-theme"
-version = "0.2.0"
+version = "1.0.0"
 description = "Q-CTRL Sphinx Theme"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
```

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/__init__.py` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,35 @@
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 """Q-CTRL Sphinx Theme"""
-from os import path
+import os
 
-__version__ = "0.2.0"
+__version__ = "1.0.0"
 __author__ = "Q-CTRL <support@q-ctrl.com>"
 
 # See https://www.sphinx-doc.org/en/master/development/theming.html#distribute-your-theme-as-a-python-package
 def setup(app):
     app.add_html_theme(
-        "qctrl_sphinx_theme", path.abspath(path.dirname(__file__))
+        "qctrl_sphinx_theme", os.path.abspath(os.path.dirname(__file__))
     )
+
+def get_environment_options():
+    """
+    Check each DocSearch and Segment theme option for an available
+    environment variable and, if one exists, set it.
+    """
+    variables = [
+        "DOCSEARCH_API_KEY",
+        "DOCSEARCH_APP_ID",
+        "DOCSEARCH_INDEX_NAME",
+        "SEGMENT_WRITE_KEY",
+    ]
+    options = {}
+    for variable in variables:
+        value = os.getenv(variable, "")
+        if value != "":
+            options[variable.lower()] = value
+    return options
```

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/layout.html` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/layout.html`

 * *Files 10% similar despite different names*

```diff
@@ -40,19 +40,21 @@
   <meta property="og:url" content="{{- url -}}">
   <meta property="og:image" content="{{- image -}}">
   <meta property="og:image:type" content="image/jpeg">
   <meta property="og:image:width" content="1200">
   <meta property="og:image:height" content="630">
   <meta property="og:image:alt" content="{{- description -}}">
   <meta property="og:locale" content="en_US">
+  <link rel="preconnect" href="https://{{- theme_docsearch_app_id -}}-dsn.algolia.net" crossOrigin="anonymous">
   <link rel="icon" href="{{- pathto('_static/favicon.ico', 1) -}}">
   <link rel="icon" type="image/svg+xml" href="{{- pathto('_static/img/q-ctrl-icon.svg', 1) -}}">
   <link rel="apple-touch-icon" href="{{- pathto('_static/img/q-ctrl-icon-180.png', 1) -}}">
   <link rel="manifest" href="{{- pathto('_static/manifest.webmanifest', 1) -}}">
   <link rel="stylesheet" href="{{- pathto('_static/css/qctrlsphinxtheme.css', 1) -}}">
+  <link rel="stylesheet" href="{{- pathto('_static/css/docsearch.css', 1) -}}">
 {% endblock %}
 
 {%- block sidebartitle %}
   <a href="{{- pathto(master_doc) -}}">
     <img src="{{- pathto('_static/img/q-ctrl-logo.svg', 1) -}}" alt="{{- project -}}" width="184" height="45">
   </a>
   {% include 'searchbox.html' %}
@@ -68,9 +70,10 @@
 {% block document %}
   <article class="DocSearch-content">
     {{ super() }}
   </article>
 {% endblock %}
 
 {% block footer %}
+  <script src="https://cdn.jsdelivr.net/npm/@docsearch/js@3"></script>
   <script src="{{- pathto('_static/js/qctrlsphinxtheme.js', 1) -}}"></script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -29,12 +29,14 @@
 
 
 
 
 
 
 
+
+
  {% endblock %} {%- block sidebartitle %} [{{-_project_-}}] {% include
 'searchbox.html' %} {% endblock %} {%- block mobile_nav %}  [{{-_project_-}}]
 {%- endblock %} {% block document %}  {{ super() }}  {% endblock %} {% block
 footer %}
  {% endblock %}
```

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/css/qctrlsphinxtheme.css`

 * *Files 3% similar despite different names*

```diff
@@ -440,7 +440,12 @@
 
 .rst-content .highlighted {
   background: #fff3cd;
   box-shadow: 0 0 0 2px #fff3cd;
   display: inline;
   font-weight: inherit;
 }
+
+input[type=color], input[type=date], input[type=datetime-local], input[type=datetime], input[type=email], input[type=month], input[type=number], input[type=password], input[type=search], input[type=tel], input[type=text], input[type=time], input[type=url], input[type=week]
+{
+  font-family: inherit;
+}
```

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/favicon.ico` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-180.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-192.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon-512.png`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-icon.svg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/q-ctrl-logo.svg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/img/social/image.jpg` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/img/social/image.jpg`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/manifest.webmanifest` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/qctrlsphinxtheme/static/pygments.css` & `qctrl_sphinx_theme-1.0.0/qctrlsphinxtheme/static/pygments.css`

 * *Files identical despite different names*

### Comparing `qctrl_sphinx_theme-0.2.0/PKG-INFO` & `qctrl_sphinx_theme-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-sphinx-theme
-Version: 0.2.0
+Version: 1.0.0
 Summary: Q-CTRL Sphinx Theme
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -50,18 +50,21 @@
 ```shell
 pip install qctrl-sphinx-theme
 ```
 
 ## Usage
 
 1. Add `qctrl-sphinx-theme` as a dev dependency in `pyproject.toml`.
-2. Set the `html_theme` config value in `docs/conf.py`.
+```toml
+[tool.poetry.dev-dependencies]
+qctrl-sphinx-theme = "~1.0.0"
+```
+1. Add the following to `docs/conf.py` (this sets the Q-CTRL Sphinx Theme as the theme for your documentation):
   ```python
   html_theme = "qctrl_sphinx_theme"
   ```
-3. Set the `html_theme_options` config value in `docs/conf.py`.
+1. Update (or create) the `html_theme_options` dictionary in `docs/conf.py` using `qctrlsphinxtheme.get_environment_options` (this checks each DocSearch and Segment theme option for an available environment variable and, if one exists, sets it). For example:
   ```python
-  html_theme_options = {
-      "segment_write_key": "<YOUR_SEGMENT_WRITE_KEY>"
-  }
+  from qctrlsphinxtheme import get_environment_options
+  html_theme_options.update(get_environment_options())
   ```
```

