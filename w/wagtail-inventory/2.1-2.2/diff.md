# Comparing `tmp/wagtail-inventory-2.1.tar.gz` & `tmp/wagtail-inventory-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-inventory-2.1.tar", last modified: Mon Jul 24 21:10:07 2023, max compression
+gzip compressed data, was "wagtail-inventory-2.2.tar", last modified: Mon Jul 31 15:37:01 2023, max compression
```

## Comparing `wagtail-inventory-2.1.tar` & `wagtail-inventory-2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.422796 wagtail-inventory-2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-24 21:10:07.422796 wagtail-inventory-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:10:07.422796 wagtail-inventory-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.418796 wagtail-inventory-2.1/wagtail_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-24 21:10:07.000000 wagtail-inventory-2.1/wagtail_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-24 21:10:07.000000 wagtail-inventory-2.1/wagtail_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:10:07.000000 wagtail-inventory-2.1/wagtail_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 21:10:07.000000 wagtail-inventory-2.1/wagtail_inventory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 21:10:07.000000 wagtail-inventory-2.1/wagtail_inventory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.418796 wagtail-inventory-2.1/wagtailinventory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.418796 wagtail-inventory-2.1/wagtailinventory/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.418796 wagtail-inventory-2.1/wagtailinventory/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/management/commands/block_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.418796 wagtail-inventory-2.1/wagtailinventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/migrations/0002_pageblock_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/migrations/0003_pageblock_id_bigautofield.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.418796 wagtail-inventory-2.1/wagtailinventory/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/test_wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.418796 wagtail-inventory-2.1/wagtailinventory/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/testapp/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:10:07.422796 wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/0002_nested_stream_block_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/0003_single_content_block_optional.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-24 21:09:49.000000 wagtail-inventory-2.1/wagtailinventory/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.262453 wagtail-inventory-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-31 15:37:01.262453 wagtail-inventory-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:37:01.262453 wagtail-inventory-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.258453 wagtail-inventory-2.2/wagtail_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-31 15:37:01.000000 wagtail-inventory-2.2/wagtail_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-31 15:37:01.000000 wagtail-inventory-2.2/wagtail_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:37:01.000000 wagtail-inventory-2.2/wagtail_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 15:37:01.000000 wagtail-inventory-2.2/wagtail_inventory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 15:37:01.000000 wagtail-inventory-2.2/wagtail_inventory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.258453 wagtail-inventory-2.2/wagtailinventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.258453 wagtail-inventory-2.2/wagtailinventory/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.258453 wagtail-inventory-2.2/wagtailinventory/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/management/commands/block_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.258453 wagtail-inventory-2.2/wagtailinventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/migrations/0002_pageblock_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/migrations/0003_pageblock_id_bigautofield.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.258453 wagtail-inventory-2.2/wagtailinventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/test_wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.258453 wagtail-inventory-2.2/wagtailinventory/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/testapp/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:01.262453 wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/0002_nested_stream_block_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/0003_single_content_block_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-31 15:36:45.000000 wagtail-inventory-2.2/wagtailinventory/wagtail_hooks.py
```

### Comparing `wagtail-inventory-2.1/LICENSE` & `wagtail-inventory-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/PKG-INFO` & `wagtail-inventory-2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: wagtail-inventory
-Version: 2.1
+Version: 2.2
 Summary: Wagtail report to filter pages by block content
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-inventory
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-inventory/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-inventory
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
@@ -73,16 +75,16 @@
 
 Compatibility
 -------------
 
 This code has been tested for compatibility with:
 
 * Python 3.8+
-* Django 3.2 (LTS), 4.1
-* Wagtail 3.0, 4.1 (LTS), 4.2
+* Django 3.2 (LTS), 4.1, 4.2 (LTS)
+* Wagtail 3.0, 4.1 (LTS), 4.2, 5.0
 
 It should be compatible with all intermediate versions, as well.
 If you find that it is not, please `file an issue <https://github.com/cfpb/wagtail-inventory/issues/new>`_.
 
 Testing
 -------
```

### Comparing `wagtail-inventory-2.1/README.rst` & `wagtail-inventory-2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
 Compatibility
 -------------
 
 This code has been tested for compatibility with:
 
 * Python 3.8+
-* Django 3.2 (LTS), 4.1
-* Wagtail 3.0, 4.1 (LTS), 4.2
+* Django 3.2 (LTS), 4.1, 4.2 (LTS)
+* Wagtail 3.0, 4.1 (LTS), 4.2, 5.0
 
 It should be compatible with all intermediate versions, as well.
 If you find that it is not, please `file an issue <https://github.com/cfpb/wagtail-inventory/issues/new>`_.
 
 Testing
 -------
```

### Comparing `wagtail-inventory-2.1/pyproject.toml` & `wagtail-inventory-2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wagtail-inventory"
-version = "2.1"
+version = "2.2"
 description = "Wagtail report to filter pages by block content"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "CC0"}
 authors = [
     {name = "CFPB", email = "tech@cfpb.gov" }
 ]
@@ -12,18 +12,20 @@
     "tqdm>=4.15.0,<5",
     "wagtail>=3",
     "django-autocomplete-light>=3.9",
 ]
 classifiers = [
     "Framework :: Django",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Framework :: Wagtail",
     "Framework :: Wagtail :: 3",
     "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "License :: Public Domain",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
 [project.optional-dependencies]
```

### Comparing `wagtail-inventory-2.1/wagtail_inventory.egg-info/PKG-INFO` & `wagtail-inventory-2.2/wagtail_inventory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: wagtail-inventory
-Version: 2.1
+Version: 2.2
 Summary: Wagtail report to filter pages by block content
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-inventory
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-inventory/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-inventory
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
@@ -73,16 +75,16 @@
 
 Compatibility
 -------------
 
 This code has been tested for compatibility with:
 
 * Python 3.8+
-* Django 3.2 (LTS), 4.1
-* Wagtail 3.0, 4.1 (LTS), 4.2
+* Django 3.2 (LTS), 4.1, 4.2 (LTS)
+* Wagtail 3.0, 4.1 (LTS), 4.2, 5.0
 
 It should be compatible with all intermediate versions, as well.
 If you find that it is not, please `file an issue <https://github.com/cfpb/wagtail-inventory/issues/new>`_.
 
 Testing
 -------
```

### Comparing `wagtail-inventory-2.1/wagtail_inventory.egg-info/SOURCES.txt` & `wagtail-inventory-2.2/wagtail_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/helpers.py` & `wagtail-inventory-2.2/wagtailinventory/helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/migrations/0001_initial.py` & `wagtail-inventory-2.2/wagtailinventory/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/migrations/0002_pageblock_unique_constraint.py` & `wagtail-inventory-2.2/wagtailinventory/migrations/0002_pageblock_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/models.py` & `wagtail-inventory-2.2/wagtailinventory/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/settings.py` & `wagtail-inventory-2.2/wagtailinventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/test_helpers.py` & `wagtail-inventory-2.2/wagtailinventory/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/test_views.py` & `wagtail-inventory-2.2/wagtailinventory/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/test_wagtail_hooks.py` & `wagtail-inventory-2.2/wagtailinventory/tests/test_wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/0001_initial.py` & `wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/0002_nested_stream_block_page.py` & `wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/0002_nested_stream_block_page.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/testapp/migrations/0003_single_content_block_optional.py` & `wagtail-inventory-2.2/wagtailinventory/tests/testapp/migrations/0003_single_content_block_optional.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/testapp/models.py` & `wagtail-inventory-2.2/wagtailinventory/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/tests/urls.py` & `wagtail-inventory-2.2/wagtailinventory/tests/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/views.py` & `wagtail-inventory-2.2/wagtailinventory/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-inventory-2.1/wagtailinventory/wagtail_hooks.py` & `wagtail-inventory-2.2/wagtailinventory/wagtail_hooks.py`

 * *Files identical despite different names*

