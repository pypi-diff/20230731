# Comparing `tmp/django-pygwalker-0.0.0.dev0.tar.gz` & `tmp/django-pygwalker-0.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pygwalker-0.0.0.dev0.tar", last modified: Sat Jul 29 23:55:52 2023, max compression
+gzip compressed data, was "django-pygwalker-0.0.0.dev1.tar", last modified: Mon Jul 31 00:04:04 2023, max compression
```

## Comparing `django-pygwalker-0.0.0.dev0.tar` & `django-pygwalker-0.0.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.520645 django-pygwalker-0.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44786 2023-07-29 23:55:52.520645 django-pygwalker-0.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 23:55:52.520645 django-pygwalker-0.0.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.516645 django-pygwalker-0.0.0.dev0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-29 23:55:52.000000 django-pygwalker-0.0.0.dev0/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.520645 django-pygwalker-0.0.0.dev0/src/django_pygwalker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44786 2023-07-29 23:55:52.000000 django-pygwalker-0.0.0.dev0/src/django_pygwalker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-29 23:55:52.000000 django-pygwalker-0.0.0.dev0/src/django_pygwalker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 23:55:52.000000 django-pygwalker-0.0.0.dev0/src/django_pygwalker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-29 23:55:52.000000 django-pygwalker-0.0.0.dev0/src/django_pygwalker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-29 23:55:52.000000 django-pygwalker-0.0.0.dev0/src/django_pygwalker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.520645 django-pygwalker-0.0.0.dev0/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.520645 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.512645 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.512645 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/templates/pygwalker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 23:55:52.520645 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pyg.html
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-29 23:55:34.000000 django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46857 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46857 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 00:04:04.000000 django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.347088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:04:04.351088 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-31 00:03:44.000000 django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/views.py
```

### Comparing `django-pygwalker-0.0.0.dev0/LICENSE` & `django-pygwalker-0.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.0.dev0/PKG-INFO` & `django-pygwalker-0.0.0.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.0.dev0
+Version: 0.0.0.dev1
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -698,22 +698,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
-[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7516/badge)](https://bestpractices.coreinfrastructure.org/projects/7516)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Django pygwalker is a utility used to create user interfaces for visual analysis, based on PyGWalker , from django querysets. 
+Turn your Django querysets into a user interfaces for visual analysis with PyGWalker.
+
+This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
+
 <br/>
 
 ## Code Quality
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/djangoaddicts/django-pygwalker/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/djangoaddicts/django-pygwalker/actions/workflows/black.yaml/badge.svg)|
@@ -728,14 +731,15 @@
 
 ### Code Coverage 
 [![Coverage Status](https://coveralls.io/repos/github/djangoaddicts/django-pygwalker/badge.svg)](https://coveralls.io/github/djangoaddicts/django-pygwalker)
 
 Dashboard:
 https://coveralls.io/github/djangoaddicts/django-pygwalker
 
+
 <br/>
 
 ## Documentation
 [![Documentation Status](https://readthedocs.org/projects/django-pygwalker/badge/?version=latest)](https://django-pygwalker.readthedocs.io/en/latest/?badge=latest)
 
 Full documentation can be found on http://django-pygwalker.readthedocs.org. 
 
@@ -749,17 +753,69 @@
 
 https://github.com/djangoaddicts/django-pygwalker/blob/main/LICENSE
 
 
 <br/>
 
 ## Installation 
+- install via pip:
+    ``` 
+    pip install django-pygwalker
+    ```
+- add the following to your INSTALLED_APPS in settings.py:
+
+    ```python 
+    djangoaddicts.pygwalker
+    ```
 
+    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
 
 <br/>
 
 ## Features
 
+### PygWalkerView
+The PygWalkerView view renders a page containing PyGWalker html. This view takes a queryset parameter and included all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
+
+A Bootstrap 5 template is included, but can be overwritten using the template_name parameter. 
+
+#### Parameters
+- **field_list:** list of model fields to include (defaults to fields defined in the model)
+- **queryset:** queryset providing data available to visualization
+- **theme:** PyGWalker theme to use for pyg html (defaults to "media")
+- **title:** title used on html render
+- **template_name:** template used when rendering page; (defaults to pygwalker/bs5/pygwalker.html)
 
 <br/>
 
-## Usage Example
+## Usage Examples
+
+```python
+from djangoaddicts.pygwalker.views import PygWalkerView
+
+class MyPygWalkerView(PygWalkerView):
+    queryset = MyModel.objects.all()
+```
+
+#### Explicitly Defined Fields
+
+```python
+from djangoaddicts.pygwalker.views import PygWalkerView
+
+class MyPygWalkerView(PygWalkerView):
+    queryset = MyModel.objects.all()
+    title = "MyModel Data Analysis"
+    theme = "light"
+    field_list = ["name", "some_field", "some_other__related_field", "id", "created_at", "updated_at"]
+```
+
+
+#### Custom Template
+Custom views/templates can be used to override the Bootstrap 5 templates provided by default view. Here is an example:
+
+```python
+from djangoaddicts.pygwalker.views import PygWalkerView
+
+class MyPygWalkerView(PygWalkerView):
+    queryset = MyModel.objects.all()
+    template_name = "my_custom_template.html"
+```
```

### Comparing `django-pygwalker-0.0.0.dev0/pyproject.toml` & `django-pygwalker-0.0.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.0.dev0/src/django_pygwalker.egg-info/PKG-INFO` & `django-pygwalker-0.0.0.dev1/src/django_pygwalker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.0.dev0
+Version: 0.0.0.dev1
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -698,22 +698,25 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
-[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7516/badge)](https://bestpractices.coreinfrastructure.org/projects/7516)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Django pygwalker is a utility used to create user interfaces for visual analysis, based on PyGWalker , from django querysets. 
+Turn your Django querysets into a user interfaces for visual analysis with PyGWalker.
+
+This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
+
 <br/>
 
 ## Code Quality
 | Workflow | Description             | Status                                                                       |
 |----------|-------------------------|------------------------------------------------------------------------------|
 |Bandit|security checks|![Bandit](https://github.com/djangoaddicts/django-pygwalker/actions/workflows/bandit.yaml/badge.svg)|
 |Black|code formatting|![Black](https://github.com/djangoaddicts/django-pygwalker/actions/workflows/black.yaml/badge.svg)|
@@ -728,14 +731,15 @@
 
 ### Code Coverage 
 [![Coverage Status](https://coveralls.io/repos/github/djangoaddicts/django-pygwalker/badge.svg)](https://coveralls.io/github/djangoaddicts/django-pygwalker)
 
 Dashboard:
 https://coveralls.io/github/djangoaddicts/django-pygwalker
 
+
 <br/>
 
 ## Documentation
 [![Documentation Status](https://readthedocs.org/projects/django-pygwalker/badge/?version=latest)](https://django-pygwalker.readthedocs.io/en/latest/?badge=latest)
 
 Full documentation can be found on http://django-pygwalker.readthedocs.org. 
 
@@ -749,17 +753,69 @@
 
 https://github.com/djangoaddicts/django-pygwalker/blob/main/LICENSE
 
 
 <br/>
 
 ## Installation 
+- install via pip:
+    ``` 
+    pip install django-pygwalker
+    ```
+- add the following to your INSTALLED_APPS in settings.py:
+
+    ```python 
+    djangoaddicts.pygwalker
+    ```
 
+    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
 
 <br/>
 
 ## Features
 
+### PygWalkerView
+The PygWalkerView view renders a page containing PyGWalker html. This view takes a queryset parameter and included all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.  
+
+A Bootstrap 5 template is included, but can be overwritten using the template_name parameter. 
+
+#### Parameters
+- **field_list:** list of model fields to include (defaults to fields defined in the model)
+- **queryset:** queryset providing data available to visualization
+- **theme:** PyGWalker theme to use for pyg html (defaults to "media")
+- **title:** title used on html render
+- **template_name:** template used when rendering page; (defaults to pygwalker/bs5/pygwalker.html)
 
 <br/>
 
-## Usage Example
+## Usage Examples
+
+```python
+from djangoaddicts.pygwalker.views import PygWalkerView
+
+class MyPygWalkerView(PygWalkerView):
+    queryset = MyModel.objects.all()
+```
+
+#### Explicitly Defined Fields
+
+```python
+from djangoaddicts.pygwalker.views import PygWalkerView
+
+class MyPygWalkerView(PygWalkerView):
+    queryset = MyModel.objects.all()
+    title = "MyModel Data Analysis"
+    theme = "light"
+    field_list = ["name", "some_field", "some_other__related_field", "id", "created_at", "updated_at"]
+```
+
+
+#### Custom Template
+Custom views/templates can be used to override the Bootstrap 5 templates provided by default view. Here is an example:
+
+```python
+from djangoaddicts.pygwalker.views import PygWalkerView
+
+class MyPygWalkerView(PygWalkerView):
+    queryset = MyModel.objects.all()
+    template_name = "my_custom_template.html"
+```
```

### Comparing `django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pyg.html` & `django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.0.dev0/src/djangoaddicts/pygwalker/views.py` & `django-pygwalker-0.0.0.dev1/src/djangoaddicts/pygwalker/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import pandas as pd
 import pygwalker as pyg
+from django.db.models import QuerySet
 from django.shortcuts import render
 from django.views.generic import View
 
 
-class PygView(View):
+class PygWalkerView(View):
     """View to create a PyGWalker visualization interface from a Django queryset.
     See https://github.com/Kanaries/pygwalker for more information on PyGWalker.
 
     class parameters:
-        field_list    - list of model fields to include
+        field_list    - list of model fields to include (defaults to fields defined in the model)
         queryset      - queryset providing data available to visualization
         theme         - PyGWalker theme to use for pyg html (defaults to "media")
         title         - title used on html render
         template_name - template used when rendering page; defaults to: pygwalker/bs5/pyg.html
 
     example:
 
-        from djangoaddicts.pygwalker.views import PygView
-        class MyPygView(PygView):
+        from djangoaddicts.pygwalker.views import PygWalkerView
+        class MyPygView(PygWalkerView):
             queryset = Order.objects.all()
             title = "Order Data Analysis"
             theme = "light"
             field_list = ["status__name", "customer", "order_id", "created_at", "updated_at", "products"]
     """
-
     field_list: list = []
-    queryset = None
-    template_name: str = "storemgr/pyg/pyg.html"
+    queryset: QuerySet = None
+    template_name: str = "pygwalker/bs5/pygwalker.html"
     theme: str = "media"
     title: str = "Data Analysis"
 
     def get(self, request):
         pd_data = pd.DataFrame(list(self.queryset.values(*self.field_list)))
         context = {"pyg": pyg.walk(pd_data, return_html=True, dark=self.theme), "title": self.title}
         return render(request, self.template_name, context)
```

