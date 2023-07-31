# Comparing `tmp/apisql-0.3.0.tar.gz` & `tmp/apisql-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apisql-0.3.0.tar", last modified: Mon Jul 31 11:06:12 2023, max compression
+gzip compressed data, was "apisql-0.3.1.tar", last modified: Mon Jul 31 11:12:47 2023, max compression
```

## Comparing `apisql-0.3.0.tar` & `apisql-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.036442 apisql-0.3.0/
--rw-r--r--   0 adam       (501) staff       (20)     1067 2021-06-14 07:10:44.000000 apisql-0.3.0/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.3.0/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.3.0/Makefile
--rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:06:12.036659 apisql-0.3.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.3.0/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.030226 apisql-0.3.0/apisql/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-07-31 11:04:34.000000 apisql-0.3.0/apisql/VERSION
--rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.3.0/apisql/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     5421 2023-07-31 11:04:14.000000 apisql-0.3.0/apisql/blueprint.py
--rw-r--r--   0 adam       (501) staff       (20)     4858 2022-09-07 07:34:48.000000 apisql-0.3.0/apisql/controllers.py
--rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.3.0/apisql/logger.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.035611 apisql-0.3.0/apisql/utils/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.3.0/apisql/utils/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.3.0/apisql/utils/file_maker.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:06:12.034489 apisql-0.3.0/apisql.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      380 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.3.0/apisql.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)      156 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-31 11:06:11.000000 apisql-0.3.0/apisql.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-07-31 11:06:12.037349 apisql-0.3.0/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1815 2021-06-15 10:19:05.000000 apisql-0.3.0/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:12:47.312764 apisql-0.3.1/
+-rw-r--r--   0 adam       (501) staff       (20)     1067 2021-06-14 07:10:44.000000 apisql-0.3.1/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.3.1/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.3.1/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:12:47.312935 apisql-0.3.1/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.3.1/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:12:47.307927 apisql-0.3.1/apisql/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-07-31 11:12:26.000000 apisql-0.3.1/apisql/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.3.1/apisql/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     5421 2023-07-31 11:04:14.000000 apisql-0.3.1/apisql/blueprint.py
+-rw-r--r--   0 adam       (501) staff       (20)     4876 2023-07-31 11:12:08.000000 apisql-0.3.1/apisql/controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.3.1/apisql/logger.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:12:47.312062 apisql-0.3.1/apisql/utils/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.3.1/apisql/utils/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.3.1/apisql/utils/file_maker.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-31 11:12:47.311283 apisql-0.3.1/apisql.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-31 11:12:47.000000 apisql-0.3.1/apisql.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      380 2023-07-31 11:12:47.000000 apisql-0.3.1/apisql.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-31 11:12:47.000000 apisql-0.3.1/apisql.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.3.1/apisql.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)      156 2023-07-31 11:12:47.000000 apisql-0.3.1/apisql.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-31 11:12:47.000000 apisql-0.3.1/apisql.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-07-31 11:12:47.313570 apisql-0.3.1/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1815 2023-07-31 11:11:42.000000 apisql-0.3.1/setup.py
```

### Comparing `apisql-0.3.0/LICENSE` & `apisql-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apisql-0.3.0/PKG-INFO` & `apisql-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apisql
-Version: 0.3.0
+Version: 0.3.1
 Summary: A flask blueprint providing a read-lny API for querying RDBMS
 Home-page: https://github.com/dataspot/apisql
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apisql-0.3.0/README.md` & `apisql-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `apisql-0.3.0/apisql/blueprint.py` & `apisql-0.3.1/apisql/blueprint.py`

 * *Files identical despite different names*

### Comparing `apisql-0.3.0/apisql/controllers.py` & `apisql-0.3.1/apisql/controllers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import math
 from decimal import Decimal
 from datetime import date
 from backports.cached_property import cached_property
 from itertools import islice
 
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, text
 
 from .logger import logger
 
 
 class Controllers():
 
     FIELD_RE = re.compile('<([-a-z()_]+)$')
@@ -43,25 +43,25 @@
         except Exception:
             logger.exception('EXC')
             raise
 
     def query_db(self, query_str, num_rows, page_size, page):
         try:
             with self.engine.connect() as connection:
-                count_query = "select count(1) from (%s) s" % query_str
+                count_query = text("select count(1) from (%s) s" % query_str)
                 logger.debug('executing %r', count_query)
                 count = connection.execute(count_query).fetchone()[0]
                 logger.debug('count %r', count)
 
                 num_rows = min(num_rows, self.max_rows, page_size)
                 pages = math.ceil(count / num_rows)
                 page = min(page, pages-1)
                 page = max(page, 0)
                 offset = page * page_size
-                query = "select * from (%s) s limit %s offset %s" % (query_str, num_rows, offset)
+                query = text("select * from (%s) s limit %s offset %s" % (query_str, num_rows, offset))
                 logger.debug('executing %r', query)
                 result = connection.execute(query)
                 rows = list(map(dict, islice(iter(result), 0, num_rows)))
                 rows = [self.jsonable(row) for row in rows]
                 logger.debug('rowcount %r', len(rows))
         except Exception as e:
             return {
```

### Comparing `apisql-0.3.0/apisql/utils/file_maker.py` & `apisql-0.3.1/apisql/utils/file_maker.py`

 * *Files identical despite different names*

### Comparing `apisql-0.3.0/apisql.egg-info/PKG-INFO` & `apisql-0.3.1/apisql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apisql
-Version: 0.3.0
+Version: 0.3.1
 Summary: A flask blueprint providing a read-lny API for querying RDBMS
 Home-page: https://github.com/dataspot/apisql
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Keywords: data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apisql-0.3.0/setup.py` & `apisql-0.3.1/setup.py`

 * *Files identical despite different names*

