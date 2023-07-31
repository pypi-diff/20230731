# Comparing `tmp/gandai-1.3.7.tar.gz` & `tmp/gandai-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.3.7.tar", last modified: Thu Jul 27 23:04:00 2023, max compression
+gzip compressed data, was "gandai-1.3.8.tar", last modified: Mon Jul 31 19:58:05 2023, max compression
```

## Comparing `gandai-1.3.7.tar` & `gandai-1.3.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.633497 gandai-1.3.7/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.7/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-27 23:04:00.633390 gandai-1.3.7/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.628603 gandai-1.3.7/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.631469 gandai-1.3.7/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.7/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.7/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-27 20:57:53.000000 gandai-1.3.7/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.3.7/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.7/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.7/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-27 21:29:01.000000 gandai-1.3.7/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.7/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.7/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    30266 2023-07-27 21:29:01.000000 gandai-1.3.7/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-26 13:45:26.000000 gandai-1.3.7/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.7/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17500 2023-07-27 21:29:01.000000 gandai-1.3.7/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-27 21:16:13.000000 gandai-1.3.7/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-27 20:52:17.000000 gandai-1.3.7/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.632190 gandai-1.3.7/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.7/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.632652 gandai-1.3.7/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.7/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.633193 gandai-1.3.7/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.7/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.7/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    21313 2023-07-27 21:23:57.000000 gandai-1.3.7/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.7/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)    11623 2023-07-27 21:01:14.000000 gandai-1.3.7/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-27 23:04:00.629073 gandai-1.3.7/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-27 23:04:00.000000 gandai-1.3.7/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-27 23:03:40.000000 gandai-1.3.7/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-27 23:04:00.633526 gandai-1.3.7/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.7/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.143560 gandai-1.3.8/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.8/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-31 19:58:05.143404 gandai-1.3.8/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.134488 gandai-1.3.8/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.141187 gandai-1.3.8/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.8/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.8/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-27 20:57:53.000000 gandai-1.3.8/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.3.8/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.8/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.8/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-27 21:29:01.000000 gandai-1.3.8/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.8/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.8/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    31257 2023-07-31 19:51:53.000000 gandai-1.3.8/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-26 13:45:26.000000 gandai-1.3.8/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.8/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17502 2023-07-31 19:04:57.000000 gandai-1.3.8/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-27 21:16:13.000000 gandai-1.3.8/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.142211 gandai-1.3.8/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.8/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.142669 gandai-1.3.8/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.8/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.143154 gandai-1.3.8/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.8/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    22049 2023-07-31 19:51:51.000000 gandai-1.3.8/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.8/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)    11690 2023-07-31 19:04:54.000000 gandai-1.3.8/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.135192 gandai-1.3.8/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-31 19:57:55.000000 gandai-1.3.8/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-31 19:58:05.143596 gandai-1.3.8/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.8/setup.py
```

### Comparing `gandai-1.3.7/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x6de0c264 (Thu Jul 27 21:23:57 2023 UTC)
-files sz: 21313
+moddate:  0xd710c864 (Mon Jul 31 19:51:51 2023 UTC)
+files sz: 22049
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -193,175 +193,175 @@
    107         292 LOAD_CONST               1 (None)
    
    105         294 BUILD_TUPLE             10
                296 LOAD_CONST              25 (<code object insert_targets_from_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 105>)
                298 MAKE_FUNCTION            4 (annotations)
                300 STORE_NAME              34 (insert_targets_from_domains)
    
-   162         302 LOAD_CONST              26 ('companies')
+   187         302 LOAD_CONST              26 ('companies')
    
-   163         304 LOAD_NAME                5 (List)
+   188         304 LOAD_NAME                5 (List)
                306 LOAD_NAME                4 (Any)
                308 BINARY_SUBSCR
    
-   162         318 LOAD_CONST              22 ('search_uid')
+   187         318 LOAD_CONST              22 ('search_uid')
    
-   163         320 LOAD_NAME               33 (int)
+   188         320 LOAD_NAME               33 (int)
    
-   162         322 LOAD_CONST              23 ('actor_key')
+   187         322 LOAD_CONST              23 ('actor_key')
    
-   163         324 LOAD_NAME               32 (str)
+   188         324 LOAD_NAME               32 (str)
    
-   162         326 LOAD_CONST              13 ('return')
+   187         326 LOAD_CONST              13 ('return')
    
-   164         328 LOAD_CONST               1 (None)
+   189         328 LOAD_CONST               1 (None)
    
-   162         330 BUILD_TUPLE              8
-               332 LOAD_CONST              27 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 162>)
+   187         330 BUILD_TUPLE              8
+               332 LOAD_CONST              27 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 187>)
                334 MAKE_FUNCTION            4 (annotations)
                336 STORE_NAME              35 (insert_companies_as_targets)
    
-   216         338 LOAD_CONST              13 ('return')
+   241         338 LOAD_CONST              13 ('return')
                340 LOAD_NAME                7 (pd)
                342 LOAD_ATTR               36 (DataFrame)
                352 BUILD_TUPLE              2
-               354 LOAD_CONST              28 (<code object top_actor_per_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 216>)
+               354 LOAD_CONST              28 (<code object top_actor_per_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 241>)
                356 MAKE_FUNCTION            4 (annotations)
                358 STORE_NAME              37 (top_actor_per_search)
    
-   254         360 LOAD_CONST              13 ('return')
+   280         360 LOAD_CONST              13 ('return')
                362 LOAD_NAME                7 (pd)
                364 LOAD_ATTR               36 (DataFrame)
                374 BUILD_TUPLE              2
-               376 LOAD_CONST              29 (<code object search_event_count_by_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 254>)
+               376 LOAD_CONST              29 (<code object search_event_count_by_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 280>)
                378 MAKE_FUNCTION            4 (annotations)
                380 STORE_NAME              38 (search_event_count_by_type)
    
-   270         382 LOAD_CONST              30 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 270>)
+   301         382 LOAD_CONST              30 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 301>)
                384 MAKE_FUNCTION            0
                386 STORE_NAME              39 (search)
    
-   312         388 LOAD_CONST              13 ('return')
+   349         388 LOAD_CONST              13 ('return')
                390 LOAD_NAME                7 (pd)
                392 LOAD_ATTR               36 (DataFrame)
                402 BUILD_TUPLE              2
-               404 LOAD_CONST              31 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 312>)
+               404 LOAD_CONST              31 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 349>)
                406 MAKE_FUNCTION            4 (annotations)
                408 STORE_NAME              40 (actor)
    
-   326         410 LOAD_CONST              46 ((None,))
+   363         410 LOAD_CONST              46 ((None,))
                412 LOAD_CONST              22 ('search_uid')
                414 LOAD_NAME               33 (int)
                416 LOAD_CONST              24 ('last_event_type')
                418 LOAD_NAME               32 (str)
                420 BUILD_TUPLE              4
-               422 LOAD_CONST              32 (<code object search_target_by_last_event_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 326>)
+               422 LOAD_CONST              32 (<code object search_target_by_last_event_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 363>)
                424 MAKE_FUNCTION            5 (defaults, annotations)
                426 STORE_NAME              41 (search_target_by_last_event_type)
    
-   456         428 LOAD_CONST              22 ('search_uid')
+   492         428 LOAD_CONST              22 ('search_uid')
                430 LOAD_NAME               33 (int)
                432 LOAD_CONST              13 ('return')
                434 LOAD_NAME                7 (pd)
                436 LOAD_ATTR               36 (DataFrame)
                446 BUILD_TUPLE              4
-               448 LOAD_CONST              33 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 456>)
+               448 LOAD_CONST              33 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 492>)
                450 MAKE_FUNCTION            4 (annotations)
                452 STORE_NAME              42 (target_count)
    
-   486         454 LOAD_CONST              22 ('search_uid')
+   522         454 LOAD_CONST              22 ('search_uid')
                456 LOAD_NAME               33 (int)
                458 LOAD_CONST              13 ('return')
                460 LOAD_NAME                7 (pd)
                462 LOAD_ATTR               36 (DataFrame)
                472 BUILD_TUPLE              4
-               474 LOAD_CONST              34 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 486>)
+               474 LOAD_CONST              34 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 522>)
                476 MAKE_FUNCTION            4 (annotations)
                478 STORE_NAME              43 (event)
    
-   498         480 LOAD_CONST              22 ('search_uid')
+   534         480 LOAD_CONST              22 ('search_uid')
                482 LOAD_NAME               33 (int)
                484 LOAD_CONST              13 ('return')
                486 LOAD_NAME                7 (pd)
                488 LOAD_ATTR               36 (DataFrame)
                498 BUILD_TUPLE              4
-               500 LOAD_CONST              35 (<code object unique_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 498>)
+               500 LOAD_CONST              35 (<code object unique_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 534>)
                502 MAKE_FUNCTION            4 (annotations)
                504 STORE_NAME              44 (unique_domains)
    
-   510         506 LOAD_CONST              13 ('return')
+   546         506 LOAD_CONST              13 ('return')
                508 LOAD_NAME                7 (pd)
                510 LOAD_ATTR               36 (DataFrame)
                520 BUILD_TUPLE              2
-               522 LOAD_CONST              36 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 510>)
+               522 LOAD_CONST              36 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 546>)
                524 MAKE_FUNCTION            4 (annotations)
                526 STORE_NAME              45 (company)
    
-   521         528 LOAD_CONST              22 ('search_uid')
+   557         528 LOAD_CONST              22 ('search_uid')
                530 LOAD_NAME               33 (int)
                532 LOAD_CONST              13 ('return')
                534 LOAD_NAME                7 (pd)
                536 LOAD_ATTR               36 (DataFrame)
                546 BUILD_TUPLE              4
-               548 LOAD_CONST              37 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 521>)
+               548 LOAD_CONST              37 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 557>)
                550 MAKE_FUNCTION            4 (annotations)
                552 STORE_NAME              46 (checkpoint)
    
-   534         554 LOAD_CONST              22 ('search_uid')
+   570         554 LOAD_CONST              22 ('search_uid')
                556 LOAD_NAME               33 (int)
                558 LOAD_CONST              13 ('return')
                560 LOAD_NAME                7 (pd)
                562 LOAD_ATTR               36 (DataFrame)
                572 BUILD_TUPLE              4
-               574 LOAD_CONST              38 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 534>)
+               574 LOAD_CONST              38 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 570>)
                576 MAKE_FUNCTION            4 (annotations)
                578 STORE_NAME              47 (comment_by_domain)
    
-   555         580 LOAD_CONST              22 ('search_uid')
+   591         580 LOAD_CONST              22 ('search_uid')
                582 LOAD_NAME               33 (int)
                584 LOAD_CONST              13 ('return')
                586 LOAD_NAME               25 (Search)
                588 BUILD_TUPLE              4
-               590 LOAD_CONST              39 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 555>)
+               590 LOAD_CONST              39 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 591>)
                592 MAKE_FUNCTION            4 (annotations)
                594 STORE_NAME              48 (find_search_by_uid)
    
-   573         596 LOAD_CONST              40 ('domain')
+   609         596 LOAD_CONST              40 ('domain')
                598 LOAD_NAME               32 (str)
                600 LOAD_CONST              13 ('return')
                602 LOAD_NAME               22 (Company)
                604 BUILD_TUPLE              4
-               606 LOAD_CONST              41 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 573>)
+               606 LOAD_CONST              41 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 609>)
                608 MAKE_FUNCTION            4 (annotations)
                610 STORE_NAME              49 (find_company_by_domain)
    
-   589         612 LOAD_CONST              42 ('event_id')
+   625         612 LOAD_CONST              42 ('event_id')
                614 LOAD_NAME               33 (int)
                616 LOAD_CONST              13 ('return')
                618 LOAD_NAME               23 (Event)
                620 BUILD_TUPLE              4
-               622 LOAD_CONST              43 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 589>)
+               622 LOAD_CONST              43 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 625>)
                624 MAKE_FUNCTION            4 (annotations)
                626 STORE_NAME              50 (find_event_by_id)
    
-   608         628 LOAD_CONST              10 ('company')
+   644         628 LOAD_CONST              10 ('company')
                630 LOAD_NAME               22 (Company)
                632 LOAD_CONST              13 ('return')
                634 LOAD_CONST               1 (None)
                636 BUILD_TUPLE              4
-               638 LOAD_CONST              44 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 608>)
+               638 LOAD_CONST              44 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 644>)
                640 MAKE_FUNCTION            4 (annotations)
                642 STORE_NAME              51 (update_company)
    
-   635         644 LOAD_CONST              17 ('search')
+   671         644 LOAD_CONST              17 ('search')
                646 LOAD_NAME               25 (Search)
                648 LOAD_CONST              13 ('return')
                650 LOAD_CONST               1 (None)
                652 BUILD_TUPLE              4
-               654 LOAD_CONST              45 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 635>)
+               654 LOAD_CONST              45 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 671>)
                656 MAKE_FUNCTION            4 (annotations)
                658 STORE_NAME              52 (update_search)
                660 LOAD_CONST               1 (None)
                662 RETURN_VALUE
    consts
       0
       None
@@ -910,256 +910,336 @@
          lnotab 0x02013401160102ff1006460128f82e09
       'domains'
       'search_uid'
       'actor_key'
       'last_event_type'
       code
          argcount  : 4
-         nlocals   : 10
+         nlocals   : 11
          stacksize : 10
          flags     : 3
          code
-            0x97007401000000000000000000007403000000000000000000007c01ac
-            01a6010000ab010000000000000000640219000000000000000000a60100
-            00ab0100000000000000007d04640384007c004400a6000000ab00000000
-            00000000007d057405000000000000000000007c057c047a0a0000a60100
-            00ab0100000000000000007d067401000000000000000000007403000000
-            000000000000007c01ac01a6010000ab0100000000000000006402190000
-            00000000000000a6010000ab0100000000000000007d04640484007c0044
-            00a6000000ab0000000000000000007d057405000000000000000000007c
-            057c047a0a0000a6010000ab0100000000000000007d0674060000000000
-            0000000000a0040000000000000000000000000000000000000000a60000
-            00ab00000000000000000035007d077c0644005d597d087c07a005000000
-            0000000000000000000000000000000000740d000000000000000000006a
-            0700000000000000006405a6010000ab01000000000000000064027c0869
-            01a6020000ab02000000000000000001007c07a005000000000000000000
-            0000000000000000000000740d000000000000000000006a070000000000
-            0000006406a6010000ab0100000000000000007c017c027c087c0364079c
-            04a6020000ab02000000000000000001008c5a7c07a00800000000000000
-            00000000000000000000000000a6000000ab000000000000000000010064
-            0864086408a6020000ab02000000000000000001006e0b23003100730477
-            0278035900770101005900010001007413000000000000000000007c06a6
-            010000ab0100000000000000007413000000000000000000007c05a00a00
-            000000000000000000000000000000000000007c04a6010000ab01000000
-            0000000000a6010000ab01000000000000000064099c027d097c095300
+            0x9700640174000000000000000000000064027402000000000000000000
+            0064037404000000000000000000006606640484047d0402007c047c017c
+            03ac05a6020000ab0200000000000000007d05640684007c004400a60000
+            00ab0000000000000000007d067407000000000000000000007c067c057a
+            0a0000a6010000ab0100000000000000007d077408000000000000000000
+            00a0050000000000000000000000000000000000000000a6000000ab0000
+            0000000000000035007d087c0744005d597d097c08a00600000000000000
+            00000000000000000000000000740f000000000000000000006a08000000
+            00000000006407a6010000ab01000000000000000064087c096901a60200
+            00ab02000000000000000001007c08a00600000000000000000000000000
+            00000000000000740f000000000000000000006a08000000000000000064
+            09a6010000ab0100000000000000007c017c027c097c03640a9c04a60200
+            00ab02000000000000000001008c5a7c08a0090000000000000000000000
+            000000000000000000a6000000ab0000000000000000000100640b640b64
+            0ba6020000ab02000000000000000001006e0b2300310073047702780359
+            00770101005900010001007415000000000000000000007c07a6010000ab
+            0100000000000000007415000000000000000000007c06a00b0000000000
+            0000000000000000000000000000007c05a6010000ab0100000000000000
+            00a6010000ab010000000000000000640c9c027d0a7c0a5300
          105           0 RESUME                   0
          
-         112           2 LOAD_GLOBAL              1 (NULL + set)
-                      14 LOAD_GLOBAL              3 (NULL + unique_domains)
-                      26 LOAD_FAST                1 (search_uid)
-                      28 KW_NAMES                 1
-                      30 PRECALL                  1
-                      34 CALL                     1
-                      44 LOAD_CONST               2 ('domain')
-                      46 BINARY_SUBSCR
-                      56 PRECALL                  1
-                      60 CALL                     1
-                      70 STORE_FAST               4 (existing_domains)
-         
-         114          72 LOAD_CONST               3 (<code object <setcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 114>)
-                      74 MAKE_FUNCTION            0
-                      76 LOAD_FAST                0 (domains)
-                      78 GET_ITER
-                      80 PRECALL                  0
-                      84 CALL                     0
-                      94 STORE_FAST               5 (new_domains)
-         
-         116          96 LOAD_GLOBAL              5 (NULL + list)
-                     108 LOAD_FAST                5 (new_domains)
-                     110 LOAD_FAST                4 (existing_domains)
-                     112 BINARY_OP               10 (-)
-                     116 PRECALL                  1
-                     120 CALL                     1
-                     130 STORE_FAST               6 (domains_to_insert)
+         113           2 LOAD_CONST               1 ('search_uid')
+                       4 LOAD_GLOBAL              0 (int)
+                      16 LOAD_CONST               2 ('last_event_type')
+                      18 LOAD_GLOBAL              2 (str)
+                      30 LOAD_CONST               3 ('return')
+                      32 LOAD_GLOBAL              4 (set)
+                      44 BUILD_TUPLE              6
+                      46 LOAD_CONST               4 (<code object downstream_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 113>)
+                      48 MAKE_FUNCTION            4 (annotations)
+                      50 STORE_FAST               4 (downstream_domains)
+         
+         140          52 PUSH_NULL
+                      54 LOAD_FAST                4 (downstream_domains)
+         
+         141          56 LOAD_FAST                1 (search_uid)
+                      58 LOAD_FAST                3 (last_event_type)
+         
+         140          60 KW_NAMES                 5
+                      62 PRECALL                  2
+                      66 CALL                     2
+                      76 STORE_FAST               5 (protected_domains)
+         
+         144          78 LOAD_CONST               6 (<code object <setcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 144>)
+                      80 MAKE_FUNCTION            0
+                      82 LOAD_FAST                0 (domains)
+                      84 GET_ITER
+                      86 PRECALL                  0
+                      90 CALL                     0
+                     100 STORE_FAST               6 (new_domains)
+         
+         146         102 LOAD_GLOBAL              7 (NULL + list)
+                     114 LOAD_FAST                6 (new_domains)
+                     116 LOAD_FAST                5 (protected_domains)
+                     118 BINARY_OP               10 (-)
+                     122 PRECALL                  1
+                     126 CALL                     1
+                     136 STORE_FAST               7 (domains_to_insert)
+         
+         148         138 LOAD_GLOBAL              8 (db)
+                     150 LOAD_METHOD              5 (connect)
+                     172 PRECALL                  0
+                     176 CALL                     0
+                     186 BEFORE_WITH
+                     188 STORE_FAST               8 (con)
+         
+         149         190 LOAD_FAST                7 (domains_to_insert)
+                     192 GET_ITER
+                 >>  194 FOR_ITER                89 (to 374)
+                     196 STORE_FAST               9 (domain)
+         
+         151         198 LOAD_FAST                8 (con)
+                     200 LOAD_METHOD              6 (execute)
          
-         117         132 LOAD_GLOBAL              1 (NULL + set)
-                     144 LOAD_GLOBAL              3 (NULL + unique_domains)
-                     156 LOAD_FAST                1 (search_uid)
-                     158 KW_NAMES                 1
-                     160 PRECALL                  1
-                     164 CALL                     1
-                     174 LOAD_CONST               2 ('domain')
-                     176 BINARY_SUBSCR
-                     186 PRECALL                  1
-                     190 CALL                     1
-                     200 STORE_FAST               4 (existing_domains)
-         
-         119         202 LOAD_CONST               4 (<code object <setcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 119>)
-                     204 MAKE_FUNCTION            0
-                     206 LOAD_FAST                0 (domains)
-                     208 GET_ITER
-                     210 PRECALL                  0
-                     214 CALL                     0
-                     224 STORE_FAST               5 (new_domains)
-         
-         121         226 LOAD_GLOBAL              5 (NULL + list)
-                     238 LOAD_FAST                5 (new_domains)
-                     240 LOAD_FAST                4 (existing_domains)
-                     242 BINARY_OP               10 (-)
-                     246 PRECALL                  1
+         152         222 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+                     234 LOAD_ATTR                8 (text)
+         
+         153         244 LOAD_CONST               7 ('\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    ')
+         
+         152         246 PRECALL                  1
                      250 CALL                     1
-                     260 STORE_FAST               6 (domains_to_insert)
          
-         123         262 LOAD_GLOBAL              6 (db)
-                     274 LOAD_METHOD              4 (connect)
-                     296 PRECALL                  0
-                     300 CALL                     0
-                     310 BEFORE_WITH
-                     312 STORE_FAST               7 (con)
-         
-         124         314 LOAD_FAST                6 (domains_to_insert)
-                     316 GET_ITER
-                 >>  318 FOR_ITER                89 (to 498)
-                     320 STORE_FAST               8 (domain)
-         
-         126         322 LOAD_FAST                7 (con)
-                     324 LOAD_METHOD              5 (execute)
-         
-         127         346 LOAD_GLOBAL             13 (NULL + sqlalchemy)
-                     358 LOAD_ATTR                7 (text)
-         
-         128         368 LOAD_CONST               5 ('\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    ')
-         
-         127         370 PRECALL                  1
-                     374 CALL                     1
-         
-         134         384 LOAD_CONST               2 ('domain')
-                     386 LOAD_FAST                8 (domain)
-                     388 BUILD_MAP                1
-         
-         126         390 PRECALL                  2
-                     394 CALL                     2
-                     404 POP_TOP
-         
-         137         406 LOAD_FAST                7 (con)
-                     408 LOAD_METHOD              5 (execute)
-         
-         138         430 LOAD_GLOBAL             13 (NULL + sqlalchemy)
-                     442 LOAD_ATTR                7 (text)
-         
-         139         452 LOAD_CONST               6 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    ')
-         
-         138         454 PRECALL                  1
-                     458 CALL                     1
-         
-         146         468 LOAD_FAST                1 (search_uid)
-         
-         147         470 LOAD_FAST                2 (actor_key)
-         
-         148         472 LOAD_FAST                8 (domain)
-         
-         149         474 LOAD_FAST                3 (last_event_type)
-         
-         145         476 LOAD_CONST               7 (('search_uid', 'actor_key', 'domain', 'type'))
-                     478 BUILD_CONST_KEY_MAP      4
-         
-         137         480 PRECALL                  2
-                     484 CALL                     2
-                     494 POP_TOP
-                     496 JUMP_BACKWARD           90 (to 318)
-         
-         153     >>  498 LOAD_FAST                7 (con)
-                     500 LOAD_METHOD              8 (commit)
-                     522 PRECALL                  0
-                     526 CALL                     0
-                     536 POP_TOP
-         
-         123         538 LOAD_CONST               8 (None)
-                     540 LOAD_CONST               8 (None)
-                     542 LOAD_CONST               8 (None)
-                     544 PRECALL                  2
-                     548 CALL                     2
-                     558 POP_TOP
-                     560 JUMP_FORWARD            11 (to 584)
-                 >>  562 PUSH_EXC_INFO
-                     564 WITH_EXCEPT_START
-                     566 POP_JUMP_FORWARD_IF_TRUE     4 (to 576)
-                     568 RERAISE                  2
-                 >>  570 COPY                     3
-                     572 POP_EXCEPT
-                     574 RERAISE                  1
-                 >>  576 POP_TOP
-                     578 POP_EXCEPT
-                     580 POP_TOP
-                     582 POP_TOP
-         
-         156     >>  584 LOAD_GLOBAL             19 (NULL + len)
-                     596 LOAD_FAST                6 (domains_to_insert)
-                     598 PRECALL                  1
-                     602 CALL                     1
+         159         260 LOAD_CONST               8 ('domain')
+                     262 LOAD_FAST                9 (domain)
+                     264 BUILD_MAP                1
+         
+         151         266 PRECALL                  2
+                     270 CALL                     2
+                     280 POP_TOP
          
-         157         612 LOAD_GLOBAL             19 (NULL + len)
-                     624 LOAD_FAST                5 (new_domains)
-                     626 LOAD_METHOD             10 (intersection)
-                     648 LOAD_FAST                4 (existing_domains)
-                     650 PRECALL                  1
-                     654 CALL                     1
-                     664 PRECALL                  1
-                     668 CALL                     1
-         
-         155         678 LOAD_CONST               9 (('inserted', 'duplicates'))
-                     680 BUILD_CONST_KEY_MAP      2
-                     682 STORE_FAST               9 (resp)
-         
-         159         684 LOAD_FAST                9 (resp)
-                     686 RETURN_VALUE
-         ExceptionTable:
-           312 to 536 -> 562 [1] lasti
-           562 to 568 -> 570 [3] lasti
-           576 to 576 -> 570 [3] lasti
+         162         282 LOAD_FAST                8 (con)
+                     284 LOAD_METHOD              6 (execute)
+         
+         163         306 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+                     318 LOAD_ATTR                8 (text)
+         
+         164         328 LOAD_CONST               9 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    ')
+         
+         163         330 PRECALL                  1
+                     334 CALL                     1
+         
+         171         344 LOAD_FAST                1 (search_uid)
+         
+         172         346 LOAD_FAST                2 (actor_key)
+         
+         173         348 LOAD_FAST                9 (domain)
+         
+         174         350 LOAD_FAST                3 (last_event_type)
+         
+         170         352 LOAD_CONST              10 (('search_uid', 'actor_key', 'domain', 'type'))
+                     354 BUILD_CONST_KEY_MAP      4
+         
+         162         356 PRECALL                  2
+                     360 CALL                     2
+                     370 POP_TOP
+                     372 JUMP_BACKWARD           90 (to 194)
+         
+         178     >>  374 LOAD_FAST                8 (con)
+                     376 LOAD_METHOD              9 (commit)
+                     398 PRECALL                  0
+                     402 CALL                     0
+                     412 POP_TOP
+         
+         148         414 LOAD_CONST              11 (None)
+                     416 LOAD_CONST              11 (None)
+                     418 LOAD_CONST              11 (None)
+                     420 PRECALL                  2
+                     424 CALL                     2
+                     434 POP_TOP
+                     436 JUMP_FORWARD            11 (to 460)
+                 >>  438 PUSH_EXC_INFO
+                     440 WITH_EXCEPT_START
+                     442 POP_JUMP_FORWARD_IF_TRUE     4 (to 452)
+                     444 RERAISE                  2
+                 >>  446 COPY                     3
+                     448 POP_EXCEPT
+                     450 RERAISE                  1
+                 >>  452 POP_TOP
+                     454 POP_EXCEPT
+                     456 POP_TOP
+                     458 POP_TOP
+         
+         181     >>  460 LOAD_GLOBAL             21 (NULL + len)
+                     472 LOAD_FAST                7 (domains_to_insert)
+                     474 PRECALL                  1
+                     478 CALL                     1
+         
+         182         488 LOAD_GLOBAL             21 (NULL + len)
+                     500 LOAD_FAST                6 (new_domains)
+                     502 LOAD_METHOD             11 (intersection)
+                     524 LOAD_FAST                5 (protected_domains)
+                     526 PRECALL                  1
+                     530 CALL                     1
+                     540 PRECALL                  1
+                     544 CALL                     1
+         
+         180         554 LOAD_CONST              12 (('inserted', 'duplicates'))
+                     556 BUILD_CONST_KEY_MAP      2
+                     558 STORE_FAST              10 (resp)
+         
+         184         560 LOAD_FAST               10 (resp)
+                     562 RETURN_VALUE
+         ExceptionTable:
+           188 to 412 -> 438 [1] lasti
+           438 to 444 -> 446 [3] lasti
+           452 to 452 -> 446 [3] lasti
          consts
             '\n    Takes in domains, inserts targets into a review stage, where they will\n    try to be enriched on process event\n    '
-            ('search_uid',)
-            'domain'
+            'search_uid'
+            'last_event_type'
+            'return'
             code
-               argcount  : 1
-               nlocals   : 2
-               stacksize : 5
+               argcount  : 2
+               nlocals   : 8
+               stacksize : 6
                flags     : 19
                code
-                  0x970068007c005d1a7d0164007c017600af067401000000000000000000
-                  006a0100000000000000007c01a6010000ab01000000000000000092028c
-                  1b5300
-               114           0 RESUME                   0
-                             2 BUILD_SET                0
-                             4 LOAD_FAST                0 (.0)
-                       >>    6 FOR_ITER                26 (to 60)
-                             8 STORE_FAST               1 (domain)
-                            10 LOAD_CONST               0 ('.')
-                            12 LOAD_FAST                1 (domain)
-                            14 CONTAINS_OP              0
-                            16 POP_JUMP_BACKWARD_IF_FALSE     6 (to 6)
-                            18 LOAD_GLOBAL              1 (NULL + helpers)
-                            30 LOAD_ATTR                1 (clean_domain)
-                            40 LOAD_FAST                1 (domain)
-                            42 PRECALL                  1
-                            46 CALL                     1
-                            56 SET_ADD                  2
-                            58 JUMP_BACKWARD           27 (to 6)
-                       >>   60 RETURN_VALUE
+                  0x970067006401a2017d027401000000000000000000007c027c02a00100
+                  000000000000000000000000000000000000007c01a6010000ab01000000
+                  00000000006400850219000000000000000000a6010000ab010000000000
+                  0000007d03740400000000000000000000a0030000000000000000000000
+                  000000000000000000a6000000ab00000000000000000035007d0464027c
+                  039b0064039d037d057c04a0040000000000000000000000000000000000
+                  000000740b000000000000000000006a0600000000000000007c05a60100
+                  00ab01000000000000000064047c006901a6020000ab0200000000000000
+                  007d06740f000000000000000000006a0800000000000000007c06a00900
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  0000007c06a00a0000000000000000000000000000000000000000a60000
+                  00ab000000000000000000ac05a6020000ab0200000000000000007d0764
+                  0064006400a6020000ab02000000000000000001006e0b23003100730477
+                  0278035900770101005900010001007417000000000000000000007c0764
+                  0619000000000000000000a6010000ab0100000000000000005300
+               113           0 RESUME                   0
+               
+               114           2 BUILD_LIST               0
+                             4 LOAD_CONST               1 (('create', 'advance', 'validate', 'send', 'accept', 'reject', 'conflict'))
+                             6 LIST_EXTEND              1
+                             8 STORE_FAST               2 (STAGES)
+               
+               124          10 LOAD_GLOBAL              1 (NULL + tuple)
+                            22 LOAD_FAST                2 (STAGES)
+                            24 LOAD_FAST                2 (STAGES)
+                            26 LOAD_METHOD              1 (index)
+                            48 LOAD_FAST                1 (last_event_type)
+                            50 PRECALL                  1
+                            54 CALL                     1
+                            64 LOAD_CONST               0 (None)
+                            66 BUILD_SLICE              2
+                            68 BINARY_SUBSCR
+                            78 PRECALL                  1
+                            82 CALL                     1
+                            92 STORE_FAST               3 (protected_stages)
+               
+               126          94 LOAD_GLOBAL              4 (db)
+                           106 LOAD_METHOD              3 (connect)
+                           128 PRECALL                  0
+                           132 CALL                     0
+                           142 BEFORE_WITH
+                           144 STORE_FAST               4 (conn)
+               
+               127         146 LOAD_CONST               2 ('\n                    SELECT distinct(domain)\n                    FROM event\n                    WHERE search_uid = :search_uid \n                    AND type IN ')
+               
+               131         148 LOAD_FAST                3 (protected_stages)
+               
+               127         150 FORMAT_VALUE             0
+                           152 LOAD_CONST               3 ('\n                ')
+                           154 BUILD_STRING             3
+                           156 STORE_FAST               5 (statement)
+               
+               133         158 LOAD_FAST                4 (conn)
+                           160 LOAD_METHOD              4 (execute)
+               
+               134         182 LOAD_GLOBAL             11 (NULL + sqlalchemy)
+                           194 LOAD_ATTR                6 (text)
+                           204 LOAD_FAST                5 (statement)
+                           206 PRECALL                  1
+                           210 CALL                     1
+               
+               135         220 LOAD_CONST               4 ('search_uid')
+                           222 LOAD_FAST                0 (search_uid)
+                           224 BUILD_MAP                1
+               
+               133         226 PRECALL                  2
+                           230 CALL                     2
+                           240 STORE_FAST               6 (result)
+               
+               137         242 LOAD_GLOBAL             15 (NULL + pd)
+                           254 LOAD_ATTR                8 (DataFrame)
+                           264 LOAD_FAST                6 (result)
+                           266 LOAD_METHOD              9 (fetchall)
+                           288 PRECALL                  0
+                           292 CALL                     0
+                           302 LOAD_FAST                6 (result)
+                           304 LOAD_METHOD             10 (keys)
+                           326 PRECALL                  0
+                           330 CALL                     0
+                           340 KW_NAMES                 5
+                           342 PRECALL                  2
+                           346 CALL                     2
+                           356 STORE_FAST               7 (df)
+               
+               126         358 LOAD_CONST               0 (None)
+                           360 LOAD_CONST               0 (None)
+                           362 LOAD_CONST               0 (None)
+                           364 PRECALL                  2
+                           368 CALL                     2
+                           378 POP_TOP
+                           380 JUMP_FORWARD            11 (to 404)
+                       >>  382 PUSH_EXC_INFO
+                           384 WITH_EXCEPT_START
+                           386 POP_JUMP_FORWARD_IF_TRUE     4 (to 396)
+                           388 RERAISE                  2
+                       >>  390 COPY                     3
+                           392 POP_EXCEPT
+                           394 RERAISE                  1
+                       >>  396 POP_TOP
+                           398 POP_EXCEPT
+                           400 POP_TOP
+                           402 POP_TOP
+               
+               138     >>  404 LOAD_GLOBAL             23 (NULL + set)
+                           416 LOAD_FAST                7 (df)
+                           418 LOAD_CONST               6 ('domain')
+                           420 BINARY_SUBSCR
+                           430 PRECALL                  1
+                           434 CALL                     1
+                           444 RETURN_VALUE
+               ExceptionTable:
+                 144 to 356 -> 382 [1] lasti
+                 382 to 388 -> 390 [3] lasti
+                 396 to 396 -> 390 [3] lasti
                consts
-                  '.'
-               names      ('helpers', 'clean_domain')
-               varnames   ('.0', 'domain')
+                  None
+                  ('create', 'advance', 'validate', 'send', 'accept', 'reject', 'conflict')
+                  '\n                    SELECT distinct(domain)\n                    FROM event\n                    WHERE search_uid = :search_uid \n                    AND type IN '
+                  '\n                '
+                  'search_uid'
+                  ('columns',)
+                  'domain'
+               names      ('tuple', 'index', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'set')
+               varnames   ('search_uid', 'last_event_type', 'STAGES', 'protected_stages', 'conn', 'statement', 'result', 'df')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
-               name       '<setcomp>'
-               firstlineno 114
-               lnotab 0x
+               name       'downstream_domains'
+               firstlineno 113
+               lnotab 0x0201080a54023401020402fc08061801260106fe100474f52e0c
+            ('search_uid', 'last_event_type')
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x970068007c005d1a7d0164007c017600af067401000000000000000000
                   006a0100000000000000007c01a6010000ab01000000000000000092028c
                   1b5300
-               119           0 RESUME                   0
+               144           0 RESUME                   0
                              2 BUILD_SET                0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                26 (to 60)
                              8 STORE_FAST               1 (domain)
                             10 LOAD_CONST               0 ('.')
                             12 LOAD_FAST                1 (domain)
                             14 CONTAINS_OP              0
@@ -1176,30 +1256,31 @@
                   '.'
                names      ('helpers', 'clean_domain')
                varnames   ('.0', 'domain')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<setcomp>'
-               firstlineno 119
+               firstlineno 144
                lnotab 0x
             '\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    '
+            'domain'
             '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    '
             ('search_uid', 'actor_key', 'domain', 'type')
             None
             ('inserted', 'duplicates')
-         names      ('set', 'unique_domains', 'list', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit', 'len', 'intersection')
-         varnames   ('domains', 'search_uid', 'actor_key', 'last_event_type', 'existing_domains', 'new_domains', 'domains_to_insert', 'con', 'domain', 'resp')
+         names      ('int', 'str', 'set', 'list', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit', 'len', 'intersection')
+         varnames   ('domains', 'search_uid', 'actor_key', 'last_event_type', 'downstream_domains', 'protected_domains', 'new_domains', 'domains_to_insert', 'con', 'domain', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_targets_from_domains'
          firstlineno 105
          lnotab
-            0x0207460218022401460218022402340108021801160102ff0e0706f810
+            0x0208321b040104ff120418022402340108021801160102ff0e0706f810
             0b1801160102ff0e0802010201020102fc04f8121028e22e211c0142fe06
             04
       'companies'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 10
@@ -1227,168 +1308,168 @@
             0000000000740f000000000000000000006a080000000000000000640ea6
             010000ab0100000000000000007c017c027c05a004000000000000000000
             00000000000000000000006402a6010000ab010000000000000000640f64
             109c04a6020000ab020000000000000000010090018c107c04a009000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             000100640364036403a6020000ab02000000000000000001006403530023
             00310073047702780359007701010059000100010064035300
-         162           0 RESUME                   0
+         187           0 RESUME                   0
          
-         166           2 LOAD_GLOBAL              1 (NULL + unique_domains)
+         191           2 LOAD_GLOBAL              1 (NULL + unique_domains)
                       14 LOAD_FAST                1 (search_uid)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 LOAD_CONST               2 ('domain')
                       34 BINARY_SUBSCR
                       44 LOAD_METHOD              1 (to_list)
                       66 PRECALL                  0
                       70 CALL                     0
                       80 STORE_FAST               3 (existing_search_domains)
          
-         167          82 LOAD_GLOBAL              4 (db)
+         192          82 LOAD_GLOBAL              4 (db)
                       94 LOAD_METHOD              3 (connect)
                      116 PRECALL                  0
                      120 CALL                     0
                      130 BEFORE_WITH
                      132 STORE_FAST               4 (con)
          
-         168         134 LOAD_FAST                0 (companies)
+         193         134 LOAD_FAST                0 (companies)
                      136 GET_ITER
                  >>  138 EXTENDED_ARG             1
                      140 FOR_ITER               270 (to 682)
                      142 STORE_FAST               5 (company)
          
-         169         144 LOAD_FAST                5 (company)
+         194         144 LOAD_FAST                5 (company)
                      146 LOAD_METHOD              4 (get)
                      168 LOAD_CONST               2 ('domain')
                      170 PRECALL                  1
                      174 CALL                     1
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 226)
          
-         170         186 LOAD_GLOBAL             11 (NULL + print)
+         195         186 LOAD_GLOBAL             11 (NULL + print)
                      198 LOAD_CONST               4 ('Missing domain: ')
                      200 LOAD_FAST                5 (company)
                      202 FORMAT_VALUE             0
                      204 LOAD_CONST               5 ('. Skipping')
                      206 BUILD_STRING             3
                      208 PRECALL                  1
                      212 CALL                     1
                      222 POP_TOP
          
-         171         224 JUMP_BACKWARD           44 (to 138)
+         196         224 JUMP_BACKWARD           44 (to 138)
          
-         174     >>  226 LOAD_FAST                5 (company)
+         199     >>  226 LOAD_FAST                5 (company)
                      228 LOAD_CONST               2 ('domain')
                      230 BINARY_SUBSCR
                      240 LOAD_FAST                3 (existing_search_domains)
                      242 CONTAINS_OP              0
                      244 POP_JUMP_FORWARD_IF_FALSE    26 (to 298)
          
-         175         246 LOAD_GLOBAL             11 (NULL + print)
+         200         246 LOAD_GLOBAL             11 (NULL + print)
                      258 LOAD_CONST               6 ('Skipping ')
                      260 LOAD_FAST                5 (company)
                      262 LOAD_CONST               2 ('domain')
                      264 BINARY_SUBSCR
                      274 FORMAT_VALUE             0
                      276 LOAD_CONST               7 (' as already a target')
                      278 BUILD_STRING             3
                      280 PRECALL                  1
                      284 CALL                     1
                      294 POP_TOP
          
-         176         296 JUMP_BACKWARD           80 (to 138)
+         201         296 JUMP_BACKWARD           80 (to 138)
          
-         178     >>  298 LOAD_GLOBAL             11 (NULL + print)
+         203     >>  298 LOAD_GLOBAL             11 (NULL + print)
                      310 LOAD_CONST               8 ('Adding ')
                      312 LOAD_FAST                5 (company)
                      314 LOAD_CONST               2 ('domain')
                      316 BINARY_SUBSCR
                      326 FORMAT_VALUE             0
                      328 LOAD_CONST               9 (' as target')
                      330 BUILD_STRING             3
                      332 PRECALL                  1
                      336 CALL                     1
                      346 POP_TOP
          
-         180         348 LOAD_FAST                4 (con)
+         205         348 LOAD_FAST                4 (con)
                      350 LOAD_METHOD              6 (execute)
          
-         181         372 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+         206         372 LOAD_GLOBAL             15 (NULL + sqlalchemy)
                      384 LOAD_ATTR                8 (text)
          
-         182         394 LOAD_CONST              10 ('\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    ')
+         207         394 LOAD_CONST              10 ('\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    ')
          
-         181         396 PRECALL                  1
+         206         396 PRECALL                  1
                      400 CALL                     1
          
-         189         410 LOAD_FAST                5 (company)
+         214         410 LOAD_FAST                5 (company)
                      412 LOAD_METHOD              4 (get)
                      434 LOAD_CONST               2 ('domain')
                      436 PRECALL                  1
                      440 CALL                     1
          
-         190         450 LOAD_FAST                5 (company)
+         215         450 LOAD_FAST                5 (company)
                      452 LOAD_METHOD              4 (get)
                      474 LOAD_CONST              11 ('name')
                      476 PRECALL                  1
                      480 CALL                     1
          
-         191         490 LOAD_FAST                5 (company)
+         216         490 LOAD_FAST                5 (company)
                      492 LOAD_METHOD              4 (get)
                      514 LOAD_CONST              12 ('description')
                      516 PRECALL                  1
                      520 CALL                     1
          
-         188         530 LOAD_CONST              13 (('domain', 'name', 'description'))
+         213         530 LOAD_CONST              13 (('domain', 'name', 'description'))
                      532 BUILD_CONST_KEY_MAP      3
          
-         180         534 PRECALL                  2
+         205         534 PRECALL                  2
                      538 CALL                     2
                      548 POP_TOP
          
-         195         550 LOAD_FAST                4 (con)
+         220         550 LOAD_FAST                4 (con)
                      552 LOAD_METHOD              6 (execute)
          
-         196         574 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+         221         574 LOAD_GLOBAL             15 (NULL + sqlalchemy)
                      586 LOAD_ATTR                8 (text)
          
-         197         596 LOAD_CONST              14 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
+         222         596 LOAD_CONST              14 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
          
-         196         598 PRECALL                  1
+         221         598 PRECALL                  1
                      602 CALL                     1
          
-         203         612 LOAD_FAST                1 (search_uid)
+         228         612 LOAD_FAST                1 (search_uid)
          
-         204         614 LOAD_FAST                2 (actor_key)
+         229         614 LOAD_FAST                2 (actor_key)
          
-         205         616 LOAD_FAST                5 (company)
+         230         616 LOAD_FAST                5 (company)
                      618 LOAD_METHOD              4 (get)
                      640 LOAD_CONST               2 ('domain')
                      642 PRECALL                  1
                      646 CALL                     1
          
-         206         656 LOAD_CONST              15 ('create')
+         231         656 LOAD_CONST              15 ('create')
          
-         202         658 LOAD_CONST              16 (('search_uid', 'actor_key', 'domain', 'type'))
+         227         658 LOAD_CONST              16 (('search_uid', 'actor_key', 'domain', 'type'))
                      660 BUILD_CONST_KEY_MAP      4
          
-         195         662 PRECALL                  2
+         220         662 PRECALL                  2
                      666 CALL                     2
                      676 POP_TOP
                      678 EXTENDED_ARG             1
                      680 JUMP_BACKWARD          272 (to 138)
          
-         210     >>  682 LOAD_FAST                4 (con)
+         235     >>  682 LOAD_FAST                4 (con)
                      684 LOAD_METHOD              9 (commit)
                      706 PRECALL                  0
                      710 CALL                     0
                      720 POP_TOP
          
-         167         722 LOAD_CONST               3 (None)
+         192         722 LOAD_CONST               3 (None)
                      724 LOAD_CONST               3 (None)
                      726 LOAD_CONST               3 (None)
                      728 PRECALL                  2
                      732 CALL                     2
                      742 POP_TOP
                      744 LOAD_CONST               3 (None)
                      746 RETURN_VALUE
@@ -1429,15 +1510,15 @@
             ('search_uid', 'actor_key', 'domain', 'type')
          names      ('unique_domains', 'to_list', 'db', 'connect', 'get', 'print', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('companies', 'search_uid', 'actor_key', 'existing_search_domains', 'con', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_companies_as_targets'
-         firstlineno 162
+         firstlineno 187
          lnotab
             0x0204500134010a012a012601020314013201020232021801160102ff0e
             082801280128fd04f8100f1801160102ff0e0702010201280102fc04f914
             0f28d5
       code
          argcount  : 0
          nlocals   : 4
@@ -1451,55 +1532,55 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d037c036302640064006400a6020000ab0200
             000000000000000100530023003100730477027803590077010100590001
             00010064005300
-         216           0 RESUME                   0
+         241           0 RESUME                   0
          
-         217           2 LOAD_GLOBAL              0 (db)
+         242           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         218          54 LOAD_CONST               1 ("\n        WITH ranked_actors AS (\n            SELECT \n                a.name,\n                s.uid AS search_uid,\n                COUNT(e.id) AS total_validate_count,\n                ROW_NUMBER() OVER (\n                    PARTITION BY s.uid\n                    ORDER BY COUNT(e.id) DESC\n                ) as rn\n            FROM \n                event e\n            INNER JOIN \n                actor a ON a.key = e.actor_key\n            INNER JOIN \n                search s ON s.uid = e.search_uid\n            WHERE\n                a.type = 'research' AND \n                e.type = 'validate' \n            GROUP BY \n                a.name, s.uid\n        )\n        SELECT \n            name, \n            search_uid, \n            total_validate_count\n        FROM \n            ranked_actors\n        WHERE \n            rn = 1;\n        ")
+         243          54 LOAD_CONST               1 ("\n        WITH ranked_actors AS (\n            SELECT \n                a.name,\n                s.uid AS search_uid,\n                COUNT(e.id) AS total_validate_count,\n                ROW_NUMBER() OVER (\n                    PARTITION BY s.uid\n                    ORDER BY COUNT(e.id) DESC\n                ) as rn\n            FROM \n                event e\n            INNER JOIN \n                actor a ON a.key = e.actor_key\n            INNER JOIN \n                search s ON s.uid = e.search_uid\n            WHERE\n                a.type = 'research' AND \n                e.type = 'validate' \n            GROUP BY \n                a.name, s.uid\n        )\n        SELECT \n            name, \n            search_uid, \n            total_validate_count\n        FROM \n            ranked_actors\n        WHERE \n            rn = 1;\n        ")
                       56 STORE_FAST               1 (statement)
          
-         250          58 LOAD_FAST                0 (conn)
+         275          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         251         136 LOAD_GLOBAL             11 (NULL + pd)
+         276         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         252         252 LOAD_FAST                3 (df)
+         277         252 LOAD_FAST                3 (df)
          
-         217         254 SWAP                     2
+         242         254 SWAP                     2
                      256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 RETURN_VALUE
@@ -1526,15 +1607,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'top_actor_per_search'
-         firstlineno 216
+         firstlineno 241
          lnotab 0x0201340104204e01740102dd
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -1549,73 +1630,76 @@
             000000000000007d027c02a0090000000000000000000000000000000000
             000000640364046405ac06a6030000ab030000000000000000a00a000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a00b00000000000000000000000000000000000000006407a6010000ab
             0100000000000000007d027c026302640064006400a6020000ab02000000
             000000000001005300230031007304770278035900770101005900010001
             0064005300
-         254           0 RESUME                   0
+         280           0 RESUME                   0
          
-         255           2 LOAD_GLOBAL              0 (db)
+         281           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         256          54 LOAD_FAST                0 (conn)
+         282          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         257          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         283          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         258         100 LOAD_CONST               1 ("\n                SELECT search_uid, type, count(DISTINCT domain)\n                FROM event\n                WHERE type in ('create','advance', 'validate', 'send', 'accept')\n                GROUP BY search_uid, type\n                ")
+         284         100 LOAD_CONST               1 ("\n                SELECT search_uid, type, count(DISTINCT domain)\n                FROM event\n                WHERE type in ('create','advance', 'validate', 'send', 'accept')\n                GROUP BY search_uid, type\n                ")
          
-         257         102 PRECALL                  1
+         283         102 PRECALL                  1
                      106 CALL                     1
          
-         256         116 PRECALL                  1
+         282         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         266         132 LOAD_GLOBAL             11 (NULL + pd)
+         292         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         267         248 LOAD_FAST                2 (df)
+         294         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (pivot)
                      272 LOAD_CONST               3 ('search_uid')
                      274 LOAD_CONST               4 ('type')
                      276 LOAD_CONST               5 ('count')
                      278 KW_NAMES                 6
                      280 PRECALL                  3
                      284 CALL                     3
-                     294 LOAD_METHOD             10 (reset_index)
+         
+         295         294 LOAD_METHOD             10 (reset_index)
                      316 PRECALL                  0
                      320 CALL                     0
-                     330 LOAD_METHOD             11 (fillna)
+         
+         296         330 LOAD_METHOD             11 (fillna)
                      352 LOAD_CONST               7 (0)
                      354 PRECALL                  1
                      358 CALL                     1
-                     368 STORE_FAST               2 (df)
          
-         268         370 LOAD_FAST                2 (df)
+         293         368 STORE_FAST               2 (df)
+         
+         298         370 LOAD_FAST                2 (df)
          
-         255         372 SWAP                     2
+         281         372 SWAP                     2
                      374 LOAD_CONST               0 (None)
                      376 LOAD_CONST               0 (None)
                      378 LOAD_CONST               0 (None)
                      380 PRECALL                  2
                      384 CALL                     2
                      394 POP_TOP
                      396 RETURN_VALUE
@@ -1647,16 +1731,16 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'pivot', 'reset_index', 'fillna')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_event_count_by_type'
-         firstlineno 254
-         lnotab 0x020134011801160102ff0eff100a74017a0102f3
+         firstlineno 280
+         lnotab 0x020134011801160102ff0eff100a74022e01240126fd020502ef
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -1676,119 +1760,124 @@
             00a6000000ab000000000000000000640364046405ac06a6040000ab0400
             000000000000007d037c03a00d0000000000000000000000000000000000
             0000006700640ba2016700640ca201ac0da6020000ab0200000000000000
             007d037c03a00e0000000000000000000000000000000000000000640ea6
             010000ab0100000000000000007d03640064006400a6020000ab02000000
             000000000001006e0b230031007304770278035900770101005900010001
             007c035300
-         270           0 RESUME                   0
+         301           0 RESUME                   0
          
-         271           2 LOAD_GLOBAL              0 (db)
+         302           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         272          54 LOAD_CONST               1 ("\n        SELECT \n            s.uid,\n            s.label,\n            (SELECT COUNT(*) \n            FROM event e\n            WHERE \n            e.search_uid = s.uid AND e.created >= EXTRACT(EPOCH FROM (NOW() - INTERVAL '7 days')) and type = 'validate'\n            ) AS recent_validate_count\n        FROM \n            search s;\n        ")
+         303          54 LOAD_CONST               1 ("\n        SELECT \n            s.uid,\n            s.label,\n            (SELECT COUNT(*) \n            FROM event e\n            WHERE \n            e.search_uid = s.uid AND e.created >= EXTRACT(EPOCH FROM (NOW() - INTERVAL '7 days')) and type = 'validate'\n            ) AS recent_validate_count\n        FROM \n            search s;\n        ")
                       56 STORE_FAST               1 (statement)
          
-         284          58 LOAD_FAST                0 (conn)
+         315          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         285         136 LOAD_GLOBAL             11 (NULL + pd)
+         316         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         287         252 LOAD_FAST                3 (df)
+         318         252 LOAD_FAST                3 (df)
                      254 LOAD_METHOD              9 (merge)
          
-         288         276 LOAD_GLOBAL             21 (NULL + top_actor_per_search)
+         319         276 LOAD_GLOBAL             21 (NULL + top_actor_per_search)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 LOAD_CONST               3 ('uid')
                      304 LOAD_CONST               4 ('search_uid')
                      306 LOAD_CONST               5 ('left')
          
-         287         308 KW_NAMES                 6
+         318         308 KW_NAMES                 6
                      310 PRECALL                  4
                      314 CALL                     4
                      324 STORE_FAST               3 (df)
          
-         291         326 LOAD_CONST               7 (<code object _set_group, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 291>)
+         322         326 LOAD_CONST               7 (<code object _set_group, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 322>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               4 (_set_group)
          
-         299         332 LOAD_FAST                3 (df)
+         330         332 LOAD_FAST                3 (df)
                      334 LOAD_METHOD             11 (apply)
                      356 LOAD_FAST                4 (_set_group)
                      358 LOAD_CONST               8 (1)
                      360 KW_NAMES                 9
                      362 PRECALL                  2
                      366 CALL                     2
                      376 LOAD_FAST                3 (df)
                      378 LOAD_CONST              10 ('group')
                      380 STORE_SUBSCR
          
-         301         384 LOAD_FAST                3 (df)
+         332         384 LOAD_FAST                3 (df)
                      386 LOAD_METHOD              9 (merge)
-                     408 LOAD_GLOBAL             25 (NULL + search_event_count_by_type)
+         
+         333         408 LOAD_GLOBAL             25 (NULL + search_event_count_by_type)
                      420 PRECALL                  0
                      424 CALL                     0
-                     434 LOAD_CONST               3 ('uid')
-                     436 LOAD_CONST               4 ('search_uid')
-                     438 LOAD_CONST               5 ('left')
-                     440 KW_NAMES                 6
+         
+         334         434 LOAD_CONST               3 ('uid')
+         
+         335         436 LOAD_CONST               4 ('search_uid')
+         
+         336         438 LOAD_CONST               5 ('left')
+         
+         332         440 KW_NAMES                 6
                      442 PRECALL                  4
                      446 CALL                     4
                      456 STORE_FAST               3 (df)
          
-         303         458 LOAD_FAST                3 (df)
+         339         458 LOAD_FAST                3 (df)
                      460 LOAD_METHOD             13 (sort_values)
          
-         304         482 BUILD_LIST               0
+         340         482 BUILD_LIST               0
                      484 LOAD_CONST              11 (('group', 'recent_validate_count', 'total_validate_count', 'label'))
                      486 LIST_EXTEND              1
          
-         305         488 BUILD_LIST               0
+         341         488 BUILD_LIST               0
                      490 LOAD_CONST              12 ((False, False, False, True))
                      492 LIST_EXTEND              1
          
-         303         494 KW_NAMES                13
+         339         494 KW_NAMES                13
                      496 PRECALL                  2
                      500 CALL                     2
                      510 STORE_FAST               3 (df)
          
-         308         512 LOAD_FAST                3 (df)
+         344         512 LOAD_FAST                3 (df)
                      514 LOAD_METHOD             14 (fillna)
                      536 LOAD_CONST              14 ('')
                      538 PRECALL                  1
                      542 CALL                     1
                      552 STORE_FAST               3 (df)
          
-         271         554 LOAD_CONST               0 (None)
+         302         554 LOAD_CONST               0 (None)
                      556 LOAD_CONST               0 (None)
                      558 LOAD_CONST               0 (None)
                      560 PRECALL                  2
                      564 CALL                     2
                      574 POP_TOP
                      576 JUMP_FORWARD            11 (to 600)
                  >>  578 PUSH_EXC_INFO
@@ -1799,15 +1888,15 @@
                      588 POP_EXCEPT
                      590 RERAISE                  1
                  >>  592 POP_TOP
                      594 POP_EXCEPT
                      596 POP_TOP
                      598 POP_TOP
          
-         310     >>  600 LOAD_FAST                3 (df)
+         346     >>  600 LOAD_FAST                3 (df)
                      602 RETURN_VALUE
          ExceptionTable:
            52 to 552 -> 578 [1] lasti
            578 to 584 -> 586 [3] lasti
            592 to 592 -> 586 [3] lasti
          consts
             None
@@ -1822,37 +1911,37 @@
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064011900000000000000000064026b04000000007202640353
                   007c0064041900000000000000000064056b040000000072026406530064
                   075300
-               291           0 RESUME                   0
+               322           0 RESUME                   0
                
-               292           2 LOAD_FAST                0 (row)
+               323           2 LOAD_FAST                0 (row)
                              4 LOAD_CONST               1 ('recent_validate_count')
                              6 BINARY_SUBSCR
                             16 LOAD_CONST               2 (0)
                             18 COMPARE_OP               4 (>)
                             24 POP_JUMP_FORWARD_IF_FALSE     2 (to 30)
                
-               293          26 LOAD_CONST               3 ('Trending Searches')
+               324          26 LOAD_CONST               3 ('Trending Searches')
                             28 RETURN_VALUE
                
-               294     >>   30 LOAD_FAST                0 (row)
+               325     >>   30 LOAD_FAST                0 (row)
                             32 LOAD_CONST               4 ('total_validate_count')
                             34 BINARY_SUBSCR
                             44 LOAD_CONST               5 (25)
                             46 COMPARE_OP               4 (>)
                             52 POP_JUMP_FORWARD_IF_FALSE     2 (to 58)
                
-               295          54 LOAD_CONST               6 ('Top Searches')
+               326          54 LOAD_CONST               6 ('Top Searches')
                             56 RETURN_VALUE
                
-               297     >>   58 LOAD_CONST               7 ('All Searches')
+               328     >>   58 LOAD_CONST               7 ('All Searches')
                             60 RETURN_VALUE
                consts
                   None
                   'recent_validate_count'
                   0
                   'Trending Searches'
                   'total_validate_count'
@@ -1861,33 +1950,33 @@
                   'All Searches'
                names      ()
                varnames   ('row',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '_set_group'
-               firstlineno 291
+               firstlineno 322
                lnotab 0x02011801040118010402
             1
             ('axis',)
             'group'
             ('group', 'recent_validate_count', 'total_validate_count', 'label')
             (False, False, False, True)
             ('by', 'ascending')
             ''
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'merge', 'top_actor_per_search', 'apply', 'search_event_count_by_type', 'sort_values', 'fillna')
          varnames   ('conn', 'statement', 'result', 'df', '_set_group')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search'
-         firstlineno 270
+         firstlineno 301
          lnotab
-            0x02013401040c4e017402180120ff1204060834024a021801060106fe12
-            052adb2e27
+            0x02013401040c4e017402180120ff12040608340218011a010201020102
+            fc12071801060106fe12052ad62e2c
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -1898,66 +1987,66 @@
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d027c02a0090000000000000000000000000000000000
             00000067006403a201ac02a6010000ab0100000000000000007d027c0263
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         312           0 RESUME                   0
+         349           0 RESUME                   0
          
-         313           2 LOAD_GLOBAL              0 (db)
+         350           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         314          54 LOAD_FAST                0 (conn)
+         351          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         315          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         352          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         316         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
+         353         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
          
-         315         102 PRECALL                  1
+         352         102 PRECALL                  1
                      106 CALL                     1
          
-         314         116 PRECALL                  1
+         351         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         321         132 LOAD_GLOBAL             11 (NULL + pd)
+         358         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         322         248 LOAD_FAST                2 (df)
+         359         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (drop)
                      272 BUILD_LIST               0
                      274 LOAD_CONST               3 (('id', 'created', 'updated'))
                      276 LIST_EXTEND              1
                      278 KW_NAMES                 2
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_FAST               2 (df)
          
-         323         296 LOAD_FAST                2 (df)
+         360         296 LOAD_FAST                2 (df)
          
-         313         298 SWAP                     2
+         350         298 SWAP                     2
                      300 LOAD_CONST               0 (None)
                      302 LOAD_CONST               0 (None)
                      304 LOAD_CONST               0 (None)
                      306 PRECALL                  2
                      310 CALL                     2
                      320 POP_TOP
                      322 RETURN_VALUE
@@ -1985,15 +2074,15 @@
             ('id', 'created', 'updated')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'drop')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'actor'
-         firstlineno 312
+         firstlineno 349
          lnotab 0x020134011801160102ff0eff10077401300102f6
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 7
          flags     : 3
          code
@@ -2016,60 +2105,60 @@
             00000000000000a00e000000000000000000000000000000000000000064
             086405a6020000ab0200000000000000007c076a0d0000000000000000a0
             0e00000000000000000000000000000000000000006409a6010000ab0100
             00000000000000640a6b0200000000ac0ba6020000ab0200000000000000
             007d05740b000000000000000000006a0f00000000000000007c05640c19
             000000000000000000a6010000ab0100000000000000007c05640c3c0000
             007c055300
-         326           0 RESUME                   0
+         363           0 RESUME                   0
          
-         327           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            (c.meta->>'year_founded') AS year_founded,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'headquarters') AS headquarters,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating,\n            c.meta as meta\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
+         364           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            (c.meta->>'year_founded') AS year_founded,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'headquarters') AS headquarters,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating,\n            c.meta as meta\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
                        4 STORE_FAST               2 (statement)
          
-         376           6 LOAD_GLOBAL              0 (db)
+         413           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               3 (conn)
          
-         377          58 LOAD_FAST                3 (conn)
+         414          58 LOAD_FAST                3 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         378          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         415          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         379         120 LOAD_FAST                0 (search_uid)
+         416         120 LOAD_FAST                0 (search_uid)
                      122 LOAD_FAST                1 (last_event_type)
                      124 LOAD_CONST               2 (('search_uid', 'last_event_type'))
                      126 BUILD_CONST_KEY_MAP      2
          
-         377         128 PRECALL                  2
+         414         128 PRECALL                  2
                      132 CALL                     2
                      142 STORE_FAST               4 (result)
          
-         381         144 LOAD_GLOBAL             11 (NULL + pd)
+         418         144 LOAD_GLOBAL             11 (NULL + pd)
                      156 LOAD_ATTR                6 (DataFrame)
                      166 LOAD_FAST                4 (result)
                      168 LOAD_METHOD              7 (fetchall)
                      190 PRECALL                  0
                      194 CALL                     0
                      204 LOAD_FAST                4 (result)
                      206 LOAD_METHOD              8 (keys)
                      228 PRECALL                  0
                      232 CALL                     0
                      242 KW_NAMES                 3
                      244 PRECALL                  2
                      248 CALL                     2
                      258 STORE_FAST               5 (targets)
          
-         376         260 LOAD_CONST               0 (None)
+         413         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 JUMP_FORWARD            11 (to 306)
                  >>  284 PUSH_EXC_INFO
@@ -2080,82 +2169,82 @@
                      294 POP_EXCEPT
                      296 RERAISE                  1
                  >>  298 POP_TOP
                      300 POP_EXCEPT
                      302 POP_TOP
                      304 POP_TOP
          
-         383     >>  306 LOAD_FAST                5 (targets)
+         420     >>  306 LOAD_FAST                5 (targets)
                      308 LOAD_FAST                5 (targets)
                      310 LOAD_CONST               4 ('last_event_type')
                      312 BINARY_SUBSCR
                      322 LOAD_FAST                1 (last_event_type)
                      324 COMPARE_OP               2 (==)
                      330 BINARY_SUBSCR
                      340 STORE_FAST               5 (targets)
          
-         384         342 LOAD_GLOBAL             19 (NULL + comment_by_domain)
+         421         342 LOAD_GLOBAL             19 (NULL + comment_by_domain)
                      354 LOAD_FAST                0 (search_uid)
                      356 PRECALL                  1
                      360 CALL                     1
                      370 STORE_FAST               6 (comments)
          
-         385         372 LOAD_FAST                5 (targets)
+         422         372 LOAD_FAST                5 (targets)
                      374 LOAD_METHOD             10 (merge)
                      396 LOAD_FAST                6 (comments)
                      398 LOAD_CONST               5 ('domain')
                      400 LOAD_CONST               6 ('left')
                      402 KW_NAMES                 7
                      404 PRECALL                  3
                      408 CALL                     3
                      418 STORE_FAST               5 (targets)
          
-         388         420 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
+         425         420 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
                      432 LOAD_FAST                0 (search_uid)
                      434 PRECALL                  1
                      438 CALL                     1
                      448 STORE_FAST               7 (search)
          
-         389         450 LOAD_FAST                5 (targets)
+         426         450 LOAD_FAST                5 (targets)
                      452 LOAD_METHOD             12 (sort_values)
          
-         390         474 LOAD_FAST                7 (search)
+         427         474 LOAD_FAST                7 (search)
                      476 LOAD_ATTR               13 (sort)
                      486 LOAD_METHOD             14 (get)
                      508 LOAD_CONST               8 ('field')
                      510 LOAD_CONST               5 ('domain')
                      512 PRECALL                  2
                      516 CALL                     2
          
-         391         526 LOAD_FAST                7 (search)
+         428         526 LOAD_FAST                7 (search)
                      528 LOAD_ATTR               13 (sort)
                      538 LOAD_METHOD             14 (get)
                      560 LOAD_CONST               9 ('order')
                      562 PRECALL                  1
                      566 CALL                     1
                      576 LOAD_CONST              10 ('asc')
                      578 COMPARE_OP               2 (==)
          
-         389         584 KW_NAMES                11
+         426         584 KW_NAMES                11
                      586 PRECALL                  2
                      590 CALL                     2
                      600 STORE_FAST               5 (targets)
          
-         393         602 LOAD_GLOBAL             11 (NULL + pd)
+         430         602 LOAD_GLOBAL             11 (NULL + pd)
                      614 LOAD_ATTR               15 (to_numeric)
                      624 LOAD_FAST                5 (targets)
                      626 LOAD_CONST              12 ('employees')
                      628 BINARY_SUBSCR
                      638 PRECALL                  1
                      642 CALL                     1
                      652 LOAD_FAST                5 (targets)
                      654 LOAD_CONST              12 ('employees')
                      656 STORE_SUBSCR
          
-         394         660 LOAD_FAST                5 (targets)
+         431         660 LOAD_FAST                5 (targets)
                      662 RETURN_VALUE
          ExceptionTable:
            56 to 258 -> 284 [1] lasti
            284 to 290 -> 292 [3] lasti
            298 to 298 -> 292 [3] lasti
          consts
             None
@@ -2173,15 +2262,15 @@
             'employees'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get', 'to_numeric')
          varnames   ('search_uid', 'last_event_type', 'statement', 'conn', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_target_by_last_event_type'
-         firstlineno 326
+         firstlineno 363
          lnotab
             0x0201043134011801260108fe100474fb2e0724011e0130031e01180134
             013afe12043a01
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
@@ -2194,59 +2283,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         456           0 RESUME                   0
+         492           0 RESUME                   0
          
-         457           2 LOAD_GLOBAL              0 (db)
+         493           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         458          54 LOAD_CONST               1 ("\n            SELECT \n                e.type AS last_event_type,\n                COUNT(e.type)\n            FROM (\n                SELECT \n                    search_uid, \n                    domain, \n                    MAX(created) AS max_created\n                FROM \n                    event\n                WHERE \n                    type NOT IN ('comment','rating','generate','criteria')\n                    and search_uid = :search_uid\n                GROUP BY \n                    domain, search_uid\n            ) AS max_event\n            JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid\n            GROUP BY e.type;\n        ")
+         494          54 LOAD_CONST               1 ("\n            SELECT \n                e.type AS last_event_type,\n                COUNT(e.type)\n            FROM (\n                SELECT \n                    search_uid, \n                    domain, \n                    MAX(created) AS max_created\n                FROM \n                    event\n                WHERE \n                    type NOT IN ('comment','rating','generate','criteria')\n                    and search_uid = :search_uid\n                GROUP BY \n                    domain, search_uid\n            ) AS max_event\n            JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid\n            GROUP BY e.type;\n        ")
                       56 STORE_FAST               2 (statement)
          
-         478          58 LOAD_FAST                1 (conn)
+         514          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         479          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         515          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         480         120 LOAD_CONST               2 ('search_uid')
+         516         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         478         126 PRECALL                  2
+         514         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         482         142 LOAD_GLOBAL             11 (NULL + pd)
+         518         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         457         258 LOAD_CONST               0 (None)
+         493         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2257,15 +2346,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         483     >>  304 LOAD_FAST                4 (df)
+         519     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2274,15 +2363,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target_count'
-         firstlineno 456
+         firstlineno 492
          lnotab 0x0201340104141801260106fe100474e72e1a
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2293,56 +2382,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         486           0 RESUME                   0
+         522           0 RESUME                   0
          
-         487           2 LOAD_GLOBAL              0 (db)
+         523           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         488          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         524          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         493          58 LOAD_FAST                1 (conn)
+         529          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         494         142 LOAD_GLOBAL             11 (NULL + pd)
+         530         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         487         258 LOAD_CONST               0 (None)
+         523         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2353,15 +2442,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         495     >>  304 LOAD_FAST                4 (df)
+         531     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2370,15 +2459,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 486
+         firstlineno 522
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2389,56 +2478,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         498           0 RESUME                   0
+         534           0 RESUME                   0
          
-         499           2 LOAD_GLOBAL              0 (db)
+         535           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         500          54 LOAD_CONST               1 ('\n                SELECT distinct(domain)\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         536          54 LOAD_CONST               1 ('\n                SELECT distinct(domain)\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         505          58 LOAD_FAST                1 (conn)
+         541          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         506         142 LOAD_GLOBAL             11 (NULL + pd)
+         542         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         499         258 LOAD_CONST               0 (None)
+         535         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2449,15 +2538,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         507     >>  304 LOAD_FAST                4 (df)
+         543     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2466,15 +2555,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'unique_domains'
-         firstlineno 498
+         firstlineno 534
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2485,53 +2574,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         510           0 RESUME                   0
+         546           0 RESUME                   0
          
-         511           2 LOAD_GLOBAL              0 (db)
+         547           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         512          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
+         548          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
                       56 STORE_FAST               1 (statement)
          
-         516          58 LOAD_FAST                0 (conn)
+         552          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         517         136 LOAD_GLOBAL             11 (NULL + pd)
+         553         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         511         252 LOAD_CONST               0 (None)
+         547         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -2542,15 +2631,15 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         518     >>  298 LOAD_FAST                3 (df)
+         554     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            52 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -2558,15 +2647,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'company'
-         firstlineno 510
+         firstlineno 546
          lnotab 0x0201340104044e0174fa2e07
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2577,56 +2666,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         521           0 RESUME                   0
+         557           0 RESUME                   0
          
-         522           2 LOAD_GLOBAL              0 (db)
+         558           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         523          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
+         559          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         529          58 LOAD_FAST                1 (conn)
+         565          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         530         142 LOAD_GLOBAL             11 (NULL + pd)
+         566         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         522         258 LOAD_CONST               0 (None)
+         558         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2637,15 +2726,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         531     >>  304 LOAD_FAST                4 (df)
+         567     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2654,15 +2743,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 521
+         firstlineno 557
          lnotab 0x020134010406540174f82e09
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2677,59 +2766,59 @@
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c04a009000000000000000000000000000000000000000064
             04a6010000ab010000000000000000a00a00000000000000000000000000
             000000000000006405640684006901a6010000ab010000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-         534           0 RESUME                   0
+         570           0 RESUME                   0
          
-         535           2 LOAD_GLOBAL              0 (db)
+         571           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         536          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         572          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         543          58 LOAD_FAST                1 (conn)
+         579          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         544          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         580          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         545         120 LOAD_CONST               2 ('search_uid')
+         581         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         543         126 PRECALL                  2
+         579         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         547         142 LOAD_GLOBAL             11 (NULL + pd)
+         583         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         535         258 LOAD_CONST               0 (None)
+         571         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2740,22 +2829,22 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         549     >>  304 LOAD_FAST                4 (df)
+         585     >>  304 LOAD_FAST                4 (df)
                      306 LOAD_METHOD              9 (groupby)
                      328 LOAD_CONST               4 ('domain')
                      330 PRECALL                  1
                      334 CALL                     1
                      344 LOAD_METHOD             10 (agg)
                      366 LOAD_CONST               5 ('comment')
-                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 549>)
+                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 585>)
                      370 MAKE_FUNCTION            0
                      372 BUILD_MAP                1
                      374 PRECALL                  1
                      378 CALL                     1
                      388 LOAD_METHOD             11 (reset_index)
                      410 PRECALL                  0
                      414 CALL                     0
@@ -2775,37 +2864,37 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               549           0 RESUME                   0
+               585           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 549
+               firstlineno 585
                lnotab 0x
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 534
+         firstlineno 570
          lnotab 0x0201340104071801260106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2820,41 +2909,41 @@
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000007d05741900
             0000000000000000007c056a0d0000000000000000a6010000ab01000000
             000000000001007c055300
-         555           0 RESUME                   0
+         591           0 RESUME                   0
          
-         556           2 LOAD_GLOBAL              0 (db)
+         592           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         557          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         593          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         562          58 LOAD_FAST                1 (conn)
+         598          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         556         142 LOAD_CONST               0 (None)
+         592         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -2865,24 +2954,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         564     >>  188 LOAD_FAST                3 (result)
+         600     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         565         210 LOAD_CONST               0 (None)
+         601         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         567     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         603     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -2890,29 +2979,29 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         568         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         604         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Search)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 STORE_FAST               5 (search)
          
-         569         386 LOAD_GLOBAL             25 (NULL + print)
+         605         386 LOAD_GLOBAL             25 (NULL + print)
                      398 LOAD_FAST                5 (search)
                      400 LOAD_ATTR               13 (label)
                      410 PRECALL                  1
                      414 CALL                     1
                      424 POP_TOP
          
-         570         426 LOAD_FAST                5 (search)
+         606         426 LOAD_FAST                5 (search)
                      428 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
            166 to 172 -> 174 [3] lasti
            180 to 180 -> 174 [3] lasti
          consts
             None
@@ -2921,15 +3010,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search', 'print', 'label')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 555
+         firstlineno 591
          lnotab 0x02013401040554fa2e081601040282012a012801
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -2943,41 +3032,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         573           0 RESUME                   0
+         609           0 RESUME                   0
          
-         574           2 LOAD_GLOBAL              0 (db)
+         610           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         575          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         611          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         580          58 LOAD_FAST                1 (conn)
+         616          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         574         142 LOAD_CONST               0 (None)
+         610         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -2988,24 +3077,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         582     >>  188 LOAD_FAST                3 (result)
+         618     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         583         210 LOAD_CONST               0 (None)
+         619         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         585     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         621     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3013,15 +3102,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         586         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         622         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3034,15 +3123,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 573
+         firstlineno 609
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3056,41 +3145,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         589           0 RESUME                   0
+         625           0 RESUME                   0
          
-         590           2 LOAD_GLOBAL              0 (db)
+         626           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         591          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         627          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         596          58 LOAD_FAST                1 (conn)
+         632          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('event_id')
                      122 LOAD_FAST                0 (event_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         590         142 LOAD_CONST               0 (None)
+         626         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3101,24 +3190,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         598     >>  188 LOAD_FAST                3 (result)
+         634     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         599         210 LOAD_CONST               0 (None)
+         635         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         601     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         637     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3126,15 +3215,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         602         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         638         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3147,15 +3236,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 589
+         firstlineno 625
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 11
          flags     : 3
          code
@@ -3166,68 +3255,68 @@
             007c006a0500000000000000007c006a0600000000000000007c006a0700
             000000000000007c006a0800000000000000007413000000000000000000
             006a0a00000000000000007c006a0b0000000000000000a6010000ab0100
             0000000000000064029c05a6020000ab02000000000000000001007c01a0
             0c0000000000000000000000000000000000000000a6000000ab00000000
             00000000000100640064006400a6020000ab020000000000000000010064
             0053002300310073047702780359007701010059000100010064005300
-         608           0 RESUME                   0
+         644           0 RESUME                   0
          
-         609           2 LOAD_GLOBAL              0 (db)
+         645           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         610          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         646          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         621          58 LOAD_FAST                1 (conn)
+         657          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         622          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         658          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         624         120 LOAD_FAST                0 (company)
+         660         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         625         132 LOAD_FAST                0 (company)
+         661         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         626         144 LOAD_FAST                0 (company)
+         662         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         627         156 LOAD_FAST                0 (company)
+         663         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         628         168 LOAD_GLOBAL             19 (NULL + json)
+         664         168 LOAD_GLOBAL             19 (NULL + json)
                      180 LOAD_ATTR               10 (dumps)
                      190 LOAD_FAST                0 (company)
                      192 LOAD_ATTR               11 (meta)
                      202 PRECALL                  1
                      206 CALL                     1
          
-         623         216 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'meta'))
+         659         216 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'meta'))
                      218 BUILD_CONST_KEY_MAP      5
          
-         621         220 PRECALL                  2
+         657         220 PRECALL                  2
                      224 CALL                     2
                      234 POP_TOP
          
-         632         236 LOAD_FAST                1 (conn)
+         668         236 LOAD_FAST                1 (conn)
                      238 LOAD_METHOD             12 (commit)
                      260 PRECALL                  0
                      264 CALL                     0
                      274 POP_TOP
          
-         609         276 LOAD_CONST               0 (None)
+         645         276 LOAD_CONST               0 (None)
                      278 LOAD_CONST               0 (None)
                      280 LOAD_CONST               0 (None)
                      282 PRECALL                  2
                      286 CALL                     2
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
@@ -3254,15 +3343,15 @@
             ('uid', 'name', 'description', 'domain', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 608
+         firstlineno 644
          lnotab 0x02013401040b180126020c010c010c010c0130fb04fe100b28e9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 10
          flags     : 3
          code
@@ -3277,79 +3366,79 @@
             00000000000000a6010000ab010000000000000000740b00000000000000
             0000006a0600000000000000007c006a0a0000000000000000a6010000ab
             0100000000000000007c006a0b000000000000000064029c05a6020000ab
             02000000000000000001007c01a00c000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         635           0 RESUME                   0
+         671           0 RESUME                   0
          
-         636           2 LOAD_GLOBAL              0 (db)
+         672           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         637          54 LOAD_FAST                1 (conn)
+         673          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         638          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         674          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         639         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion,\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         675         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion,\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         638         102 PRECALL                  1
+         674         102 PRECALL                  1
                      106 CALL                     1
          
-         651         116 LOAD_GLOBAL             11 (NULL + json)
+         687         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (sort)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         652         164 LOAD_GLOBAL             11 (NULL + json)
+         688         164 LOAD_GLOBAL             11 (NULL + json)
                      176 LOAD_ATTR                6 (dumps)
                      186 LOAD_FAST                0 (search)
                      188 LOAD_ATTR                8 (inclusion)
                      198 PRECALL                  1
                      202 CALL                     1
          
-         653         212 LOAD_GLOBAL             11 (NULL + json)
+         689         212 LOAD_GLOBAL             11 (NULL + json)
                      224 LOAD_ATTR                6 (dumps)
                      234 LOAD_FAST                0 (search)
                      236 LOAD_ATTR                9 (exclusion)
                      246 PRECALL                  1
                      250 CALL                     1
          
-         654         260 LOAD_GLOBAL             11 (NULL + json)
+         690         260 LOAD_GLOBAL             11 (NULL + json)
                      272 LOAD_ATTR                6 (dumps)
                      282 LOAD_FAST                0 (search)
                      284 LOAD_ATTR               10 (meta)
                      294 PRECALL                  1
                      298 CALL                     1
          
-         655         308 LOAD_FAST                0 (search)
+         691         308 LOAD_FAST                0 (search)
                      310 LOAD_ATTR               11 (uid)
          
-         650         320 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'meta', 'uid'))
+         686         320 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'meta', 'uid'))
                      322 BUILD_CONST_KEY_MAP      5
          
-         637         324 PRECALL                  2
+         673         324 PRECALL                  2
                      328 CALL                     2
                      338 POP_TOP
          
-         658         340 LOAD_FAST                1 (conn)
+         694         340 LOAD_FAST                1 (conn)
                      342 LOAD_METHOD             12 (commit)
                      364 PRECALL                  0
                      368 CALL                     0
                      378 POP_TOP
          
-         636         380 LOAD_CONST               0 (None)
+         672         380 LOAD_CONST               0 (None)
                      382 LOAD_CONST               0 (None)
                      384 LOAD_CONST               0 (None)
                      386 PRECALL                  2
                      390 CALL                     2
                      400 POP_TOP
                      402 LOAD_CONST               0 (None)
                      404 RETURN_VALUE
@@ -3376,22 +3465,22 @@
             ('sort', 'inclusion', 'exclusion', 'meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 635
+         firstlineno 671
          lnotab 0x020134011801160102ff0e0d30013001300130010cfb04f3101528ea
       (None,)
    names      ('json', 'dataclasses', 'asdict', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'google.cloud.sql.connector', 'Connector', 'gandai', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Checkpoint', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'str', 'int', 'insert_targets_from_domains', 'insert_companies_as_targets', 'DataFrame', 'top_actor_per_search', 'search_event_count_by_type', 'search', 'actor', 'search_target_by_last_event_type', 'target_count', 'event', 'unique_domains', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'find_event_by_id', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c011002080108010c010c010c0214020c010c01200214
       060c0e1015100f1013100d02010eff020102ff020102ff020102ff020202
-      fe083902010eff020102ff020102ff020202fe083616261610062a160e12
-      7f00031a1e1a0c1a0c160b1a0d1a15101210101013101b
+      fe085202010eff020102ff020102ff020202fe0836162716150630160e12
+      7f00021a1e1a0c1a0c160b1a0d1a15101210101013101b
```

### Comparing `gandai-1.3.7/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.3.8/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1adbc264 (Thu Jul 27 21:01:14 2023 UTC)
-files sz: 11623
+moddate:  0xd605c864 (Mon Jul 31 19:04:54 2023 UTC)
+files sz: 11690
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c036d045a0401
@@ -103,26 +103,26 @@
                180 LOAD_CONST              10 (<code object GoogleMapsWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 17>)
                182 MAKE_FUNCTION            0
                184 LOAD_CONST              11 ('GoogleMapsWrapper')
                186 PRECALL                  2
                190 CALL                     2
                200 STORE_NAME              23 (GoogleMapsWrapper)
    
-   172         202 PUSH_NULL
+   173         202 PUSH_NULL
                204 LOAD_BUILD_CLASS
-               206 LOAD_CONST              12 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 172>)
+               206 LOAD_CONST              12 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 173>)
                208 MAKE_FUNCTION            0
                210 LOAD_CONST              13 ('GrataWrapper')
                212 PRECALL                  2
                216 CALL                     2
                226 STORE_NAME              24 (GrataWrapper)
    
-   344         228 PUSH_NULL
+   345         228 PUSH_NULL
                230 LOAD_BUILD_CLASS
-               232 LOAD_CONST              14 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 344>)
+               232 LOAD_CONST              14 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 345>)
                234 MAKE_FUNCTION            0
                236 LOAD_CONST              15 ('SourceScrubWrapper')
                238 PRECALL                  2
                242 CALL                     2
                252 STORE_NAME              25 (SourceScrubWrapper)
                254 LOAD_CONST               1 (None)
                256 RETURN_VALUE
@@ -278,21 +278,21 @@
                      212 MAKE_FUNCTION            5 (defaults, annotations)
          
           91         214 PRECALL                  0
                      218 CALL                     0
          
           92         228 STORE_NAME              16 (build_target_from_place_id)
          
-         162         230 LOAD_CONST              18 ('place_ids')
+         163         230 LOAD_CONST              18 ('place_ids')
                      232 LOAD_NAME               11 (list)
                      234 LOAD_CONST              19 ('search')
                      236 LOAD_NAME               14 (models)
                      238 LOAD_ATTR               17 (Search)
                      248 BUILD_TUPLE              4
-                     250 LOAD_CONST              20 (<code object build_place_ids_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 162>)
+                     250 LOAD_CONST              20 (<code object build_place_ids_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 163>)
                      252 MAKE_FUNCTION            4 (annotations)
                      254 STORE_NAME              18 (build_place_ids_async)
                      256 LOAD_CONST              14 (None)
                      258 RETURN_VALUE
          consts
             'GoogleMapsWrapper'
             'San Diego, CA'
@@ -887,224 +887,224 @@
                            172 PRECALL                  1
                            176 CALL                     1
                            186 POP_TOP
                
                106         188 LOAD_CONST               5 (None)
                            190 RETURN_VALUE
                
-               108     >>  192 LOAD_GLOBAL             13 (NULL + helpers)
+               109     >>  192 LOAD_GLOBAL             13 (NULL + helpers)
                            204 LOAD_ATTR                7 (clean_domain)
                            214 LOAD_FAST                3 (place)
                            216 LOAD_CONST               3 ('website')
                            218 BINARY_SUBSCR
                            228 PRECALL                  1
                            232 CALL                     1
                            242 LOAD_FAST                4 (existing_search_domains)
                            244 CONTAINS_OP              0
                            246 POP_JUMP_FORWARD_IF_FALSE    29 (to 306)
                
-               109         248 LOAD_GLOBAL             11 (NULL + print)
+               110         248 LOAD_GLOBAL             11 (NULL + print)
                            260 LOAD_CONST               6 ('skipping ')
                            262 LOAD_FAST                3 (place)
                            264 LOAD_CONST               3 ('website')
                            266 BINARY_SUBSCR
                            276 FORMAT_VALUE             0
                            278 LOAD_CONST               7 (' - already in search_uid ')
                            280 LOAD_FAST                1 (search_uid)
                            282 FORMAT_VALUE             0
                            284 BUILD_STRING             4
                            286 PRECALL                  1
                            290 CALL                     1
                            300 POP_TOP
                
-               110         302 LOAD_CONST               5 (None)
+               111         302 LOAD_CONST               5 (None)
                            304 RETURN_VALUE
                
-               112     >>  306 LOAD_CONST               8 (' ')
+               113     >>  306 LOAD_CONST               8 (' ')
                            308 LOAD_METHOD              8 (join)
                
-               114         330 LOAD_CONST               9 ('Q: Based on these reviews:')
+               115         330 LOAD_CONST               9 ('Q: Based on these reviews:')
                
-               115         332 LOAD_CONST              10 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 115>)
+               116         332 LOAD_CONST              10 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 116>)
                            334 MAKE_FUNCTION            0
                            336 LOAD_FAST                3 (place)
                            338 LOAD_CONST              11 ('reviews')
                            340 BINARY_SUBSCR
                            350 GET_ITER
                            352 PRECALL                  0
                            356 CALL                     0
                            366 FORMAT_VALUE             0
                
-               116         368 LOAD_CONST              12 ('as well as what you already know about ')
+               117         368 LOAD_CONST              12 ('as well as what you already know about ')
                            370 LOAD_FAST                3 (place)
                            372 LOAD_CONST               3 ('website')
                            374 BINARY_SUBSCR
                            384 FORMAT_VALUE             0
                            386 LOAD_CONST              13 (',')
                            388 BUILD_STRING             3
                
-               117         390 LOAD_CONST              14 ('what products and services does ')
+               118         390 LOAD_CONST              14 ('what products and services does ')
                            392 LOAD_FAST                3 (place)
                            394 LOAD_CONST              15 ('name')
                            396 BINARY_SUBSCR
                            406 FORMAT_VALUE             0
                            408 LOAD_CONST              16 (' offer?')
                            410 BUILD_STRING             3
                
-               113         412 BUILD_LIST               4
+               114         412 BUILD_LIST               4
                
-               112         414 PRECALL                  1
+               113         414 PRECALL                  1
                            418 CALL                     1
                            428 STORE_FAST               5 (gpt_prompt)
                
-               120         430 LOAD_FAST                2 (append_to_prompt)
+               121         430 LOAD_FAST                2 (append_to_prompt)
                            432 POP_JUMP_FORWARD_IF_FALSE     8 (to 450)
                
-               121         434 LOAD_FAST                5 (gpt_prompt)
+               122         434 LOAD_FAST                5 (gpt_prompt)
                            436 LOAD_CONST               8 (' ')
                            438 LOAD_FAST                2 (append_to_prompt)
                            440 BINARY_OP                0 (+)
                            444 BINARY_OP               13 (+=)
                            448 STORE_FAST               5 (gpt_prompt)
                
-               124     >>  450 LOAD_GLOBAL             19 (NULL + models)
+               125     >>  450 LOAD_GLOBAL             19 (NULL + models)
                            462 LOAD_ATTR               10 (Company)
                
-               125         472 LOAD_FAST                3 (place)
+               126         472 LOAD_FAST                3 (place)
                            474 LOAD_CONST              15 ('name')
                            476 BINARY_SUBSCR
                
-               126         486 LOAD_GLOBAL             13 (NULL + helpers)
+               127         486 LOAD_GLOBAL             13 (NULL + helpers)
                            498 LOAD_ATTR                7 (clean_domain)
                            508 LOAD_FAST                3 (place)
                            510 LOAD_CONST               3 ('website')
                            512 BINARY_SUBSCR
                            522 PRECALL                  1
                            526 CALL                     1
                
-               127         536 LOAD_CONST              17 ('')
+               128         536 LOAD_CONST              17 ('')
                
-               124         538 KW_NAMES                18
+               125         538 KW_NAMES                18
                            540 PRECALL                  3
                            544 CALL                     3
                            554 STORE_FAST               6 (company)
                
-               130         556 LOAD_GLOBAL              5 (NULL + query)
+               131         556 LOAD_GLOBAL              5 (NULL + query)
                            568 LOAD_ATTR               11 (insert_company)
                            578 LOAD_FAST                6 (company)
                            580 PRECALL                  1
                            584 CALL                     1
                            594 POP_TOP
                
-               133         596 LOAD_GLOBAL              5 (NULL + query)
+               134         596 LOAD_GLOBAL              5 (NULL + query)
                            608 LOAD_ATTR               12 (find_company_by_domain)
                            618 LOAD_FAST                6 (company)
                            620 LOAD_ATTR               13 (domain)
                            630 PRECALL                  1
                            634 CALL                     1
                            644 STORE_FAST               6 (company)
                
-               134         646 LOAD_CONST              19 ('google_places')
+               135         646 LOAD_CONST              19 ('google_places')
                            648 LOAD_FAST                6 (company)
                            650 LOAD_ATTR               14 (meta)
                            660 CONTAINS_OP              1
                            662 POP_JUMP_FORWARD_IF_FALSE    10 (to 684)
                
-               135         664 BUILD_MAP                0
+               136         664 BUILD_MAP                0
                            666 LOAD_FAST                6 (company)
                            668 LOAD_ATTR               14 (meta)
                            678 LOAD_CONST              19 ('google_places')
                            680 STORE_SUBSCR
                
-               136     >>  684 LOAD_FAST                3 (place)
+               137     >>  684 LOAD_FAST                3 (place)
                            686 LOAD_FAST                6 (company)
                            688 LOAD_ATTR               14 (meta)
                            698 LOAD_CONST              19 ('google_places')
                            700 BINARY_SUBSCR
                            710 LOAD_FAST                0 (place_id)
                            712 STORE_SUBSCR
                
-               137         716 LOAD_GLOBAL              5 (NULL + query)
+               138         716 LOAD_GLOBAL              5 (NULL + query)
                            728 LOAD_ATTR               15 (update_company)
                            738 LOAD_FAST                6 (company)
                            740 PRECALL                  1
                            744 CALL                     1
                            754 POP_TOP
                
-               140         756 LOAD_GLOBAL             11 (NULL + print)
+               141         756 LOAD_GLOBAL             11 (NULL + print)
                            768 LOAD_CONST              20 ('adding ')
                            770 LOAD_FAST                6 (company)
                            772 LOAD_ATTR               13 (domain)
                            782 FORMAT_VALUE             0
                            784 LOAD_CONST              21 (' - search_uid ')
                            786 LOAD_FAST                1 (search_uid)
                            788 FORMAT_VALUE             0
                            790 BUILD_STRING             4
                            792 PRECALL                  1
                            796 CALL                     1
                            806 POP_TOP
                
-               141         808 LOAD_GLOBAL              5 (NULL + query)
+               142         808 LOAD_GLOBAL              5 (NULL + query)
                            820 LOAD_ATTR               16 (insert_event)
                
-               142         830 LOAD_GLOBAL             19 (NULL + models)
+               143         830 LOAD_GLOBAL             19 (NULL + models)
                            842 LOAD_ATTR               17 (Event)
                
-               143         852 LOAD_FAST                1 (search_uid)
+               144         852 LOAD_FAST                1 (search_uid)
                
-               144         854 LOAD_CONST              22 ('chatgpt')
+               145         854 LOAD_CONST              22 ('chatgpt')
                
-               145         856 LOAD_CONST              23 ('comment')
+               146         856 LOAD_CONST              23 ('comment')
                
-               146         858 LOAD_FAST                6 (company)
+               147         858 LOAD_FAST                6 (company)
                            860 LOAD_ATTR               13 (domain)
                
-               147         870 LOAD_CONST              23 ('comment')
+               148         870 LOAD_CONST              23 ('comment')
                            872 LOAD_CONST              24 ('chatgpt - ')
                            874 LOAD_GLOBAL             37 (NULL + gpt)
                            886 LOAD_ATTR               19 (ask_gpt)
                            896 LOAD_FAST                5 (gpt_prompt)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 FORMAT_VALUE             0
                            914 BUILD_STRING             2
                            916 BUILD_MAP                1
                
-               142         918 KW_NAMES                25
+               143         918 KW_NAMES                25
                            920 PRECALL                  5
                            924 CALL                     5
                
-               141         934 PRECALL                  1
+               142         934 PRECALL                  1
                            938 CALL                     1
                            948 POP_TOP
                
-               151         950 LOAD_GLOBAL              5 (NULL + query)
+               152         950 LOAD_GLOBAL              5 (NULL + query)
                            962 LOAD_ATTR               16 (insert_event)
                
-               152         972 LOAD_GLOBAL             19 (NULL + models)
+               153         972 LOAD_GLOBAL             19 (NULL + models)
                            984 LOAD_ATTR               17 (Event)
                
-               153         994 LOAD_FAST                1 (search_uid)
+               154         994 LOAD_FAST                1 (search_uid)
                
-               154         996 LOAD_CONST              26 ('google')
+               155         996 LOAD_CONST              26 ('google')
                
-               155         998 LOAD_CONST              27 ('create')
+               156         998 LOAD_CONST              27 ('create')
                
-               156        1000 LOAD_FAST                6 (company)
+               157        1000 LOAD_FAST                6 (company)
                           1002 LOAD_ATTR               13 (domain)
                
-               152        1012 KW_NAMES                28
+               153        1012 KW_NAMES                28
                           1014 PRECALL                  4
                           1018 CALL                     4
                
-               151        1028 PRECALL                  1
+               152        1028 PRECALL                  1
                           1032 CALL                     1
                           1042 POP_TOP
                
-               160        1044 LOAD_FAST                6 (company)
+               161        1044 LOAD_FAST                6 (company)
                           1046 RETURN_VALUE
                consts
                   'takes in an (eriched) place and inserts it as a company'
                   ('search_uid',)
                   'domain'
                   'website'
                   'no website for '
@@ -1117,15 +1117,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                         00
-                     115           0 RESUME                   0
+                     116           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                                    8 STORE_FAST               1 (review)
                                   10 LOAD_FAST                1 (review)
                                   12 LOAD_CONST               0 ('text')
                                   14 BINARY_SUBSCR
@@ -1136,15 +1136,15 @@
                         'text'
                      names      ()
                      varnames   ('.0', 'review')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '<listcomp>'
-                     firstlineno 115
+                     firstlineno 116
                      lnotab 0x
                   'reviews'
                   'as well as what you already know about '
                   ','
                   'what products and services does '
                   'name'
                   ' offer?'
@@ -1164,15 +1164,15 @@
                varnames   ('place_id', 'search_uid', 'append_to_prompt', 'place', 'existing_search_domains', 'gpt_prompt', 'company')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'build_target_from_place_id'
                firstlineno 91
                lnotab
-                  0x02073402280102ff0a0224fe0204080124010402380136010402180202
+                  0x02073402280102ff0a0224fe0204080124010403380136010402180202
                   012401160116fc02ff10080401100316010e01320102fd12062803320112
                   011401200128033401160116010201020102010c0130fb10ff100a160116
                   010201020102010cfc10ff1009
             'place_ids'
             'search'
             code
                argcount  : 2
@@ -1183,49 +1183,49 @@
                   0x9700740100000000000000000000740200000000000000000000ac01a6
                   010000ab01000000000000000035007d027c0044005d297d037c02a00200
                   000000000000000000000000000000000000007406000000000000000000
                   006a0400000000000000007c037c016a050000000000000000ac02a60300
                   00ab03000000000000000001008c2a0900640064006400a6020000ab0200
                   000000000000000100640053002300310073047702780359007701010059
                   000100010064005300
-               162           0 RESUME                   0
+               163           0 RESUME                   0
                
-               163           2 LOAD_GLOBAL              1 (NULL + ThreadPoolExecutor)
+               164           2 LOAD_GLOBAL              1 (NULL + ThreadPoolExecutor)
                             14 LOAD_GLOBAL              2 (MAX_WORKERS)
                             26 KW_NAMES                 1
                             28 PRECALL                  1
                             32 CALL                     1
                             42 BEFORE_WITH
                             44 STORE_FAST               2 (executor)
                
-               164          46 LOAD_FAST                0 (place_ids)
+               165          46 LOAD_FAST                0 (place_ids)
                             48 GET_ITER
                        >>   50 FOR_ITER                41 (to 134)
                             52 STORE_FAST               3 (place_id)
                
-               165          54 LOAD_FAST                2 (executor)
+               166          54 LOAD_FAST                2 (executor)
                             56 LOAD_METHOD              2 (submit)
                
-               166          78 LOAD_GLOBAL              6 (GoogleMapsWrapper)
+               167          78 LOAD_GLOBAL              6 (GoogleMapsWrapper)
                             90 LOAD_ATTR                4 (build_target_from_place_id)
                
-               167         100 LOAD_FAST                3 (place_id)
+               168         100 LOAD_FAST                3 (place_id)
                
-               168         102 LOAD_FAST                1 (search)
+               169         102 LOAD_FAST                1 (search)
                            104 LOAD_ATTR                5 (uid)
                
-               165         114 KW_NAMES                 2
+               166         114 KW_NAMES                 2
                            116 PRECALL                  3
                            120 CALL                     3
                            130 POP_TOP
                            132 JUMP_BACKWARD           42 (to 50)
                
-               164     >>  134 NOP
+               165     >>  134 NOP
                
-               163         136 LOAD_CONST               0 (None)
+               164         136 LOAD_CONST               0 (None)
                            138 LOAD_CONST               0 (None)
                            140 LOAD_CONST               0 (None)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 POP_TOP
                            158 LOAD_CONST               0 (None)
                            160 RETURN_VALUE
@@ -1252,15 +1252,15 @@
                   ('place_id', 'search_uid')
                names      ('ThreadPoolExecutor', 'MAX_WORKERS', 'submit', 'GoogleMapsWrapper', 'build_target_from_place_id', 'uid')
                varnames   ('place_ids', 'search', 'executor', 'place_id')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'build_place_ids_async'
-               firstlineno 162
+               firstlineno 163
                lnotab 0x02012c0108011801160102010cfd14ff02ff
             ('San Diego, CA',)
             (25,)
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'str', 'tuple', 'get_loc', 'dict', 'enrich', 'List', 'int', 'list', 'fetch_unique_place_ids', '_fetch_place_ids', 'models', 'Company', 'build_target_from_place_id', 'Search', 'build_place_ids_async')
          varnames   ()
          freevars   ()
@@ -1268,95 +1268,95 @@
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GoogleMapsWrapper'
          firstlineno 17
          lnotab
             0x0a01020110ff0e01020402010eff0e010204020202ff040102ff02010e
             ff020102ff020202fe06ff0e010216020202ff040102ff020102ff020102
             ff020202fe06ff0e010227020202ff040102ff020102ff020102ff02020c
-            fe06ff0e010246
+            fe06ff0e010247
       'GoogleMapsWrapper'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006401a60100
             00ab010000000000000000640264039c025a0564046506640565076a0800
             00000000000000640665096606640784045a0a640565076a080000000000
             0000006406650b6604640884045a0c640465066406650b6604640984045a
             0d640a650e6a0f00000000000000006406640b6604640c84045a10640565
             076a0800000000000000006406650b6604640d84045a11640b5300
-         172           0 RESUME                   0
+         173           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GrataWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         174          10 PUSH_NULL
+         175          10 PUSH_NULL
                       12 LOAD_NAME                3 (secrets)
                       14 LOAD_ATTR                4 (access_secret_version)
                       24 LOAD_CONST               1 ('GRATA_API_TOKEN')
                       26 PRECALL                  1
                       30 CALL                     1
          
-         175          40 LOAD_CONST               2 ('application/json')
+         176          40 LOAD_CONST               2 ('application/json')
          
-         173          42 LOAD_CONST               3 (('Authorization', 'Content-Type'))
+         174          42 LOAD_CONST               3 (('Authorization', 'Content-Type'))
                       44 BUILD_CONST_KEY_MAP      2
                       46 STORE_NAME               5 (HEADERS)
          
-         178          48 LOAD_CONST               4 ('domain')
+         179          48 LOAD_CONST               4 ('domain')
                       50 LOAD_NAME                6 (str)
                       52 LOAD_CONST               5 ('search')
                       54 LOAD_NAME                7 (models)
                       56 LOAD_ATTR                8 (Search)
                       66 LOAD_CONST               6 ('return')
                       68 LOAD_NAME                9 (list)
                       70 BUILD_TUPLE              6
-                      72 LOAD_CONST               7 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 178>)
+                      72 LOAD_CONST               7 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 179>)
                       74 MAKE_FUNCTION            4 (annotations)
                       76 STORE_NAME              10 (find_similar)
          
-         200          78 LOAD_CONST               5 ('search')
+         201          78 LOAD_CONST               5 ('search')
                       80 LOAD_NAME                7 (models)
                       82 LOAD_ATTR                8 (Search)
                       92 LOAD_CONST               6 ('return')
                       94 LOAD_NAME               11 (dict)
                       96 BUILD_TUPLE              4
-                      98 LOAD_CONST               8 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 200>)
+                      98 LOAD_CONST               8 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 201>)
                      100 MAKE_FUNCTION            4 (annotations)
                      102 STORE_NAME              12 (find_by_criteria)
          
-         211         104 LOAD_CONST               4 ('domain')
+         212         104 LOAD_CONST               4 ('domain')
                      106 LOAD_NAME                6 (str)
                      108 LOAD_CONST               6 ('return')
                      110 LOAD_NAME               11 (dict)
                      112 BUILD_TUPLE              4
-                     114 LOAD_CONST               9 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 211>)
+                     114 LOAD_CONST               9 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 212>)
                      116 MAKE_FUNCTION            4 (annotations)
                      118 STORE_NAME              13 (enrich)
          
-         222         120 LOAD_CONST              10 ('targets')
+         223         120 LOAD_CONST              10 ('targets')
                      122 LOAD_NAME               14 (pd)
                      124 LOAD_ATTR               15 (DataFrame)
                      134 LOAD_CONST               6 ('return')
                      136 LOAD_CONST              11 (None)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              12 (<code object enrich_targets_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 222>)
+                     140 LOAD_CONST              12 (<code object enrich_targets_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 223>)
                      142 MAKE_FUNCTION            4 (annotations)
                      144 STORE_NAME              16 (enrich_targets_async)
          
-         237         146 LOAD_CONST               5 ('search')
+         238         146 LOAD_CONST               5 ('search')
                      148 LOAD_NAME                7 (models)
                      150 LOAD_ATTR                8 (Search)
                      160 LOAD_CONST               6 ('return')
                      162 LOAD_NAME               11 (dict)
                      164 BUILD_TUPLE              4
-                     166 LOAD_CONST              13 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 237>)
+                     166 LOAD_CONST              13 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 238>)
                      168 MAKE_FUNCTION            4 (annotations)
                      170 STORE_NAME              17 (_get_api_filter)
                      172 LOAD_CONST              11 (None)
                      174 RETURN_VALUE
          consts
             'GrataWrapper'
             'GRATA_API_TOKEN'
@@ -1378,81 +1378,81 @@
                   010000ab01000000000000000001007407000000000000000000006a0400
                   0000000000000064057400000000000000000000006a0500000000000000
                   007c03ac06a6030000ab0300000000000000007d047c04a0060000000000
                   000000000000000000000000000000a6000000ab0000000000000000007d
                   057c05a007000000000000000000000000000000000000000064076700a6
                   020000ab0200000000000000007c0564083c0000007c0564081900000000
                   00000000005300
-               178           0 RESUME                   0
+               179           0 RESUME                   0
                
-               179           2 LOAD_GLOBAL              0 (GrataWrapper)
+               180           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                1 (search)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (api_filters)
                
-               181          54 LOAD_FAST                0 (domain)
+               182          54 LOAD_FAST                0 (domain)
                
-               182          56 LOAD_FAST                2 (api_filters)
+               183          56 LOAD_FAST                2 (api_filters)
                
-               183          58 LOAD_CONST               1 ('grata_employees_estimates_range')
+               184          58 LOAD_CONST               1 ('grata_employees_estimates_range')
                
-               182          60 BINARY_SUBSCR
+               183          60 BINARY_SUBSCR
                
-               185          70 LOAD_FAST                2 (api_filters)
+               186          70 LOAD_FAST                2 (api_filters)
                             72 LOAD_CONST               2 ('headquarters')
                             74 BINARY_SUBSCR
                
-               186          84 LOAD_FAST                2 (api_filters)
+               187          84 LOAD_FAST                2 (api_filters)
                             86 LOAD_CONST               3 ('ownership')
                             88 BINARY_SUBSCR
                
-               180          98 LOAD_CONST               4 (('domain', 'grata_employees_estimates_range', 'headquarters', 'ownership'))
+               181          98 LOAD_CONST               4 (('domain', 'grata_employees_estimates_range', 'headquarters', 'ownership'))
                            100 BUILD_CONST_KEY_MAP      4
                            102 STORE_FAST               3 (similiar_filters)
                
-               188         104 LOAD_GLOBAL              5 (NULL + print)
+               189         104 LOAD_GLOBAL              5 (NULL + print)
                            116 LOAD_FAST                3 (similiar_filters)
                            118 PRECALL                  1
                            122 CALL                     1
                            132 POP_TOP
                
-               189         134 LOAD_GLOBAL              7 (NULL + requests)
+               190         134 LOAD_GLOBAL              7 (NULL + requests)
                            146 LOAD_ATTR                4 (post)
                
-               190         156 LOAD_CONST               5 ('https://search.grata.com/api/v1.2/search-similar/')
+               191         156 LOAD_CONST               5 ('https://search.grata.com/api/v1.2/search-similar/')
                
-               191         158 LOAD_GLOBAL              0 (GrataWrapper)
+               192         158 LOAD_GLOBAL              0 (GrataWrapper)
                            170 LOAD_ATTR                5 (HEADERS)
                
-               192         180 LOAD_FAST                3 (similiar_filters)
+               193         180 LOAD_FAST                3 (similiar_filters)
                
-               189         182 KW_NAMES                 6
+               190         182 KW_NAMES                 6
                            184 PRECALL                  3
                            188 CALL                     3
                            198 STORE_FAST               4 (response)
                
-               194         200 LOAD_FAST                4 (response)
+               195         200 LOAD_FAST                4 (response)
                            202 LOAD_METHOD              6 (json)
                            224 PRECALL                  0
                            228 CALL                     0
                            238 STORE_FAST               5 (data)
                
-               196         240 LOAD_FAST                5 (data)
+               197         240 LOAD_FAST                5 (data)
                            242 LOAD_METHOD              7 (get)
                            264 LOAD_CONST               7 ('results')
                            266 BUILD_LIST               0
                            268 PRECALL                  2
                            272 CALL                     2
                            282 LOAD_FAST                5 (data)
                            284 LOAD_CONST               8 ('companies')
                            286 STORE_SUBSCR
                
-               198         290 LOAD_FAST                5 (data)
+               199         290 LOAD_FAST                5 (data)
                            292 LOAD_CONST               8 ('companies')
                            294 BINARY_SUBSCR
                            304 RETURN_VALUE
                consts
                   None
                   'grata_employees_estimates_range'
                   'headquarters'
@@ -1464,15 +1464,15 @@
                   'companies'
                names      ('GrataWrapper', '_get_api_filter', 'print', 'requests', 'post', 'HEADERS', 'json', 'get')
                varnames   ('domain', 'search', 'api_filters', 'similiar_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 178
+               firstlineno 179
                lnotab
                   0x020134020201020102ff0a030e010efa06081e0116010201160102fd12
                   0528023202
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
@@ -1481,52 +1481,52 @@
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000007c00a6010000ab0100000000000000007d017405000000
                   000000000000006a03000000000000000064017400000000000000000000
                   006a0400000000000000007c01ac02a6030000ab0300000000000000007d
                   027c02a0050000000000000000000000000000000000000000a6000000ab
                   0000000000000000007d03740d0000000000000000000064037c03a60200
                   00ab02000000000000000001007c036404190000000000000000005300
-               200           0 RESUME                   0
+               201           0 RESUME                   0
                
-               201           2 LOAD_GLOBAL              0 (GrataWrapper)
+               202           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                0 (search)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               1 (api_filters)
                
-               202          54 LOAD_GLOBAL              5 (NULL + requests)
+               203          54 LOAD_GLOBAL              5 (NULL + requests)
                             66 LOAD_ATTR                3 (post)
                
-               203          76 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/search/')
+               204          76 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/search/')
                
-               204          78 LOAD_GLOBAL              0 (GrataWrapper)
+               205          78 LOAD_GLOBAL              0 (GrataWrapper)
                             90 LOAD_ATTR                4 (HEADERS)
                
-               205         100 LOAD_FAST                1 (api_filters)
+               206         100 LOAD_FAST                1 (api_filters)
                
-               202         102 KW_NAMES                 2
+               203         102 KW_NAMES                 2
                            104 PRECALL                  3
                            108 CALL                     3
                            118 STORE_FAST               2 (response)
                
-               207         120 LOAD_FAST                2 (response)
+               208         120 LOAD_FAST                2 (response)
                            122 LOAD_METHOD              5 (json)
                            144 PRECALL                  0
                            148 CALL                     0
                            158 STORE_FAST               3 (data)
                
-               208         160 LOAD_GLOBAL             13 (NULL + print)
+               209         160 LOAD_GLOBAL             13 (NULL + print)
                            172 LOAD_CONST               3 ('find_by_criteria: ')
                            174 LOAD_FAST                3 (data)
                            176 PRECALL                  2
                            180 CALL                     2
                            190 POP_TOP
                
-               209         192 LOAD_FAST                3 (data)
+               210         192 LOAD_FAST                3 (data)
                            194 LOAD_CONST               4 ('companies')
                            196 BINARY_SUBSCR
                            206 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1.2/search/'
                   ('headers', 'json')
@@ -1534,15 +1534,15 @@
                   'companies'
                names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'json', 'print')
                varnames   ('search', 'api_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 200
+               firstlineno 201
                lnotab 0x0201340116010201160102fd120528012001
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
@@ -1550,58 +1550,58 @@
                   0000000000000000006a03000000000000000064027c006901ac03a60300
                   00ab0300000000000000007d017c01a00400000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d027c02a005000000
                   00000000000000000000000000000000006404a6010000ab010000000000
                   0000007c0264053c0000007c02a005000000000000000000000000000000
                   00000000006406a6010000ab0100000000000000007c0264073c0000007c
                   025300
-               211           0 RESUME                   0
+               212           0 RESUME                   0
                
-               212           2 LOAD_GLOBAL              1 (NULL + requests)
+               213           2 LOAD_GLOBAL              1 (NULL + requests)
                             14 LOAD_ATTR                1 (post)
                
-               213          24 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/enrich/')
+               214          24 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/enrich/')
                
-               214          26 LOAD_GLOBAL              4 (GrataWrapper)
+               215          26 LOAD_GLOBAL              4 (GrataWrapper)
                             38 LOAD_ATTR                3 (HEADERS)
                
-               215          48 LOAD_CONST               2 ('domain')
+               216          48 LOAD_CONST               2 ('domain')
                             50 LOAD_FAST                0 (domain)
                             52 BUILD_MAP                1
                
-               212          54 KW_NAMES                 3
+               213          54 KW_NAMES                 3
                             56 PRECALL                  3
                             60 CALL                     3
                             70 STORE_FAST               1 (response)
                
-               217          72 LOAD_FAST                1 (response)
+               218          72 LOAD_FAST                1 (response)
                             74 LOAD_METHOD              4 (json)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 STORE_FAST               2 (data)
                
-               218         112 LOAD_FAST                2 (data)
+               219         112 LOAD_FAST                2 (data)
                            114 LOAD_METHOD              5 (get)
                            136 LOAD_CONST               4 ('social_linkedin')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 LOAD_FAST                2 (data)
                            154 LOAD_CONST               5 ('linkedin')
                            156 STORE_SUBSCR
                
-               219         160 LOAD_FAST                2 (data)
+               220         160 LOAD_FAST                2 (data)
                            162 LOAD_METHOD              5 (get)
                            184 LOAD_CONST               6 ('ownership_status')
                            186 PRECALL                  1
                            190 CALL                     1
                            200 LOAD_FAST                2 (data)
                            202 LOAD_CONST               7 ('ownership')
                            204 STORE_SUBSCR
                
-               220         208 LOAD_FAST                2 (data)
+               221         208 LOAD_FAST                2 (data)
                            210 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1.2/enrich/'
                   'domain'
                   ('headers', 'json')
                   'social_linkedin'
@@ -1610,40 +1610,40 @@
                   'ownership'
                names      ('requests', 'post', 'GrataWrapper', 'HEADERS', 'json', 'get')
                varnames   ('domain', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 211
+               firstlineno 212
                lnotab 0x020116010201160106fd1205280130013001
             'targets'
             None
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x8700870197006401740000000000000000000000640264006604880188
                   0066026403840c8a0164005300
                              0 MAKE_CELL                0 (targets)
                              2 MAKE_CELL                1 (enrich_company_by_domain)
                
-               222           4 RESUME                   0
+               223           4 RESUME                   0
                
-               223           6 LOAD_CONST               1 ('domain')
+               224           6 LOAD_CONST               1 ('domain')
                              8 LOAD_GLOBAL              0 (str)
                             20 LOAD_CONST               2 ('return')
                             22 LOAD_CONST               0 (None)
                             24 BUILD_TUPLE              4
                             26 LOAD_CLOSURE             1 (enrich_company_by_domain)
                             28 LOAD_CLOSURE             0 (targets)
                             30 BUILD_TUPLE              2
-                            32 LOAD_CONST               3 (<code object enrich_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 223>)
+                            32 LOAD_CONST               3 (<code object enrich_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 224>)
                             34 MAKE_FUNCTION           12 (annotations, closure)
                             36 STORE_DEREF              1 (enrich_company_by_domain)
                             38 LOAD_CONST               0 (None)
                             40 RETURN_VALUE
                consts
                   None
                   'domain'
@@ -1668,87 +1668,87 @@
                         00000089048905640519000000000000000000a00b000000000000000000
                         0000000000000000000000a6000000ab000000000000000000a6020000ab
                         0200000000000000000100640064006400a6020000ab0200000000000000
                         000100640053002300310073047702780359007701010059000100010064
                         005300
                                    0 COPY_FREE_VARS           2
                      
-                     223           2 RESUME                   0
+                     224           2 RESUME                   0
                      
-                     224           4 LOAD_GLOBAL              1 (NULL + query)
+                     225           4 LOAD_GLOBAL              1 (NULL + query)
                                   16 LOAD_ATTR                1 (find_company_by_domain)
                                   26 LOAD_FAST                0 (domain)
                                   28 PRECALL                  1
                                   32 CALL                     1
                                   42 STORE_FAST               1 (company)
                      
-                     225          44 LOAD_CONST               1 ('company_uid')
+                     226          44 LOAD_CONST               1 ('company_uid')
                                   46 LOAD_FAST                1 (company)
                                   48 LOAD_ATTR                2 (meta)
                                   58 LOAD_METHOD              3 (keys)
                                   80 PRECALL                  0
                                   84 CALL                     0
                                   94 CONTAINS_OP              1
                                   96 POP_JUMP_FORWARD_IF_FALSE    88 (to 274)
                      
-                     227          98 LOAD_GLOBAL              8 (GrataWrapper)
+                     228          98 LOAD_GLOBAL              8 (GrataWrapper)
                                  110 LOAD_METHOD              5 (enrich)
                                  132 LOAD_FAST                0 (domain)
                                  134 PRECALL                  1
                                  138 CALL                     1
                                  148 STORE_FAST               2 (resp)
                      
-                     228         150 LOAD_FAST                2 (resp)
+                     229         150 LOAD_FAST                2 (resp)
                                  152 LOAD_METHOD              6 (get)
                                  174 LOAD_CONST               2 ('description')
                                  176 PRECALL                  1
                                  180 CALL                     1
                                  190 LOAD_FAST                1 (company)
                                  192 STORE_ATTR               7 (description)
                      
-                     229         202 BUILD_MAP                0
+                     230         202 BUILD_MAP                0
                                  204 LOAD_FAST                1 (company)
                                  206 LOAD_ATTR                2 (meta)
                                  216 DICT_UPDATE              1
                                  218 LOAD_FAST                2 (resp)
                                  220 DICT_UPDATE              1
                                  222 LOAD_FAST                1 (company)
                                  224 STORE_ATTR               2 (meta)
                      
-                     230         234 LOAD_GLOBAL              1 (NULL + query)
+                     231         234 LOAD_GLOBAL              1 (NULL + query)
                                  246 LOAD_ATTR                8 (update_company)
                                  256 LOAD_FAST                1 (company)
                                  258 PRECALL                  1
                                  262 CALL                     1
                                  272 POP_TOP
                      
-                     232     >>  274 LOAD_GLOBAL             19 (NULL + ThreadPoolExecutor)
+                     233     >>  274 LOAD_GLOBAL             19 (NULL + ThreadPoolExecutor)
                                  286 LOAD_CONST               3 (5)
                                  288 KW_NAMES                 4
                                  290 PRECALL                  1
                                  294 CALL                     1
                                  304 BEFORE_WITH
                                  306 STORE_FAST               3 (executor)
                      
-                     233         308 LOAD_FAST                3 (executor)
+                     234         308 LOAD_FAST                3 (executor)
                                  310 LOAD_METHOD             10 (map)
                      
-                     234         332 LOAD_DEREF               4 (enrich_company_by_domain)
+                     235         332 LOAD_DEREF               4 (enrich_company_by_domain)
                                  334 LOAD_DEREF               5 (targets)
                                  336 LOAD_CONST               5 ('domain')
                                  338 BINARY_SUBSCR
                                  348 LOAD_METHOD             11 (tolist)
                                  370 PRECALL                  0
                                  374 CALL                     0
                      
-                     233         384 PRECALL                  2
+                     234         384 PRECALL                  2
                                  388 CALL                     2
                                  398 POP_TOP
                      
-                     232         400 LOAD_CONST               0 (None)
+                     233         400 LOAD_CONST               0 (None)
                                  402 LOAD_CONST               0 (None)
                                  404 LOAD_CONST               0 (None)
                                  406 PRECALL                  2
                                  410 CALL                     2
                                  420 POP_TOP
                                  422 LOAD_CONST               0 (None)
                                  424 RETURN_VALUE
@@ -1778,23 +1778,23 @@
                         'domain'
                      names      ('query', 'find_company_by_domain', 'meta', 'keys', 'GrataWrapper', 'enrich', 'get', 'description', 'update_company', 'ThreadPoolExecutor', 'map', 'tolist')
                      varnames   ('domain', 'company', 'resp', 'executor')
                      freevars   ('enrich_company_by_domain', 'targets')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       'enrich_company_by_domain'
-                     firstlineno 223
+                     firstlineno 224
                      lnotab 0x04012801360234013401200128022201180134ff10ff
                names      ('str',)
                varnames   ('targets',)
                freevars   ()
                cellvars   ('targets', 'enrich_company_by_domain')
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich_targets_async'
-               firstlineno 222
+               firstlineno 223
                lnotab 0x0601
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 8
                flags     : 3
                code
@@ -1820,356 +1820,356 @@
                   00000000000000000000000000000064706471a6020000ab020000000000
                   00000002007c01a6000000ab00000000000000000002007c02a6000000ab
                   00000000000000000064729c0264739c065300
                              0 MAKE_CELL                0 (search)
                              2 MAKE_CELL                3 (COUNTRIES)
                              4 MAKE_CELL                4 (STATES)
                
-               237           6 RESUME                   0
+               238           6 RESUME                   0
                
-               238           8 BUILD_MAP                0
+               239           8 BUILD_MAP                0
                
-               239          10 LOAD_CONST               1 ('AL')
+               240          10 LOAD_CONST               1 ('AL')
                             12 LOAD_CONST               2 ('Alabama')
                
-               238          14 MAP_ADD                  1
+               239          14 MAP_ADD                  1
                
-               240          16 LOAD_CONST               3 ('AK')
+               241          16 LOAD_CONST               3 ('AK')
                             18 LOAD_CONST               4 ('Alaska')
                
-               238          20 MAP_ADD                  1
+               239          20 MAP_ADD                  1
                
-               241          22 LOAD_CONST               5 ('AZ')
+               242          22 LOAD_CONST               5 ('AZ')
                             24 LOAD_CONST               6 ('Arizona')
                
-               238          26 MAP_ADD                  1
+               239          26 MAP_ADD                  1
                
-               242          28 LOAD_CONST               7 ('AR')
+               243          28 LOAD_CONST               7 ('AR')
                             30 LOAD_CONST               8 ('Arkansas')
                
-               238          32 MAP_ADD                  1
+               239          32 MAP_ADD                  1
                
-               243          34 LOAD_CONST               9 ('CA')
+               244          34 LOAD_CONST               9 ('CA')
                             36 LOAD_CONST              10 ('California')
                
-               238          38 MAP_ADD                  1
+               239          38 MAP_ADD                  1
                
-               244          40 LOAD_CONST              11 ('CO')
+               245          40 LOAD_CONST              11 ('CO')
                             42 LOAD_CONST              12 ('Colorado')
                
-               238          44 MAP_ADD                  1
+               239          44 MAP_ADD                  1
                
-               245          46 LOAD_CONST              13 ('CT')
+               246          46 LOAD_CONST              13 ('CT')
                             48 LOAD_CONST              14 ('Connecticut')
                
-               238          50 MAP_ADD                  1
+               239          50 MAP_ADD                  1
                
-               246          52 LOAD_CONST              15 ('DE')
+               247          52 LOAD_CONST              15 ('DE')
                             54 LOAD_CONST              16 ('Delaware')
                
-               238          56 MAP_ADD                  1
+               239          56 MAP_ADD                  1
                
-               247          58 LOAD_CONST              17 ('FL')
+               248          58 LOAD_CONST              17 ('FL')
                             60 LOAD_CONST              18 ('Florida')
                
-               238          62 MAP_ADD                  1
+               239          62 MAP_ADD                  1
                
-               248          64 LOAD_CONST              19 ('GA')
+               249          64 LOAD_CONST              19 ('GA')
                             66 LOAD_CONST              20 ('Georgia')
                
-               238          68 MAP_ADD                  1
+               239          68 MAP_ADD                  1
                
-               249          70 LOAD_CONST              21 ('HI')
+               250          70 LOAD_CONST              21 ('HI')
                             72 LOAD_CONST              22 ('Hawaii')
                
-               238          74 MAP_ADD                  1
+               239          74 MAP_ADD                  1
                
-               250          76 LOAD_CONST              23 ('ID')
+               251          76 LOAD_CONST              23 ('ID')
                             78 LOAD_CONST              24 ('Idaho')
                
-               238          80 MAP_ADD                  1
+               239          80 MAP_ADD                  1
                
-               251          82 LOAD_CONST              25 ('IL')
+               252          82 LOAD_CONST              25 ('IL')
                             84 LOAD_CONST              26 ('Illinois')
                
-               238          86 MAP_ADD                  1
+               239          86 MAP_ADD                  1
                
-               252          88 LOAD_CONST              27 ('IN')
+               253          88 LOAD_CONST              27 ('IN')
                             90 LOAD_CONST              28 ('Indiana')
                
-               238          92 MAP_ADD                  1
+               239          92 MAP_ADD                  1
                
-               253          94 LOAD_CONST              29 ('IA')
+               254          94 LOAD_CONST              29 ('IA')
                             96 LOAD_CONST              30 ('Iowa')
                
-               238          98 MAP_ADD                  1
+               239          98 MAP_ADD                  1
                
-               254         100 LOAD_CONST              31 ('KS')
+               255         100 LOAD_CONST              31 ('KS')
                            102 LOAD_CONST              32 ('Kansas')
                
-               238         104 MAP_ADD                  1
+               239         104 MAP_ADD                  1
                
-               255         106 LOAD_CONST              33 ('KY')
+               256         106 LOAD_CONST              33 ('KY')
                            108 LOAD_CONST              34 ('Kentucky')
                
-               238         110 MAP_ADD                  1
+               239         110 MAP_ADD                  1
                            112 BUILD_MAP                0
                
-               256         114 LOAD_CONST              35 ('LA')
+               257         114 LOAD_CONST              35 ('LA')
                            116 LOAD_CONST              36 ('Louisiana')
                
-               238         118 MAP_ADD                  1
+               239         118 MAP_ADD                  1
                
-               257         120 LOAD_CONST              37 ('ME')
+               258         120 LOAD_CONST              37 ('ME')
                            122 LOAD_CONST              38 ('Maine')
                
-               238         124 MAP_ADD                  1
+               239         124 MAP_ADD                  1
                
-               258         126 LOAD_CONST              39 ('MD')
+               259         126 LOAD_CONST              39 ('MD')
                            128 LOAD_CONST              40 ('Maryland')
                
-               238         130 MAP_ADD                  1
+               239         130 MAP_ADD                  1
                
-               259         132 LOAD_CONST              41 ('MA')
+               260         132 LOAD_CONST              41 ('MA')
                            134 LOAD_CONST              42 ('Massachusetts')
                
-               238         136 MAP_ADD                  1
+               239         136 MAP_ADD                  1
                
-               260         138 LOAD_CONST              43 ('MI')
+               261         138 LOAD_CONST              43 ('MI')
                            140 LOAD_CONST              44 ('Michigan')
                
-               238         142 MAP_ADD                  1
+               239         142 MAP_ADD                  1
                
-               261         144 LOAD_CONST              45 ('MN')
+               262         144 LOAD_CONST              45 ('MN')
                            146 LOAD_CONST              46 ('Minnesota')
                
-               238         148 MAP_ADD                  1
+               239         148 MAP_ADD                  1
                
-               262         150 LOAD_CONST              47 ('MS')
+               263         150 LOAD_CONST              47 ('MS')
                            152 LOAD_CONST              48 ('Mississippi')
                
-               238         154 MAP_ADD                  1
+               239         154 MAP_ADD                  1
                
-               263         156 LOAD_CONST              49 ('MO')
+               264         156 LOAD_CONST              49 ('MO')
                            158 LOAD_CONST              50 ('Missouri')
                
-               238         160 MAP_ADD                  1
+               239         160 MAP_ADD                  1
                
-               264         162 LOAD_CONST              51 ('MT')
+               265         162 LOAD_CONST              51 ('MT')
                            164 LOAD_CONST              52 ('Montana')
                
-               238         166 MAP_ADD                  1
+               239         166 MAP_ADD                  1
                
-               265         168 LOAD_CONST              53 ('NE')
+               266         168 LOAD_CONST              53 ('NE')
                            170 LOAD_CONST              54 ('Nebraska')
                
-               238         172 MAP_ADD                  1
+               239         172 MAP_ADD                  1
                
-               266         174 LOAD_CONST              55 ('NV')
+               267         174 LOAD_CONST              55 ('NV')
                            176 LOAD_CONST              56 ('Nevada')
                
-               238         178 MAP_ADD                  1
+               239         178 MAP_ADD                  1
                
-               267         180 LOAD_CONST              57 ('NH')
+               268         180 LOAD_CONST              57 ('NH')
                            182 LOAD_CONST              58 ('New Hampshire')
                
-               238         184 MAP_ADD                  1
+               239         184 MAP_ADD                  1
                
-               268         186 LOAD_CONST              59 ('NJ')
+               269         186 LOAD_CONST              59 ('NJ')
                            188 LOAD_CONST              60 ('New Jersey')
                
-               238         190 MAP_ADD                  1
+               239         190 MAP_ADD                  1
                
-               269         192 LOAD_CONST              61 ('NM')
+               270         192 LOAD_CONST              61 ('NM')
                            194 LOAD_CONST              62 ('New Mexico')
                
-               238         196 MAP_ADD                  1
+               239         196 MAP_ADD                  1
                
-               270         198 LOAD_CONST              63 ('NY')
+               271         198 LOAD_CONST              63 ('NY')
                            200 LOAD_CONST              64 ('New York')
                
-               238         202 MAP_ADD                  1
+               239         202 MAP_ADD                  1
                
-               271         204 LOAD_CONST              65 ('NC')
+               272         204 LOAD_CONST              65 ('NC')
                            206 LOAD_CONST              66 ('North Carolina')
                
-               238         208 MAP_ADD                  1
+               239         208 MAP_ADD                  1
                
-               272         210 LOAD_CONST              67 ('ND')
+               273         210 LOAD_CONST              67 ('ND')
                            212 LOAD_CONST              68 ('North Dakota')
                
-               238         214 MAP_ADD                  1
+               239         214 MAP_ADD                  1
                            216 DICT_UPDATE              1
                            218 BUILD_MAP                0
                
-               273         220 LOAD_CONST              69 ('OH')
+               274         220 LOAD_CONST              69 ('OH')
                            222 LOAD_CONST              70 ('Ohio')
                
-               238         224 MAP_ADD                  1
+               239         224 MAP_ADD                  1
                
-               274         226 LOAD_CONST              71 ('OK')
+               275         226 LOAD_CONST              71 ('OK')
                            228 LOAD_CONST              72 ('Oklahoma')
                
-               238         230 MAP_ADD                  1
+               239         230 MAP_ADD                  1
                
-               275         232 LOAD_CONST              73 ('OR')
+               276         232 LOAD_CONST              73 ('OR')
                            234 LOAD_CONST              74 ('Oregon')
                
-               238         236 MAP_ADD                  1
+               239         236 MAP_ADD                  1
                
-               276         238 LOAD_CONST              75 ('PA')
+               277         238 LOAD_CONST              75 ('PA')
                            240 LOAD_CONST              76 ('Pennsylvania')
                
-               238         242 MAP_ADD                  1
+               239         242 MAP_ADD                  1
                
-               277         244 LOAD_CONST              77 ('RI')
+               278         244 LOAD_CONST              77 ('RI')
                            246 LOAD_CONST              78 ('Rhode Island')
                
-               238         248 MAP_ADD                  1
+               239         248 MAP_ADD                  1
                
-               278         250 LOAD_CONST              79 ('SC')
+               279         250 LOAD_CONST              79 ('SC')
                            252 LOAD_CONST              80 ('South Carolina')
                
-               238         254 MAP_ADD                  1
+               239         254 MAP_ADD                  1
                
-               279         256 LOAD_CONST              81 ('SD')
+               280         256 LOAD_CONST              81 ('SD')
                            258 LOAD_CONST              82 ('South Dakota')
                
-               238         260 MAP_ADD                  1
+               239         260 MAP_ADD                  1
                
-               280         262 LOAD_CONST              83 ('TN')
+               281         262 LOAD_CONST              83 ('TN')
                            264 LOAD_CONST              84 ('Tennessee')
                
-               238         266 MAP_ADD                  1
+               239         266 MAP_ADD                  1
                
-               281         268 LOAD_CONST              85 ('TX')
+               282         268 LOAD_CONST              85 ('TX')
                            270 LOAD_CONST              86 ('Texas')
                
-               238         272 MAP_ADD                  1
+               239         272 MAP_ADD                  1
                
-               282         274 LOAD_CONST              87 ('UT')
+               283         274 LOAD_CONST              87 ('UT')
                            276 LOAD_CONST              88 ('Utah')
                
-               238         278 MAP_ADD                  1
+               239         278 MAP_ADD                  1
                
-               283         280 LOAD_CONST              89 ('VT')
+               284         280 LOAD_CONST              89 ('VT')
                            282 LOAD_CONST              90 ('Vermont')
                
-               238         284 MAP_ADD                  1
+               239         284 MAP_ADD                  1
                
-               284         286 LOAD_CONST              91 ('VA')
+               285         286 LOAD_CONST              91 ('VA')
                            288 LOAD_CONST              92 ('Virginia')
                
-               238         290 MAP_ADD                  1
+               239         290 MAP_ADD                  1
                
-               285         292 LOAD_CONST              93 ('WA')
+               286         292 LOAD_CONST              93 ('WA')
                            294 LOAD_CONST              94 ('Washington')
                
-               238         296 MAP_ADD                  1
+               239         296 MAP_ADD                  1
                
-               286         298 LOAD_CONST              95 ('WV')
+               287         298 LOAD_CONST              95 ('WV')
                            300 LOAD_CONST              96 ('West Virginia')
                
-               238         302 MAP_ADD                  1
+               239         302 MAP_ADD                  1
                
-               287         304 LOAD_CONST              97 ('WI')
+               288         304 LOAD_CONST              97 ('WI')
                            306 LOAD_CONST              98 ('Wisconsin')
                
-               238         308 MAP_ADD                  1
+               239         308 MAP_ADD                  1
                
-               288         310 LOAD_CONST              99 ('WY')
+               289         310 LOAD_CONST              99 ('WY')
                            312 LOAD_CONST             100 ('Wyoming')
                
-               238         314 MAP_ADD                  1
+               239         314 MAP_ADD                  1
                            316 DICT_UPDATE              1
                            318 STORE_DEREF              4 (STATES)
                
-               292         320 LOAD_CONST             101 ('United States')
+               293         320 LOAD_CONST             101 ('United States')
                
-               293         322 LOAD_CONST             102 ('Canada')
+               294         322 LOAD_CONST             102 ('Canada')
                
-               294         324 LOAD_CONST             103 ('Mexico')
+               295         324 LOAD_CONST             103 ('Mexico')
                
-               295         326 LOAD_CONST             104 ('United Kingdom')
+               296         326 LOAD_CONST             104 ('United Kingdom')
                
-               291         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
+               292         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
                            330 BUILD_CONST_KEY_MAP      4
                            332 STORE_DEREF              3 (COUNTRIES)
                
-               298         334 LOAD_CONST             106 ('return')
+               299         334 LOAD_CONST             106 ('return')
                            336 LOAD_GLOBAL              0 (list)
                            348 BUILD_TUPLE              2
                            350 LOAD_CLOSURE             3 (COUNTRIES)
                            352 LOAD_CLOSURE             4 (STATES)
                            354 LOAD_CLOSURE             0 (search)
                            356 BUILD_TUPLE              3
-                           358 LOAD_CONST             107 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 298>)
+                           358 LOAD_CONST             107 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 299>)
                            360 MAKE_FUNCTION           12 (annotations, closure)
                            362 STORE_FAST               1 (_hq_include)
                
-               323         364 LOAD_CONST             106 ('return')
+               324         364 LOAD_CONST             106 ('return')
                            366 LOAD_GLOBAL              0 (list)
                            378 BUILD_TUPLE              2
                            380 LOAD_CLOSURE             4 (STATES)
                            382 LOAD_CLOSURE             0 (search)
                            384 BUILD_TUPLE              2
-                           386 LOAD_CONST             108 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 323>)
+                           386 LOAD_CONST             108 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 324>)
                            388 MAKE_FUNCTION           12 (annotations, closure)
                            390 STORE_FAST               2 (_hq_exclude)
                
-               330         392 LOAD_CONST             109 ('any')
+               331         392 LOAD_CONST             109 ('any')
                
-               331         394 LOAD_DEREF               0 (search)
+               332         394 LOAD_DEREF               0 (search)
                            396 LOAD_ATTR                1 (inclusion)
                            406 LOAD_METHOD              2 (get)
                            428 LOAD_CONST             110 ('keywords')
                            430 BUILD_LIST               0
                            432 PRECALL                  2
                            436 CALL                     2
                
-               332         446 LOAD_DEREF               0 (search)
+               333         446 LOAD_DEREF               0 (search)
                            448 LOAD_ATTR                3 (exclusion)
                            458 LOAD_METHOD              2 (get)
                            480 LOAD_CONST             110 ('keywords')
                            482 BUILD_LIST               0
                            484 PRECALL                  2
                            488 CALL                     2
                
-               333         498 LOAD_DEREF               0 (search)
+               334         498 LOAD_DEREF               0 (search)
                            500 LOAD_ATTR                1 (inclusion)
                            510 LOAD_METHOD              2 (get)
                
-               334         532 LOAD_CONST             111 ('employees_range')
+               335         532 LOAD_CONST             111 ('employees_range')
                            534 BUILD_LIST               0
                
-               333         536 PRECALL                  2
+               334         536 PRECALL                  2
                            540 CALL                     2
                
-               336         550 LOAD_DEREF               0 (search)
+               337         550 LOAD_DEREF               0 (search)
                            552 LOAD_ATTR                1 (inclusion)
                            562 LOAD_METHOD              2 (get)
                            584 LOAD_CONST             112 ('ownership')
                            586 LOAD_CONST             113 ('')
                            588 PRECALL                  2
                            592 CALL                     2
                
-               338         602 PUSH_NULL
+               339         602 PUSH_NULL
                            604 LOAD_FAST                1 (_hq_include)
                            606 PRECALL                  0
                            610 CALL                     0
                
-               339         620 PUSH_NULL
+               340         620 PUSH_NULL
                            622 LOAD_FAST                2 (_hq_exclude)
                            624 PRECALL                  0
                            628 CALL                     0
                
-               337         638 LOAD_CONST             114 (('include', 'exclude'))
+               338         638 LOAD_CONST             114 (('include', 'exclude'))
                            640 BUILD_CONST_KEY_MAP      2
                
-               329         642 LOAD_CONST             115 (('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters'))
+               330         642 LOAD_CONST             115 (('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters'))
                            644 BUILD_CONST_KEY_MAP      6
                            646 RETURN_VALUE
                consts
                   None
                   'AL'
                   'Alabama'
                   'AK'
@@ -2298,134 +2298,134 @@
                         010000ab01000000000000000001008c207405000000000000000000007c
                         03a6010000ab01000000000000000064046b040000000072227c0344005d
                         1f7d067c00a0030000000000000000000000000000000000000000640389
                         077c06190000000000000000006901a6010000ab01000000000000000001
                         008c207c005300
                                    0 COPY_FREE_VARS           3
                      
-                     298           2 RESUME                   0
+                     299           2 RESUME                   0
                      
-                     299           4 BUILD_LIST               0
+                     300           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (include)
                      
-                     300           8 LOAD_DEREF               9 (search)
+                     301           8 LOAD_DEREF               9 (search)
                                   10 LOAD_ATTR                0 (inclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('city')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 STORE_FAST               1 (cities)
                      
-                     301          62 LOAD_DEREF               9 (search)
+                     302          62 LOAD_DEREF               9 (search)
                                   64 LOAD_ATTR                0 (inclusion)
                                   74 LOAD_METHOD              1 (get)
                                   96 LOAD_CONST               2 ('state')
                                   98 BUILD_LIST               0
                                  100 PRECALL                  2
                                  104 CALL                     2
                                  114 STORE_FAST               2 (states)
                      
-                     302         116 LOAD_DEREF               9 (search)
+                     303         116 LOAD_DEREF               9 (search)
                                  118 LOAD_ATTR                0 (inclusion)
                                  128 LOAD_METHOD              1 (get)
                                  150 LOAD_CONST               3 ('country')
                                  152 BUILD_LIST               0
                                  154 PRECALL                  2
                                  158 CALL                     2
                                  168 STORE_FAST               3 (countries)
                      
-                     304         170 LOAD_GLOBAL              5 (NULL + len)
+                     305         170 LOAD_GLOBAL              5 (NULL + len)
                                  182 LOAD_FAST                1 (cities)
                                  184 PRECALL                  1
                                  188 CALL                     1
                                  198 LOAD_CONST               4 (0)
                                  200 COMPARE_OP               4 (>)
                                  206 POP_JUMP_FORWARD_IF_FALSE    46 (to 300)
                      
-                     306         208 LOAD_DEREF               8 (STATES)
+                     307         208 LOAD_DEREF               8 (STATES)
                                  210 LOAD_FAST                2 (states)
                                  212 LOAD_CONST               4 (0)
                                  214 BINARY_SUBSCR
                                  224 BINARY_SUBSCR
                                  234 STORE_FAST               4 (state)
                      
-                     307         236 LOAD_FAST                1 (cities)
+                     308         236 LOAD_FAST                1 (cities)
                                  238 GET_ITER
                              >>  240 FOR_ITER                27 (to 296)
                                  242 STORE_FAST               5 (city)
                      
-                     308         244 LOAD_FAST                0 (include)
+                     309         244 LOAD_FAST                0 (include)
                                  246 LOAD_METHOD              3 (append)
                      
-                     309         268 LOAD_FAST                5 (city)
+                     310         268 LOAD_FAST                5 (city)
                                  270 LOAD_FAST                4 (state)
                                  272 LOAD_CONST               5 ('United States')
                                  274 LOAD_CONST               6 (('city', 'state', 'country'))
                                  276 BUILD_CONST_KEY_MAP      3
                      
-                     308         278 PRECALL                  1
+                     309         278 PRECALL                  1
                                  282 CALL                     1
                                  292 POP_TOP
                                  294 JUMP_BACKWARD           28 (to 240)
                      
-                     311     >>  296 LOAD_FAST                0 (include)
+                     312     >>  296 LOAD_FAST                0 (include)
                                  298 RETURN_VALUE
                      
-                     313     >>  300 LOAD_GLOBAL              5 (NULL + len)
+                     314     >>  300 LOAD_GLOBAL              5 (NULL + len)
                                  312 LOAD_FAST                2 (states)
                                  314 PRECALL                  1
                                  318 CALL                     1
                                  328 LOAD_CONST               4 (0)
                                  330 COMPARE_OP               4 (>)
                                  336 POP_JUMP_FORWARD_IF_FALSE    34 (to 406)
                      
-                     314         338 LOAD_FAST                2 (states)
+                     315         338 LOAD_FAST                2 (states)
                                  340 GET_ITER
                              >>  342 FOR_ITER                31 (to 406)
                                  344 STORE_FAST               4 (state)
                      
-                     316         346 LOAD_FAST                0 (include)
+                     317         346 LOAD_FAST                0 (include)
                                  348 LOAD_METHOD              3 (append)
                                  370 LOAD_CONST               2 ('state')
                                  372 LOAD_DEREF               8 (STATES)
                                  374 LOAD_FAST                4 (state)
                                  376 BINARY_SUBSCR
                                  386 BUILD_MAP                1
                                  388 PRECALL                  1
                                  392 CALL                     1
                                  402 POP_TOP
                                  404 JUMP_BACKWARD           32 (to 342)
                      
-                     318     >>  406 LOAD_GLOBAL              5 (NULL + len)
+                     319     >>  406 LOAD_GLOBAL              5 (NULL + len)
                                  418 LOAD_FAST                3 (countries)
                                  420 PRECALL                  1
                                  424 CALL                     1
                                  434 LOAD_CONST               4 (0)
                                  436 COMPARE_OP               4 (>)
                                  442 POP_JUMP_FORWARD_IF_FALSE    34 (to 512)
                      
-                     319         444 LOAD_FAST                3 (countries)
+                     320         444 LOAD_FAST                3 (countries)
                                  446 GET_ITER
                              >>  448 FOR_ITER                31 (to 512)
                                  450 STORE_FAST               6 (country)
                      
-                     320         452 LOAD_FAST                0 (include)
+                     321         452 LOAD_FAST                0 (include)
                                  454 LOAD_METHOD              3 (append)
                                  476 LOAD_CONST               3 ('country')
                                  478 LOAD_DEREF               7 (COUNTRIES)
                                  480 LOAD_FAST                6 (country)
                                  482 BINARY_SUBSCR
                                  492 BUILD_MAP                1
                                  494 PRECALL                  1
                                  498 CALL                     1
                                  508 POP_TOP
                                  510 JUMP_BACKWARD           32 (to 448)
                      
-                     321     >>  512 LOAD_FAST                0 (include)
+                     322     >>  512 LOAD_FAST                0 (include)
                                  514 RETURN_VALUE
                      consts
                         None
                         'city'
                         'state'
                         'country'
                         0
@@ -2433,15 +2433,15 @@
                         ('city', 'state', 'country')
                      names      ('inclusion', 'get', 'len', 'append')
                      varnames   ('include', 'cities', 'states', 'countries', 'state', 'city', 'country')
                      freevars   ('COUNTRIES', 'STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_include'
-                     firstlineno 298
+                     firstlineno 299
                      lnotab
                         0x0401040136013601360226021c01080118010aff12030402260108023c
                         02260108013c01
                   code
                      argcount  : 0
                      nlocals   : 2
                      stacksize : 6
@@ -2450,69 +2450,69 @@
                         0x9502970067007d0089036a000000000000000000a00100000000000000
                         0000000000000000000000000064016700a6020000ab0200000000000000
                         0044005d1f7d017c00a00200000000000000000000000000000000000000
                         00640189027c01190000000000000000006901a6010000ab010000000000
                         00000001008c207c005300
                                    0 COPY_FREE_VARS           2
                      
-                     323           2 RESUME                   0
+                     324           2 RESUME                   0
                      
-                     324           4 BUILD_LIST               0
+                     325           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (exclude)
                      
-                     325           8 LOAD_DEREF               3 (search)
+                     326           8 LOAD_DEREF               3 (search)
                                   10 LOAD_ATTR                0 (exclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                31 (to 126)
                                   64 STORE_FAST               1 (state)
                      
-                     326          66 LOAD_FAST                0 (exclude)
+                     327          66 LOAD_FAST                0 (exclude)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_DEREF               2 (STATES)
                                   94 LOAD_FAST                1 (state)
                                   96 BINARY_SUBSCR
                                  106 BUILD_MAP                1
                                  108 PRECALL                  1
                                  112 CALL                     1
                                  122 POP_TOP
                                  124 JUMP_BACKWARD           32 (to 62)
                      
-                     327     >>  126 LOAD_FAST                0 (exclude)
+                     328     >>  126 LOAD_FAST                0 (exclude)
                                  128 RETURN_VALUE
                      consts
                         None
                         'state'
                      names      ('exclusion', 'get', 'append')
                      varnames   ('exclude', 'state')
                      freevars   ('STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_exclude'
-                     firstlineno 323
+                     firstlineno 324
                      lnotab 0x040104013a013c01
                   'any'
                   'keywords'
                   'employees_range'
                   'ownership'
                   ''
                   ('include', 'exclude')
                   ('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters')
                names      ('list', 'inclusion', 'get', 'exclusion')
                varnames   ('search', '_hq_include', '_hq_exclude')
                freevars   ()
                cellvars   ('search', 'COUNTRIES', 'STATES')
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       '_get_api_filter'
-               firstlineno 237
+               firstlineno 238
                lnotab
                   0x0801020104ff020204fe020304fd020404fc020504fb020604fa020704
                   f9020804f8020904f7020a04f6020b04f5020c04f4020d04f3020e04f202
                   0f04f1021004f0021104ef041204ee021304ed021404ec021504eb021604
                   ea021704e9021804e8021904e7021a04e6021b04e5021c04e4021d04e302
                   1e04e2021f04e1022004e0022104df022204de062304dd022404dc022504
                   db022604da022704d9022804d8022904d7022a04d6022b04d5022c04d402
@@ -2520,58 +2520,58 @@
                   0102fc06071e191c07020134013401220104ff0e033402120112fe04f8
          names      ('__name__', '__module__', '__qualname__', 'secrets', 'access_secret_version', 'HEADERS', 'str', 'models', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', 'pd', 'DataFrame', 'enrich_targets_async', '_get_api_filter')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GrataWrapper'
-         firstlineno 172
+         firstlineno 173
          lnotab 0x0a021e0102fe06051e161a0b100b1a0f
       'GrataWrapper'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a026401650364026504640365056606640484045a
             0664026504640365056604640584045a0764016503640365056604640684
             045a0864075300
-         344           0 RESUME                   0
+         345           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SourceScrubWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         345          10 LOAD_CONST               1 ('domain')
+         346          10 LOAD_CONST               1 ('domain')
                       12 LOAD_NAME                3 (str)
                       14 LOAD_CONST               2 ('search')
                       16 LOAD_NAME                4 (Search)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (dict)
                       22 BUILD_TUPLE              6
-                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 345>)
+                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 346>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               6 (find_similar)
          
-         348          30 LOAD_CONST               2 ('search')
+         349          30 LOAD_CONST               2 ('search')
                       32 LOAD_NAME                4 (Search)
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                5 (dict)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 348>)
+                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 349>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (find_by_criteria)
          
-         351          46 LOAD_CONST               1 ('domain')
+         352          46 LOAD_CONST               1 ('domain')
                       48 LOAD_NAME                3 (str)
                       50 LOAD_CONST               3 ('return')
                       52 LOAD_NAME                5 (dict)
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 351>)
+                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 352>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (enrich)
                       62 LOAD_CONST               7 (None)
                       64 RETURN_VALUE
          consts
             'SourceScrubWrapper'
             'domain'
@@ -2579,81 +2579,81 @@
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               345           0 RESUME                   0
+               346           0 RESUME                   0
                
-               346           2 LOAD_CONST               0 (None)
+               347           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain', 'search')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 345
+               firstlineno 346
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               348           0 RESUME                   0
+               349           0 RESUME                   0
                
-               349           2 LOAD_CONST               0 (None)
+               350           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('search',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 348
+               firstlineno 349
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               351           0 RESUME                   0
+               352           0 RESUME                   0
                
-               352           2 LOAD_CONST               0 (None)
+               353           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 351
+               firstlineno 352
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'Search', 'dict', 'find_similar', 'find_by_criteria', 'enrich')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'SourceScrubWrapper'
-         firstlineno 344
+         firstlineno 345
          lnotab 0x0a0114031003
       'SourceScrubWrapper'
    names      ('time', 'pandas', 'pd', 'concurrent.futures', 'ThreadPoolExecutor', 'functools', 'partial', 'typing', 'List', 'googlemaps', 'requests', 'gandai', 'gpt', 'helpers', 'models', 'query', 'secrets', 'gandai.models', 'Search', 'Client', 'access_secret_version', 'gmaps', 'MAX_WORKERS', 'GoogleMapsWrapper', 'GrataWrapper', 'SourceScrubWrapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c010c02080108021c010c023e0104031a7f00
-      1c1a7f002d
+      1d1a7f002d
```

### Comparing `gandai-1.3.7/gandai/analytics.py` & `gandai-1.3.8/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/auth.py` & `gandai-1.3.8/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/db.py` & `gandai-1.3.8/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/gpt.py` & `gandai-1.3.8/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/main.py` & `gandai-1.3.8/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.3.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/migrations/db_seed.py` & `gandai-1.3.8/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/migrations/dealcloud.py` & `gandai-1.3.8/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/migrations/sql/schema.sql` & `gandai-1.3.8/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/models.py` & `gandai-1.3.8/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/query.py` & `gandai-1.3.8/gandai/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,24 +105,49 @@
 def insert_targets_from_domains(
     domains: List[str], search_uid: int, actor_key: str, last_event_type: str
 ) -> None:
     """
     Takes in domains, inserts targets into a review stage, where they will
     try to be enriched on process event
     """
-    existing_domains = set(unique_domains(search_uid=search_uid)['domain'])
-    
-    new_domains = {helpers.clean_domain(domain) for domain in domains if "." in domain}
 
-    domains_to_insert = list(new_domains - existing_domains)
-    existing_domains = set(unique_domains(search_uid=search_uid)['domain'])
-    
+    def downstream_domains(search_uid: int, last_event_type: str) -> set:
+        STAGES = [
+            "create",
+            "advance",
+            "validate",
+            "send",
+            "accept",
+            "reject",
+            "conflict",
+        ]
+
+        protected_stages = tuple(STAGES[STAGES.index(last_event_type): :])
+
+        with db.connect() as conn:
+            statement = f"""
+                    SELECT distinct(domain)
+                    FROM event
+                    WHERE search_uid = :search_uid 
+                    AND type IN {protected_stages}
+                """
+            result = conn.execute(
+                sqlalchemy.text(statement),
+                {"search_uid": search_uid},
+            )
+            df = pd.DataFrame(result.fetchall(), columns=result.keys())
+        return set(df["domain"])
+
+    protected_domains: set = downstream_domains(
+        search_uid=search_uid, last_event_type=last_event_type
+    )
+
     new_domains = {helpers.clean_domain(domain) for domain in domains if "." in domain}
 
-    domains_to_insert = list(new_domains - existing_domains)
+    domains_to_insert = list(new_domains - protected_domains)
 
     with db.connect() as con:
         for domain in domains_to_insert:
             # should these be in same transaction?
             con.execute(
                 sqlalchemy.text(
                     """
@@ -145,20 +170,20 @@
                 {
                     "search_uid": search_uid,
                     "actor_key": actor_key,
                     "domain": domain,
                     "type": last_event_type,
                 },
             )
-        
+
         con.commit()
 
     resp = {
         "inserted": len(domains_to_insert),
-        "duplicates": len(new_domains.intersection(existing_domains)),
+        "duplicates": len(new_domains.intersection(protected_domains)),
     }
     return resp
 
 
 def insert_companies_as_targets(
     companies: List[Any], search_uid: int, actor_key: str
 ) -> None:
@@ -246,31 +271,37 @@
         WHERE 
             rn = 1;
         """
 
         result = conn.execute(sqlalchemy.text(statement))
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
         return df
-    
+
+
 def search_event_count_by_type() -> pd.DataFrame:
     with db.connect() as conn:
         result = conn.execute(
             sqlalchemy.text(
                 """
                 SELECT search_uid, type, count(DISTINCT domain)
                 FROM event
                 WHERE type in ('create','advance', 'validate', 'send', 'accept')
                 GROUP BY search_uid, type
                 """
             )
         )
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
-        df = df.pivot(index="search_uid", columns="type", values="count").reset_index().fillna(0)
+        df = (
+            df.pivot(index="search_uid", columns="type", values="count")
+            .reset_index()
+            .fillna(0)
+        )
         return df
 
+
 def search():
     with db.connect() as conn:
         statement = """
         SELECT 
             s.uid,
             s.label,
             (SELECT COUNT(*) 
@@ -294,36 +325,42 @@
             elif row["total_validate_count"] > 25:
                 return "Top Searches"
             else:
                 return "All Searches"
 
         df["group"] = df.apply(_set_group, axis=1)
 
-        df = df.merge(search_event_count_by_type(), left_on="uid", right_on="search_uid", how="left")
+        df = df.merge(
+            search_event_count_by_type(),
+            left_on="uid",
+            right_on="search_uid",
+            how="left",
+        )
 
         df = df.sort_values(
-            by=["group", "recent_validate_count","total_validate_count", "label"],
+            by=["group", "recent_validate_count", "total_validate_count", "label"],
             ascending=[False, False, False, True],
         )
 
         df = df.fillna("")
         # df['label'] = df['label'] + "      (" + df['name'] + ")"
     return df
 
+
 def actor() -> pd.DataFrame:
     with db.connect() as conn:
         result = conn.execute(
             sqlalchemy.text(
                 """
                 SELECT * FROM actor
                 """
             )
         )
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
-        df = df.drop(columns=["id","created","updated"])
+        df = df.drop(columns=["id", "created", "updated"])
         return df
 
 
 def search_target_by_last_event_type(search_uid: int, last_event_type: str = None):
     statement = """
         SELECT 
             e.id, 
@@ -386,55 +423,55 @@
 
     # handle sorting
     search = find_search_by_uid(search_uid)
     targets = targets.sort_values(
         by=search.sort.get("field", "domain"),
         ascending=search.sort.get("order") == "asc",
     )
-    targets['employees'] = pd.to_numeric(targets['employees'])
+    targets["employees"] = pd.to_numeric(targets["employees"])
     return targets
 
 
 # def search_target_export(search_uid: int) -> pd.DataFrame:
 #     """Returns all the targets not in rejected or created"""
 
 #     statement = """
-#         SELECT 
-#             e.id, 
-#             e.search_uid, 
-#             e.domain, 
-#             e.type AS last_event_type, 
+#         SELECT
+#             e.id,
+#             e.search_uid,
+#             e.domain,
+#             e.type AS last_event_type,
 #             to_timestamp(e.created) AS updated,
 #             c.meta as meta,
 #             (r.data->>'rating') AS rating
 #         FROM (
-#             SELECT 
-#                 search_uid, 
-#                 domain, 
+#             SELECT
+#                 search_uid,
+#                 domain,
 #                 MAX(created) AS max_created
-#             FROM 
+#             FROM
 #                 event
-#             WHERE 
-#                 type NOT IN ('comment','rating','generate','criteria') 
+#             WHERE
+#                 type NOT IN ('comment','rating','generate','criteria')
 #                 AND search_uid = :search_uid
-#             GROUP BY 
+#             GROUP BY
 #                 domain, search_uid
 #         ) AS max_event
-#         JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid 
+#         JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid
 #         JOIN company c ON c.domain = e.domain
 #         LEFT JOIN (
-#             SELECT 
+#             SELECT
 #                 search_uid,
-#                 domain, 
+#                 domain,
 #                 MAX(created) AS max_created
-#             FROM 
+#             FROM
 #                 event
-#             WHERE 
+#             WHERE
 #                 type = 'rating'
-#             GROUP BY 
+#             GROUP BY
 #                 domain, search_uid
 #         ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid
 #         LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;
 #     """
 #     with db.connect() as conn:
 #         result = conn.execute(
 #             sqlalchemy.text(statement),
@@ -448,15 +485,14 @@
 #         #         meta, left_on=["domain"], right_on=["domain"], how="left"
 #         #     )
 #         #     targets = targets.drop(columns=["meta"])
 #         #     targets = targets.sort_values(by=["last_event_type", "domain"])
 #     return targets
 
 
-
 def target_count(search_uid: int) -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
             SELECT 
                 e.type AS last_event_type,
                 COUNT(e.type)
             FROM (
```

### Comparing `gandai-1.3.7/gandai/secrets.py` & `gandai-1.3.8/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.7/gandai/sources.py` & `gandai-1.3.8/gandai/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             "domain"
         ].to_list()
 
         if "website" not in place:
             print(f"no website for {place_id}")
             return
 
+        # actually this should cache the result on the company....
         if helpers.clean_domain(place["website"]) in existing_search_domains:
             print(f"skipping {place['website']} - already in search_uid {search_uid}")
             return
 
         gpt_prompt = (" ").join(
             [
                 f"Q: Based on these reviews:",
```

### Comparing `gandai-1.3.7/gandai.egg-info/SOURCES.txt` & `gandai-1.3.8/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

