# Comparing `tmp/django-log-reader-1.1.5.tar.gz` & `tmp/django-log-reader-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-log-reader-1.1.5.tar", last modified: Thu Nov 11 08:04:09 2021, max compression
+gzip compressed data, was "django-log-reader-1.1.6.tar", last modified: Mon Jul 31 07:54:06 2023, max compression
```

## Comparing `django-log-reader-1.1.5.tar` & `django-log-reader-1.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/
--rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/PKG-INFO
--rw-r--r--   0 imankarimi   (501) staff       (20)     1068 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/LICENSE
--rw-r--r--   0 imankarimi   (501) staff       (20)      138 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/MANIFEST.in
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/docs/
--rw-r--r--   0 imankarimi   (501) staff       (20)      541 2021-11-10 13:29:08.000000 django-log-reader-1.1.5/docs/run-and-demo.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)     1061 2021-11-10 13:29:08.000000 django-log-reader-1.1.5/docs/index.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)      546 2021-11-10 13:29:08.000000 django-log-reader-1.1.5/docs/requirements.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)     1432 2021-11-11 07:08:11.000000 django-log-reader-1.1.5/docs/installation.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)     2222 2021-11-11 07:08:11.000000 django-log-reader-1.1.5/README.md
--rw-r--r--   0 imankarimi   (501) staff       (20)     1476 2021-11-11 08:03:37.000000 django-log-reader-1.1.5/setup.py
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/django_log_reader.egg-info/
--rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/django_log_reader.egg-info/PKG-INFO
--rw-r--r--   0 imankarimi   (501) staff       (20)        1 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/django_log_reader.egg-info/not-zip-safe
--rw-r--r--   0 imankarimi   (501) staff       (20)      672 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/django_log_reader.egg-info/SOURCES.txt
--rw-r--r--   0 imankarimi   (501) staff       (20)       11 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/django_log_reader.egg-info/top_level.txt
--rw-r--r--   0 imankarimi   (501) staff       (20)        1 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/django_log_reader.egg-info/dependency_links.txt
--rw-r--r--   0 imankarimi   (501) staff       (20)       38 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/setup.cfg
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/migrations/
--rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/migrations/__init__.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      414 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/models.py
--rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/__init__.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      183 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/apps.py
--rw-r--r--   0 imankarimi   (501) staff       (20)     1341 2021-11-11 07:32:55.000000 django-log-reader-1.1.5/log_reader/admin.py
--rw-r--r--   0 imankarimi   (501) staff       (20)     1545 2021-11-11 08:02:45.000000 django-log-reader-1.1.5/log_reader/utils.py
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/static/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/static/log_reader/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/static/log_reader/css/
--rw-r--r--   0 imankarimi   (501) staff       (20)      165 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/static/log_reader/css/log_reader.css
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/static/log_reader/js/
--rw-r--r--   0 imankarimi   (501) staff       (20)      367 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/static/log_reader/js/log_reader.js
--rw-r--r--   0 imankarimi   (501) staff       (20)      954 2021-11-11 07:08:11.000000 django-log-reader-1.1.5/log_reader/settings.py
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/templates/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/templates/log_reader/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2021-11-11 08:04:09.000000 django-log-reader-1.1.5/log_reader/templates/log_reader/admin/
--rw-r--r--   0 imankarimi   (501) staff       (20)     4273 2021-11-10 20:56:19.000000 django-log-reader-1.1.5/log_reader/templates/log_reader/admin/change_list.html
--rw-r--r--   0 imankarimi   (501) staff       (20)       60 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/tests.py
--rw-r--r--   0 imankarimi   (501) staff       (20)       63 2021-10-12 17:38:53.000000 django-log-reader-1.1.5/log_reader/views.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.216064 django-log-reader-1.1.6/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1068 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/LICENSE
+-rw-r--r--   0 imankarimi   (501) staff       (20)      138 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/MANIFEST.in
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 07:54:06.215266 django-log-reader-1.1.6/PKG-INFO
+-rw-r--r--   0 imankarimi   (501) staff       (20)     2222 2021-11-11 07:08:11.000000 django-log-reader-1.1.6/README.md
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.145530 django-log-reader-1.1.6/django_log_reader.egg-info/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/PKG-INFO
+-rw-r--r--   0 imankarimi   (501) staff       (20)      672 2023-07-31 07:54:06.000000 django-log-reader-1.1.6/django_log_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/not-zip-safe
+-rw-r--r--   0 imankarimi   (501) staff       (20)       11 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/top_level.txt
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.160813 django-log-reader-1.1.6/docs/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1061 2021-11-10 13:29:08.000000 django-log-reader-1.1.6/docs/index.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1432 2021-11-11 07:08:11.000000 django-log-reader-1.1.6/docs/installation.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)      546 2021-11-10 13:29:08.000000 django-log-reader-1.1.6/docs/requirements.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)      541 2021-11-10 13:29:08.000000 django-log-reader-1.1.6/docs/run-and-demo.rst
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.197737 django-log-reader-1.1.6/log_reader/
+-rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/__init__.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1341 2021-11-11 07:32:55.000000 django-log-reader-1.1.6/log_reader/admin.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      183 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/apps.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.200723 django-log-reader-1.1.6/log_reader/migrations/
+-rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/migrations/__init__.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      530 2023-07-31 07:44:51.000000 django-log-reader-1.1.6/log_reader/models.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      954 2021-11-11 07:08:11.000000 django-log-reader-1.1.6/log_reader/settings.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.075829 django-log-reader-1.1.6/log_reader/static/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.080953 django-log-reader-1.1.6/log_reader/static/log_reader/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.201631 django-log-reader-1.1.6/log_reader/static/log_reader/css/
+-rw-r--r--   0 imankarimi   (501) staff       (20)      165 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/static/log_reader/css/log_reader.css
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.206821 django-log-reader-1.1.6/log_reader/static/log_reader/js/
+-rw-r--r--   0 imankarimi   (501) staff       (20)      367 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/static/log_reader/js/log_reader.js
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.086167 django-log-reader-1.1.6/log_reader/templates/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.086826 django-log-reader-1.1.6/log_reader/templates/log_reader/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.210309 django-log-reader-1.1.6/log_reader/templates/log_reader/admin/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4273 2021-11-10 20:56:19.000000 django-log-reader-1.1.6/log_reader/templates/log_reader/admin/change_list.html
+-rw-r--r--   0 imankarimi   (501) staff       (20)       60 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/tests.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1661 2023-07-31 07:44:51.000000 django-log-reader-1.1.6/log_reader/utils.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)       63 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/views.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)       38 2023-07-31 07:54:06.216334 django-log-reader-1.1.6/setup.cfg
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1476 2023-07-31 07:54:00.000000 django-log-reader-1.1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-log-reader-1.1.5/PKG-INFO` & `django-log-reader-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-reader
-Version: 1.1.5
+Version: 1.1.6
 Summary: Read & Download log files on the admin page
 Home-page: https://github.com/imankarimi/django-log-reader
 Author: Iman Karimi
 Author-email: imankarimi.mail@gmail.com
 License: MIT License
 Description: # Django Log Reader
         **Django Log Reader** allows you to read &amp; download log files on the admin page.
```

### Comparing `django-log-reader-1.1.5/LICENSE` & `django-log-reader-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/docs/run-and-demo.rst` & `django-log-reader-1.1.6/docs/run-and-demo.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/docs/index.rst` & `django-log-reader-1.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/docs/requirements.rst` & `django-log-reader-1.1.6/docs/requirements.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/docs/installation.rst` & `django-log-reader-1.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/README.md` & `django-log-reader-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/setup.py` & `django-log-reader-1.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-log-reader',
-    version='1.1.5',
+    version='1.1.6',
     zip_safe=False,
     packages=find_packages(),
     include_package_data=True,
     description='Read & Download log files on the admin page',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/imankarimi/django-log-reader',
```

### Comparing `django-log-reader-1.1.5/django_log_reader.egg-info/PKG-INFO` & `django-log-reader-1.1.6/django_log_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-reader
-Version: 1.1.5
+Version: 1.1.6
 Summary: Read & Download log files on the admin page
 Home-page: https://github.com/imankarimi/django-log-reader
 Author: Iman Karimi
 Author-email: imankarimi.mail@gmail.com
 License: MIT License
 Description: # Django Log Reader
         **Django Log Reader** allows you to read &amp; download log files on the admin page.
```

### Comparing `django-log-reader-1.1.5/django_log_reader.egg-info/SOURCES.txt` & `django-log-reader-1.1.6/django_log_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/log_reader/admin.py` & `django-log-reader-1.1.6/log_reader/admin.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/log_reader/utils.py` & `django-log-reader-1.1.6/log_reader/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import unicode_literals
 
+import django
 import os
 # import re
 import subprocess
-from subprocess import PIPE
 from fnmatch import fnmatch
-from django.utils.translation import ugettext_lazy as _
+from subprocess import PIPE
+
+if django.get_version() >= '4':
+    from django.utils.translation import gettext_lazy as _
+else:
+    from django.utils.translation import ugettext_lazy as _
 
 from log_reader import settings
 
 
 def get_log_files(directory):
     for (dir_path, dir_names, filenames) in os.walk(directory):
         log_files = []
```

### Comparing `django-log-reader-1.1.5/log_reader/settings.py` & `django-log-reader-1.1.6/log_reader/settings.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.5/log_reader/templates/log_reader/admin/change_list.html` & `django-log-reader-1.1.6/log_reader/templates/log_reader/admin/change_list.html`

 * *Files identical despite different names*

