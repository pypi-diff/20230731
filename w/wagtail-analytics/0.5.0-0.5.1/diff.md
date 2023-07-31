# Comparing `tmp/wagtail-analytics-0.5.0.tar.gz` & `tmp/wagtail-analytics-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-analytics-0.5.0.tar", last modified: Fri Jun  2 08:23:19 2023, max compression
+gzip compressed data, was "wagtail-analytics-0.5.1.tar", last modified: Mon Jul 31 06:53:39 2023, max compression
```

## Comparing `wagtail-analytics-0.5.0.tar` & `wagtail-analytics-0.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.954166 wagtail-analytics-0.5.0/
--rw-r--r--   0 robmoorman   (501) staff       (20)      156 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      672 2023-06-02 08:23:19.953436 wagtail-analytics-0.5.0/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-06-02 08:23:19.954394 wagtail-analytics-0.5.0/setup.cfg
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.924188 wagtail-analytics-0.5.0/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.929609 wagtail-analytics-0.5.0/src/wagtail_analytics/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      298 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/forms.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.930307 wagtail-analytics-0.5.0/src/wagtail_analytics/lib/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/lib/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     7714 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/lib/analytics.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.930672 wagtail-analytics-0.5.0/src/wagtail_analytics/locales/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/locales/.gitkeep
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.935124 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/
--rw-r--r--   0 robmoorman   (501) staff       (20)     2484 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0001_initial.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      556 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      477 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0003_analyticssettings_plausible_enabled.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      520 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      383 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0005_remove_analyticssettings_google_analytics_view_id.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      612 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2878 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/models.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      505 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/settings.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.925610 wagtail-analytics-0.5.0/src/wagtail_analytics/static/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.946895 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/
--rw-r--r--   0 robmoorman   (501) staff       (20)   579244 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.js
--rw-r--r--   0 robmoorman   (501) staff       (20)   226227 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js
--rw-r--r--   0 robmoorman   (501) staff       (20)      811 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.css
--rw-r--r--   0 robmoorman   (501) staff       (20)   428366 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.js
--rw-r--r--   0 robmoorman   (501) staff       (20)      521 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.css
--rw-r--r--   0 robmoorman   (501) staff       (20)   172812 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.js
--rw-r--r--   0 robmoorman   (501) staff       (20)     1088 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/LICENSE.md
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.947445 wagtail-analytics-0.5.0/src/wagtail_analytics/static/moment/
--rwxr-xr-x   0 robmoorman   (501) staff       (20)    58824 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/moment/moment.min.js
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.949945 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/.gitkeep
--rw-r--r--   0 robmoorman   (501) staff       (20)       60 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/main.css
--rw-r--r--   0 robmoorman   (501) staff       (20)     2357 2023-03-15 15:11:00.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/main.js
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.925947 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.951737 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/
--rw-r--r--   0 robmoorman   (501) staff       (20)      462 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/body.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     2527 2023-03-15 15:10:05.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.952259 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1029 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html
--rw-r--r--   0 robmoorman   (501) staff       (20)     1439 2023-03-15 15:19:37.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/head.html
--rw-r--r--   0 robmoorman   (501) staff       (20)      416 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/types.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     4248 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/views.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2684 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.0/src/wagtail_analytics/wagtail_hooks.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-06-02 08:23:19.952847 wagtail-analytics-0.5.0/src/wagtail_analytics.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1708 2023-06-02 08:23:19.000000 wagtail-analytics-0.5.0/src/wagtail_analytics.egg-info/SOURCES.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.733230 wagtail-analytics-0.5.1/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      156 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      672 2023-07-31 06:53:39.732836 wagtail-analytics-0.5.1/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-07-31 06:53:39.733320 wagtail-analytics-0.5.1/setup.cfg
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.709162 wagtail-analytics-0.5.1/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.714184 wagtail-analytics-0.5.1/src/wagtail_analytics/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      298 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/forms.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.714909 wagtail-analytics-0.5.1/src/wagtail_analytics/lib/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/lib/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     7714 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/lib/analytics.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.715293 wagtail-analytics-0.5.1/src/wagtail_analytics/locales/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/locales/.gitkeep
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.719254 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2484 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0001_initial.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      556 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      477 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0003_analyticssettings_plausible_enabled.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      520 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      383 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0005_remove_analyticssettings_google_analytics_view_id.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      612 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2878 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      505 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/settings.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.710471 wagtail-analytics-0.5.1/src/wagtail_analytics/static/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.727997 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/
+-rw-r--r--   0 robmoorman   (501) staff       (20)   579244 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.bundle.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)   226227 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)      811 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.css
+-rw-r--r--   0 robmoorman   (501) staff       (20)   428366 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)      521 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.min.css
+-rw-r--r--   0 robmoorman   (501) staff       (20)   172812 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.min.js
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1088 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/LICENSE.md
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.728544 wagtail-analytics-0.5.1/src/wagtail_analytics/static/moment/
+-rwxr-xr-x   0 robmoorman   (501) staff       (20)    58824 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/moment/moment.min.js
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.730122 wagtail-analytics-0.5.1/src/wagtail_analytics/static/wagtailanalytics/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/wagtailanalytics/.gitkeep
+-rw-r--r--   0 robmoorman   (501) staff       (20)       60 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/wagtailanalytics/main.css
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2357 2023-03-15 15:11:00.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/static/wagtailanalytics/main.js
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.710914 wagtail-analytics-0.5.1/src/wagtail_analytics/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.731541 wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      462 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/body.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2527 2023-03-15 15:10:05.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.732025 wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1029 2023-02-24 13:01:45.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1439 2023-03-15 15:19:37.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/head.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)      416 2023-06-01 15:10:38.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/types.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     4248 2023-06-02 08:20:10.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/views.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     3025 2023-07-31 06:51:25.000000 wagtail-analytics-0.5.1/src/wagtail_analytics/wagtail_hooks.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-07-31 06:53:39.732420 wagtail-analytics-0.5.1/src/wagtail_analytics.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1708 2023-07-31 06:53:39.000000 wagtail-analytics-0.5.1/src/wagtail_analytics.egg-info/SOURCES.txt
```

### Comparing `wagtail-analytics-0.5.0/PKG-INFO` & `wagtail-analytics-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-analytics
-Version: 0.5.0
+Version: 0.5.1
 Author: Moori
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: Unix
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
 Classifier: Framework :: Wagtail :: 5
```

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/lib/analytics.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/lib/analytics.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0001_initial.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0002_analyticssettings_google_site_verification.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0004_analyticssettings_plausible_domain.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/migrations/0006_analyticssettings_google_analytics_measurement_id.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/models.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.js` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.css` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.css`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.js` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.css` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.min.css`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/Chart.min.js` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/chart.js/LICENSE.md` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/chart.js/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/moment/moment.min.js` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/static/wagtailanalytics/main.js` & `wagtail-analytics-0.5.1/src/wagtail_analytics/static/wagtailanalytics/main.js`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html` & `wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/dashboard.html`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html` & `wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/edit_handlers/sessions.html`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/templates/wagtail_analytics/head.html` & `wagtail-analytics-0.5.1/src/wagtail_analytics/templates/wagtail_analytics/head.html`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/views.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics/wagtail_hooks.py` & `wagtail-analytics-0.5.1/src/wagtail_analytics/wagtail_hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+from django.contrib.auth.models import Permission
 from django.templatetags.static import static
 from django.urls import include, path, re_path, reverse
 from django.utils.html import format_html, format_html_join
 from django.utils.translation import gettext_lazy as _
 from wagtail import hooks
 from wagtail.admin.menu import Menu, MenuItem, SubmenuMenuItem
 
 from wagtail_analytics import settings as wagtail_analytics_settings
 from wagtail_analytics import views
+from wagtail_analytics.models import AnalyticsSettings
 
 wagtail_analytics_menu = Menu(
     register_hook_name="register_wagtail_analytics_menu_item",
     construct_hook_name="construct_wagtail_analytics_menu",
 )
 
 
 class WagtailAnalyticsMenuItem(MenuItem):
     def is_shown(self, request):
-        # TODO: Fix permissions
-        return request.user.is_superuser
+        return request.user.has_perm("wagtail_analytics.view_analyticssettings")
+
+
+@hooks.register("register_permissions")
+def register_permissions():
+    app = "wagtail_analytics"
+    model = "analyticssettings"
+
+    return Permission.objects.filter(
+        content_type__app_label=app, codename__in=[f"view_{model}"]
+    )
 
 
 @hooks.register("register_admin_urls")
 def urlconf_analytics():
     return [
         path(
             "%s/" % wagtail_analytics_settings.PATH_PREFIX,
@@ -37,25 +48,25 @@
 
 
 @hooks.register("register_admin_menu_item")
 def register_menu():
     return SubmenuMenuItem(
         wagtail_analytics_settings.MENU_LABEL,
         wagtail_analytics_menu,
-        classnames="icon icon-fa-bar-chart",
+        classnames="icon icon-view",
         order=wagtail_analytics_settings.MENU_ORDER,
     )
 
 
 @hooks.register("register_wagtail_analytics_menu_item")
 def register_menu_item():
     return WagtailAnalyticsMenuItem(
         _("Dashboard"),
         reverse("wagtail-analytics-dashboard"),
-        classnames="icon icon-fa-tachometer",
+        classnames="icon icon-view",
         order=0,
     )
 
 
 @hooks.register("insert_editor_css")
 def insert_analytics_css():
     css_files = ["chart.js/Chart.min.css", "wagtailanalytics/main.css"]
```

### Comparing `wagtail-analytics-0.5.0/src/wagtail_analytics.egg-info/SOURCES.txt` & `wagtail-analytics-0.5.1/src/wagtail_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

