# Comparing `tmp/django-log-reader-1.1.7.tar.gz` & `tmp/django-log-reader-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-log-reader-1.1.7.tar", last modified: Mon Jul 31 11:04:42 2023, max compression
+gzip compressed data, was "django-log-reader-1.1.8.tar", last modified: Mon Jul 31 12:01:52 2023, max compression
```

## Comparing `django-log-reader-1.1.7.tar` & `django-log-reader-1.1.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.854853 django-log-reader-1.1.7/
--rw-r--r--   0 imankarimi   (501) staff       (20)     1068 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/LICENSE
--rw-r--r--   0 imankarimi   (501) staff       (20)      138 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/MANIFEST.in
--rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 11:04:42.853841 django-log-reader-1.1.7/PKG-INFO
--rw-r--r--   0 imankarimi   (501) staff       (20)     2222 2021-11-11 07:08:11.000000 django-log-reader-1.1.7/README.md
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.827394 django-log-reader-1.1.7/django_log_reader.egg-info/
--rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/PKG-INFO
--rw-r--r--   0 imankarimi   (501) staff       (20)      672 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/SOURCES.txt
--rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/dependency_links.txt
--rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/not-zip-safe
--rw-r--r--   0 imankarimi   (501) staff       (20)       11 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/top_level.txt
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.832099 django-log-reader-1.1.7/docs/
--rw-r--r--   0 imankarimi   (501) staff       (20)     1061 2021-11-10 13:29:08.000000 django-log-reader-1.1.7/docs/index.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)     1432 2021-11-11 07:08:11.000000 django-log-reader-1.1.7/docs/installation.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)      546 2021-11-10 13:29:08.000000 django-log-reader-1.1.7/docs/requirements.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)      541 2021-11-10 13:29:08.000000 django-log-reader-1.1.7/docs/run-and-demo.rst
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.843794 django-log-reader-1.1.7/log_reader/
--rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/__init__.py
--rw-r--r--   0 imankarimi   (501) staff       (20)     1408 2023-07-31 11:01:51.000000 django-log-reader-1.1.7/log_reader/admin.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      183 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/apps.py
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.845095 django-log-reader-1.1.7/log_reader/migrations/
--rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/migrations/__init__.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      530 2023-07-31 07:44:51.000000 django-log-reader-1.1.7/log_reader/models.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      954 2021-11-11 07:08:11.000000 django-log-reader-1.1.7/log_reader/settings.py
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.813908 django-log-reader-1.1.7/log_reader/static/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.814432 django-log-reader-1.1.7/log_reader/static/log_reader/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.846089 django-log-reader-1.1.7/log_reader/static/log_reader/css/
--rw-r--r--   0 imankarimi   (501) staff       (20)      220 2023-07-31 11:00:51.000000 django-log-reader-1.1.7/log_reader/static/log_reader/css/log_reader.css
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.847478 django-log-reader-1.1.7/log_reader/static/log_reader/js/
--rw-r--r--   0 imankarimi   (501) staff       (20)      367 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/static/log_reader/js/log_reader.js
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.814860 django-log-reader-1.1.7/log_reader/templates/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.815009 django-log-reader-1.1.7/log_reader/templates/log_reader/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.852132 django-log-reader-1.1.7/log_reader/templates/log_reader/admin/
--rw-r--r--   0 imankarimi   (501) staff       (20)     4767 2023-07-31 11:01:03.000000 django-log-reader-1.1.7/log_reader/templates/log_reader/admin/change_list.html
--rw-r--r--   0 imankarimi   (501) staff       (20)       60 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/tests.py
--rw-r--r--   0 imankarimi   (501) staff       (20)     1965 2023-07-31 11:02:24.000000 django-log-reader-1.1.7/log_reader/utils.py
--rw-r--r--   0 imankarimi   (501) staff       (20)       63 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/views.py
--rw-r--r--   0 imankarimi   (501) staff       (20)       38 2023-07-31 11:04:42.855151 django-log-reader-1.1.7/setup.cfg
--rw-r--r--   0 imankarimi   (501) staff       (20)     1476 2023-07-31 11:03:50.000000 django-log-reader-1.1.7/setup.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.280640 django-log-reader-1.1.8/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1068 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/LICENSE
+-rw-r--r--   0 imankarimi   (501) staff       (20)      138 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/MANIFEST.in
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 12:01:52.269778 django-log-reader-1.1.8/PKG-INFO
+-rw-r--r--   0 imankarimi   (501) staff       (20)     2222 2021-11-11 07:08:11.000000 django-log-reader-1.1.8/README.md
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.226142 django-log-reader-1.1.8/django_log_reader.egg-info/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 12:01:52.000000 django-log-reader-1.1.8/django_log_reader.egg-info/PKG-INFO
+-rw-r--r--   0 imankarimi   (501) staff       (20)      672 2023-07-31 12:01:52.000000 django-log-reader-1.1.8/django_log_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 12:01:52.000000 django-log-reader-1.1.8/django_log_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 12:01:52.000000 django-log-reader-1.1.8/django_log_reader.egg-info/not-zip-safe
+-rw-r--r--   0 imankarimi   (501) staff       (20)       11 2023-07-31 12:01:52.000000 django-log-reader-1.1.8/django_log_reader.egg-info/top_level.txt
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.230351 django-log-reader-1.1.8/docs/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1061 2021-11-10 13:29:08.000000 django-log-reader-1.1.8/docs/index.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1432 2021-11-11 07:08:11.000000 django-log-reader-1.1.8/docs/installation.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)      546 2021-11-10 13:29:08.000000 django-log-reader-1.1.8/docs/requirements.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)      541 2021-11-10 13:29:08.000000 django-log-reader-1.1.8/docs/run-and-demo.rst
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.248671 django-log-reader-1.1.8/log_reader/
+-rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/log_reader/__init__.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1408 2023-07-31 11:01:51.000000 django-log-reader-1.1.8/log_reader/admin.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      183 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/log_reader/apps.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.252483 django-log-reader-1.1.8/log_reader/migrations/
+-rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/log_reader/migrations/__init__.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      530 2023-07-31 07:44:51.000000 django-log-reader-1.1.8/log_reader/models.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      954 2021-11-11 07:08:11.000000 django-log-reader-1.1.8/log_reader/settings.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.217530 django-log-reader-1.1.8/log_reader/static/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.218067 django-log-reader-1.1.8/log_reader/static/log_reader/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.254536 django-log-reader-1.1.8/log_reader/static/log_reader/css/
+-rw-r--r--   0 imankarimi   (501) staff       (20)      220 2023-07-31 11:00:51.000000 django-log-reader-1.1.8/log_reader/static/log_reader/css/log_reader.css
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.264379 django-log-reader-1.1.8/log_reader/static/log_reader/js/
+-rw-r--r--   0 imankarimi   (501) staff       (20)      367 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/log_reader/static/log_reader/js/log_reader.js
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.218650 django-log-reader-1.1.8/log_reader/templates/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.218873 django-log-reader-1.1.8/log_reader/templates/log_reader/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 12:01:52.265806 django-log-reader-1.1.8/log_reader/templates/log_reader/admin/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4723 2023-07-31 12:00:15.000000 django-log-reader-1.1.8/log_reader/templates/log_reader/admin/change_list.html
+-rw-r--r--   0 imankarimi   (501) staff       (20)       60 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/log_reader/tests.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1965 2023-07-31 11:02:24.000000 django-log-reader-1.1.8/log_reader/utils.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)       63 2021-10-12 17:38:53.000000 django-log-reader-1.1.8/log_reader/views.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)       38 2023-07-31 12:01:52.281444 django-log-reader-1.1.8/setup.cfg
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1476 2023-07-31 12:01:41.000000 django-log-reader-1.1.8/setup.py
```

### Comparing `django-log-reader-1.1.7/LICENSE` & `django-log-reader-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/PKG-INFO` & `django-log-reader-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-reader
-Version: 1.1.7
+Version: 1.1.8
 Summary: Read & Download log files on the admin page
 Home-page: https://github.com/imankarimi/django-log-reader
 Author: Iman Karimi
 Author-email: imankarimi.mail@gmail.com
 License: MIT License
 Description: # Django Log Reader
         **Django Log Reader** allows you to read &amp; download log files on the admin page.
```

### Comparing `django-log-reader-1.1.7/README.md` & `django-log-reader-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/django_log_reader.egg-info/PKG-INFO` & `django-log-reader-1.1.8/django_log_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-reader
-Version: 1.1.7
+Version: 1.1.8
 Summary: Read & Download log files on the admin page
 Home-page: https://github.com/imankarimi/django-log-reader
 Author: Iman Karimi
 Author-email: imankarimi.mail@gmail.com
 License: MIT License
 Description: # Django Log Reader
         **Django Log Reader** allows you to read &amp; download log files on the admin page.
```

### Comparing `django-log-reader-1.1.7/django_log_reader.egg-info/SOURCES.txt` & `django-log-reader-1.1.8/django_log_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/docs/index.rst` & `django-log-reader-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/docs/installation.rst` & `django-log-reader-1.1.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/docs/requirements.rst` & `django-log-reader-1.1.8/docs/requirements.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/docs/run-and-demo.rst` & `django-log-reader-1.1.8/docs/run-and-demo.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/log_reader/admin.py` & `django-log-reader-1.1.8/log_reader/admin.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/log_reader/models.py` & `django-log-reader-1.1.8/log_reader/models.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/log_reader/settings.py` & `django-log-reader-1.1.8/log_reader/settings.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/log_reader/templates/log_reader/admin/change_list.html` & `django-log-reader-1.1.8/log_reader/templates/log_reader/admin/change_list.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 {% block pretitle %}
     <h1>File Logs</h1>
 {% endblock %}
 
 {% block content %}
     <div id="content-main">
         <div class="module filtered" id="changelist">
-            {% if django_version >= '3' %}
-                <div class="changelist-form-container">{% endif %}
-            {% if file_contents %}
-                <div id="toolbar">
-                    <form id="changelist-search" method="get">
-                        <div><!-- DIV needed for valid HTML -->
-                            <label for="searchbar"><img src="{% static "admin/img/search.svg" %}" alt="Search"></label>
-                            <input type="text" size="40" name="q" value="{{ request.GET.q }}" id="searchbar" autofocus="">
-                            <input type="submit" value="Search">
-                        </div>
-                    </form>
+            {% if django_version >= '3' %}<div class="changelist-form-container">{% endif %}
+
+            <div id="toolbar">
+                <form id="changelist-search" method="get">
+                    <div><!-- DIV needed for valid HTML -->
+                        <label for="searchbar"><img src="{% static "admin/img/search.svg" %}" alt="Search"></label>
+                        <input type="text" size="40" name="q" value="{{ request.GET.q }}" id="searchbar" autofocus="">
+                        <input type="submit" value="Search">
+                    </div>
+                </form>
+                {% if file_contents %}
                     <button id="DownloadLogFile" type="submit">Download</button>
-                </div>
-            {% endif %}
+                {% endif %}
+            </div>
 
             {% if file_contents %}
                 <form id="changelist-form" method="post" novalidate=""{% if django_version < '3' %} style="width: auto;margin-right: 280px;" {% endif %}>
                     <div class="results">
                         <table id="result_list">
                             <thead>
                             <tr>
```

### Comparing `django-log-reader-1.1.7/log_reader/utils.py` & `django-log-reader-1.1.8/log_reader/utils.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.7/setup.py` & `django-log-reader-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-log-reader',
-    version='1.1.7',
+    version='1.1.8',
     zip_safe=False,
     packages=find_packages(),
     include_package_data=True,
     description='Read & Download log files on the admin page',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/imankarimi/django-log-reader',
```

