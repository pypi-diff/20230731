# Comparing `tmp/adm-boundary-manager-0.0.3.tar.gz` & `tmp/adm-boundary-manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adm-boundary-manager-0.0.3.tar", last modified: Fri Jul  7 08:25:06 2023, max compression
+gzip compressed data, was "adm-boundary-manager-0.0.4.tar", last modified: Mon Jul 31 10:54:41 2023, max compression
```

## Comparing `adm-boundary-manager-0.0.3.tar` & `adm-boundary-manager-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:25:06.517403 adm-boundary-manager-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-07 08:25:06.517403 adm-boundary-manager-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:25:06.513403 adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-07 08:25:06.000000 adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-07 08:25:06.000000 adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:25:06.000000 adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 08:25:06.000000 adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 08:25:06.000000 adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:25:06.517403 adm-boundary-manager-0.0.3/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/boundary_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:25:06.517403 adm-boundary-manager-0.0.3/adminboundarymanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:25:06.513403 adm-boundary-manager-0.0.3/adminboundarymanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:25:06.517403 adm-boundary-manager-0.0.3/adminboundarymanager/templates/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/adminboundarymanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 08:24:44.000000 adm-boundary-manager-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 08:25:06.517403 adm-boundary-manager-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.494392 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 10:54:41.000000 adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.494392 adm-boundary-manager-0.0.4/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/boundary_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.494392 adm-boundary-manager-0.0.4/adminboundarymanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/adminboundarymanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 10:54:25.000000 adm-boundary-manager-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 10:54:41.498392 adm-boundary-manager-0.0.4/setup.cfg
```

### Comparing `adm-boundary-manager-0.0.3/PKG-INFO` & `adm-boundary-manager-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/PKG-INFO` & `adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `adm-boundary-manager-0.0.3/adm_boundary_manager.egg-info/SOURCES.txt` & `adm-boundary-manager-0.0.4/adm_boundary_manager.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 adminboundarymanager/urls.py
 adminboundarymanager/utils.py
 adminboundarymanager/views.py
 adminboundarymanager/wagtail_hooks.py
 adminboundarymanager/migrations/0001_initial.py
 adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
 adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
+adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
 adminboundarymanager/migrations/__init__.py
 adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
 adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
```

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/boundary_loader.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/boundary_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/countries.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/countries.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/errors.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/errors.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/forms.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/forms.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/migrations/0001_initial.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/models.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from django_countries.fields import CountryField
 from django_countries.widgets import CountrySelectWidget
 from modelcluster.fields import ParentalKey
 from modelcluster.models import ClusterableModel
-from shapely import geometry, unary_union
+from shapely import geometry, unary_union, Polygon
+from wagtail.admin.forms.models import (
+    WagtailAdminModelForm,
+)
 from wagtail.admin.panels import FieldPanel, InlinePanel
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 from wagtail.models import Orderable
 from wagtailcache.cache import clear_cache
 
 from adminboundarymanager.countries import get_country_info
@@ -80,26 +83,75 @@
             gid_1 = self.gid_1.split(".")[1].split("_")[0]
             gid_2 = self.gid_1.split(".")[1].split("_")[1]
             info.update({"id1": gid_1, "id2": gid_2, "name": self.name_2})
 
         return info
 
 
+class AdminBoundaryForm(WagtailAdminModelForm):
+    def is_valid(self):
+        form_is_valid = super().is_valid()
+
+        countries_formset = self.formsets.get("countries")
+        countries_cleaned_data = countries_formset.cleaned_data
+
+        countries = []
+        for country in countries_cleaned_data:
+            to_delete = country.get("DELETE")
+
+            if not to_delete:
+                country_obj = Country(country=country.get("country"))
+                countries.append(country_obj)
+
+        cleaned_data = self.cleaned_data
+        countries_must_share_boundaries = cleaned_data.get("countries_must_share_boundaries")
+
+        if countries_must_share_boundaries and len(countries) > 1:
+            bounds_polygons = []
+            for country in countries:
+                bounds_polygons.append(country.country_bounds_polygon)
+
+            union_polygon = bounds_polygons[0]
+            for polygon in bounds_polygons[1:]:
+                union_polygon = union_polygon.union(polygon)
+
+            connected = isinstance(union_polygon, Polygon)
+            if not connected:
+                error = _("One or more selected countries do not share boundaries. "
+                          "Please make sure all the countries are in one region and share boundaries")
+                # add error
+                self.formsets.get("countries")._non_form_errors.append(error)
+
+                return False
+
+        return form_is_valid
+
+
 @register_setting
 class AdminBoundarySettings(BaseSiteSetting, ClusterableModel):
+    base_form_class = AdminBoundaryForm
+
     DATA_SOURCE_CHOICES = (
         ("codabs", "OCHA Administrative Boundary Common Operational Datasets (COD-ABS)"),
         ("gadm41", "Global Administrative Areas 4.1 (GADM)")
     )
 
     data_source = models.CharField(max_length=100, choices=DATA_SOURCE_CHOICES, default="codabs",
                                    verbose_name=_("Boundary Data Source"), help_text="Source of the boundaries data")
+    countries_must_share_boundaries = models.BooleanField(default=True,
+                                                          verbose_name=_(
+                                                              "Countries must share boundaries - If more than one"),
+                                                          help_text=_(
+                                                              "Validation to ensure that the selected countries share "
+                                                              "boundaries with each other. Used if two or more "
+                                                              "countries are set."))
 
     panels = [
         FieldPanel("data_source"),
+        FieldPanel("countries_must_share_boundaries"),
         InlinePanel("countries", heading=_("Countries"), label=_("Country")),
     ]
 
     @cached_property
     def countries_list(self):
         countries = []
         for country in self.countries.all():
@@ -110,51 +162,53 @@
                 **country.country_info
             })
 
         return countries
 
     @cached_property
     def combined_countries_bounds(self):
-        polygons = []
+        bounds_polygons = self.get_country_bounds_polygons()
+        combined_polygon = unary_union(bounds_polygons)
+        return list(combined_polygon.bounds)
+
+    def get_country_bounds_polygons(self):
+        bounds_polygons = []
         for country in self.countries_list:
             if country.get("bbox"):
                 bbox = country.get("bbox")
                 polygon = geometry.box(*bbox, ccw=True)
-                polygons.append(polygon)
-
-        combined_polygon = unary_union(polygons)
-        return list(combined_polygon.bounds)
-
-    @cached_property
-    def boundary_search_url(self):
-        return reverse("admin_boundary_search")
-
-    @cached_property
-    def boundary_detail_url(self):
-        return reverse("admin_boundary_detail", args=(1,)).replace("/1", "")
+                bounds_polygons.append(polygon)
+        return bounds_polygons
 
     @cached_property
     def boundary_tiles_url(self):
         return reverse("admin_boundary_tiles", args=[0, 0, 0]).replace("/0/0/0", r"/{z}/{x}/{y}")
 
 
-class Countries(Orderable):
+class Country(Orderable):
     parent = ParentalKey(AdminBoundarySettings, on_delete=models.CASCADE, related_name='countries')
     country = CountryField(blank_label=_("Select Country"), verbose_name=_("country"))
 
     panels = [
         FieldPanel("country", widget=CountrySelectWidget()),
     ]
 
     @cached_property
     def country_info(self):
         country_info = get_country_info(self.country.alpha3)
         return country_info
 
     @cached_property
+    def country_bounds_polygon(self):
+        country_info = self.country_info
+        bbox = country_info.get("bbox")
+        polygon = geometry.box(*bbox, ccw=True)
+        return polygon
+
+    @cached_property
     def country_info_str(self):
         country_info = get_country_info(self.country.alpha3)
         if country_info:
             return json.dumps(country_info)
         return {}
```

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/serializers.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/serializers.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html` & `adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html` & `adm-boundary-manager-0.0.4/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/urls.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/urls.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/utils.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/utils.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/views.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/views.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/adminboundarymanager/wagtail_hooks.py` & `adm-boundary-manager-0.0.4/adminboundarymanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.0.3/setup.cfg` & `adm-boundary-manager-0.0.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = adm-boundary-manager
-version = 0.0.3
+version = 0.0.4
 description = Load, manage and visualize Administrative Boundaries Data in Wagtail
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/adm-boundary-manager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

