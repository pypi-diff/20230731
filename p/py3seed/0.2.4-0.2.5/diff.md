# Comparing `tmp/py3seed-0.2.4.tar.gz` & `tmp/py3seed-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.4.tar", last modified: Fri Jul 28 10:36:44 2023, max compression
+gzip compressed data, was "py3seed-0.2.5.tar", last modified: Mon Jul 31 01:41:22 2023, max compression
```

## Comparing `py3seed-0.2.4.tar` & `py3seed-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.795853 py3seed-0.2.4/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.4/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-28 10:36:44.796016 py3seed-0.2.4/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.4/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.4/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-28 10:36:44.796732 py3seed-0.2.4/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.4/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.773677 py3seed-0.2.4/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.787240 py3seed-0.2.4/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.4/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.4/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.4/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.4/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.790856 py3seed-0.2.4/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.4/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    21243 2023-07-28 10:28:30.000000 py3seed-0.2.4/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.4/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.4/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.4/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.4/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.4/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.4/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.4/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.4/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.789708 py3seed-0.2.4/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-28 10:36:44.000000 py3seed-0.2.4/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-28 10:36:44.795354 py3seed-0.2.4/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.4/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6731 2023-07-28 10:31:34.000000 py3seed-0.2.4/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.4/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.4/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.4/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.989797 py3seed-0.2.5/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.5/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 01:41:22.989955 py3seed-0.2.5/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.5/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.5/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-31 01:41:22.990884 py3seed-0.2.5/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.5/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.957958 py3seed-0.2.5/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.975713 py3seed-0.2.5/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.5/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.5/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.5/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.5/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.982360 py3seed-0.2.5/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.5/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    21745 2023-07-31 01:40:37.000000 py3seed-0.2.5/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.5/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.5/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.5/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.5/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.5/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.5/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.5/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.5/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.980148 py3seed-0.2.5/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.989203 py3seed-0.2.5/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.5/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6731 2023-07-28 10:31:34.000000 py3seed-0.2.5/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.5/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.5/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.5/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.4/LICENSE` & `py3seed-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/PKG-INFO` & `py3seed-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.4/setup.cfg` & `py3seed-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.4
+version = 0.2.5
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.4/src/py3seed/__init__.py` & `py3seed-0.2.5/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/__main__.py` & `py3seed-0.2.5/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/admin.py` & `py3seed-0.2.5/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/cachesupport.py` & `py3seed-0.2.5/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/commands/gen.py` & `py3seed-0.2.5/src/py3seed/commands/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,79 +41,36 @@
     # trim_blocks=True and lstrip_blocks=True -> make sure lines of {% ... %} and {# ... #} will be removed completely in render result
     # keep_trailing_newline=True -> keep trailing newline to so that you can use indent filter to include the macro with a tailing newline
     #
     # For extension, plrease refer to https://jinja.palletsprojects.com/en/3.0.x/extensions/#loopcontrols-extension
     #
     env = Environment(trim_blocks=True, lstrip_blocks=True, keep_trailing_newline=True, extensions=['jinja2.ext.loopcontrols'])
 
-    def split(value, separator):
-        """ Split a string. """
-        return value.split(separator)
-
-    def items(value):
-        """ Return items of a dict. """
-        return value.items()
-
-    def keys(value):
-        """ Return keys of a dict. """
-        return value.keys()
-
-    def quote(value):
-        """ Add single quote to value if it is str, else return its __str__. """
-        if isinstance(value, str):
-            return '\'' + value + '\''
-        else:
-            return str(value)
-
-    def basename(value):
-        """ Return file name from a path. """
-        return os.path.basename(value)
-
-    def urlquote(value, charset='utf-8'):
-        """ Url Quote. """
-        return url_quote(value, charset)
-
-    def right(s: str, width: int = 4):
-        """ Do indent, if content is not blank, add leading indent. """
-        s = filters.do_indent(s, width)
-        if s:
-            s = " " * width + s
-        #
-        return s
-
-    env.filters['split'] = split
-    env.filters['items'] = items
-    env.filters['keys'] = keys
-    env.filters['quote'] = quote
-    env.filters['basename'] = basename
-    env.filters['urlquote'] = urlquote
-    env.filters['right'] = right
-
     def update_query(**new_values):
         """ Update query. """
         args = request.args.copy()
         for key, value in new_values.items():
             args[key] = value
         return url_encode(args)
 
     def new_model(class_name):
         """ New a model by class name. """
         klass = globals()[class_name]
         return klass()
 
-    def match_field(fields, matcher):
+    def match_field(fields_, matcher):
         """ Get the first matching field from columns.
         e.g,
         - match_field(columns, 'name|title|\\w+_name')
         """
         matcher = re.compile(matcher if matcher.startswith('(') else f'({matcher})')
-        if isinstance(fields, dict):
-            fields = fields.keys()
+        if isinstance(fields_, dict):
+            fields_ = fields_.keys()
         #
-        for f in fields:
+        for f in fields_:
             if matcher.match(f):
                 return f
         # If no matching, return nothing
         return None
 
     def parse_layout_fields(layout):
         """ Get layout fields.
@@ -133,14 +90,72 @@
         return os.path.exists(fp)
 
     env.globals['update_query'] = update_query
     env.globals['new_model'] = new_model
     env.globals['match_field'] = match_field
     env.globals['parse_layout_fields'] = parse_layout_fields
     env.globals['exists'] = exists
+
+    def split(value, separator):
+        """ Split a string. """
+        return value.split(separator)
+
+    def items(value):
+        """ Return items of a dict. """
+        return value.items()
+
+    def keys(value):
+        """ Return keys of a dict. """
+        return value.keys()
+
+    def quote(value):
+        """ Add single quote to value if it is str, else return its __str__. """
+        if isinstance(value, str):
+            return '\'' + value + '\''
+        else:
+            return str(value)
+
+    def basename(value):
+        """ Return file name from a path. """
+        return os.path.basename(value)
+
+    def urlquote(value, charset='utf-8'):
+        """ Url Quote. """
+        return url_quote(value, charset)
+
+    def right(s: str, width: int = 4):
+        """ Do indent, if content is not blank, add leading indent. """
+        s = filters.do_indent(s, width)
+        if s:
+            s = ' ' * width + s
+        #
+        return s
+
+    def last_name(path):
+        """ Get last name from path, e.g, user.name -> name, user -> user. """
+        return path.split('.')[-1]
+
+    def fields(layout, matcher=None):
+        """ Get the first field matched. """
+        _fields = parse_layout_fields(layout)
+        if matcher:
+            f = match_field(_fields, matcher)
+            return f
+        else:
+            return _fields[0] if _fields else None
+
+    env.filters['split'] = split
+    env.filters['items'] = items
+    env.filters['keys'] = keys
+    env.filters['quote'] = quote
+    env.filters['basename'] = basename
+    env.filters['urlquote'] = urlquote
+    env.filters['right'] = right
+    env.filters['last_name'] = last_name
+    env.filters['fields'] = fields
     #
     return env
 
 
 def _gen(ds: str = None):
     """ Gen. """
     include_domains = [d.strip() for d in ds.split(',')] if ds else []
@@ -374,15 +389,15 @@
             #     ...
             o_path = os.path.join(o_base, o_name)
             if not os.path.exists(o_path):
                 os.mkdir(o_path)
             # if output is not the same as template, need to copy includes folder
             t_includes = os.path.join(t_path, INCLUDES_FOLDER)
             o_includes = os.path.join(o_path, INCLUDES_FOLDER)
-            if t_path != o_path  and os.path.exists(t_includes):
+            if t_path != o_path and os.path.exists(t_includes):
                 logger.debug(f'Copy {t_includes} -> {o_includes}')
                 shutil.copytree(t_includes, o_includes)
             # Can use this context value in sub folders and files
             if out_values:
                 context[out_key] = out_values[i]
             # Render recursively
             for f in sorted(os.listdir(t_path)):
```

### Comparing `py3seed-0.2.4/src/py3seed/error.py` & `py3seed-0.2.5/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/inflection.py` & `py3seed-0.2.5/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/log.py` & `py3seed-0.2.5/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/merge3.py` & `py3seed-0.2.5/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/model.py` & `py3seed-0.2.5/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/mongosupport.py` & `py3seed-0.2.5/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/utils.py` & `py3seed-0.2.5/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed/websupport.py` & `py3seed-0.2.5/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.5/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.4/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.5/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/tests/test_cachesupport.py` & `py3seed-0.2.5/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/tests/test_gen.py` & `py3seed-0.2.5/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/tests/test_merge3.py` & `py3seed-0.2.5/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/tests/test_model.py` & `py3seed-0.2.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.4/tests/test_mongosupport.py` & `py3seed-0.2.5/tests/test_mongosupport.py`

 * *Files identical despite different names*

