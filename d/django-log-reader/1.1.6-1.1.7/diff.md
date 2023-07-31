# Comparing `tmp/django-log-reader-1.1.6.tar.gz` & `tmp/django-log-reader-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-log-reader-1.1.6.tar", last modified: Mon Jul 31 07:54:06 2023, max compression
+gzip compressed data, was "django-log-reader-1.1.7.tar", last modified: Mon Jul 31 11:04:42 2023, max compression
```

## Comparing `django-log-reader-1.1.6.tar` & `django-log-reader-1.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.216064 django-log-reader-1.1.6/
--rw-r--r--   0 imankarimi   (501) staff       (20)     1068 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/LICENSE
--rw-r--r--   0 imankarimi   (501) staff       (20)      138 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/MANIFEST.in
--rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 07:54:06.215266 django-log-reader-1.1.6/PKG-INFO
--rw-r--r--   0 imankarimi   (501) staff       (20)     2222 2021-11-11 07:08:11.000000 django-log-reader-1.1.6/README.md
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.145530 django-log-reader-1.1.6/django_log_reader.egg-info/
--rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/PKG-INFO
--rw-r--r--   0 imankarimi   (501) staff       (20)      672 2023-07-31 07:54:06.000000 django-log-reader-1.1.6/django_log_reader.egg-info/SOURCES.txt
--rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/dependency_links.txt
--rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/not-zip-safe
--rw-r--r--   0 imankarimi   (501) staff       (20)       11 2023-07-31 07:54:05.000000 django-log-reader-1.1.6/django_log_reader.egg-info/top_level.txt
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.160813 django-log-reader-1.1.6/docs/
--rw-r--r--   0 imankarimi   (501) staff       (20)     1061 2021-11-10 13:29:08.000000 django-log-reader-1.1.6/docs/index.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)     1432 2021-11-11 07:08:11.000000 django-log-reader-1.1.6/docs/installation.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)      546 2021-11-10 13:29:08.000000 django-log-reader-1.1.6/docs/requirements.rst
--rw-r--r--   0 imankarimi   (501) staff       (20)      541 2021-11-10 13:29:08.000000 django-log-reader-1.1.6/docs/run-and-demo.rst
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.197737 django-log-reader-1.1.6/log_reader/
--rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/__init__.py
--rw-r--r--   0 imankarimi   (501) staff       (20)     1341 2021-11-11 07:32:55.000000 django-log-reader-1.1.6/log_reader/admin.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      183 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/apps.py
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.200723 django-log-reader-1.1.6/log_reader/migrations/
--rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/migrations/__init__.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      530 2023-07-31 07:44:51.000000 django-log-reader-1.1.6/log_reader/models.py
--rw-r--r--   0 imankarimi   (501) staff       (20)      954 2021-11-11 07:08:11.000000 django-log-reader-1.1.6/log_reader/settings.py
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.075829 django-log-reader-1.1.6/log_reader/static/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.080953 django-log-reader-1.1.6/log_reader/static/log_reader/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.201631 django-log-reader-1.1.6/log_reader/static/log_reader/css/
--rw-r--r--   0 imankarimi   (501) staff       (20)      165 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/static/log_reader/css/log_reader.css
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.206821 django-log-reader-1.1.6/log_reader/static/log_reader/js/
--rw-r--r--   0 imankarimi   (501) staff       (20)      367 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/static/log_reader/js/log_reader.js
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.086167 django-log-reader-1.1.6/log_reader/templates/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.086826 django-log-reader-1.1.6/log_reader/templates/log_reader/
-drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 07:54:06.210309 django-log-reader-1.1.6/log_reader/templates/log_reader/admin/
--rw-r--r--   0 imankarimi   (501) staff       (20)     4273 2021-11-10 20:56:19.000000 django-log-reader-1.1.6/log_reader/templates/log_reader/admin/change_list.html
--rw-r--r--   0 imankarimi   (501) staff       (20)       60 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/tests.py
--rw-r--r--   0 imankarimi   (501) staff       (20)     1661 2023-07-31 07:44:51.000000 django-log-reader-1.1.6/log_reader/utils.py
--rw-r--r--   0 imankarimi   (501) staff       (20)       63 2021-10-12 17:38:53.000000 django-log-reader-1.1.6/log_reader/views.py
--rw-r--r--   0 imankarimi   (501) staff       (20)       38 2023-07-31 07:54:06.216334 django-log-reader-1.1.6/setup.cfg
--rw-r--r--   0 imankarimi   (501) staff       (20)     1476 2023-07-31 07:54:00.000000 django-log-reader-1.1.6/setup.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.854853 django-log-reader-1.1.7/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1068 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/LICENSE
+-rw-r--r--   0 imankarimi   (501) staff       (20)      138 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/MANIFEST.in
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 11:04:42.853841 django-log-reader-1.1.7/PKG-INFO
+-rw-r--r--   0 imankarimi   (501) staff       (20)     2222 2021-11-11 07:08:11.000000 django-log-reader-1.1.7/README.md
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.827394 django-log-reader-1.1.7/django_log_reader.egg-info/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4095 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/PKG-INFO
+-rw-r--r--   0 imankarimi   (501) staff       (20)      672 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 imankarimi   (501) staff       (20)        1 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/not-zip-safe
+-rw-r--r--   0 imankarimi   (501) staff       (20)       11 2023-07-31 11:04:42.000000 django-log-reader-1.1.7/django_log_reader.egg-info/top_level.txt
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.832099 django-log-reader-1.1.7/docs/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1061 2021-11-10 13:29:08.000000 django-log-reader-1.1.7/docs/index.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1432 2021-11-11 07:08:11.000000 django-log-reader-1.1.7/docs/installation.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)      546 2021-11-10 13:29:08.000000 django-log-reader-1.1.7/docs/requirements.rst
+-rw-r--r--   0 imankarimi   (501) staff       (20)      541 2021-11-10 13:29:08.000000 django-log-reader-1.1.7/docs/run-and-demo.rst
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.843794 django-log-reader-1.1.7/log_reader/
+-rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/__init__.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1408 2023-07-31 11:01:51.000000 django-log-reader-1.1.7/log_reader/admin.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      183 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/apps.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.845095 django-log-reader-1.1.7/log_reader/migrations/
+-rw-r--r--   0 imankarimi   (501) staff       (20)        0 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/migrations/__init__.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      530 2023-07-31 07:44:51.000000 django-log-reader-1.1.7/log_reader/models.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)      954 2021-11-11 07:08:11.000000 django-log-reader-1.1.7/log_reader/settings.py
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.813908 django-log-reader-1.1.7/log_reader/static/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.814432 django-log-reader-1.1.7/log_reader/static/log_reader/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.846089 django-log-reader-1.1.7/log_reader/static/log_reader/css/
+-rw-r--r--   0 imankarimi   (501) staff       (20)      220 2023-07-31 11:00:51.000000 django-log-reader-1.1.7/log_reader/static/log_reader/css/log_reader.css
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.847478 django-log-reader-1.1.7/log_reader/static/log_reader/js/
+-rw-r--r--   0 imankarimi   (501) staff       (20)      367 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/static/log_reader/js/log_reader.js
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.814860 django-log-reader-1.1.7/log_reader/templates/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.815009 django-log-reader-1.1.7/log_reader/templates/log_reader/
+drwxr-xr-x   0 imankarimi   (501) staff       (20)        0 2023-07-31 11:04:42.852132 django-log-reader-1.1.7/log_reader/templates/log_reader/admin/
+-rw-r--r--   0 imankarimi   (501) staff       (20)     4767 2023-07-31 11:01:03.000000 django-log-reader-1.1.7/log_reader/templates/log_reader/admin/change_list.html
+-rw-r--r--   0 imankarimi   (501) staff       (20)       60 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/tests.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1965 2023-07-31 11:02:24.000000 django-log-reader-1.1.7/log_reader/utils.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)       63 2021-10-12 17:38:53.000000 django-log-reader-1.1.7/log_reader/views.py
+-rw-r--r--   0 imankarimi   (501) staff       (20)       38 2023-07-31 11:04:42.855151 django-log-reader-1.1.7/setup.cfg
+-rw-r--r--   0 imankarimi   (501) staff       (20)     1476 2023-07-31 11:03:50.000000 django-log-reader-1.1.7/setup.py
```

### Comparing `django-log-reader-1.1.6/LICENSE` & `django-log-reader-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/PKG-INFO` & `django-log-reader-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-reader
-Version: 1.1.6
+Version: 1.1.7
 Summary: Read & Download log files on the admin page
 Home-page: https://github.com/imankarimi/django-log-reader
 Author: Iman Karimi
 Author-email: imankarimi.mail@gmail.com
 License: MIT License
 Description: # Django Log Reader
         **Django Log Reader** allows you to read &amp; download log files on the admin page.
```

### Comparing `django-log-reader-1.1.6/README.md` & `django-log-reader-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/django_log_reader.egg-info/PKG-INFO` & `django-log-reader-1.1.7/django_log_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-reader
-Version: 1.1.6
+Version: 1.1.7
 Summary: Read & Download log files on the admin page
 Home-page: https://github.com/imankarimi/django-log-reader
 Author: Iman Karimi
 Author-email: imankarimi.mail@gmail.com
 License: MIT License
 Description: # Django Log Reader
         **Django Log Reader** allows you to read &amp; download log files on the admin page.
```

### Comparing `django-log-reader-1.1.6/django_log_reader.egg-info/SOURCES.txt` & `django-log-reader-1.1.7/django_log_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/docs/index.rst` & `django-log-reader-1.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/docs/installation.rst` & `django-log-reader-1.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/docs/requirements.rst` & `django-log-reader-1.1.7/docs/requirements.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/docs/run-and-demo.rst` & `django-log-reader-1.1.7/docs/run-and-demo.rst`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/log_reader/admin.py` & `django-log-reader-1.1.7/log_reader/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         info = self.model._meta.app_label, self.model._meta.module_name
         return [
             path(r'', self.admin_site.admin_view(self.changelist_view), name='%s_%s_changelist' % info),
         ]
 
     def changelist_view(self, request, extra_context=None):
         filename = request.GET.get('file_name', settings.LOG_READER_DEFAULT_FILE)
-        is_valid, file_contents = read_file_lines(file_name=filename)
+        search = request.GET.get('q', None) or None
+        is_valid, file_contents = read_file_lines(file_name=filename, search=search)
         if not is_valid:
             self.message_user(request, file_contents, level=messages.ERROR)
         log_files = get_log_files(settings.LOG_READER_DIR_PATH)
 
         context = dict(
             self.admin_site.each_context(request),
             log_files=log_files,
```

### Comparing `django-log-reader-1.1.6/log_reader/models.py` & `django-log-reader-1.1.7/log_reader/models.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/log_reader/settings.py` & `django-log-reader-1.1.7/log_reader/settings.py`

 * *Files identical despite different names*

### Comparing `django-log-reader-1.1.6/log_reader/templates/log_reader/admin/change_list.html` & `django-log-reader-1.1.7/log_reader/templates/log_reader/admin/change_list.html`

 * *Files 15% similar despite different names*

```diff
@@ -26,14 +26,21 @@
 {% block content %}
     <div id="content-main">
         <div class="module filtered" id="changelist">
             {% if django_version >= '3' %}
                 <div class="changelist-form-container">{% endif %}
             {% if file_contents %}
                 <div id="toolbar">
+                    <form id="changelist-search" method="get">
+                        <div><!-- DIV needed for valid HTML -->
+                            <label for="searchbar"><img src="{% static "admin/img/search.svg" %}" alt="Search"></label>
+                            <input type="text" size="40" name="q" value="{{ request.GET.q }}" id="searchbar" autofocus="">
+                            <input type="submit" value="Search">
+                        </div>
+                    </form>
                     <button id="DownloadLogFile" type="submit">Download</button>
                 </div>
             {% endif %}
 
             {% if file_contents %}
                 <form id="changelist-form" method="post" novalidate=""{% if django_version < '3' %} style="width: auto;margin-right: 280px;" {% endif %}>
                     <div class="results">
```

### Comparing `django-log-reader-1.1.6/log_reader/utils.py` & `django-log-reader-1.1.7/log_reader/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,26 +20,35 @@
         log_files = []
         all_files = list(filter(lambda x: x.find('~') == -1, filenames))
         log_files.extend([x for x in all_files if fnmatch(x, settings.LOG_READER_FILES_PATTERN) and x not in settings.LOG_READER_EXCLUDE_FILES])
         return list(set(log_files))
     return []
 
 
-def read_file_lines(file_name):
+def read_file_lines(file_name, search=None):
     if file_name not in get_log_files(settings.LOG_READER_DIR_PATH):
         return False, _("%s file, not found. Please try again." % file_name)
 
     try:
         file_path = '%s/%s' % (settings.LOG_READER_DIR_PATH, file_name)
-        result = subprocess.run(
-            ['tail', '-%s' % settings.LOG_READER_MAX_READ_LINES, file_path],
-            stdout=PIPE,
-            stderr=PIPE,
-            encoding="utf8",
-        )
+
+        if search:
+            result = subprocess.run(
+                ['grep', '-m %s' % settings.LOG_READER_MAX_READ_LINES, search, file_path],
+                stdout=PIPE,
+                stderr=PIPE,
+                encoding="utf8",
+            )
+        else:
+            result = subprocess.run(
+                ['tail', '-%s' % settings.LOG_READER_MAX_READ_LINES, file_path],
+                stdout=PIPE,
+                stderr=PIPE,
+                encoding="utf8",
+            )
         content = repr(result.stdout) if result.stdout else None
     except Exception as e:
         return False, str(e)
 
     return True, split_file_content(content)
```

### Comparing `django-log-reader-1.1.6/setup.py` & `django-log-reader-1.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-log-reader',
-    version='1.1.6',
+    version='1.1.7',
     zip_safe=False,
     packages=find_packages(),
     include_package_data=True,
     description='Read & Download log files on the admin page',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/imankarimi/django-log-reader',
```

