# Comparing `tmp/apisql-0.2.9.tar.gz` & `tmp/apisql-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apisql-0.2.9.tar", last modified: Thu Jul 27 09:13:49 2023, max compression
+gzip compressed data, was "apisql-0.3.0.tar", last modified: Mon Jul 31 11:06:12 2023, max compression
```

## Comparing `apisql-0.2.9.tar` & `apisql-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.363555 apisql-0.2.9/
--rw-r--r--   0 adam       (501) staff       (20)     1067 2021-06-14 07:10:44.000000 apisql-0.2.9/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.2.9/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.2.9/Makefile
--rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-27 09:13:49.363738 apisql-0.2.9/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.2.9/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.357478 apisql-0.2.9/apisql/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-07-27 08:59:13.000000 apisql-0.2.9/apisql/VERSION
--rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.2.9/apisql/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     5092 2023-07-27 08:58:47.000000 apisql-0.2.9/apisql/blueprint.py
--rw-r--r--   0 adam       (501) staff       (20)     4858 2022-09-07 07:34:48.000000 apisql-0.2.9/apisql/controllers.py
--rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.2.9/apisql/logger.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.362765 apisql-0.2.9/apisql/utils/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.2.9/apisql/utils/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.2.9/apisql/utils/file_maker.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.361737 apisql-0.2.9/apisql.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      380 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.2.9/apisql.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)      156 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-07-27 09:13:49.364367 apisql-0.2.9/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1815 2021-06-15 10:19:05.000000 apisql-0.2.9/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.036442 apisql-0.3.0/
+-rw-r--r--   0 adam       (501) staff       (20)     1067 2021-06-14 07:10:44.000000 apisql-0.3.0/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.3.0/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.3.0/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:06:12.036659 apisql-0.3.0/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.3.0/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.030226 apisql-0.3.0/apisql/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-07-31 11:04:34.000000 apisql-0.3.0/apisql/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.3.0/apisql/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     5421 2023-07-31 11:04:14.000000 apisql-0.3.0/apisql/blueprint.py
+-rw-r--r--   0 adam       (501) staff       (20)     4858 2022-09-07 07:34:48.000000 apisql-0.3.0/apisql/controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.3.0/apisql/logger.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.035611 apisql-0.3.0/apisql/utils/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.3.0/apisql/utils/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.3.0/apisql/utils/file_maker.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.034489 apisql-0.3.0/apisql.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      380 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.3.0/apisql.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)      156 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-07-31 11:06:12.037349 apisql-0.3.0/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1815 2021-06-15 10:19:05.000000 apisql-0.3.0/setup.py
```

### Comparing `apisql-0.2.9/LICENSE` & `apisql-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apisql-0.2.9/PKG-INFO` & `apisql-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apisql
-Version: 0.2.9
+Version: 0.3.0
 Summary: A flask blueprint providing a read-lny API for querying RDBMS
 Home-page: https://github.com/dataspot/apisql
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apisql-0.2.9/README.md` & `apisql-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `apisql-0.2.9/apisql/blueprint.py` & `apisql-0.3.0/apisql/blueprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 MAX_ROWS = int(os.environ.get('APISQL__MAX_ROWS', 100))
 CONNECTION_STRING = os.environ.get('APISQL__DATABASE_URL')
 
 
 class APISQLBlueprint(Blueprint):
 
-    def __init__(self, connection_string=CONNECTION_STRING, engine=None, max_rows=MAX_ROWS, debug=False):
+    def __init__(self, connection_string=CONNECTION_STRING, engine=None, max_rows=MAX_ROWS, debug=False, cache=None):
         super().__init__('apisql', 'apisql')
         self.controllers = Controllers(
             connection_string, max_rows, debug, engine
         )
         if debug:
             logger.setLevel(logging.DEBUG)
         else:
@@ -38,14 +38,15 @@
         )
         self.add_url_rule(
             '/download',
             'download',
             self.download,
             methods=['GET', 'POST']
         )
+        self.cache = cache
 
     def query(self):
         results = dict(total=0, rows=[])
         if not self.detect_bot():
             try:
                 num_rows = int(request.values.get('num_rows', self.max_rows))
                 page_size = int(request.values.get('page_size', num_rows))
@@ -53,15 +54,21 @@
             except Exception:
                 abort(400)
             sql = request.values.get('query')
             try:
                 sql = codecs.decode(sql.encode('ascii'), 'base64').decode('utf8')
             except Exception:
                 pass
-            results = self.controllers.query_db(sql, num_rows=num_rows, page_size=page_size, page=page)
+            key = '::'.join([sql, str(num_rows), str(page_size), str(page)])
+            if self.cache is not None:
+                results = self.cache.get(key)
+            if results is None:
+                results = self.controllers.query_db(sql, num_rows=num_rows, page_size=page_size, page=page)
+                if self.cache is not None:
+                    self.cache.set(key, results)
         return jsonpify(results)
 
     def download(self):
         format = request.values.get('format', 'csv')
 
         file_name = request.values.get('filename')
         # Create a default value here in case this parameter is not provided
```

### Comparing `apisql-0.2.9/apisql/controllers.py` & `apisql-0.3.0/apisql/controllers.py`

 * *Files identical despite different names*

### Comparing `apisql-0.2.9/apisql/utils/file_maker.py` & `apisql-0.3.0/apisql/utils/file_maker.py`

 * *Files identical despite different names*

### Comparing `apisql-0.2.9/apisql.egg-info/PKG-INFO` & `apisql-0.3.0/apisql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apisql
-Version: 0.2.9
+Version: 0.3.0
 Summary: A flask blueprint providing a read-lny API for querying RDBMS
 Home-page: https://github.com/dataspot/apisql
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apisql-0.2.9/setup.py` & `apisql-0.3.0/setup.py`

 * *Files identical despite different names*

