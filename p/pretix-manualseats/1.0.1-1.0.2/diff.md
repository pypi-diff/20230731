# Comparing `tmp/pretix-manualseats-1.0.1.tar.gz` & `tmp/pretix-manualseats-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-manualseats-1.0.1.tar", last modified: Mon Jul 31 00:24:22 2023, max compression
+gzip compressed data, was "pretix-manualseats-1.0.2.tar", last modified: Mon Jul 31 09:41:15 2023, max compression
```

## Comparing `pretix-manualseats-1.0.1.tar` & `pretix-manualseats-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/icons/seat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/seating-edit.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.762298 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/import.html
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/mapping.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pretix_manualseats/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 00:24:22.000000 pretix-manualseats-1.0.1/pretix_manualseats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 00:24:22.770298 pretix-manualseats-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:24:22.766298 pretix-manualseats-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 00:21:40.000000 pretix-manualseats-1.0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.701289 pretix-manualseats-1.0.2/pretix_manualseats/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.701289 pretix-manualseats-1.0.2/pretix_manualseats/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.701289 pretix-manualseats-1.0.2/pretix_manualseats/locale/de_Informal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.701289 pretix-manualseats-1.0.2/pretix_manualseats/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/icons/seat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/seating-edit.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.701289 pretix-manualseats-1.0.2/pretix_manualseats/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.701289 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/event/assign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/event/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/event/mapping.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/organizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/organizer/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/organizer/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pretix_manualseats/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/pretix_manualseats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 09:41:15.000000 pretix-manualseats-1.0.2/pretix_manualseats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-31 09:41:15.000000 pretix-manualseats-1.0.2/pretix_manualseats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:41:15.000000 pretix-manualseats-1.0.2/pretix_manualseats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 09:41:15.000000 pretix-manualseats-1.0.2/pretix_manualseats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 09:41:15.000000 pretix-manualseats-1.0.2/pretix_manualseats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:15.705289 pretix-manualseats-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 09:39:31.000000 pretix-manualseats-1.0.2/tests/test_main.py
```

### Comparing `pretix-manualseats-1.0.1/LICENSE` & `pretix-manualseats-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/PKG-INFO` & `pretix-manualseats-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-manualseats
-Version: 1.0.1
+Version: 1.0.2
 Summary: Manually assign tickets to seats.
 Author-email: Moritz Lerch <dev@moritz-lerch.de>
 Maintainer-email: Moritz Lerch <dev@moritz-lerch.de>
 License: Apache
 Project-URL: homepage, https://github.com/moritzlerch/pretix-manualseats
 Project-URL: repository, https://github.com/moritzlerch/pretix-manualseats
 Keywords: pretix
```

### Comparing `pretix-manualseats-1.0.1/README.rst` & `pretix-manualseats-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/apps.py` & `pretix-manualseats-1.0.2/pretix_manualseats/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/locale/de/LC_MESSAGES/django.po` & `pretix-manualseats-1.0.2/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 19:45+0200\n"
+"POT-Creation-Date: 2023-07-31 10:33+0200\n"
 "PO-Revision-Date: \n"
 "Last-Translator: Moritz Lerch\n"
 "Language-Team: \n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_manualseats/apps.py:12 pretix_manualseats/signals.py:19
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:7
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:9
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:9
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:7
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:9
-#: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:7
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:9
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:9
 msgid "Manual Seats"
 msgstr "Manuelle Sitzplätze"
 
 #: pretix_manualseats/apps.py:14
 msgid "Manually assign tickets to seats."
 msgstr "Tickets manuell Sitzplätzen zuweisen."
 
 #: pretix_manualseats/signals.py:31
-msgid "Seating Mapping"
-msgstr "Sitzplatz-Zuordnung"
+#: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:7
+msgid "Category Mapping"
+msgstr "Kategorie-Zuordnung"
 
 #: pretix_manualseats/signals.py:43
-msgid "Seating Importer"
-msgstr "Sitzplatz-Import"
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:7
+msgid "Seat Assignment"
+msgstr "Sitzplatz-Zuweisung"
 
 #: pretix_manualseats/signals.py:70
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:6
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:9
 msgid "Seating Plans"
 msgstr "Sitzpläne"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:14
-msgid "Seating Plan Import"
-msgstr "Sitzplan-Import"
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:14
+msgid "Assignment of Seats to Order Positions"
+msgstr "Zuweisung von Sitzplätzen zu Bestellpositionen"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:21
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:21
 msgid "Download CSV"
 msgstr "CSV herunterladen"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:26
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:26
 msgid "Upload CSV"
 msgstr "CSV hochladen"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:36
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:36
 msgid "Clear assigned seats"
 msgstr "Zugewiesene Sitzplätze leeren"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:43
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:43
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:27
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:20
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:53
 msgid "Save"
 msgstr "Speichern"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:50
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:50
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:28
 msgid "Please select a seating plan for your current event."
-msgstr "Bitte wählen Sie einen Sitzplan für die aktuelle Veranstaltung aus."
+msgstr "Bitte wähle einen Sitzplan für die aktuelle Veranstaltung aus."
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:52
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:52
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:30
 msgid "Manage event seating plan"
 msgstr "Sitzplan der Veranstaltung auswählen"
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:12
 #, python-format
 msgid "You have imported only one seating plan."
 msgid_plural "You have imported %(counter)s seating plans."
-msgstr[0] "Sie haben genau einen Sitzplan importiert."
-msgstr[1] "Sie haben %(counter)s Sitzpläne importiert."
+msgstr[0] "Du hast genau einen Sitzplan importiert."
+msgstr[1] "Du hast %(counter)s Sitzpläne importiert."
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:20
 msgid "Seating plan selection"
 msgstr "Auswahl des Sitzplans"
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:34
 msgid ""
 "There are currently no seating plans configured on your organizer account."
-msgstr "Derzeit sind keine Sitzpläne in Ihrem Veranstalterkonto konfiguriert."
+msgstr "Derzeit sind keine Sitzpläne in deinem Veranstalterkonto konfiguriert."
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:38
 msgid "Manage seating plans"
 msgstr "Sitzpläne verwalten"
 
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:13
-msgid "Seating Plan Mapping"
-msgstr "Sitzplan-Zuordnung"
+msgid "Mapping of Seating Plan Categories to Products"
+msgstr "Zuordnung von Sitzplan-Kategorien zu Produkten"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:4
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:6
 msgid "Delete seating plan"
 msgstr "Sitzplan löschen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:11
 #: pretix_manualseats/views.py:512
 msgid ""
 "You cannot delete the seating plan because it is used in at least one of "
 "your events."
 msgstr ""
-"Sie können den Sitzplan nicht löschen, da er in einer Ihrer Veranstaltungen "
-"verwendet wird."
+"Du kannst den Sitzplan nicht löschen, da er in mindestens einer deiner "
+"Veranstaltungen verwendet wird."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:16
 #, python-format
 msgid "Are you sure you want to delete the seating plan „%(name)s“?"
-msgstr "Sind Sie sicher, dass Sie den Sitzplan „%(name)s“ löschen möchten?"
+msgstr "Bist du sicher, dass du den Sitzplan „%(name)s“ löschen möchtest?"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:22
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:50
 msgid "Cancel"
 msgstr "Abbrechen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:25
@@ -138,30 +138,30 @@
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:21
 msgid ""
 "Pretix requires your seating plan to be in a particular format that enables "
 "it to comprehend not just the visual representation of the plan, but also "
 "its structure and numbering details."
 msgstr ""
-"Pretix erfordert, dass Ihr Sitzplan in einem bestimmten Format vorliegt, das "
-"es ermöglicht, nicht nur die visuelle Darstellung des Plans, sondern auch "
-"seine Struktur und Nummerierungsdetails zu erfassen."
+"Pretix benötigt deinen Sitzplan in einem bestimmten Format, damit es nicht "
+"nur die visuelle Darstellung versteht, sondern auch die Struktur und die "
+"Nummerierung der Plätze."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:24
 msgid ""
 "At <a href=\"https://seats.pretix.eu\">seats.pretix.eu</a>, you can access a "
 "graphical seating plan editor, which allows you to create and edit seating "
 "plans in the specified format. Once you're done, you can save the plan to "
 "your computer and upload it here to associate it with your events."
 msgstr ""
-"Unter <a href=\"https://seats.pretix.eu\">seats.pretix.eu</a> können Sie auf "
-"einen grafischen Sitzplan-Editor zugreifen, mit dem Sie Sitzpläne im "
-"angegebenen Format erstellen und bearbeiten können. Sobald Sie fertig sind, "
-"können Sie den Plan auf Ihrem Computer speichern und hier hochladen, um ihn "
-"mit Ihren Veranstaltungen zu verknüpfen."
+"Auf <a href=\"https://seats.pretix.eu\">seats.pretix.eu</a> findest du einen "
+"grafischen Sitzplan-Editor, mit dem du Sitzpläne im geforderten Format "
+"erstellen und bearbeiten kannst. Sobald du fertig bist, speichere den Plan "
+"auf deinem Computer und lade ihn hier hoch, um ihn mit deinen "
+"Veranstaltungen zu verknüpfen."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:29
 msgid "Go to editor"
 msgstr "Zum Editor"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:35
 msgid "Download layout"
@@ -169,15 +169,15 @@
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:40
 msgid "Upload layout"
 msgstr "Layout hochladen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:13
 msgid "You haven't added any seating plan yet."
-msgstr "Sie haben noch keinen Sitzplan hinzugefügt."
+msgstr "Du hast noch keinen Sitzplan hinzugefügt."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:19
 msgid "Add seating plan"
 msgstr "Sitzplan hinzufügen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:30
 msgid "Name"
@@ -201,27 +201,26 @@
 
 #: pretix_manualseats/views.py:40
 msgid ""
 "If disabled, you will need to manually assign seats in the backend. Note "
 "that this can mean people will not know their seat after their purchase and "
 "it might not be written on their ticket."
 msgstr ""
-"Wenn deaktiviert, müssen Sie die Plätze manuell im Backend zuweisen. "
-"Beachten Sie, dass dies dazu führen kann, dass die Käufer ihren Platz nach "
-"dem Kauf nicht kennen und er möglicherweise nicht auf ihrem Ticket vermerkt "
-"ist."
+"Wenn deaktiviert, musst du die Plätze manuell im Backend zuweisen. Beachte, "
+"dass dies dazu führen kann, dass die Käufer ihren Platz nach dem Kauf nicht "
+"kennen und er möglicherweise nicht auf ihrem Ticket vermerkt ist."
 
 #: pretix_manualseats/views.py:89 pretix_manualseats/views.py:188
 msgid "None"
 msgstr "Kein Sitzplan"
 
 #: pretix_manualseats/views.py:122 pretix_manualseats/views.py:209
 #: pretix_manualseats/views.py:317 pretix_manualseats/views.py:474
 msgid "Your changes have been saved."
-msgstr "Ihre Änderungen wurden gespeichert."
+msgstr "Deine Änderungen wurden gespeichert."
 
 #: pretix_manualseats/views.py:217
 msgid "Raw Data"
 msgstr "Rohdaten"
 
 #: pretix_manualseats/views.py:218
 msgid "Header should equal"
@@ -236,16 +235,16 @@
 msgstr "Alle Sitzplatzzuweisungen wurden entfernt."
 
 #: pretix_manualseats/views.py:294
 msgid ""
 "The CSV input format is invalid. Please check if you have included the "
 "headers."
 msgstr ""
-"Das CSV-Eingabeformat ist ungültig. Bitte prüfen Sie, ob Sie die CSV-Header "
-"eingefügt haben."
+"Das CSV-Eingabeformat ist ungültig. Bitte prüfe, ob du die CSV-Header "
+"eingefügt hast."
 
 #: pretix_manualseats/views.py:307
 #, python-brace-format
 msgid "Unable to match order ({orderposition_secret})."
 msgstr "Bestellung ({orderposition_secret}) konnte nicht zugeordnet werden."
 
 #: pretix_manualseats/views.py:311
@@ -259,34 +258,34 @@
 
 #: pretix_manualseats/views.py:385
 msgid "The new seating plan has been added."
 msgstr "Der neue Sitzplan wurde hinzugefügt."
 
 #: pretix_manualseats/views.py:396 pretix_manualseats/views.py:487
 msgid "Your changes could not be saved."
-msgstr "Ihre Änderungen konnten nicht gespeichert werden."
+msgstr "Deine Änderungen konnten nicht gespeichert werden."
 
 #: pretix_manualseats/views.py:409
 msgid "The requested seating plan does not exist. Can't copy!"
 msgstr "Der angeforderte Sitzplan existiert nicht. Kopieren nicht möglich!"
 
 #: pretix_manualseats/views.py:418
 msgid "Copy"
 msgstr "Kopie"
 
 #: pretix_manualseats/views.py:456
 msgid ""
 "You cannot change this plan any more since it is already used in at least "
 "one of your events. Please create a copy instead."
 msgstr ""
-"Sie können diesen Plan nicht mehr ändern, da er bereits in mindestens einer "
-"Ihrer Veranstaltungen verwendet wird. Erstellen Sie stattdessen eine Kopie."
+"Du kannst diesen Plan nicht mehr ändern, da er bereits in mindestens einer "
+"deiner Veranstaltungen verwendet wird. Erstelle stattdessen eine Kopie."
 
 #: pretix_manualseats/views.py:470
 msgid "Your changes could not be saved. The plan already is in use."
 msgstr ""
-"Ihre Änderungen konnten nicht gespeichert werden. Der Plan wird bereits "
+"Deine Änderungen konnten nicht gespeichert werden. Der Plan wird bereits "
 "verwendet."
 
 #: pretix_manualseats/views.py:522
 msgid "The selected plan has been deleted."
 msgstr "Der ausgewählte Sitzplan wurde gelöscht."
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-manualseats-1.0.2/pretix_manualseats/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-30 19:45+0200\n"
+"POT-Creation-Date: 2023-07-31 10:33+0200\n"
 "PO-Revision-Date: \n"
 "Last-Translator: Moritz Lerch\n"
 "Language-Team: \n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_manualseats/apps.py:12 pretix_manualseats/signals.py:19
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:7
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:9
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:9
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:7
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:9
-#: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:7
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:9
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:9
 msgid "Manual Seats"
 msgstr "Manuelle Sitzplätze"
 
 #: pretix_manualseats/apps.py:14
 msgid "Manually assign tickets to seats."
 msgstr "Tickets manuell Sitzplätzen zuweisen."
 
 #: pretix_manualseats/signals.py:31
-msgid "Seating Mapping"
-msgstr "Sitzplatz-Zuordnung"
+#: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:7
+msgid "Category Mapping"
+msgstr "Kategorie-Zuordnung"
 
 #: pretix_manualseats/signals.py:43
-msgid "Seating Importer"
-msgstr "Sitzplatz-Import"
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:7
+msgid "Seat Assignment"
+msgstr "Sitzplatz-Zuweisung"
 
 #: pretix_manualseats/signals.py:70
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:6
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:9
 msgid "Seating Plans"
 msgstr "Sitzpläne"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:14
-msgid "Seating Plan Import"
-msgstr "Sitzplan-Import"
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:14
+msgid "Assignment of Seats to Order Positions"
+msgstr "Zuweisung von Sitzplätzen zu Bestellpositionen"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:21
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:21
 msgid "Download CSV"
 msgstr "CSV herunterladen"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:26
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:26
 msgid "Upload CSV"
 msgstr "CSV hochladen"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:36
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:36
 msgid "Clear assigned seats"
 msgstr "Zugewiesene Sitzplätze leeren"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:43
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:43
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:27
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:20
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:53
 msgid "Save"
 msgstr "Speichern"
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:50
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:50
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:28
 msgid "Please select a seating plan for your current event."
-msgstr "Bitte wähle einen Sitzplan für die aktuelle Veranstaltung aus."
+msgstr "Bitte wählen Sie einen Sitzplan für die aktuelle Veranstaltung aus."
 
-#: pretix_manualseats/templates/pretix_manualseats/event/import.html:52
+#: pretix_manualseats/templates/pretix_manualseats/event/assign.html:52
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:30
 msgid "Manage event seating plan"
 msgstr "Sitzplan der Veranstaltung auswählen"
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:12
 #, python-format
 msgid "You have imported only one seating plan."
 msgid_plural "You have imported %(counter)s seating plans."
-msgstr[0] "Du hast genau einen Sitzplan importiert."
-msgstr[1] "Du hast %(counter)s Sitzpläne importiert."
+msgstr[0] "Sie haben genau einen Sitzplan importiert."
+msgstr[1] "Sie haben %(counter)s Sitzpläne importiert."
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:20
 msgid "Seating plan selection"
 msgstr "Auswahl des Sitzplans"
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:34
 msgid ""
 "There are currently no seating plans configured on your organizer account."
-msgstr "Derzeit sind keine Sitzpläne in deinem Veranstalterkonto konfiguriert."
+msgstr "Derzeit sind keine Sitzpläne in Ihrem Veranstalterkonto konfiguriert."
 
 #: pretix_manualseats/templates/pretix_manualseats/event/index.html:38
 msgid "Manage seating plans"
 msgstr "Sitzpläne verwalten"
 
 #: pretix_manualseats/templates/pretix_manualseats/event/mapping.html:13
-msgid "Seating Plan Mapping"
-msgstr "Sitzplan-Zuordnung"
+msgid "Mapping of Seating Plan Categories to Products"
+msgstr "Zuordnung von Sitzplan-Kategorien zu Produkten"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:4
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:6
 msgid "Delete seating plan"
 msgstr "Sitzplan löschen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:11
 #: pretix_manualseats/views.py:512
 msgid ""
 "You cannot delete the seating plan because it is used in at least one of "
 "your events."
 msgstr ""
-"Du kannst den Sitzplan nicht löschen, da er in mindestens einer deiner "
-"Veranstaltungen verwendet wird."
+"Sie können den Sitzplan nicht löschen, da er in einer Ihrer Veranstaltungen "
+"verwendet wird."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:16
 #, python-format
 msgid "Are you sure you want to delete the seating plan „%(name)s“?"
-msgstr "Bist du sicher, dass du den Sitzplan „%(name)s“ löschen möchtest?"
+msgstr "Sind Sie sicher, dass Sie den Sitzplan „%(name)s“ löschen möchten?"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:22
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:50
 msgid "Cancel"
 msgstr "Abbrechen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/delete.html:25
@@ -138,30 +138,30 @@
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:21
 msgid ""
 "Pretix requires your seating plan to be in a particular format that enables "
 "it to comprehend not just the visual representation of the plan, but also "
 "its structure and numbering details."
 msgstr ""
-"Pretix benötigt deinen Sitzplan in einem bestimmten Format, damit es nicht "
-"nur die visuelle Darstellung versteht, sondern auch die Struktur und die "
-"Nummerierung der Plätze."
+"Pretix erfordert, dass Ihr Sitzplan in einem bestimmten Format vorliegt, das "
+"es ermöglicht, nicht nur die visuelle Darstellung des Plans, sondern auch "
+"seine Struktur und Nummerierungsdetails zu erfassen."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:24
 msgid ""
 "At <a href=\"https://seats.pretix.eu\">seats.pretix.eu</a>, you can access a "
 "graphical seating plan editor, which allows you to create and edit seating "
 "plans in the specified format. Once you're done, you can save the plan to "
 "your computer and upload it here to associate it with your events."
 msgstr ""
-"Auf <a href=\"https://seats.pretix.eu\">seats.pretix.eu</a> findest du einen "
-"grafischen Sitzplan-Editor, mit dem du Sitzpläne im geforderten Format "
-"erstellen und bearbeiten kannst. Sobald du fertig bist, speichere den Plan "
-"auf deinem Computer und lade ihn hier hoch, um ihn mit deinen "
-"Veranstaltungen zu verknüpfen."
+"Unter <a href=\"https://seats.pretix.eu\">seats.pretix.eu</a> können Sie auf "
+"einen grafischen Sitzplan-Editor zugreifen, mit dem Sie Sitzpläne im "
+"angegebenen Format erstellen und bearbeiten können. Sobald Sie fertig sind, "
+"können Sie den Plan auf Ihrem Computer speichern und hier hochladen, um ihn "
+"mit Ihren Veranstaltungen zu verknüpfen."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:29
 msgid "Go to editor"
 msgstr "Zum Editor"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:35
 msgid "Download layout"
@@ -169,15 +169,15 @@
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/form.html:40
 msgid "Upload layout"
 msgstr "Layout hochladen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:13
 msgid "You haven't added any seating plan yet."
-msgstr "Du hast noch keinen Sitzplan hinzugefügt."
+msgstr "Sie haben noch keinen Sitzplan hinzugefügt."
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:19
 msgid "Add seating plan"
 msgstr "Sitzplan hinzufügen"
 
 #: pretix_manualseats/templates/pretix_manualseats/organizer/index.html:30
 msgid "Name"
@@ -201,26 +201,27 @@
 
 #: pretix_manualseats/views.py:40
 msgid ""
 "If disabled, you will need to manually assign seats in the backend. Note "
 "that this can mean people will not know their seat after their purchase and "
 "it might not be written on their ticket."
 msgstr ""
-"Wenn deaktiviert, musst du die Plätze manuell im Backend zuweisen. Beachte, "
-"dass dies dazu führen kann, dass die Käufer ihren Platz nach dem Kauf nicht "
-"kennen und er möglicherweise nicht auf ihrem Ticket vermerkt ist."
+"Wenn deaktiviert, müssen Sie die Plätze manuell im Backend zuweisen. "
+"Beachten Sie, dass dies dazu führen kann, dass die Käufer ihren Platz nach "
+"dem Kauf nicht kennen und er möglicherweise nicht auf ihrem Ticket vermerkt "
+"ist."
 
 #: pretix_manualseats/views.py:89 pretix_manualseats/views.py:188
 msgid "None"
 msgstr "Kein Sitzplan"
 
 #: pretix_manualseats/views.py:122 pretix_manualseats/views.py:209
 #: pretix_manualseats/views.py:317 pretix_manualseats/views.py:474
 msgid "Your changes have been saved."
-msgstr "Deine Änderungen wurden gespeichert."
+msgstr "Ihre Änderungen wurden gespeichert."
 
 #: pretix_manualseats/views.py:217
 msgid "Raw Data"
 msgstr "Rohdaten"
 
 #: pretix_manualseats/views.py:218
 msgid "Header should equal"
@@ -235,16 +236,16 @@
 msgstr "Alle Sitzplatzzuweisungen wurden entfernt."
 
 #: pretix_manualseats/views.py:294
 msgid ""
 "The CSV input format is invalid. Please check if you have included the "
 "headers."
 msgstr ""
-"Das CSV-Eingabeformat ist ungültig. Bitte prüfe, ob du die CSV-Header "
-"eingefügt hast."
+"Das CSV-Eingabeformat ist ungültig. Bitte prüfen Sie, ob Sie die CSV-Header "
+"eingefügt haben."
 
 #: pretix_manualseats/views.py:307
 #, python-brace-format
 msgid "Unable to match order ({orderposition_secret})."
 msgstr "Bestellung ({orderposition_secret}) konnte nicht zugeordnet werden."
 
 #: pretix_manualseats/views.py:311
@@ -258,34 +259,34 @@
 
 #: pretix_manualseats/views.py:385
 msgid "The new seating plan has been added."
 msgstr "Der neue Sitzplan wurde hinzugefügt."
 
 #: pretix_manualseats/views.py:396 pretix_manualseats/views.py:487
 msgid "Your changes could not be saved."
-msgstr "Deine Änderungen konnten nicht gespeichert werden."
+msgstr "Ihre Änderungen konnten nicht gespeichert werden."
 
 #: pretix_manualseats/views.py:409
 msgid "The requested seating plan does not exist. Can't copy!"
 msgstr "Der angeforderte Sitzplan existiert nicht. Kopieren nicht möglich!"
 
 #: pretix_manualseats/views.py:418
 msgid "Copy"
 msgstr "Kopie"
 
 #: pretix_manualseats/views.py:456
 msgid ""
 "You cannot change this plan any more since it is already used in at least "
 "one of your events. Please create a copy instead."
 msgstr ""
-"Du kannst diesen Plan nicht mehr ändern, da er bereits in mindestens einer "
-"deiner Veranstaltungen verwendet wird. Erstelle stattdessen eine Kopie."
+"Sie können diesen Plan nicht mehr ändern, da er bereits in mindestens einer "
+"Ihrer Veranstaltungen verwendet wird. Erstellen Sie stattdessen eine Kopie."
 
 #: pretix_manualseats/views.py:470
 msgid "Your changes could not be saved. The plan already is in use."
 msgstr ""
-"Deine Änderungen konnten nicht gespeichert werden. Der Plan wird bereits "
+"Ihre Änderungen konnten nicht gespeichert werden. Der Plan wird bereits "
 "verwendet."
 
 #: pretix_manualseats/views.py:522
 msgid "The selected plan has been deleted."
 msgstr "Der ausgewählte Sitzplan wurde gelöscht."
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/signals.py` & `pretix-manualseats-1.0.2/pretix_manualseats/signals.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,29 +24,29 @@
                     "organizer": request.event.organizer.slug,
                 },
             ),
             "active": (url.namespace == "plugins:pretix_manualseats"),
             "icon": seat_icon,
             "children": [
                 {
-                    "label": _("Seating Mapping"),
+                    "label": _("Category Mapping"),
                     "url": reverse(
                         "plugins:pretix_manualseats:mapping",
                         kwargs={
                             "event": request.event.slug,
                             "organizer": request.organizer.slug,
                         },
                     ),
                     "active": (url.namespace == "plugins:pretix_manualseats"),
                     "icon": seat_icon,
                 },
                 {
-                    "label": _("Seating Importer"),
+                    "label": _("Seat Assignment"),
                     "url": reverse(
-                        "plugins:pretix_manualseats:import",
+                        "plugins:pretix_manualseats:assign",
                         kwargs={
                             "event": request.event.slug,
                             "organizer": request.organizer.slug,
                         },
                     ),
                     "active": (url.namespace == "plugins:pretix_manualseats"),
                     "icon": seat_icon,
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js` & `pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/icons/seat.svg` & `pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/icons/seat.svg`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/static/pretix_manualseats/seating-edit.js` & `pretix-manualseats-1.0.2/pretix_manualseats/static/pretix_manualseats/seating-edit.js`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/import.html` & `pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/event/assign.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {% extends "pretixcontrol/event/base.html" %}
 {% load i18n %}
 {% load compress %}
 {% load static %}
 {% load bootstrap3 %}
 {% load eventurl %}
-{% block title %}{% trans "Seating Plan Import" %}{% endblock %}
+{% block title %}{% trans "Seat Assignment" %}{% endblock %}
 {% block content %}
     <h1>{% trans "Manual Seats" %} 💺</h1>
 
     {% if seatingplan %}
        <form method="post" class="form-horizontal">{% csrf_token %}
             <fieldset>
-                <legend>{% trans "Seating Plan Import" %}</i></legend>
+                <legend>{% trans "Assignment of Seats to Order Positions" %}</i></legend>
                 
                 <div class="form-group">
                     <div class="col-md-9 col-md-offset-3">
                         <div class="btn-group btn-group-justified">
                             <div class="btn-group" role="group">
                                 <button type="button" class="btn btn-default" id="download_assignedseats">
                                     <span class="fa fa-download"></span> {% trans "Download CSV" %}
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends "pretixcontrol/event/base.html" %} {% load i18n %} {% load compress
 %} {% load static %} {% load bootstrap3 %} {% load eventurl %} {% block title
-%}{% trans "Seating Plan Import" %}{% endblock %} {% block content %}
+%}{% trans "Seat Assignment" %}{% endblock %} {% block content %}
 ****** {% trans "Manual Seats" %} ðº ******
 {% if seatingplan %}
-{% csrf_token %}  {% trans "Seating Plan Import" %}
+{% csrf_token %}  {% trans "Assignment of Seats to Order Positions" %}
   {% trans "Download CSV" %}
   {% trans "Upload CSV" %}
 {% bootstrap_field form.data layout="control" %}
   {% trans "Clear assigned seats" %}
   {% trans "Save" %}
 {% else %}
 {% trans "Please select a seating plan for your current event." %}
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/index.html` & `pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/event/index.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/event/mapping.html` & `pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/event/mapping.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {% extends "pretixcontrol/event/base.html" %}
 {% load i18n %}
 {% load compress %}
 {% load static %}
 {% load bootstrap3 %}
 {% load eventurl %}
-{% block title %}{% trans "Seating Plan Mapping" %}{% endblock %}
+{% block title %}{% trans "Category Mapping" %}{% endblock %}
 {% block content %}
     <h1>{% trans "Manual Seats" %} 💺</h1>
     {% if seatingplan %}
        <form method="post" class="form-horizontal">{% csrf_token %}
             <fieldset>
-                <legend>{% trans "Seating Plan Mapping" %}</legend>
+                <legend>{% trans "Mapping of Seating Plan Categories to Products" %}</legend>
                 {% for field in form %}
                     {% bootstrap_field field layout="control" %}
                 {% endfor %}
             </fieldset>
             <div class="form-group submit-group">
                 <button type="submit" class="btn btn-primary btn-save">
                     <i class="fa fa-save"></i> {% trans "Save" %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends "pretixcontrol/event/base.html" %} {% load i18n %} {% load compress
 %} {% load static %} {% load bootstrap3 %} {% load eventurl %} {% block title
-%}{% trans "Seating Plan Mapping" %}{% endblock %} {% block content %}
+%}{% trans "Category Mapping" %}{% endblock %} {% block content %}
 ****** {% trans "Manual Seats" %} ðº ******
 {% if seatingplan %}
-{% csrf_token %}  {% trans "Seating Plan Mapping" %} {% for field in form %} {%
-bootstrap_field field layout="control" %} {% endfor %}
+{% csrf_token %}  {% trans "Mapping of Seating Plan Categories to Products" %}
+{% for field in form %} {% bootstrap_field field layout="control" %} {% endfor
+%}
   {% trans "Save" %}
 {% else %}
 {% trans "Please select a seating plan for your current event." %}
 organizer=request.organizer.slug event=request.event.slug %}" class="btn btn-
 info">  {% trans "Manage event seating plan" %}
 {%endif%} {% endblock %}
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html` & `pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/organizer/delete.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/form.html` & `pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/organizer/form.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/templates/pretix_manualseats/organizer/index.html` & `pretix-manualseats-1.0.2/pretix_manualseats/templates/pretix_manualseats/organizer/index.html`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/urls.py` & `pretix-manualseats-1.0.2/pretix_manualseats/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     ),
     path(
         "control/event/<str:organizer>/<str:event>/manualseats/mapping/",
         views.EventMapping.as_view(),
         name="mapping",
     ),
     path(
-        "control/event/<str:organizer>/<str:event>/manualseats/import/",
-        views.EventImport.as_view(),
-        name="import",
+        "control/event/<str:organizer>/<str:event>/manualseats/assign/",
+        views.EventAssign.as_view(),
+        name="assign",
     ),
     path(
         "control/organizer/<str:organizer>/manualseats/",
         views.OrganizerSeatingPlanList.as_view(),
         name="index",
     ),
     path(
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats/views.py` & `pretix-manualseats-1.0.2/pretix_manualseats/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,34 +207,34 @@
                     queryset.save()
 
         messages.success(self.request, _("Your changes have been saved."))
 
         return super().form_valid(form)
 
 
-class EventImportForm(forms.Form):
+class EventAssignForm(forms.Form):
     data = forms.CharField(
         widget=forms.Textarea(),
         label=_("Raw Data"),
         help_text=_("Header should equal")
         + ": <code>seat_guid,orderposition_secret</code>",
         required=False,
     )
 
     pass
 
 
-class EventImport(EventPermissionRequiredMixin, FormView):
-    template_name = "pretix_manualseats/event/import.html"
+class EventAssign(EventPermissionRequiredMixin, FormView):
+    template_name = "pretix_manualseats/event/assign.html"
     permission = "can_change_orders"
-    form_class = EventImportForm
+    form_class = EventAssignForm
 
     def get_success_url(self) -> str:
         return reverse(
-            "plugins:pretix_manualseats:import",
+            "plugins:pretix_manualseats:assign",
             kwargs={
                 "organizer": self.get_event().organizer.slug,
                 "event": self.get_event().slug,
             },
         )
 
     def get_context_data(self, **kwargs):
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats.egg-info/PKG-INFO` & `pretix-manualseats-1.0.2/pretix_manualseats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-manualseats
-Version: 1.0.1
+Version: 1.0.2
 Summary: Manually assign tickets to seats.
 Author-email: Moritz Lerch <dev@moritz-lerch.de>
 Maintainer-email: Moritz Lerch <dev@moritz-lerch.de>
 License: Apache
 Project-URL: homepage, https://github.com/moritzlerch/pretix-manualseats
 Project-URL: repository, https://github.com/moritzlerch/pretix-manualseats
 Keywords: pretix
```

### Comparing `pretix-manualseats-1.0.1/pretix_manualseats.egg-info/SOURCES.txt` & `pretix-manualseats-1.0.2/pretix_manualseats.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 pretix_manualseats.egg-info/entry_points.txt
 pretix_manualseats.egg-info/top_level.txt
 pretix_manualseats/locale/de/LC_MESSAGES/django.po
 pretix_manualseats/locale/de_Informal/LC_MESSAGES/django.po
 pretix_manualseats/static/pretix_manualseats/assignedseats-edit.js
 pretix_manualseats/static/pretix_manualseats/seating-edit.js
 pretix_manualseats/static/pretix_manualseats/icons/seat.svg
-pretix_manualseats/templates/pretix_manualseats/event/import.html
+pretix_manualseats/templates/pretix_manualseats/event/assign.html
 pretix_manualseats/templates/pretix_manualseats/event/index.html
 pretix_manualseats/templates/pretix_manualseats/event/mapping.html
 pretix_manualseats/templates/pretix_manualseats/organizer/delete.html
 pretix_manualseats/templates/pretix_manualseats/organizer/form.html
 pretix_manualseats/templates/pretix_manualseats/organizer/index.html
 tests/test_main.py
```

### Comparing `pretix-manualseats-1.0.1/pyproject.toml` & `pretix-manualseats-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-manualseats-1.0.1/setup.cfg` & `pretix-manualseats-1.0.2/setup.cfg`

 * *Files identical despite different names*

