# Comparing `tmp/django_custom_admin_pages-0.2.1.tar.gz` & `tmp/django_custom_admin_pages-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_custom_admin_pages-0.2.1.tar", max compression
+gzip compressed data, was "django_custom_admin_pages-0.2.2.tar", max compression
```

## Comparing `django_custom_admin_pages-0.2.1.tar` & `django_custom_admin_pages-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1496 2023-07-29 15:36:01.096792 django_custom_admin_pages-0.2.1/LICENSE
--rw-r--r--   0        0        0     5526 2023-07-30 22:20:48.373159 django_custom_admin_pages-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.1/django_custom_admin_pages/__init__.py
--rw-r--r--   0        0        0     5638 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.1/django_custom_admin_pages/admin.py
--rw-r--r--   0        0        0      482 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.1/django_custom_admin_pages/apps.py
--rw-r--r--   0        0        0       61 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.1/django_custom_admin_pages/default_settings.py
--rw-r--r--   0        0        0      344 2023-07-30 22:17:55.133161 django_custom_admin_pages-0.2.1/django_custom_admin_pages/templates/base_custom_admin.html
--rw-r--r--   0        0        0      777 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.1/django_custom_admin_pages/urls.py
--rw-r--r--   0        0        0       43 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.1/django_custom_admin_pages/views/__init__.py
--rw-r--r--   0        0        0     2408 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.1/django_custom_admin_pages/views/admin_base_view.py
--rw-r--r--   0        0        0     1718 2023-07-30 22:29:41.463153 django_custom_admin_pages-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6608 1970-01-01 00:00:00.000000 django_custom_admin_pages-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-07-29 15:36:01.096792 django_custom_admin_pages-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5627 2023-07-30 23:40:04.183108 django_custom_admin_pages-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/__init__.py
+-rw-r--r--   0        0        0     5638 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/admin.py
+-rw-r--r--   0        0        0      482 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/apps.py
+-rw-r--r--   0        0        0       61 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/default_settings.py
+-rw-r--r--   0        0        0      344 2023-07-30 22:17:55.133161 django_custom_admin_pages-0.2.2/django_custom_admin_pages/templates/base_custom_admin.html
+-rw-r--r--   0        0        0      777 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/urls.py
+-rw-r--r--   0        0        0       43 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/views/__init__.py
+-rw-r--r--   0        0        0     2408 2023-07-30 21:00:31.363211 django_custom_admin_pages-0.2.2/django_custom_admin_pages/views/admin_base_view.py
+-rw-r--r--   0        0        0     1921 2023-07-30 23:38:34.063109 django_custom_admin_pages-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6932 1970-01-01 00:00:00.000000 django_custom_admin_pages-0.2.2/PKG-INFO
```

### Comparing `django_custom_admin_pages-0.2.1/LICENSE` & `django_custom_admin_pages-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.1/README.md` & `django_custom_admin_pages-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Django Custom Admin Pages
-This app is in the process from being ported from an existing project into an installable app. 
+A django app that lets you add standard class-based views to the django admin index and navigation. Create a view, register it like you would a ModelAdmin, and it appears in the Django Admin Nav.
 
-_This app is currently in beta and only tested in django 3.2 / python 3.10_
 
 ## Installation
 
 1. Install the app from pypi `pip install django_custom_admin_pages`
 2. Remove `django.contrib.admin` from your installed apps
 3. In your django settings file add the following lines to your `INSTALLED_APPS``:
 
@@ -22,14 +21,16 @@
 
 ```python
 from django_custom_admin_pages.admin import CustomAdminConfig
 class MyCustomAdminSite(CustomAdminConfig):
    pass
 ```
 
+_This app is currently in beta and only tested in django 3.2 / python 3.10_
+
 
 ## Usage
 
 This app is for custom admin views which aren't associated with a specific model. Add dashboards and other custom admin views here.
 
 To create a new custom admin view:
```

### Comparing `django_custom_admin_pages-0.2.1/django_custom_admin_pages/admin.py` & `django_custom_admin_pages-0.2.2/django_custom_admin_pages/admin.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.1/django_custom_admin_pages/urls.py` & `django_custom_admin_pages-0.2.2/django_custom_admin_pages/urls.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.1/django_custom_admin_pages/views/admin_base_view.py` & `django_custom_admin_pages-0.2.2/django_custom_admin_pages/views/admin_base_view.py`

 * *Files identical despite different names*

### Comparing `django_custom_admin_pages-0.2.1/pyproject.toml` & `django_custom_admin_pages-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 name = "django-custom-admin-pages"
-version = "0.2.1"
+version = "0.2.2"
 description = "A django app that lets you add standard class-based views to the django admin index and navigation."
 authors = ["lekjos"]
 license = "BSD"
 readme = "README.md"
 homepage = "https://github.com/lekjos/django-custom-admin-pages"
 repository = "https://github.com/lekjos/django-custom-admin-pages"
 keywords = ["django", "django-admin", "django admin"]
 classifiers = [
     "Environment :: Web Environment",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Framework :: Django :: 3.2", 
     "Topic :: Software Development :: Libraries :: Python Modules", 
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 include = [
     "LICENSE.md",
 ]
 exclude = [
     "django_custom_admin_pages/boot_django.py",
     "django_custom_admin_pages/conftest.py",
```

### Comparing `django_custom_admin_pages-0.2.1/PKG-INFO` & `django_custom_admin_pages-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: django-custom-admin-pages
-Version: 0.2.1
+Version: 0.2.2
 Summary: A django app that lets you add standard class-based views to the django admin index and navigation.
 Home-page: https://github.com/lekjos/django-custom-admin-pages
 License: BSD
 Keywords: django,django-admin,django admin
 Author: lekjos
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/lekjos/django-custom-admin-pages
 Description-Content-Type: text/markdown
 
 # Django Custom Admin Pages
-This app is in the process from being ported from an existing project into an installable app. 
+A django app that lets you add standard class-based views to the django admin index and navigation. Create a view, register it like you would a ModelAdmin, and it appears in the Django Admin Nav.
 
-_This app is currently in beta and only tested in django 3.2 / python 3.10_
 
 ## Installation
 
 1. Install the app from pypi `pip install django_custom_admin_pages`
 2. Remove `django.contrib.admin` from your installed apps
 3. In your django settings file add the following lines to your `INSTALLED_APPS``:
 
@@ -47,14 +50,16 @@
 
 ```python
 from django_custom_admin_pages.admin import CustomAdminConfig
 class MyCustomAdminSite(CustomAdminConfig):
    pass
 ```
 
+_This app is currently in beta and only tested in django 3.2 / python 3.10_
+
 
 ## Usage
 
 This app is for custom admin views which aren't associated with a specific model. Add dashboards and other custom admin views here.
 
 To create a new custom admin view:
```

