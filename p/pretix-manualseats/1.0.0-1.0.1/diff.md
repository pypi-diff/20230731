# Comparing `tmp/pretix-manualseats-1.0.0.tar.gz` & `tmp/pretix-manualseats-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-manualseats-1.0.0.tar", last modified: Mon Jul 31 00:02:53 2023, max compression
+gzip compressed data, was "pretix-manualseats-1.0.1.tar", last modified: Mon Jul 31 00:24:22 2023, max compression
```

## Comparing `pretix-manualseats-1.0.0.tar` & `pretix-manualseats-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.014366 pretix-manualseats-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 00:02:53.014366 pretix-manualseats-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.010365 pretix-manualseats-1.0.0/pretix_manualseats/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.006365 pretix-manualseats-1.0.0/pretix_manualseats/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.006365 pretix-manualseats-1.0.0/pretix_manualseats/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.010365 pretix-manualseats-1.0.0/pretix_manualseats/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.006365 pretix-manualseats-1.0.0/pretix_manualseats/locale/de_Informal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.010365 pretix-manualseats-1.0.0/pretix_manualseats/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.006365 pretix-manualseats-1.0.0/pretix_manualseats/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.010365 pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.010365 pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/icons/seat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/seating-edit.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.006365 pretix-manualseats-1.0.0/pretix_manualseats/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.006365 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.010365 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/event/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/event/import.html
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/event/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/event/mapping.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.014366 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/organizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/organizer/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/organizer/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pretix_manualseats/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.010365 pretix-manualseats-1.0.0/pretix_manualseats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 00:02:52.000000 pretix-manualseats-1.0.0/pretix_manualseats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-31 00:02:52.000000 pretix-manualseats-1.0.0/pretix_manualseats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:02:52.000000 pretix-manualseats-1.0.0/pretix_manualseats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 00:02:52.000000 pretix-manualseats-1.0.0/pretix_manualseats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 00:02:52.000000 pretix-manualseats-1.0.0/pretix_manualseats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 00:02:53.014366 pretix-manualseats-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:02:53.014366 pretix-manualseats-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 00:01:07.000000 pretix-manualseats-1.0.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/icons/seat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/seating-edit.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/import.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/mapping.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 00:24:22.770298 pretix-manualseats-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/tests/test_main.py
```

### Comparing `pretix-manualseats-1.0.0/LICENSE` & `pretix-manualseats-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/PKG-INFO` & `pretix-manualseats-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-manualseats
-Version: 1.0.0
+Version: 1.0.1
 Summary: Manually assign tickets to seats.
 Author-email: Moritz Lerch <dev@moritz-lerch.de>
 Maintainer-email: Moritz Lerch <dev@moritz-lerch.de>
 License: Apache
 Project-URL: homepage, https://github.com/moritzlerch/pretix-manualseats
 Project-URL: repository, https://github.com/moritzlerch/pretix-manualseats
 Keywords: pretix
```

### Comparing `pretix-manualseats-1.0.0/README.rst` & `pretix-manualseats-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/apps.py` & `pretix-manualseats-1.0.1/pretix_manualseats/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/locale/de/LC_MESSAGES/django.po` & `pretix-manualseats-1.0.1/pretix_manualseats/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/signals.py` & `pretix-manualseats-1.0.1/pretix_manualseats/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js` & `pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/icons/seat.svg` & `pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/icons/seat.svg`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/static/pretix_manualseats/seating-edit.js` & `pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/seating-edit.js`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/event/import.html` & `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/import.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/event/index.html` & `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/index.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/event/mapping.html` & `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/mapping.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html` & `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/organizer/form.html` & `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/form.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/templates/pretix_manualseats/organizer/index.html` & `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/index.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/urls.py` & `pretix-manualseats-1.0.1/pretix_manualseats/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats/views.py` & `pretix-manualseats-1.0.1/pretix_manualseats/views.py`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats.egg-info/PKG-INFO` & `pretix-manualseats-1.0.1/pretix_manualseats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-manualseats
-Version: 1.0.0
+Version: 1.0.1
 Summary: Manually assign tickets to seats.
 Author-email: Moritz Lerch <dev@moritz-lerch.de>
 Maintainer-email: Moritz Lerch <dev@moritz-lerch.de>
 License: Apache
 Project-URL: homepage, https://github.com/moritzlerch/pretix-manualseats
 Project-URL: repository, https://github.com/moritzlerch/pretix-manualseats
 Keywords: pretix
```

### Comparing `pretix-manualseats-1.0.0/pretix_manualseats.egg-info/SOURCES.txt` & `pretix-manualseats-1.0.1/pretix_manualseats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/pyproject.toml` & `pretix-manualseats-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.0/setup.cfg` & `pretix-manualseats-1.0.1/setup.cfg`

 * *Files identical despite different names*

