# Comparing `tmp/wagtail-rangefilter-0.1.1.tar.gz` & `tmp/wagtail-rangefilter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-rangefilter-0.1.1.tar", last modified: Mon Dec  5 14:23:57 2022, max compression
+gzip compressed data, was "wagtail-rangefilter-0.2.0.tar", last modified: Mon Jul 31 12:46:09 2023, max compression
```

## Comparing `wagtail-rangefilter-0.1.1.tar` & `wagtail-rangefilter-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      753 2022-12-05 14:16:40.921893 wagtail-rangefilter-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       38 2022-09-19 11:05:08.979031 wagtail-rangefilter-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1489 2022-09-20 11:14:32.028114 wagtail-rangefilter-0.1.1/LICENSE
--rw-r--r--   0        0        0     1642 2022-09-21 08:32:35.966448 wagtail-rangefilter-0.1.1/README.md
--rw-r--r--   0        0        0     1743 2022-09-21 09:15:00.700252 wagtail-rangefilter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      140 2022-12-05 14:21:16.170613 wagtail-rangefilter-0.1.1/src/wagtail_rangefilter/__init__.py
--rw-r--r--   0        0        0      190 2022-09-19 10:57:20.620006 wagtail-rangefilter-0.1.1/src/wagtail_rangefilter/apps.py
--rw-r--r--   0        0        0     2257 2022-09-20 08:18:35.702265 wagtail-rangefilter-0.1.1/src/wagtail_rangefilter/filters.py
--rw-r--r--   0        0        0     1615 2022-12-05 14:18:34.607897 wagtail-rangefilter-0.1.1/src/wagtail_rangefilter/templates/wagtail_rangefilter/date_filter.html
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 wagtail-rangefilter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1042 2023-07-31 12:40:35.691341 wagtail-rangefilter-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      946 2023-07-31 12:24:01.476389 wagtail-rangefilter-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1489 2022-09-20 11:14:32.028114 wagtail-rangefilter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1794 2023-07-31 12:29:18.511026 wagtail-rangefilter-0.2.0/README.md
+-rw-r--r--   0        0        0     1710 2023-07-31 12:24:01.476389 wagtail-rangefilter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-07-31 12:41:41.871091 wagtail-rangefilter-0.2.0/src/wagtail_rangefilter/__init__.py
+-rw-r--r--   0        0        0      190 2022-09-19 10:57:20.620006 wagtail-rangefilter-0.2.0/src/wagtail_rangefilter/apps.py
+-rw-r--r--   0        0        0     2257 2022-09-20 08:18:35.702265 wagtail-rangefilter-0.2.0/src/wagtail_rangefilter/filters.py
+-rw-r--r--   0        0        0     1615 2022-12-05 14:18:34.607897 wagtail-rangefilter-0.2.0/src/wagtail_rangefilter/templates/wagtail_rangefilter/date_filter.html
+-rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 wagtail-rangefilter-0.2.0/PKG-INFO
```

### Comparing `wagtail-rangefilter-0.1.1/LICENSE` & `wagtail-rangefilter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-rangefilter-0.1.1/README.md` & `wagtail-rangefilter-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 - [Documentation](https://github.com/wunderweiss/wagtail-rangefilter/blob/main/README.md)
 - [Changelog](https://github.com/wunderweiss/wagtail-rangefilter/blob/main/CHANGELOG.md)
 - [Contributing](https://github.com/wunderweiss/wagtail-rangefilter/blob/main/CONTRIBUTING.md)
 
 ## Supported versions
 
-- Python 3.7, 3.8, 3.9, 3.10
-- Django 3.2, 4.0, 4.1
-- Wagtail 2.15, 3.0, 4.0
+- Python 3.8, 3.9, 3.10, 3.11
+- Django 3.2, 4.1, 4.2
+- Wagtail 4.1, 4.2, 5.0
 
 ## Installation
 
 ```shell
 pip install wagtail-rangefilter
 ```
 
@@ -50,7 +50,19 @@
 ```
 
 ## Development
 
 ```shell
 pip install -e '.[testing]' -U
 ```
+
+## Running the testapp
+
+```shell
+tox -e interactive
+```
+
+Alternative:
+```shell
+cp tests/local.py.example tests/local.py
+python manage.py runserver
+```
```

### Comparing `wagtail-rangefilter-0.1.1/pyproject.toml` & `wagtail-rangefilter-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,35 +18,34 @@
 dynamic = [
     "version",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Framework :: Wagtail",
-    "Framework :: Wagtail :: 2",
-    "Framework :: Wagtail :: 3",
     "Framework :: Wagtail :: 4",
+    "Framework :: Wagtail :: 5",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "django-admin-rangefilter",
     "Django>=3.2",
-    "wagtail>=2.15",
+    "wagtail>=4.1",
 ]
 
 [project.optional-dependencies]
 testing = [
     "coverage~=6.4.4",
     "tox~=3.26.0",
 ]
```

### Comparing `wagtail-rangefilter-0.1.1/src/wagtail_rangefilter/filters.py` & `wagtail-rangefilter-0.2.0/src/wagtail_rangefilter/filters.py`

 * *Files identical despite different names*

### Comparing `wagtail-rangefilter-0.1.1/src/wagtail_rangefilter/templates/wagtail_rangefilter/date_filter.html` & `wagtail-rangefilter-0.2.0/src/wagtail_rangefilter/templates/wagtail_rangefilter/date_filter.html`

 * *Files identical despite different names*

### Comparing `wagtail-rangefilter-0.1.1/PKG-INFO` & `wagtail-rangefilter-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: wagtail-rangefilter
-Version: 0.1.1
+Version: 0.2.0
 Summary: Integrates django-admin-rangefilter into Wagtail's ModelAdmin
 Keywords: django,rangefilter,wagtail
 Author-email: Stefan Hammer <stefan.hammer@wunderweiss.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django-admin-rangefilter
 Requires-Dist: Django>=3.2
-Requires-Dist: wagtail>=2.15
+Requires-Dist: wagtail>=4.1
 Requires-Dist: coverage~=6.4.4 ; extra == "testing"
 Requires-Dist: tox~=3.26.0 ; extra == "testing"
 Project-URL: Bug Tracker, https://github.com/wunderweiss/wagtail-rangefilter/issues
 Project-URL: Changelog, https://github.com/wunderweiss/wagtail-rangefilter/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://github.com/wunderweiss/wagtail-rangefilter
 Provides-Extra: testing
 
@@ -48,17 +47,17 @@
 
 - [Documentation](https://github.com/wunderweiss/wagtail-rangefilter/blob/main/README.md)
 - [Changelog](https://github.com/wunderweiss/wagtail-rangefilter/blob/main/CHANGELOG.md)
 - [Contributing](https://github.com/wunderweiss/wagtail-rangefilter/blob/main/CONTRIBUTING.md)
 
 ## Supported versions
 
-- Python 3.7, 3.8, 3.9, 3.10
-- Django 3.2, 4.0, 4.1
-- Wagtail 2.15, 3.0, 4.0
+- Python 3.8, 3.9, 3.10, 3.11
+- Django 3.2, 4.1, 4.2
+- Wagtail 4.1, 4.2, 5.0
 
 ## Installation
 
 ```shell
 pip install wagtail-rangefilter
 ```
 
@@ -87,7 +86,19 @@
 
 ## Development
 
 ```shell
 pip install -e '.[testing]' -U
 ```
 
+## Running the testapp
+
+```shell
+tox -e interactive
+```
+
+Alternative:
+```shell
+cp tests/local.py.example tests/local.py
+python manage.py runserver
+```
+
```

