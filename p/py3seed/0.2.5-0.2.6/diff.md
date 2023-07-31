# Comparing `tmp/py3seed-0.2.5.tar.gz` & `tmp/py3seed-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.5.tar", last modified: Mon Jul 31 01:41:22 2023, max compression
+gzip compressed data, was "py3seed-0.2.6.tar", last modified: Mon Jul 31 12:57:18 2023, max compression
```

## Comparing `py3seed-0.2.5.tar` & `py3seed-0.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.989797 py3seed-0.2.5/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.5/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 01:41:22.989955 py3seed-0.2.5/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.5/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.5/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-31 01:41:22.990884 py3seed-0.2.5/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.5/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.957958 py3seed-0.2.5/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.975713 py3seed-0.2.5/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.5/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.5/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.5/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.5/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.982360 py3seed-0.2.5/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.5/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    21745 2023-07-31 01:40:37.000000 py3seed-0.2.5/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.5/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.5/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.5/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.5/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.5/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.5/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.5/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.5/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.980148 py3seed-0.2.5/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-31 01:41:22.000000 py3seed-0.2.5/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 01:41:22.989203 py3seed-0.2.5/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.5/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6731 2023-07-28 10:31:34.000000 py3seed-0.2.5/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.5/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.5/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.5/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.452658 py3seed-0.2.6/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.6/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 12:57:18.452846 py3seed-0.2.6/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.6/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.6/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-31 12:57:18.453701 py3seed-0.2.6/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.6/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.414588 py3seed-0.2.6/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.441412 py3seed-0.2.6/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.6/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.6/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.6/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.6/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.445358 py3seed-0.2.6/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.6/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    23008 2023-07-31 12:55:44.000000 py3seed-0.2.6/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.6/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.6/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.6/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.6/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-31 04:55:20.000000 py3seed-0.2.6/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.6/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.6/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.6/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.444293 py3seed-0.2.6/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-31 12:57:18.000000 py3seed-0.2.6/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-31 12:57:18.452021 py3seed-0.2.6/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.6/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6832 2023-07-31 12:50:18.000000 py3seed-0.2.6/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.6/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.6/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.6/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.5/LICENSE` & `py3seed-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/PKG-INFO` & `py3seed-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.5/setup.cfg` & `py3seed-0.2.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.5
+version = 0.2.6
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.5/src/py3seed/__init__.py` & `py3seed-0.2.6/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/__main__.py` & `py3seed-0.2.6/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/admin.py` & `py3seed-0.2.6/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/cachesupport.py` & `py3seed-0.2.6/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/commands/gen.py` & `py3seed-0.2.6/src/py3seed/commands/gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,32 +130,46 @@
         #
         return s
 
     def last_name(path):
         """ Get last name from path, e.g, user.name -> name, user -> user. """
         return path.split('.')[-1]
 
-    def fields(layout, matcher=None):
-        """ Get the first field matched. """
-        _fields = parse_layout_fields(layout)
+    def fields(layout_or_schema, matcher=None):
+        """ Get the matched fields from layout or schema. """
+        if isinstance(layout_or_schema, list):  # layout is [[{}, ...], ...]
+            _fields = parse_layout_fields(layout_or_schema)
+        elif isinstance(layout_or_schema, dict):  # schema is dict {type: 'object', properties: {name, type, ... }}
+            _fields = list(layout_or_schema['properties'].keys())
+        else:
+            raise ValueError(f'Unsupported type to calculate fields: {type(layout_or_schema)}')
+        #
         if matcher:
-            f = match_field(_fields, matcher)
-            return f
+            # NOTE: in jinja2, you need to escape regex str, e.g, \w -> \\w
+            # e.g, {{ set title_fields = layout|fields('title|name|\\w*name') }}
+            matcher = re.compile(matcher if matcher.startswith('(') else f'({matcher})')
+            return [f for f in _fields if matcher.match(f)]
         else:
-            return _fields[0] if _fields else None
+            return _fields
+
+    def field(layout_or_schema, matcher=None):
+        """ Get the first matched field from layout or schema. """
+        fields_ = fields(layout_or_schema, matcher)
+        return fields_[0] if fields_ else None
 
     env.filters['split'] = split
     env.filters['items'] = items
     env.filters['keys'] = keys
     env.filters['quote'] = quote
     env.filters['basename'] = basename
     env.filters['urlquote'] = urlquote
     env.filters['right'] = right
     env.filters['last_name'] = last_name
     env.filters['fields'] = fields
+    env.filters['field'] = field
     #
     return env
 
 
 def _gen(ds: str = None):
     """ Gen. """
     include_domains = [d.strip() for d in ds.split(',')] if ds else []
@@ -228,15 +242,15 @@
                 views.append({
                     'model': model_setting,
                     'blueprint': blueprint,
                     'domains': domains,
                     'action': l['action'],
                     'params': l['params'],
                     'rows': l['rows'],
-                    'layout': layout,
+                    'layout': layout,  # NOTE: layout stores the original layout string, parsed layout is stored in rows
                     **generate_names(name)
                 })
             # Views may be empty if no views match
             if not views:
                 continue
             #
             model_setting['views'] = views
@@ -296,15 +310,15 @@
         logger.info(f'Blueprints:')
         for bp in blueprints:  # Blueprints
             bp_name = bp['name']
             logger.info(f'{bp_name}/')
             for v in bp['views']:  # Views
                 v_name = v['name']
                 logger.info(f'  {v_name}')
-        #
+        # models & blueprints can be used in all templates
         context = {
             'models': model_settings,
             'blueprints': blueprints,
         }
         #
         # Do generation logic for each includes
         #
@@ -326,33 +340,36 @@
       {{#models}}
       {{model}}
     """
     t_path = os.path.join(t_base, name)
     t_name = ''.join(name.split())  # Remove all the whitespace chars from name
     out_names = [t_name]  # if no matched list or varible syntax, process directly
     logger.debug(f'Render {t_path} -> {out_names}')
+    # For each value v in out_values, will put v into context using out_key
     out_key, out_values = None, []
     #
     # Check list syntax, i.e, {{#name}}
     # This syntax iterate over every item of the list; do not generate anything if empty list and false value
     #
     match_list = re.search('(\\{\\{#[a-zA-Z._]+\\}\\})', t_name)
     if match_list:
         syntax = match_list.group(1)  # => {{#views}}
         key = syntax[3:-2]  # => views
         if key == 'blueprints':
-            out_key = '__blueprint'
+            out_key = 'blueprint'
+            # blueprints can be access at context level
             out_values = context['blueprints']
             out_names = [t_name.replace(syntax, v['name']) for v in out_values]
         elif key == 'views':
-            out_key = '__view'
-            out_values = context['__blueprint']['views']  # views under current blueprint
+            out_key = 'view'
+            # views under current blueprint
+            out_values = context['blueprint']['views']
             out_names = [t_name.replace(syntax, v['name']) for v in out_values]
         elif key == 'models':
-            out_key = '__model'
+            out_key = 'model'
             # models can be accessed at context level, NOTE: models is dict, {name: {names, schema}}}, so we use values() here
             out_values = list(context['models'].values())
             # names of blueprints/views are kebab formats because them will be used in the url directly, while modal names are always in camel case because of PEP8
             out_names = [t_name.replace(syntax, v['name_kebab']) for v in out_values]
         else:
             raise TemplateError(f'Unsupported list syntax: {syntax}')
     else:
@@ -361,20 +378,21 @@
         # This syntax return the value of the varible
         #
         match_variable = re.search('(\\{\\{[a-zA-Z._]+\\}\\})', t_name)
         if match_variable:
             syntax = match_list.group(1)
             key = syntax[2:-2]
             if key in ['blueprint', 'view']:
-                out_key == f'__{key}'
-                out_values = [context[f'__{key}']]
+                out_key = key
+                out_values = [context[out_key]]
                 out_names = [t_name.replace(syntax, v['name']) for v in out_values]
             elif key in ['model']:
-                out_key == f'__{key}'
-                out_values = [context[f'__{key}']]
+                out_key = key
+                out_values = [context[out_key]]
+                # Output folder/file names are in kebab format, but not camel case
                 out_names = [t_name.replace(syntax, v['name_kebab']) for v in out_values]
             else:
                 raise TemplateError(f'Unsupported varible syntax: {syntax}')
     #
     # Render folder recursively
     #
     if os.path.isdir(t_path):
@@ -391,23 +409,26 @@
             if not os.path.exists(o_path):
                 os.mkdir(o_path)
             # if output is not the same as template, need to copy includes folder
             t_includes = os.path.join(t_path, INCLUDES_FOLDER)
             o_includes = os.path.join(o_path, INCLUDES_FOLDER)
             if t_path != o_path and os.path.exists(t_includes):
                 logger.debug(f'Copy {t_includes} -> {o_includes}')
-                shutil.copytree(t_includes, o_includes)
-            # Can use this context value in sub folders and files
-            if out_values:
+                shutil.copytree(t_includes, o_includes, dirs_exist_ok=True)
+            # Can use this context value for inner templates
+            if out_key:
                 context[out_key] = out_values[i]
             # Render recursively
             for f in sorted(os.listdir(t_path)):
                 # Only process files
                 if os.path.isfile(os.path.join(t_path, f)):
                     _recursive_render(t_path, o_path, f, context, env)
+            # Remove out_key from context
+            if out_key:
+                del context[out_key]
             #
             if os.path.exists(o_includes):
                 shutil.rmtree(o_includes)
     #
     # Render file
     #
     else:
@@ -434,15 +455,14 @@
                 shutil.copyfile(t_path, o_path)
         # Change working folder to ., so that jinja2 works ok
         abs_o_base = os.path.abspath(o_base)
         with work_in(abs_o_base):
             logger.info(f'Working at {abs_o_base}')
             # Set jinja2's path
             env.loader = FileSystemLoader('.')
-            o_context = {k: v for k, v in context.items() if not k.startswith('__')}
             #
             for i, o_name in enumerate(out_names):
                 o_file_raw = o_name.replace('.jinja2', '')
                 #
                 # AutoMerge
                 # Check if output with additional suffix exsit, if yes, go into below merging logic, otherwise, render(overwrite) directly
                 #
@@ -464,34 +484,33 @@
                     o_file = o_file_0
                 elif os.path.exists(o_file_1):
                     if os.path.exists(o_file_111):
                         logger.warning(f'Please solve last merging conflicts of {o_file_raw}')
                         continue
                     # THIS, copy from exsiting file
                     shutil.copyfile(o_file_raw, o_file_11)
-                    shutil.copymode(o_file_raw, o_file_11)
                     # OTHER, newly genearted file
                     o_file = o_file_111
                 else:
                     o_file = o_file_raw
                 #
                 logger.info(f'Render {o_file}')
-                # Remove __ so that object can be accessed in template
+                # Push current key to context
                 if out_key:
-                    o_context[out_key[2:]] = out_values[i]
+                    context[out_key] = out_values[i]
                 #
                 # Render file
                 #
                 try:
                     tmpl = env.get_template(o_name)
                 except TemplateSyntaxError as exception:
                     exception.translated = False
                     raise
                 #
-                rendered = tmpl.render(**o_context)
+                rendered = tmpl.render(**context)
                 with open(o_file, 'w', encoding='utf-8') as f:
                     f.write(rendered)
                 #
                 # Perform 3-way merge
                 #
                 if os.path.exists(o_file_1):
                     logger.info(f'Perform 3-way merge of {o_file_raw}')
@@ -514,14 +533,17 @@
                     if '=======' in merged:
                         logger.warning(f'Please solve merging conflicts of {o_file_raw}')
                     else:
                         # Rename .111 to .1 for next merging
                         os.rename(o_file_111, o_file_1)
                         # Remove .11
                         os.remove(o_file_11)
+                # Remove out_key from context
+                if out_key:
+                    del context[out_key]
                 # Remove template file
                 if t_path != os.path.join(o_base, o_name):
                     os.remove(o_name)
 
 
 def main(args: List[str]) -> bool:
     """ Main. """
```

### Comparing `py3seed-0.2.5/src/py3seed/error.py` & `py3seed-0.2.6/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/inflection.py` & `py3seed-0.2.6/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/log.py` & `py3seed-0.2.6/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/merge3.py` & `py3seed-0.2.6/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/model.py` & `py3seed-0.2.6/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/mongosupport.py` & `py3seed-0.2.6/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/utils.py` & `py3seed-0.2.6/src/py3seed/utils.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed/websupport.py` & `py3seed-0.2.6/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.6/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.5/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.6/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/tests/test_cachesupport.py` & `py3seed-0.2.6/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/tests/test_gen.py` & `py3seed-0.2.6/tests/test_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,7 +222,9 @@
 UserStatus: {'normal': 'Normal', 'rejected': 'Rejected'},
 UserRole: {1: 'Member', 2: 'Editor', 9: 'Admin'},
 }
 '''
     # global functions
     env_txt = open('www/templates/public/env.txt', encoding='utf-8').read()
     assert 'iamhere.html: True' in env_txt
+    assert 'User title fields: [\'name\']' in env_txt
+    assert 'User title field: name' in env_txt
```

### Comparing `py3seed-0.2.5/tests/test_merge3.py` & `py3seed-0.2.6/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/tests/test_model.py` & `py3seed-0.2.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.5/tests/test_mongosupport.py` & `py3seed-0.2.6/tests/test_mongosupport.py`

 * *Files identical despite different names*

