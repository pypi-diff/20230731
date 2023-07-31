# Comparing `tmp/gandai-1.3.8.tar.gz` & `tmp/gandai-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.3.8.tar", last modified: Mon Jul 31 19:58:05 2023, max compression
+gzip compressed data, was "gandai-1.3.9.tar", last modified: Mon Jul 31 21:41:42 2023, max compression
```

## Comparing `gandai-1.3.8.tar` & `gandai-1.3.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.143560 gandai-1.3.8/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.8/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-31 19:58:05.143404 gandai-1.3.8/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.134488 gandai-1.3.8/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.141187 gandai-1.3.8/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.8/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.8/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-27 20:57:53.000000 gandai-1.3.8/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.3.8/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.8/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.8/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-27 21:29:01.000000 gandai-1.3.8/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.8/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.8/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    31257 2023-07-31 19:51:53.000000 gandai-1.3.8/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-26 13:45:26.000000 gandai-1.3.8/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.8/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    17502 2023-07-31 19:04:57.000000 gandai-1.3.8/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-27 21:16:13.000000 gandai-1.3.8/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-27 20:52:17.000000 gandai-1.3.8/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.142211 gandai-1.3.8/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.8/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.142669 gandai-1.3.8/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.8/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.143154 gandai-1.3.8/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.8/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.8/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    22049 2023-07-31 19:51:51.000000 gandai-1.3.8/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.8/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)    11690 2023-07-31 19:04:54.000000 gandai-1.3.8/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 19:58:05.135192 gandai-1.3.8/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-31 19:58:05.000000 gandai-1.3.8/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-31 19:57:55.000000 gandai-1.3.8/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-31 19:58:05.143596 gandai-1.3.8/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.8/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 21:41:42.777782 gandai-1.3.9/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.9/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-31 21:41:42.777649 gandai-1.3.9/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 21:41:42.770744 gandai-1.3.9/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.9/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 21:41:42.775462 gandai-1.3.9/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.9/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.9/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-27 20:57:53.000000 gandai-1.3.9/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.3.9/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.9/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.9/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3765 2023-07-31 21:32:32.000000 gandai-1.3.9/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.9/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-31 21:20:15.000000 gandai-1.3.9/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-31 21:32:32.000000 gandai-1.3.9/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.9/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    31257 2023-07-31 21:20:14.000000 gandai-1.3.9/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-26 13:45:26.000000 gandai-1.3.9/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.9/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17532 2023-07-31 21:32:32.000000 gandai-1.3.9/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-27 20:52:17.000000 gandai-1.3.9/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-27 20:52:17.000000 gandai-1.3.9/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.9/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1647 2023-07-31 21:16:20.000000 gandai-1.3.9/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)      399 2023-07-31 21:16:20.000000 gandai-1.3.9/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     3005 2023-07-31 21:16:20.000000 gandai-1.3.9/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 21:41:42.776410 gandai-1.3.9/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.9/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 21:41:42.776860 gandai-1.3.9/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.9/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.9/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.9/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.9/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.9/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 21:41:42.777370 gandai-1.3.9/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.9/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.9/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.9/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    22050 2023-07-31 21:16:20.000000 gandai-1.3.9/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.9/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)    11625 2023-07-31 21:16:20.000000 gandai-1.3.9/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-31 21:41:42.771339 gandai-1.3.9/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-31 21:41:42.000000 gandai-1.3.9/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-31 21:41:42.000000 gandai-1.3.9/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-31 21:41:42.000000 gandai-1.3.9/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-31 21:41:42.000000 gandai-1.3.9/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-31 21:41:33.000000 gandai-1.3.9/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-31 21:41:42.777825 gandai-1.3.9/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.9/setup.py
```

### Comparing `gandai-1.3.8/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x9ddec264 (Thu Jul 27 21:16:13 2023 UTC)
-files sz: 1631
+moddate:  0xa424c864 (Mon Jul 31 21:16:20 2023 UTC)
+files sz: 1647
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064016c016d025a030100640064026c046d
-      055a056d065a066d075a070100020065056a0800000000000000006403a6
+      055a056d065a066d075a070100020065076a0800000000000000006403a6
       010000ab01000000000000000065005f0900000000000000006410640565
-      0a6406650b6604640784055a0c640865076a0d0000000000000000640965
+      0a6406650b6604640784055a0c640865056a0d0000000000000000640965
       0a6604640a84045a0e6411640c650a640d650b6409650f6606640e84055a
       10640f84005a1164015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (openai)
@@ -24,26 +24,26 @@
                 12 LOAD_CONST               1 (None)
                 14 IMPORT_NAME              1 (plotly.express)
                 16 IMPORT_FROM              2 (express)
                 18 STORE_NAME               3 (px)
                 20 POP_TOP
    
      4          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               2 (('secrets', 'query', 'models'))
+                24 LOAD_CONST               2 (('models', 'query', 'secrets'))
                 26 IMPORT_NAME              4 (gandai)
-                28 IMPORT_FROM              5 (secrets)
-                30 STORE_NAME               5 (secrets)
+                28 IMPORT_FROM              5 (models)
+                30 STORE_NAME               5 (models)
                 32 IMPORT_FROM              6 (query)
                 34 STORE_NAME               6 (query)
-                36 IMPORT_FROM              7 (models)
-                38 STORE_NAME               7 (models)
+                36 IMPORT_FROM              7 (secrets)
+                38 STORE_NAME               7 (secrets)
                 40 POP_TOP
    
      6          42 PUSH_NULL
-                44 LOAD_NAME                5 (secrets)
+                44 LOAD_NAME                7 (secrets)
                 46 LOAD_ATTR                8 (access_secret_version)
                 56 LOAD_CONST               3 ('OPENAI_KEY')
                 58 PRECALL                  1
                 62 CALL                     1
                 72 LOAD_NAME                0 (openai)
                 74 STORE_ATTR               9 (api_key)
    
@@ -53,45 +53,45 @@
                 90 LOAD_CONST               6 ('max_tokens')
                 92 LOAD_NAME               11 (int)
                 94 BUILD_TUPLE              4
                 96 LOAD_CONST               7 (<code object ask_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 9>)
                 98 MAKE_FUNCTION            5 (defaults, annotations)
                100 STORE_NAME              12 (ask_gpt)
    
-    18         102 LOAD_CONST               8 ('search')
-               104 LOAD_NAME                7 (models)
+    19         102 LOAD_CONST               8 ('search')
+               104 LOAD_NAME                5 (models)
                106 LOAD_ATTR               13 (Search)
                116 LOAD_CONST               9 ('return')
                118 LOAD_NAME               10 (str)
                120 BUILD_TUPLE              4
-               122 LOAD_CONST              10 (<code object get_suggested_search_phrase, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 18>)
+               122 LOAD_CONST              10 (<code object get_suggested_search_phrase, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 19>)
                124 MAKE_FUNCTION            4 (annotations)
                126 STORE_NAME              14 (get_suggested_search_phrase)
    
-    27         128 LOAD_CONST              17 ((25,))
+    31         128 LOAD_CONST              17 ((25,))
                130 LOAD_CONST              12 ('area')
                132 LOAD_NAME               10 (str)
                134 LOAD_CONST              13 ('top_n')
                136 LOAD_NAME               11 (int)
                138 LOAD_CONST               9 ('return')
                140 LOAD_NAME               15 (list)
                142 BUILD_TUPLE              6
-               144 LOAD_CONST              14 (<code object get_top_zip_codes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 27>)
+               144 LOAD_CONST              14 (<code object get_top_zip_codes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 31>)
                146 MAKE_FUNCTION            5 (defaults, annotations)
                148 STORE_NAME              16 (get_top_zip_codes)
    
-    35         150 LOAD_CONST              15 (<code object summarize_search_by, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 35>)
+    39         150 LOAD_CONST              15 (<code object summarize_search_by, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 39>)
                152 MAKE_FUNCTION            0
                154 STORE_NAME              17 (summarize_search_by)
                156 LOAD_CONST               1 (None)
                158 RETURN_VALUE
    consts
       0
       None
-      ('secrets', 'query', 'models')
+      ('models', 'query', 'secrets')
       'OPENAI_KEY'
       60
       'prompt'
       'max_tokens'
       code
          argcount  : 2
          nlocals   : 3
@@ -153,54 +153,56 @@
             0x97007401000000000000000000006a0100000000000000007c006a0200
             000000000000006401ac02a6020000ab0200000000000000007d017c0164
             0319000000000000000000a0030000000000000000000000000000000000
             000000a6000000ab00000000000000000001007409000000000000000000
             0064047c01640319000000000000000000a0030000000000000000000000
             000000000000000000a6000000ab0000000000000000009b009d026405ac
             06a6020000ab0200000000000000007d027c025300
-          18           0 RESUME                   0
+          19           0 RESUME                   0
          
-          19           2 LOAD_GLOBAL              1 (NULL + query)
+          20           2 LOAD_GLOBAL              1 (NULL + query)
                       14 LOAD_ATTR                1 (search_target_by_last_event_type)
-                      24 LOAD_FAST                0 (search)
+         
+          21          24 LOAD_FAST                0 (search)
                       26 LOAD_ATTR                2 (uid)
                       36 LOAD_CONST               1 ('accept')
-                      38 KW_NAMES                 2
+         
+          20          38 KW_NAMES                 2
                       40 PRECALL                  2
                       44 CALL                     2
                       54 STORE_FAST               1 (accepted)
          
-          20          56 LOAD_FAST                1 (accepted)
+          23          56 LOAD_FAST                1 (accepted)
                       58 LOAD_CONST               3 ('description')
                       60 BINARY_SUBSCR
                       70 LOAD_METHOD              3 (tolist)
                       92 PRECALL                  0
                       96 CALL                     0
                      106 POP_TOP
          
-          21         108 LOAD_GLOBAL              9 (NULL + ask_gpt)
+          24         108 LOAD_GLOBAL              9 (NULL + ask_gpt)
          
-          22         120 LOAD_CONST               4 ('What search phrase would you use to search Google Maps to find companies that look like this: ')
+          25         120 LOAD_CONST               4 ('What search phrase would you use to search Google Maps to find companies that look like this: ')
                      122 LOAD_FAST                1 (accepted)
                      124 LOAD_CONST               3 ('description')
                      126 BINARY_SUBSCR
                      136 LOAD_METHOD              3 (tolist)
                      158 PRECALL                  0
                      162 CALL                     0
                      172 FORMAT_VALUE             0
                      174 BUILD_STRING             2
          
-          23         176 LOAD_CONST               5 (60)
+          26         176 LOAD_CONST               5 (60)
          
-          21         178 KW_NAMES                 6
+          24         178 KW_NAMES                 6
                      180 PRECALL                  2
                      184 CALL                     2
                      194 STORE_FAST               2 (resp)
          
-          25         196 LOAD_FAST                2 (resp)
+          28         196 LOAD_FAST                2 (resp)
                      198 RETURN_VALUE
          consts
             None
             'accept'
             ('search_uid', 'last_event_type')
             'description'
             'What search phrase would you use to search Google Maps to find companies that look like this: '
@@ -208,49 +210,49 @@
             ('max_tokens',)
          names      ('query', 'search_target_by_last_event_type', 'uid', 'tolist', 'ask_gpt')
          varnames   ('search', 'accepted', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
          name       'get_suggested_search_phrase'
-         firstlineno 18
-         lnotab 0x0201360134010c01380102fe1204
+         firstlineno 19
+         lnotab 0x020116010eff120334010c01380102fe1204
       25
       'area'
       'top_n'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
             0x970074010000000000000000000064017c019b0064027c009b0064039d
             056404ac05a6020000ab0200000000000000007d02740300000000000000
             0000007c02a6010000ab0100000000000000005300
-          27           0 RESUME                   0
+          31           0 RESUME                   0
          
-          28           2 LOAD_GLOBAL              1 (NULL + ask_gpt)
+          32           2 LOAD_GLOBAL              1 (NULL + ask_gpt)
          
-          29          14 LOAD_CONST               1 ('As a python array List[str], the top ')
+          33          14 LOAD_CONST               1 ('As a python array List[str], the top ')
                       16 LOAD_FAST                1 (top_n)
                       18 FORMAT_VALUE             0
                       20 LOAD_CONST               2 (' zip codes in ')
                       22 LOAD_FAST                0 (area)
                       24 FORMAT_VALUE             0
                       26 LOAD_CONST               3 (' are:')
                       28 BUILD_STRING             5
          
-          30          30 LOAD_CONST               4 (1000)
+          34          30 LOAD_CONST               4 (1000)
          
-          28          32 KW_NAMES                 5
+          32          32 KW_NAMES                 5
                       34 PRECALL                  2
                       38 CALL                     2
                       48 STORE_FAST               2 (resp)
          
-          32          50 LOAD_GLOBAL              3 (NULL + eval)
+          36          50 LOAD_GLOBAL              3 (NULL + eval)
                       62 LOAD_FAST                2 (resp)
                       64 PRECALL                  1
                       68 CALL                     1
                       78 RETURN_VALUE
          consts
             None
             'As a python array List[str], the top '
@@ -260,15 +262,15 @@
             ('max_tokens',)
          names      ('ask_gpt', 'eval')
          varnames   ('area', 'top_n', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
          name       'get_top_zip_codes'
-         firstlineno 27
+         firstlineno 31
          lnotab 0x02010c01100102fe1204
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -286,45 +288,45 @@
             00ab0100000000000000000100640b640c84007c00640819000000000000
             000000a0050000000000000000000000000000000000000000a6000000ab
             000000000000000000a00600000000000000000000000000000000000000
             006402a6010000ab0100000000000000004400a6000000ab000000000000
             0000009b0064099d037d01740700000000000000000000740f0000000000
             00000000007c01640dac0ea6020000ab020000000000000000a6010000ab
             010000000000000000010064005300
-          35           0 RESUME                   0
+          39           0 RESUME                   0
          
-          37           2 LOAD_GLOBAL              1 (NULL + px)
+          40           2 LOAD_GLOBAL              1 (NULL + px)
                       14 LOAD_ATTR                1 (histogram)
                       24 LOAD_FAST                0 (targets)
                       26 LOAD_CONST               1 ('employees')
                       28 LOAD_CONST               2 (20)
                       30 LOAD_CONST               3 (400)
                       32 LOAD_CONST               3 (400)
                       34 KW_NAMES                 4
                       36 PRECALL                  5
                       40 CALL                     5
                       50 LOAD_METHOD              2 (show)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 POP_TOP
          
-          39          88 LOAD_GLOBAL              7 (NULL + print)
+          42          88 LOAD_GLOBAL              7 (NULL + print)
                      100 LOAD_FAST                0 (targets)
                      102 LOAD_CONST               5 ('ownership')
                      104 BINARY_SUBSCR
                      114 LOAD_METHOD              4 (value_counts)
                      136 PRECALL                  0
                      140 CALL                     0
                      150 PRECALL                  1
                      154 CALL                     1
                      164 POP_TOP
          
-          41         166 LOAD_CONST               6 ('\n    The top three geographic areas, based on the ')
+          44         166 LOAD_CONST               6 ('\n    The top three geographic areas, based on the ')
          
-          42         168 LOAD_CONST               7 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 42>)
+          45         168 LOAD_CONST               7 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 45>)
                      170 MAKE_FUNCTION            0
                      172 LOAD_FAST                0 (targets)
                      174 LOAD_CONST               8 ('description')
                      176 BINARY_SUBSCR
                      186 LOAD_METHOD              5 (dropna)
                      208 PRECALL                  0
                      212 CALL                     0
@@ -332,32 +334,32 @@
                      244 LOAD_CONST               2 (20)
                      246 PRECALL                  1
                      250 CALL                     1
                      260 GET_ITER
                      262 PRECALL                  0
                      266 CALL                     0
          
-          41         276 FORMAT_VALUE             0
+          44         276 FORMAT_VALUE             0
                      278 LOAD_CONST               9 (' are:\n    ')
                      280 BUILD_STRING             3
                      282 STORE_FAST               1 (GPT_PROMPT)
          
-          45         284 LOAD_GLOBAL              7 (NULL + print)
+          48         284 LOAD_GLOBAL              7 (NULL + print)
                      296 LOAD_GLOBAL             15 (NULL + ask_gpt)
                      308 LOAD_FAST                1 (GPT_PROMPT)
                      310 KW_NAMES                10
                      312 PRECALL                  1
                      316 CALL                     1
                      326 PRECALL                  1
                      330 CALL                     1
                      340 POP_TOP
          
-          47         342 LOAD_CONST              11 ('\n    Give me the company type, products and services, and end markets ')
+          50         342 LOAD_CONST              11 ('\n    Give me the company type, products and services, and end markets ')
          
-          48         344 LOAD_CONST              12 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 48>)
+          51         344 LOAD_CONST              12 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 51>)
                      346 MAKE_FUNCTION            0
                      348 LOAD_FAST                0 (targets)
                      350 LOAD_CONST               8 ('description')
                      352 BINARY_SUBSCR
                      362 LOAD_METHOD              5 (dropna)
                      384 PRECALL                  0
                      388 CALL                     0
@@ -365,20 +367,20 @@
                      420 LOAD_CONST               2 (20)
                      422 PRECALL                  1
                      426 CALL                     1
                      436 GET_ITER
                      438 PRECALL                  0
                      442 CALL                     0
          
-          47         452 FORMAT_VALUE             0
+          50         452 FORMAT_VALUE             0
                      454 LOAD_CONST               9 (' are:\n    ')
                      456 BUILD_STRING             3
                      458 STORE_FAST               1 (GPT_PROMPT)
          
-          51         460 LOAD_GLOBAL              7 (NULL + print)
+          54         460 LOAD_GLOBAL              7 (NULL + print)
                      472 LOAD_GLOBAL             15 (NULL + ask_gpt)
                      484 LOAD_FAST                1 (GPT_PROMPT)
                      486 LOAD_CONST              13 (100)
                      488 KW_NAMES                14
                      490 PRECALL                  2
                      494 CALL                     2
                      504 PRECALL                  1
@@ -396,15 +398,15 @@
             '\n    The top three geographic areas, based on the '
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code 0x970067007c005d047d017c0191028c055300
-                42           0 RESUME                   0
+                45           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                 4 (to 16)
                              8 STORE_FAST               1 (desc)
                             10 LOAD_FAST                1 (desc)
                             12 LIST_APPEND              2
                             14 JUMP_BACKWARD            5 (to 6)
@@ -412,27 +414,27 @@
                consts
                names      ()
                varnames   ('.0', 'desc')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
                name       '<listcomp>'
-               firstlineno 42
+               firstlineno 45
                lnotab 0x
             'description'
             ' are:\n    '
             ('prompt',)
             '\n    Give me the company type, products and services, and end markets '
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code 0x970067007c005d047d017c0191028c055300
-                48           0 RESUME                   0
+                51           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                 4 (to 16)
                              8 STORE_FAST               1 (desc)
                             10 LOAD_FAST                1 (desc)
                             12 LIST_APPEND              2
                             14 JUMP_BACKWARD            5 (to 6)
@@ -440,29 +442,29 @@
                consts
                names      ()
                varnames   ('.0', 'desc')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
                name       '<listcomp>'
-               firstlineno 48
+               firstlineno 51
                lnotab 0x
             100
             ('prompt', 'max_tokens')
          names      ('px', 'histogram', 'show', 'print', 'value_counts', 'dropna', 'sample', 'ask_gpt')
          varnames   ('targets', 'GPT_PROMPT')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
          name       'summarize_search_by'
-         firstlineno 35
-         lnotab 0x020256024e0202016cff08043a0202016cff0804
+         firstlineno 39
+         lnotab 0x020156024e0202016cff08043a0202016cff0804
       (60,)
       (25,)
-   names      ('openai', 'plotly.express', 'express', 'px', 'gandai', 'secrets', 'query', 'models', 'access_secret_version', 'api_key', 'str', 'int', 'ask_gpt', 'Search', 'get_suggested_search_phrase', 'list', 'get_top_zip_codes', 'summarize_search_by')
+   names      ('openai', 'plotly.express', 'express', 'px', 'gandai', 'models', 'query', 'secrets', 'access_secret_version', 'api_key', 'str', 'int', 'ask_gpt', 'Search', 'get_suggested_search_phrase', 'list', 'get_top_zip_codes', 'summarize_search_by')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010c0214022a0312091a091608
+   lnotab 0x00ff020108010c0214022a03120a1a0c1608
```

### Comparing `gandai-1.3.8/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x01d9c264 (Thu Jul 27 20:52:17 2023 UTC)
-files sz: 402
+moddate:  0xa424c864 (Mon Jul 31 21:16:20 2023 UTC)
+files sz: 399
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640265016a020000000000000000640365016a
@@ -13,29 +13,29 @@
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (pandas)
                  8 STORE_NAME               1 (pd)
    
-     3          10 LOAD_CONST               2 ('df')
+     4          10 LOAD_CONST               2 ('df')
                 12 LOAD_NAME                1 (pd)
                 14 LOAD_ATTR                2 (DataFrame)
                 24 LOAD_CONST               3 ('return')
                 26 LOAD_NAME                1 (pd)
                 28 LOAD_ATTR                2 (DataFrame)
                 38 BUILD_TUPLE              4
-                40 LOAD_CONST               4 (<code object clean_columns, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py", line 3>)
+                40 LOAD_CONST               4 (<code object clean_columns, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py", line 4>)
                 42 MAKE_FUNCTION            4 (annotations)
                 44 STORE_NAME               3 (clean_columns)
    
-     8          46 LOAD_CONST               3 ('return')
+     9          46 LOAD_CONST               3 ('return')
                 48 LOAD_NAME                4 (str)
                 50 BUILD_TUPLE              2
-                52 LOAD_CONST               5 (<code object clean_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py", line 8>)
+                52 LOAD_CONST               5 (<code object clean_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py", line 9>)
                 54 MAKE_FUNCTION            4 (annotations)
                 56 STORE_NAME               5 (clean_domain)
                 58 LOAD_CONST               1 (None)
                 60 RETURN_VALUE
    consts
       0
       None
@@ -45,42 +45,42 @@
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code
             0x9700640184007c006a0000000000000000004400a6000000ab00000000
             00000000007c005f0000000000000000007c005300
-           3           0 RESUME                   0
+           4           0 RESUME                   0
          
-           4           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py", line 4>)
+           5           2 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py", line 5>)
                        4 MAKE_FUNCTION            0
                        6 LOAD_FAST                0 (df)
                        8 LOAD_ATTR                0 (columns)
                       18 GET_ITER
                       20 PRECALL                  0
                       24 CALL                     0
                       34 LOAD_FAST                0 (df)
                       36 STORE_ATTR               0 (columns)
          
-           5          46 LOAD_FAST                0 (df)
+           6          46 LOAD_FAST                0 (df)
                       48 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 19
                code
                   0x970067007c005d3e7d017c01a000000000000000000000000000000000
                   0000000000a6000000ab000000000000000000a001000000000000000000
                   000000000000000000000064006401a6020000ab020000000000000000a0
                   01000000000000000000000000000000000000000064026403a6020000ab
                   02000000000000000091028c3f5300
-                 4           0 RESUME                   0
+                 5           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                62 (to 132)
                              8 STORE_FAST               1 (col)
                             10 LOAD_FAST                1 (col)
                             12 LOAD_METHOD              0 (lower)
                             34 PRECALL                  0
@@ -105,23 +105,23 @@
                   ''
                names      ('lower', 'replace')
                varnames   ('.0', 'col')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py'
                name       '<listcomp>'
-               firstlineno 4
+               firstlineno 5
                lnotab 0x
          names      ('columns',)
          varnames   ('df',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py'
          name       'clean_columns'
-         firstlineno 3
+         firstlineno 4
          lnotab 0x02012c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
@@ -130,26 +130,26 @@
             000000a6000000ab0000000000000000007d007c00a00200000000000000
             0000000000000000000000000064016402a6020000ab0200000000000000
             00a002000000000000000000000000000000000000000064036402a60200
             00ab020000000000000000a0020000000000000000000000000000000000
             00000064046402a6020000ab0200000000000000007d007c00a003000000
             00000000000000000000000000000000006405a6010000ab010000000000
             0000006406190000000000000000005300
-           8           0 RESUME                   0
+           9           0 RESUME                   0
          
-          10           2 LOAD_FAST                0 (url)
+          11           2 LOAD_FAST                0 (url)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 LOAD_METHOD              1 (strip)
                       62 PRECALL                  0
                       66 CALL                     0
                       76 STORE_FAST               0 (url)
          
-          11          78 LOAD_FAST                0 (url)
+          12          78 LOAD_FAST                0 (url)
                       80 LOAD_METHOD              2 (replace)
                      102 LOAD_CONST               1 ('http://')
                      104 LOAD_CONST               2 ('')
                      106 PRECALL                  2
                      110 CALL                     2
                      120 LOAD_METHOD              2 (replace)
                      142 LOAD_CONST               3 ('https://')
@@ -159,15 +159,15 @@
                      160 LOAD_METHOD              2 (replace)
                      182 LOAD_CONST               4 ('www.')
                      184 LOAD_CONST               2 ('')
                      186 PRECALL                  2
                      190 CALL                     2
                      200 STORE_FAST               0 (url)
          
-          12         202 LOAD_FAST                0 (url)
+          13         202 LOAD_FAST                0 (url)
                      204 LOAD_METHOD              3 (split)
                      226 LOAD_CONST               5 ('/')
                      228 PRECALL                  1
                      232 CALL                     1
                      242 LOAD_CONST               6 (0)
                      244 BINARY_SUBSCR
                      254 RETURN_VALUE
@@ -181,17 +181,17 @@
             0
          names      ('lower', 'strip', 'replace', 'split')
          varnames   ('url',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py'
          name       'clean_domain'
-         firstlineno 8
+         firstlineno 9
          lnotab 0x02024c017c01
    names      ('pandas', 'pd', 'DataFrame', 'clean_columns', 'str', 'clean_domain')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/helpers.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108022405
+   lnotab 0x00ff020108032405
```

### Comparing `gandai-1.3.8/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x01d9c264 (Thu Jul 27 20:52:17 2023 UTC)
-files sz: 3030
+moddate:  0xa424c864 (Mon Jul 31 21:16:20 2023 UTC)
+files sz: 3005
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a0401
@@ -79,20 +79,20 @@
                110 LOAD_CONST              10 ('return')
                112 LOAD_CONST               4 (None)
                114 BUILD_TUPLE              4
                116 LOAD_CONST              11 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 13>)
                118 MAKE_FUNCTION            4 (annotations)
                120 STORE_NAME              20 (process_event)
    
-    76         122 LOAD_CONST              12 ('search_uid')
+    75         122 LOAD_CONST              12 ('search_uid')
                124 LOAD_NAME               19 (int)
                126 LOAD_CONST              10 ('return')
                128 LOAD_NAME               19 (int)
                130 BUILD_TUPLE              4
-               132 LOAD_CONST              13 (<code object process_events, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 76>)
+               132 LOAD_CONST              13 (<code object process_events, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 75>)
                134 MAKE_FUNCTION            4 (annotations)
                136 STORE_NAME              21 (process_events)
                138 LOAD_CONST               4 (None)
                140 RETURN_VALUE
    consts
       0
       ('ThreadPoolExecutor',)
@@ -191,213 +191,213 @@
                      158 LOAD_ATTR                6 (meta)
                      168 LOAD_METHOD              7 (keys)
                      190 PRECALL                  0
                      194 CALL                     0
                      204 CONTAINS_OP              1
                      206 POP_JUMP_FORWARD_IF_FALSE   174 (to 556)
          
-          35         208 LOAD_GLOBAL             17 (NULL + grata)
+          34         208 LOAD_GLOBAL             17 (NULL + grata)
                      220 LOAD_ATTR                9 (enrich)
                      230 LOAD_FAST                3 (company)
                      232 LOAD_ATTR                5 (domain)
                      242 PRECALL                  1
                      246 CALL                     1
                      256 STORE_FAST               4 (resp)
          
-          36         258 LOAD_FAST                4 (resp)
+          35         258 LOAD_FAST                4 (resp)
                      260 LOAD_METHOD             10 (get)
                      282 LOAD_CONST               4 ('status')
                      284 PRECALL                  1
                      288 CALL                     1
                      298 LOAD_CONST               5 (404)
                      300 COMPARE_OP               2 (==)
                      306 POP_JUMP_FORWARD_IF_FALSE    20 (to 348)
          
-          37         308 LOAD_GLOBAL             23 (NULL + print)
+          36         308 LOAD_GLOBAL             23 (NULL + print)
                      320 LOAD_FAST                3 (company)
                      322 FORMAT_VALUE             0
                      324 LOAD_CONST               6 (' not found')
                      326 BUILD_STRING             2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 POP_TOP
                      344 EXTENDED_ARG             1
                      346 JUMP_FORWARD           345 (to 1038)
          
-          39     >>  348 LOAD_GLOBAL             23 (NULL + print)
+          38     >>  348 LOAD_GLOBAL             23 (NULL + print)
                      360 LOAD_FAST                4 (resp)
                      362 PRECALL                  1
                      366 CALL                     1
                      376 POP_TOP
          
-          40         378 LOAD_FAST                4 (resp)
+          39         378 LOAD_FAST                4 (resp)
                      380 LOAD_METHOD             10 (get)
                      402 LOAD_CONST               7 ('name')
                      404 PRECALL                  1
                      408 CALL                     1
                      418 LOAD_FAST                3 (company)
                      420 STORE_ATTR              12 (name)
          
-          41         430 LOAD_FAST                4 (resp)
+          40         430 LOAD_FAST                4 (resp)
                      432 LOAD_METHOD             10 (get)
                      454 LOAD_CONST               8 ('description')
                      456 PRECALL                  1
                      460 CALL                     1
                      470 LOAD_FAST                3 (company)
                      472 STORE_ATTR              13 (description)
          
-          42         482 BUILD_MAP                0
+          41         482 BUILD_MAP                0
                      484 LOAD_FAST                3 (company)
                      486 LOAD_ATTR                6 (meta)
                      496 DICT_UPDATE              1
                      498 LOAD_FAST                4 (resp)
                      500 DICT_UPDATE              1
                      502 LOAD_FAST                3 (company)
                      504 STORE_ATTR               6 (meta)
          
-          43         514 LOAD_GLOBAL              1 (NULL + query)
+          42         514 LOAD_GLOBAL              1 (NULL + query)
                      526 LOAD_ATTR               14 (update_company)
                      536 LOAD_FAST                3 (company)
                      538 PRECALL                  1
                      542 CALL                     1
                      552 POP_TOP
                      554 JUMP_FORWARD           241 (to 1038)
          
-          45     >>  556 LOAD_GLOBAL             23 (NULL + print)
+          44     >>  556 LOAD_GLOBAL             23 (NULL + print)
                      568 LOAD_FAST                3 (company)
                      570 FORMAT_VALUE             0
                      572 LOAD_CONST               9 (' already enriched.')
                      574 BUILD_STRING             2
                      576 PRECALL                  1
                      580 CALL                     1
                      590 POP_TOP
                      592 JUMP_FORWARD           222 (to 1038)
          
-          47     >>  594 LOAD_FAST                1 (e)
+          46     >>  594 LOAD_FAST                1 (e)
                      596 LOAD_ATTR                3 (type)
                      606 LOAD_CONST              10 ('validate')
                      608 COMPARE_OP               2 (==)
                      614 POP_JUMP_FORWARD_IF_FALSE    71 (to 758)
          
-          48         616 LOAD_GLOBAL              1 (NULL + query)
+          47         616 LOAD_GLOBAL              1 (NULL + query)
                      628 LOAD_ATTR               15 (find_search_by_uid)
                      638 LOAD_FAST                2 (search_uid)
                      640 PRECALL                  1
                      644 CALL                     1
                      654 STORE_FAST               5 (search)
          
-          49         656 LOAD_GLOBAL             17 (NULL + grata)
+          48         656 LOAD_GLOBAL             17 (NULL + grata)
                      668 LOAD_ATTR               16 (find_similar)
                      678 LOAD_FAST                1 (e)
                      680 LOAD_ATTR                5 (domain)
                      690 LOAD_FAST                5 (search)
                      692 KW_NAMES                11
                      694 PRECALL                  2
                      698 CALL                     2
                      708 STORE_FAST               6 (grata_companies)
          
-          50         710 LOAD_GLOBAL              1 (NULL + query)
+          49         710 LOAD_GLOBAL              1 (NULL + query)
                      722 LOAD_ATTR               17 (insert_companies_as_targets)
          
-          51         732 LOAD_FAST                6 (grata_companies)
+          50         732 LOAD_FAST                6 (grata_companies)
                      734 LOAD_FAST                2 (search_uid)
                      736 LOAD_CONST              12 ('grata')
          
-          50         738 KW_NAMES                13
+          49         738 KW_NAMES                13
                      740 PRECALL                  3
                      744 CALL                     3
                      754 POP_TOP
                      756 JUMP_FORWARD           140 (to 1038)
          
-          54     >>  758 LOAD_FAST                1 (e)
+          53     >>  758 LOAD_FAST                1 (e)
                      760 LOAD_ATTR                3 (type)
                      770 LOAD_CONST              14 ('send')
                      772 COMPARE_OP               2 (==)
                      778 POP_JUMP_FORWARD_IF_FALSE     1 (to 782)
          
-          55         780 JUMP_FORWARD           128 (to 1038)
+          54         780 JUMP_FORWARD           128 (to 1038)
          
-          56     >>  782 LOAD_FAST                1 (e)
+          55     >>  782 LOAD_FAST                1 (e)
                      784 LOAD_ATTR                3 (type)
                      794 LOAD_CONST              15 ('accept')
                      796 COMPARE_OP               2 (==)
                      802 POP_JUMP_FORWARD_IF_FALSE     1 (to 806)
          
-          57         804 JUMP_FORWARD           116 (to 1038)
+          56         804 JUMP_FORWARD           116 (to 1038)
          
-          58     >>  806 LOAD_FAST                1 (e)
+          57     >>  806 LOAD_FAST                1 (e)
                      808 LOAD_ATTR                3 (type)
                      818 LOAD_CONST              16 ('reject')
                      820 COMPARE_OP               2 (==)
                      826 POP_JUMP_FORWARD_IF_FALSE     1 (to 830)
          
-          59         828 JUMP_FORWARD           104 (to 1038)
+          58         828 JUMP_FORWARD           104 (to 1038)
          
-          60     >>  830 LOAD_FAST                1 (e)
+          59     >>  830 LOAD_FAST                1 (e)
                      832 LOAD_ATTR                3 (type)
                      842 LOAD_CONST              17 ('conflict')
                      844 COMPARE_OP               2 (==)
                      850 POP_JUMP_FORWARD_IF_FALSE     1 (to 854)
          
-          61         852 JUMP_FORWARD            92 (to 1038)
+          60         852 JUMP_FORWARD            92 (to 1038)
          
-          62     >>  854 LOAD_FAST                1 (e)
+          61     >>  854 LOAD_FAST                1 (e)
                      856 LOAD_ATTR                3 (type)
                      866 LOAD_CONST              18 ('criteria')
                      868 COMPARE_OP               2 (==)
                      874 POP_JUMP_FORWARD_IF_FALSE    81 (to 1038)
          
-          63         876 LOAD_GLOBAL             23 (NULL + print)
+          62         876 LOAD_GLOBAL             23 (NULL + print)
                      888 LOAD_CONST              19 ('criteria search for ')
                      890 LOAD_FAST                2 (search_uid)
                      892 FORMAT_VALUE             0
                      894 BUILD_STRING             2
                      896 PRECALL                  1
                      900 CALL                     1
                      910 POP_TOP
          
-          64         912 LOAD_GLOBAL              1 (NULL + query)
+          63         912 LOAD_GLOBAL              1 (NULL + query)
                      924 LOAD_ATTR               15 (find_search_by_uid)
                      934 LOAD_FAST                2 (search_uid)
                      936 PRECALL                  1
                      940 CALL                     1
                      950 STORE_FAST               5 (search)
          
-          65         952 LOAD_GLOBAL             17 (NULL + grata)
+          64         952 LOAD_GLOBAL             17 (NULL + grata)
                      964 LOAD_ATTR               18 (find_by_criteria)
                      974 LOAD_FAST                5 (search)
                      976 PRECALL                  1
                      980 CALL                     1
                      990 STORE_FAST               6 (grata_companies)
          
-          66         992 LOAD_GLOBAL              1 (NULL + query)
+          65         992 LOAD_GLOBAL              1 (NULL + query)
                     1004 LOAD_ATTR               17 (insert_companies_as_targets)
          
-          67        1014 LOAD_FAST                6 (grata_companies)
+          66        1014 LOAD_FAST                6 (grata_companies)
                     1016 LOAD_FAST                2 (search_uid)
                     1018 LOAD_CONST              12 ('grata')
          
-          66        1020 KW_NAMES                13
+          65        1020 KW_NAMES                13
                     1022 PRECALL                  3
                     1026 CALL                     3
                     1036 POP_TOP
          
-          72     >> 1038 LOAD_GLOBAL              1 (NULL + query)
+          71     >> 1038 LOAD_GLOBAL              1 (NULL + query)
                     1050 LOAD_ATTR               19 (insert_checkpoint)
                     1060 LOAD_GLOBAL             41 (NULL + Checkpoint)
                     1072 LOAD_FAST                1 (e)
                     1074 LOAD_ATTR               21 (id)
                     1084 KW_NAMES                20
                     1086 PRECALL                  1
                     1090 CALL                     1
                     1100 PRECALL                  1
                     1104 CALL                     1
                     1114 POP_TOP
          
-          73        1116 LOAD_GLOBAL             23 (NULL + print)
+          72        1116 LOAD_GLOBAL             23 (NULL + print)
                     1128 LOAD_CONST              21 ('processed: ')
                     1130 LOAD_FAST                1 (e)
                     1132 FORMAT_VALUE             0
                     1134 BUILD_STRING             2
                     1136 PRECALL                  1
                     1140 CALL                     1
                     1150 POP_TOP
@@ -431,15 +431,15 @@
          varnames   ('event_id', 'e', 'search_uid', 'company', 'resp', 'search', 'grata_companies')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
          firstlineno 13
          lnotab
-            0x020628010e02160104011602320336063201320128021e013401340120
+            0x020628010e02160104011602320336053201320128021e013401340120
             012a022602160128013601160106ff140416010201160102011601020116
             0102011601240128012801160106ff12064e01
       'search_uid'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
@@ -456,33 +456,33 @@
             00ab0100000000000000007a0a0000a6010000ab0100000000000000007d
             03740d000000000000000000006404ac05a6010000ab0100000000000000
             0035007d047c04a007000000000000000000000000000000000000000074
             10000000000000000000007c03a6020000ab020000000000000000010064
             0664066406a6020000ab02000000000000000001006e0b23003100730477
             0278035900770101005900010001007413000000000000000000007c03a6
             010000ab0100000000000000005300
-          76           0 RESUME                   0
+          75           0 RESUME                   0
          
-          81           2 LOAD_GLOBAL              1 (NULL + query)
+          80           2 LOAD_GLOBAL              1 (NULL + query)
                       14 LOAD_ATTR                1 (event)
                       24 LOAD_FAST                0 (search_uid)
                       26 KW_NAMES                 1
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_FAST               1 (events)
          
-          82          44 LOAD_GLOBAL              1 (NULL + query)
+          81          44 LOAD_GLOBAL              1 (NULL + query)
                       56 LOAD_ATTR                2 (checkpoint)
                       66 LOAD_FAST                0 (search_uid)
                       68 KW_NAMES                 1
                       70 PRECALL                  1
                       74 CALL                     1
                       84 STORE_FAST               2 (checkpoints)
          
-          84          86 LOAD_GLOBAL              7 (NULL + list)
+          83          86 LOAD_GLOBAL              7 (NULL + list)
                       98 LOAD_GLOBAL              9 (NULL + set)
                      110 LOAD_FAST                1 (events)
                      112 LOAD_CONST               2 ('id')
                      114 BINARY_SUBSCR
                      124 LOAD_METHOD              5 (tolist)
                      146 PRECALL                  0
                      150 CALL                     0
@@ -498,31 +498,31 @@
                      236 PRECALL                  1
                      240 CALL                     1
                      250 BINARY_OP               10 (-)
                      254 PRECALL                  1
                      258 CALL                     1
                      268 STORE_FAST               3 (q)
          
-          91         270 LOAD_GLOBAL             13 (NULL + ThreadPoolExecutor)
+          90         270 LOAD_GLOBAL             13 (NULL + ThreadPoolExecutor)
                      282 LOAD_CONST               4 (4)
                      284 KW_NAMES                 5
                      286 PRECALL                  1
                      290 CALL                     1
                      300 BEFORE_WITH
                      302 STORE_FAST               4 (executor)
          
-          92         304 LOAD_FAST                4 (executor)
+          91         304 LOAD_FAST                4 (executor)
                      306 LOAD_METHOD              7 (map)
                      328 LOAD_GLOBAL             16 (process_event)
                      340 LOAD_FAST                3 (q)
                      342 PRECALL                  2
                      346 CALL                     2
                      356 POP_TOP
          
-          91         358 LOAD_CONST               6 (None)
+          90         358 LOAD_CONST               6 (None)
                      360 LOAD_CONST               6 (None)
                      362 LOAD_CONST               6 (None)
                      364 PRECALL                  2
                      368 CALL                     2
                      378 POP_TOP
                      380 JUMP_FORWARD            11 (to 404)
                  >>  382 PUSH_EXC_INFO
@@ -533,15 +533,15 @@
                      392 POP_EXCEPT
                      394 RERAISE                  1
                  >>  396 POP_TOP
                      398 POP_EXCEPT
                      400 POP_TOP
                      402 POP_TOP
          
-          94     >>  404 LOAD_GLOBAL             19 (NULL + len)
+          93     >>  404 LOAD_GLOBAL             19 (NULL + len)
                      416 LOAD_FAST                3 (q)
                      418 PRECALL                  1
                      422 CALL                     1
                      432 RETURN_VALUE
          ExceptionTable:
            302 to 356 -> 382 [1] lasti
            382 to 388 -> 390 [3] lasti
@@ -556,17 +556,17 @@
             None
          names      ('query', 'event', 'checkpoint', 'list', 'set', 'tolist', 'ThreadPoolExecutor', 'map', 'process_event', 'len')
          varnames   ('search_uid', 'events', 'checkpoints', 'q', 'executor')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_events'
-         firstlineno 76
+         firstlineno 75
          lnotab 0x02052a012a02b807220136ff2e03
    names      ('concurrent.futures', 'ThreadPoolExecutor', 'dataclasses', 'dataclass', 'field', 'time', 'pandas', 'pd', 'dacite', 'from_dict', 'gandai', 'query', 'gandai.models', 'Checkpoint', 'Company', 'Event', 'gandai.sources', 'GrataWrapper', 'grata', 'int', 'process_event', 'process_events')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c0110010c0208010c020c0114010c03103f
+   lnotab 0x00ff02010c0110010c0208010c020c0114010c03103e
```

### Comparing `gandai-1.3.8/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd710c864 (Mon Jul 31 19:51:51 2023 UTC)
-files sz: 22049
+moddate:  0xa424c864 (Mon Jul 31 21:16:20 2023 UTC)
+files sz: 22050
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
```

### Comparing `gandai-1.3.8/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.3.9/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,62 +1,62 @@
 magic:    0xa70d0d0a
-moddate:  0xd605c864 (Mon Jul 31 19:04:54 2023 UTC)
-files sz: 11690
+moddate:  0xa424c864 (Mon Jul 31 21:16:20 2023 UTC)
+files sz: 11625
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a02640064026c036d045a0401
-      00640064036c056d065a060100640064046c076d085a080100640064016c
-      095a09640064016c0a5a0a640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d
-      0f5a0f6d105a100100640064066c116d125a120100020065096a13000000
+      0x9700640064016c005a00640064026c016d025a020100640064036c036d
+      045a040100640064046c056d065a060100640064016c075a07640064016c
+      085a09640064016c0a5a0a640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d
+      0f5a0f6d105a100100640064066c116d125a120100020065076a13000000
       0000000000020065106a1400000000000000006407a6010000ab01000000
       0000000000ac08a6010000ab0100000000000000005a1564095a16020047
       00640a8400640ba6020000ab0200000000000000005a1702004700640c84
       00640da6020000ab0200000000000000005a1802004700640e8400640fa6
       020000ab0200000000000000005a1964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (time)
                  8 STORE_NAME               0 (time)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (pandas)
-                16 STORE_NAME               2 (pd)
+                12 LOAD_CONST               2 (('ThreadPoolExecutor',))
+                14 IMPORT_NAME              1 (concurrent.futures)
+                16 IMPORT_FROM              2 (ThreadPoolExecutor)
+                18 STORE_NAME               2 (ThreadPoolExecutor)
+                20 POP_TOP
    
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('ThreadPoolExecutor',))
-                22 IMPORT_NAME              3 (concurrent.futures)
-                24 IMPORT_FROM              4 (ThreadPoolExecutor)
-                26 STORE_NAME               4 (ThreadPoolExecutor)
-                28 POP_TOP
+     3          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('partial',))
+                26 IMPORT_NAME              3 (functools)
+                28 IMPORT_FROM              4 (partial)
+                30 STORE_NAME               4 (partial)
+                32 POP_TOP
    
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('partial',))
-                34 IMPORT_NAME              5 (functools)
-                36 IMPORT_FROM              6 (partial)
-                38 STORE_NAME               6 (partial)
-                40 POP_TOP
+     4          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               4 (('List',))
+                38 IMPORT_NAME              5 (typing)
+                40 IMPORT_FROM              6 (List)
+                42 STORE_NAME               6 (List)
+                44 POP_TOP
    
-     5          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('List',))
-                46 IMPORT_NAME              7 (typing)
-                48 IMPORT_FROM              8 (List)
-                50 STORE_NAME               8 (List)
-                52 POP_TOP
+     6          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               1 (None)
+                50 IMPORT_NAME              7 (googlemaps)
+                52 STORE_NAME               7 (googlemaps)
    
      7          54 LOAD_CONST               0 (0)
                 56 LOAD_CONST               1 (None)
-                58 IMPORT_NAME              9 (googlemaps)
-                60 STORE_NAME               9 (googlemaps)
+                58 IMPORT_NAME              8 (pandas)
+                60 STORE_NAME               9 (pd)
    
      8          62 LOAD_CONST               0 (0)
                 64 LOAD_CONST               1 (None)
                 66 IMPORT_NAME             10 (requests)
                 68 STORE_NAME              10 (requests)
    
     10          70 LOAD_CONST               0 (0)
@@ -78,15 +78,15 @@
                100 LOAD_CONST               6 (('Search',))
                102 IMPORT_NAME             17 (gandai.models)
                104 IMPORT_FROM             18 (Search)
                106 STORE_NAME              18 (Search)
                108 POP_TOP
    
     13         110 PUSH_NULL
-               112 LOAD_NAME                9 (googlemaps)
+               112 LOAD_NAME                7 (googlemaps)
                114 LOAD_ATTR               19 (Client)
                124 PUSH_NULL
                126 LOAD_NAME               16 (secrets)
                128 LOAD_ATTR               20 (access_secret_version)
                138 LOAD_CONST               7 ('GOOLE_MAPS_KEY')
                140 PRECALL                  1
                144 CALL                     1
@@ -112,17 +112,17 @@
                206 LOAD_CONST              12 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 173>)
                208 MAKE_FUNCTION            0
                210 LOAD_CONST              13 ('GrataWrapper')
                212 PRECALL                  2
                216 CALL                     2
                226 STORE_NAME              24 (GrataWrapper)
    
-   345         228 PUSH_NULL
+   343         228 PUSH_NULL
                230 LOAD_BUILD_CLASS
-               232 LOAD_CONST              14 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 345>)
+               232 LOAD_CONST              14 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 343>)
                234 MAKE_FUNCTION            0
                236 LOAD_CONST              15 ('SourceScrubWrapper')
                238 PRECALL                  2
                242 CALL                     2
                252 STORE_NAME              25 (SourceScrubWrapper)
                254 LOAD_CONST               1 (None)
                256 RETURN_VALUE
@@ -1342,21 +1342,21 @@
                      134 LOAD_CONST               6 ('return')
                      136 LOAD_CONST              11 (None)
                      138 BUILD_TUPLE              4
                      140 LOAD_CONST              12 (<code object enrich_targets_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 223>)
                      142 MAKE_FUNCTION            4 (annotations)
                      144 STORE_NAME              16 (enrich_targets_async)
          
-         238         146 LOAD_CONST               5 ('search')
+         236         146 LOAD_CONST               5 ('search')
                      148 LOAD_NAME                7 (models)
                      150 LOAD_ATTR                8 (Search)
                      160 LOAD_CONST               6 ('return')
                      162 LOAD_NAME               11 (dict)
                      164 BUILD_TUPLE              4
-                     166 LOAD_CONST              13 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 238>)
+                     166 LOAD_CONST              13 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 236>)
                      168 MAKE_FUNCTION            4 (annotations)
                      170 STORE_NAME              17 (_get_api_filter)
                      172 LOAD_CONST              11 (None)
                      174 RETURN_VALUE
          consts
             'GrataWrapper'
             'GRATA_API_TOKEN'
@@ -1727,24 +1727,22 @@
                                  290 PRECALL                  1
                                  294 CALL                     1
                                  304 BEFORE_WITH
                                  306 STORE_FAST               3 (executor)
                      
                      234         308 LOAD_FAST                3 (executor)
                                  310 LOAD_METHOD             10 (map)
-                     
-                     235         332 LOAD_DEREF               4 (enrich_company_by_domain)
+                                 332 LOAD_DEREF               4 (enrich_company_by_domain)
                                  334 LOAD_DEREF               5 (targets)
                                  336 LOAD_CONST               5 ('domain')
                                  338 BINARY_SUBSCR
                                  348 LOAD_METHOD             11 (tolist)
                                  370 PRECALL                  0
                                  374 CALL                     0
-                     
-                     234         384 PRECALL                  2
+                                 384 PRECALL                  2
                                  388 CALL                     2
                                  398 POP_TOP
                      
                      233         400 LOAD_CONST               0 (None)
                                  402 LOAD_CONST               0 (None)
                                  404 LOAD_CONST               0 (None)
                                  406 PRECALL                  2
@@ -1779,15 +1777,15 @@
                      names      ('query', 'find_company_by_domain', 'meta', 'keys', 'GrataWrapper', 'enrich', 'get', 'description', 'update_company', 'ThreadPoolExecutor', 'map', 'tolist')
                      varnames   ('domain', 'company', 'resp', 'executor')
                      freevars   ('enrich_company_by_domain', 'targets')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       'enrich_company_by_domain'
                      firstlineno 224
-                     lnotab 0x04012801360234013401200128022201180134ff10ff
+                     lnotab 0x040128013602340134012001280222015cff
                names      ('str',)
                varnames   ('targets',)
                freevars   ()
                cellvars   ('targets', 'enrich_company_by_domain')
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich_targets_async'
                firstlineno 223
@@ -1820,356 +1818,356 @@
                   00000000000000000000000000000064706471a6020000ab020000000000
                   00000002007c01a6000000ab00000000000000000002007c02a6000000ab
                   00000000000000000064729c0264739c065300
                              0 MAKE_CELL                0 (search)
                              2 MAKE_CELL                3 (COUNTRIES)
                              4 MAKE_CELL                4 (STATES)
                
-               238           6 RESUME                   0
+               236           6 RESUME                   0
                
-               239           8 BUILD_MAP                0
+               237           8 BUILD_MAP                0
                
-               240          10 LOAD_CONST               1 ('AL')
+               238          10 LOAD_CONST               1 ('AL')
                             12 LOAD_CONST               2 ('Alabama')
                
-               239          14 MAP_ADD                  1
+               237          14 MAP_ADD                  1
                
-               241          16 LOAD_CONST               3 ('AK')
+               239          16 LOAD_CONST               3 ('AK')
                             18 LOAD_CONST               4 ('Alaska')
                
-               239          20 MAP_ADD                  1
+               237          20 MAP_ADD                  1
                
-               242          22 LOAD_CONST               5 ('AZ')
+               240          22 LOAD_CONST               5 ('AZ')
                             24 LOAD_CONST               6 ('Arizona')
                
-               239          26 MAP_ADD                  1
+               237          26 MAP_ADD                  1
                
-               243          28 LOAD_CONST               7 ('AR')
+               241          28 LOAD_CONST               7 ('AR')
                             30 LOAD_CONST               8 ('Arkansas')
                
-               239          32 MAP_ADD                  1
+               237          32 MAP_ADD                  1
                
-               244          34 LOAD_CONST               9 ('CA')
+               242          34 LOAD_CONST               9 ('CA')
                             36 LOAD_CONST              10 ('California')
                
-               239          38 MAP_ADD                  1
+               237          38 MAP_ADD                  1
                
-               245          40 LOAD_CONST              11 ('CO')
+               243          40 LOAD_CONST              11 ('CO')
                             42 LOAD_CONST              12 ('Colorado')
                
-               239          44 MAP_ADD                  1
+               237          44 MAP_ADD                  1
                
-               246          46 LOAD_CONST              13 ('CT')
+               244          46 LOAD_CONST              13 ('CT')
                             48 LOAD_CONST              14 ('Connecticut')
                
-               239          50 MAP_ADD                  1
+               237          50 MAP_ADD                  1
                
-               247          52 LOAD_CONST              15 ('DE')
+               245          52 LOAD_CONST              15 ('DE')
                             54 LOAD_CONST              16 ('Delaware')
                
-               239          56 MAP_ADD                  1
+               237          56 MAP_ADD                  1
                
-               248          58 LOAD_CONST              17 ('FL')
+               246          58 LOAD_CONST              17 ('FL')
                             60 LOAD_CONST              18 ('Florida')
                
-               239          62 MAP_ADD                  1
+               237          62 MAP_ADD                  1
                
-               249          64 LOAD_CONST              19 ('GA')
+               247          64 LOAD_CONST              19 ('GA')
                             66 LOAD_CONST              20 ('Georgia')
                
-               239          68 MAP_ADD                  1
+               237          68 MAP_ADD                  1
                
-               250          70 LOAD_CONST              21 ('HI')
+               248          70 LOAD_CONST              21 ('HI')
                             72 LOAD_CONST              22 ('Hawaii')
                
-               239          74 MAP_ADD                  1
+               237          74 MAP_ADD                  1
                
-               251          76 LOAD_CONST              23 ('ID')
+               249          76 LOAD_CONST              23 ('ID')
                             78 LOAD_CONST              24 ('Idaho')
                
-               239          80 MAP_ADD                  1
+               237          80 MAP_ADD                  1
                
-               252          82 LOAD_CONST              25 ('IL')
+               250          82 LOAD_CONST              25 ('IL')
                             84 LOAD_CONST              26 ('Illinois')
                
-               239          86 MAP_ADD                  1
+               237          86 MAP_ADD                  1
                
-               253          88 LOAD_CONST              27 ('IN')
+               251          88 LOAD_CONST              27 ('IN')
                             90 LOAD_CONST              28 ('Indiana')
                
-               239          92 MAP_ADD                  1
+               237          92 MAP_ADD                  1
                
-               254          94 LOAD_CONST              29 ('IA')
+               252          94 LOAD_CONST              29 ('IA')
                             96 LOAD_CONST              30 ('Iowa')
                
-               239          98 MAP_ADD                  1
+               237          98 MAP_ADD                  1
                
-               255         100 LOAD_CONST              31 ('KS')
+               253         100 LOAD_CONST              31 ('KS')
                            102 LOAD_CONST              32 ('Kansas')
                
-               239         104 MAP_ADD                  1
+               237         104 MAP_ADD                  1
                
-               256         106 LOAD_CONST              33 ('KY')
+               254         106 LOAD_CONST              33 ('KY')
                            108 LOAD_CONST              34 ('Kentucky')
                
-               239         110 MAP_ADD                  1
+               237         110 MAP_ADD                  1
                            112 BUILD_MAP                0
                
-               257         114 LOAD_CONST              35 ('LA')
+               255         114 LOAD_CONST              35 ('LA')
                            116 LOAD_CONST              36 ('Louisiana')
                
-               239         118 MAP_ADD                  1
+               237         118 MAP_ADD                  1
                
-               258         120 LOAD_CONST              37 ('ME')
+               256         120 LOAD_CONST              37 ('ME')
                            122 LOAD_CONST              38 ('Maine')
                
-               239         124 MAP_ADD                  1
+               237         124 MAP_ADD                  1
                
-               259         126 LOAD_CONST              39 ('MD')
+               257         126 LOAD_CONST              39 ('MD')
                            128 LOAD_CONST              40 ('Maryland')
                
-               239         130 MAP_ADD                  1
+               237         130 MAP_ADD                  1
                
-               260         132 LOAD_CONST              41 ('MA')
+               258         132 LOAD_CONST              41 ('MA')
                            134 LOAD_CONST              42 ('Massachusetts')
                
-               239         136 MAP_ADD                  1
+               237         136 MAP_ADD                  1
                
-               261         138 LOAD_CONST              43 ('MI')
+               259         138 LOAD_CONST              43 ('MI')
                            140 LOAD_CONST              44 ('Michigan')
                
-               239         142 MAP_ADD                  1
+               237         142 MAP_ADD                  1
                
-               262         144 LOAD_CONST              45 ('MN')
+               260         144 LOAD_CONST              45 ('MN')
                            146 LOAD_CONST              46 ('Minnesota')
                
-               239         148 MAP_ADD                  1
+               237         148 MAP_ADD                  1
                
-               263         150 LOAD_CONST              47 ('MS')
+               261         150 LOAD_CONST              47 ('MS')
                            152 LOAD_CONST              48 ('Mississippi')
                
-               239         154 MAP_ADD                  1
+               237         154 MAP_ADD                  1
                
-               264         156 LOAD_CONST              49 ('MO')
+               262         156 LOAD_CONST              49 ('MO')
                            158 LOAD_CONST              50 ('Missouri')
                
-               239         160 MAP_ADD                  1
+               237         160 MAP_ADD                  1
                
-               265         162 LOAD_CONST              51 ('MT')
+               263         162 LOAD_CONST              51 ('MT')
                            164 LOAD_CONST              52 ('Montana')
                
-               239         166 MAP_ADD                  1
+               237         166 MAP_ADD                  1
                
-               266         168 LOAD_CONST              53 ('NE')
+               264         168 LOAD_CONST              53 ('NE')
                            170 LOAD_CONST              54 ('Nebraska')
                
-               239         172 MAP_ADD                  1
+               237         172 MAP_ADD                  1
                
-               267         174 LOAD_CONST              55 ('NV')
+               265         174 LOAD_CONST              55 ('NV')
                            176 LOAD_CONST              56 ('Nevada')
                
-               239         178 MAP_ADD                  1
+               237         178 MAP_ADD                  1
                
-               268         180 LOAD_CONST              57 ('NH')
+               266         180 LOAD_CONST              57 ('NH')
                            182 LOAD_CONST              58 ('New Hampshire')
                
-               239         184 MAP_ADD                  1
+               237         184 MAP_ADD                  1
                
-               269         186 LOAD_CONST              59 ('NJ')
+               267         186 LOAD_CONST              59 ('NJ')
                            188 LOAD_CONST              60 ('New Jersey')
                
-               239         190 MAP_ADD                  1
+               237         190 MAP_ADD                  1
                
-               270         192 LOAD_CONST              61 ('NM')
+               268         192 LOAD_CONST              61 ('NM')
                            194 LOAD_CONST              62 ('New Mexico')
                
-               239         196 MAP_ADD                  1
+               237         196 MAP_ADD                  1
                
-               271         198 LOAD_CONST              63 ('NY')
+               269         198 LOAD_CONST              63 ('NY')
                            200 LOAD_CONST              64 ('New York')
                
-               239         202 MAP_ADD                  1
+               237         202 MAP_ADD                  1
                
-               272         204 LOAD_CONST              65 ('NC')
+               270         204 LOAD_CONST              65 ('NC')
                            206 LOAD_CONST              66 ('North Carolina')
                
-               239         208 MAP_ADD                  1
+               237         208 MAP_ADD                  1
                
-               273         210 LOAD_CONST              67 ('ND')
+               271         210 LOAD_CONST              67 ('ND')
                            212 LOAD_CONST              68 ('North Dakota')
                
-               239         214 MAP_ADD                  1
+               237         214 MAP_ADD                  1
                            216 DICT_UPDATE              1
                            218 BUILD_MAP                0
                
-               274         220 LOAD_CONST              69 ('OH')
+               272         220 LOAD_CONST              69 ('OH')
                            222 LOAD_CONST              70 ('Ohio')
                
-               239         224 MAP_ADD                  1
+               237         224 MAP_ADD                  1
                
-               275         226 LOAD_CONST              71 ('OK')
+               273         226 LOAD_CONST              71 ('OK')
                            228 LOAD_CONST              72 ('Oklahoma')
                
-               239         230 MAP_ADD                  1
+               237         230 MAP_ADD                  1
                
-               276         232 LOAD_CONST              73 ('OR')
+               274         232 LOAD_CONST              73 ('OR')
                            234 LOAD_CONST              74 ('Oregon')
                
-               239         236 MAP_ADD                  1
+               237         236 MAP_ADD                  1
                
-               277         238 LOAD_CONST              75 ('PA')
+               275         238 LOAD_CONST              75 ('PA')
                            240 LOAD_CONST              76 ('Pennsylvania')
                
-               239         242 MAP_ADD                  1
+               237         242 MAP_ADD                  1
                
-               278         244 LOAD_CONST              77 ('RI')
+               276         244 LOAD_CONST              77 ('RI')
                            246 LOAD_CONST              78 ('Rhode Island')
                
-               239         248 MAP_ADD                  1
+               237         248 MAP_ADD                  1
                
-               279         250 LOAD_CONST              79 ('SC')
+               277         250 LOAD_CONST              79 ('SC')
                            252 LOAD_CONST              80 ('South Carolina')
                
-               239         254 MAP_ADD                  1
+               237         254 MAP_ADD                  1
                
-               280         256 LOAD_CONST              81 ('SD')
+               278         256 LOAD_CONST              81 ('SD')
                            258 LOAD_CONST              82 ('South Dakota')
                
-               239         260 MAP_ADD                  1
+               237         260 MAP_ADD                  1
                
-               281         262 LOAD_CONST              83 ('TN')
+               279         262 LOAD_CONST              83 ('TN')
                            264 LOAD_CONST              84 ('Tennessee')
                
-               239         266 MAP_ADD                  1
+               237         266 MAP_ADD                  1
                
-               282         268 LOAD_CONST              85 ('TX')
+               280         268 LOAD_CONST              85 ('TX')
                            270 LOAD_CONST              86 ('Texas')
                
-               239         272 MAP_ADD                  1
+               237         272 MAP_ADD                  1
                
-               283         274 LOAD_CONST              87 ('UT')
+               281         274 LOAD_CONST              87 ('UT')
                            276 LOAD_CONST              88 ('Utah')
                
-               239         278 MAP_ADD                  1
+               237         278 MAP_ADD                  1
                
-               284         280 LOAD_CONST              89 ('VT')
+               282         280 LOAD_CONST              89 ('VT')
                            282 LOAD_CONST              90 ('Vermont')
                
-               239         284 MAP_ADD                  1
+               237         284 MAP_ADD                  1
                
-               285         286 LOAD_CONST              91 ('VA')
+               283         286 LOAD_CONST              91 ('VA')
                            288 LOAD_CONST              92 ('Virginia')
                
-               239         290 MAP_ADD                  1
+               237         290 MAP_ADD                  1
                
-               286         292 LOAD_CONST              93 ('WA')
+               284         292 LOAD_CONST              93 ('WA')
                            294 LOAD_CONST              94 ('Washington')
                
-               239         296 MAP_ADD                  1
+               237         296 MAP_ADD                  1
                
-               287         298 LOAD_CONST              95 ('WV')
+               285         298 LOAD_CONST              95 ('WV')
                            300 LOAD_CONST              96 ('West Virginia')
                
-               239         302 MAP_ADD                  1
+               237         302 MAP_ADD                  1
                
-               288         304 LOAD_CONST              97 ('WI')
+               286         304 LOAD_CONST              97 ('WI')
                            306 LOAD_CONST              98 ('Wisconsin')
                
-               239         308 MAP_ADD                  1
+               237         308 MAP_ADD                  1
                
-               289         310 LOAD_CONST              99 ('WY')
+               287         310 LOAD_CONST              99 ('WY')
                            312 LOAD_CONST             100 ('Wyoming')
                
-               239         314 MAP_ADD                  1
+               237         314 MAP_ADD                  1
                            316 DICT_UPDATE              1
                            318 STORE_DEREF              4 (STATES)
                
-               293         320 LOAD_CONST             101 ('United States')
+               291         320 LOAD_CONST             101 ('United States')
                
-               294         322 LOAD_CONST             102 ('Canada')
+               292         322 LOAD_CONST             102 ('Canada')
                
-               295         324 LOAD_CONST             103 ('Mexico')
+               293         324 LOAD_CONST             103 ('Mexico')
                
-               296         326 LOAD_CONST             104 ('United Kingdom')
+               294         326 LOAD_CONST             104 ('United Kingdom')
                
-               292         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
+               290         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
                            330 BUILD_CONST_KEY_MAP      4
                            332 STORE_DEREF              3 (COUNTRIES)
                
-               299         334 LOAD_CONST             106 ('return')
+               297         334 LOAD_CONST             106 ('return')
                            336 LOAD_GLOBAL              0 (list)
                            348 BUILD_TUPLE              2
                            350 LOAD_CLOSURE             3 (COUNTRIES)
                            352 LOAD_CLOSURE             4 (STATES)
                            354 LOAD_CLOSURE             0 (search)
                            356 BUILD_TUPLE              3
-                           358 LOAD_CONST             107 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 299>)
+                           358 LOAD_CONST             107 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 297>)
                            360 MAKE_FUNCTION           12 (annotations, closure)
                            362 STORE_FAST               1 (_hq_include)
                
-               324         364 LOAD_CONST             106 ('return')
+               322         364 LOAD_CONST             106 ('return')
                            366 LOAD_GLOBAL              0 (list)
                            378 BUILD_TUPLE              2
                            380 LOAD_CLOSURE             4 (STATES)
                            382 LOAD_CLOSURE             0 (search)
                            384 BUILD_TUPLE              2
-                           386 LOAD_CONST             108 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 324>)
+                           386 LOAD_CONST             108 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 322>)
                            388 MAKE_FUNCTION           12 (annotations, closure)
                            390 STORE_FAST               2 (_hq_exclude)
                
-               331         392 LOAD_CONST             109 ('any')
+               329         392 LOAD_CONST             109 ('any')
                
-               332         394 LOAD_DEREF               0 (search)
+               330         394 LOAD_DEREF               0 (search)
                            396 LOAD_ATTR                1 (inclusion)
                            406 LOAD_METHOD              2 (get)
                            428 LOAD_CONST             110 ('keywords')
                            430 BUILD_LIST               0
                            432 PRECALL                  2
                            436 CALL                     2
                
-               333         446 LOAD_DEREF               0 (search)
+               331         446 LOAD_DEREF               0 (search)
                            448 LOAD_ATTR                3 (exclusion)
                            458 LOAD_METHOD              2 (get)
                            480 LOAD_CONST             110 ('keywords')
                            482 BUILD_LIST               0
                            484 PRECALL                  2
                            488 CALL                     2
                
-               334         498 LOAD_DEREF               0 (search)
+               332         498 LOAD_DEREF               0 (search)
                            500 LOAD_ATTR                1 (inclusion)
                            510 LOAD_METHOD              2 (get)
                
-               335         532 LOAD_CONST             111 ('employees_range')
+               333         532 LOAD_CONST             111 ('employees_range')
                            534 BUILD_LIST               0
                
-               334         536 PRECALL                  2
+               332         536 PRECALL                  2
                            540 CALL                     2
                
-               337         550 LOAD_DEREF               0 (search)
+               335         550 LOAD_DEREF               0 (search)
                            552 LOAD_ATTR                1 (inclusion)
                            562 LOAD_METHOD              2 (get)
                            584 LOAD_CONST             112 ('ownership')
                            586 LOAD_CONST             113 ('')
                            588 PRECALL                  2
                            592 CALL                     2
                
-               339         602 PUSH_NULL
+               337         602 PUSH_NULL
                            604 LOAD_FAST                1 (_hq_include)
                            606 PRECALL                  0
                            610 CALL                     0
                
-               340         620 PUSH_NULL
+               338         620 PUSH_NULL
                            622 LOAD_FAST                2 (_hq_exclude)
                            624 PRECALL                  0
                            628 CALL                     0
                
-               338         638 LOAD_CONST             114 (('include', 'exclude'))
+               336         638 LOAD_CONST             114 (('include', 'exclude'))
                            640 BUILD_CONST_KEY_MAP      2
                
-               330         642 LOAD_CONST             115 (('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters'))
+               328         642 LOAD_CONST             115 (('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters'))
                            644 BUILD_CONST_KEY_MAP      6
                            646 RETURN_VALUE
                consts
                   None
                   'AL'
                   'Alabama'
                   'AK'
@@ -2298,134 +2296,134 @@
                         010000ab01000000000000000001008c207405000000000000000000007c
                         03a6010000ab01000000000000000064046b040000000072227c0344005d
                         1f7d067c00a0030000000000000000000000000000000000000000640389
                         077c06190000000000000000006901a6010000ab01000000000000000001
                         008c207c005300
                                    0 COPY_FREE_VARS           3
                      
-                     299           2 RESUME                   0
+                     297           2 RESUME                   0
                      
-                     300           4 BUILD_LIST               0
+                     298           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (include)
                      
-                     301           8 LOAD_DEREF               9 (search)
+                     299           8 LOAD_DEREF               9 (search)
                                   10 LOAD_ATTR                0 (inclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('city')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 STORE_FAST               1 (cities)
                      
-                     302          62 LOAD_DEREF               9 (search)
+                     300          62 LOAD_DEREF               9 (search)
                                   64 LOAD_ATTR                0 (inclusion)
                                   74 LOAD_METHOD              1 (get)
                                   96 LOAD_CONST               2 ('state')
                                   98 BUILD_LIST               0
                                  100 PRECALL                  2
                                  104 CALL                     2
                                  114 STORE_FAST               2 (states)
                      
-                     303         116 LOAD_DEREF               9 (search)
+                     301         116 LOAD_DEREF               9 (search)
                                  118 LOAD_ATTR                0 (inclusion)
                                  128 LOAD_METHOD              1 (get)
                                  150 LOAD_CONST               3 ('country')
                                  152 BUILD_LIST               0
                                  154 PRECALL                  2
                                  158 CALL                     2
                                  168 STORE_FAST               3 (countries)
                      
-                     305         170 LOAD_GLOBAL              5 (NULL + len)
+                     303         170 LOAD_GLOBAL              5 (NULL + len)
                                  182 LOAD_FAST                1 (cities)
                                  184 PRECALL                  1
                                  188 CALL                     1
                                  198 LOAD_CONST               4 (0)
                                  200 COMPARE_OP               4 (>)
                                  206 POP_JUMP_FORWARD_IF_FALSE    46 (to 300)
                      
-                     307         208 LOAD_DEREF               8 (STATES)
+                     305         208 LOAD_DEREF               8 (STATES)
                                  210 LOAD_FAST                2 (states)
                                  212 LOAD_CONST               4 (0)
                                  214 BINARY_SUBSCR
                                  224 BINARY_SUBSCR
                                  234 STORE_FAST               4 (state)
                      
-                     308         236 LOAD_FAST                1 (cities)
+                     306         236 LOAD_FAST                1 (cities)
                                  238 GET_ITER
                              >>  240 FOR_ITER                27 (to 296)
                                  242 STORE_FAST               5 (city)
                      
-                     309         244 LOAD_FAST                0 (include)
+                     307         244 LOAD_FAST                0 (include)
                                  246 LOAD_METHOD              3 (append)
                      
-                     310         268 LOAD_FAST                5 (city)
+                     308         268 LOAD_FAST                5 (city)
                                  270 LOAD_FAST                4 (state)
                                  272 LOAD_CONST               5 ('United States')
                                  274 LOAD_CONST               6 (('city', 'state', 'country'))
                                  276 BUILD_CONST_KEY_MAP      3
                      
-                     309         278 PRECALL                  1
+                     307         278 PRECALL                  1
                                  282 CALL                     1
                                  292 POP_TOP
                                  294 JUMP_BACKWARD           28 (to 240)
                      
-                     312     >>  296 LOAD_FAST                0 (include)
+                     310     >>  296 LOAD_FAST                0 (include)
                                  298 RETURN_VALUE
                      
-                     314     >>  300 LOAD_GLOBAL              5 (NULL + len)
+                     312     >>  300 LOAD_GLOBAL              5 (NULL + len)
                                  312 LOAD_FAST                2 (states)
                                  314 PRECALL                  1
                                  318 CALL                     1
                                  328 LOAD_CONST               4 (0)
                                  330 COMPARE_OP               4 (>)
                                  336 POP_JUMP_FORWARD_IF_FALSE    34 (to 406)
                      
-                     315         338 LOAD_FAST                2 (states)
+                     313         338 LOAD_FAST                2 (states)
                                  340 GET_ITER
                              >>  342 FOR_ITER                31 (to 406)
                                  344 STORE_FAST               4 (state)
                      
-                     317         346 LOAD_FAST                0 (include)
+                     315         346 LOAD_FAST                0 (include)
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
                      
-                     319     >>  406 LOAD_GLOBAL              5 (NULL + len)
+                     317     >>  406 LOAD_GLOBAL              5 (NULL + len)
                                  418 LOAD_FAST                3 (countries)
                                  420 PRECALL                  1
                                  424 CALL                     1
                                  434 LOAD_CONST               4 (0)
                                  436 COMPARE_OP               4 (>)
                                  442 POP_JUMP_FORWARD_IF_FALSE    34 (to 512)
                      
-                     320         444 LOAD_FAST                3 (countries)
+                     318         444 LOAD_FAST                3 (countries)
                                  446 GET_ITER
                              >>  448 FOR_ITER                31 (to 512)
                                  450 STORE_FAST               6 (country)
                      
-                     321         452 LOAD_FAST                0 (include)
+                     319         452 LOAD_FAST                0 (include)
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
                      
-                     322     >>  512 LOAD_FAST                0 (include)
+                     320     >>  512 LOAD_FAST                0 (include)
                                  514 RETURN_VALUE
                      consts
                         None
                         'city'
                         'state'
                         'country'
                         0
@@ -2433,15 +2431,15 @@
                         ('city', 'state', 'country')
                      names      ('inclusion', 'get', 'len', 'append')
                      varnames   ('include', 'cities', 'states', 'countries', 'state', 'city', 'country')
                      freevars   ('COUNTRIES', 'STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_include'
-                     firstlineno 299
+                     firstlineno 297
                      lnotab
                         0x0401040136013601360226021c01080118010aff12030402260108023c
                         02260108013c01
                   code
                      argcount  : 0
                      nlocals   : 2
                      stacksize : 6
@@ -2450,69 +2448,69 @@
                         0x9502970067007d0089036a000000000000000000a00100000000000000
                         0000000000000000000000000064016700a6020000ab0200000000000000
                         0044005d1f7d017c00a00200000000000000000000000000000000000000
                         00640189027c01190000000000000000006901a6010000ab010000000000
                         00000001008c207c005300
                                    0 COPY_FREE_VARS           2
                      
-                     324           2 RESUME                   0
+                     322           2 RESUME                   0
                      
-                     325           4 BUILD_LIST               0
+                     323           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (exclude)
                      
-                     326           8 LOAD_DEREF               3 (search)
+                     324           8 LOAD_DEREF               3 (search)
                                   10 LOAD_ATTR                0 (exclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                31 (to 126)
                                   64 STORE_FAST               1 (state)
                      
-                     327          66 LOAD_FAST                0 (exclude)
+                     325          66 LOAD_FAST                0 (exclude)
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
                      
-                     328     >>  126 LOAD_FAST                0 (exclude)
+                     326     >>  126 LOAD_FAST                0 (exclude)
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
-                     firstlineno 324
+                     firstlineno 322
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
-               firstlineno 238
+               firstlineno 236
                lnotab
                   0x0801020104ff020204fe020304fd020404fc020504fb020604fa020704
                   f9020804f8020904f7020a04f6020b04f5020c04f4020d04f3020e04f202
                   0f04f1021004f0021104ef041204ee021304ed021404ec021504eb021604
                   ea021704e9021804e8021904e7021a04e6021b04e5021c04e4021d04e302
                   1e04e2021f04e1022004e0022104df022204de062304dd022404dc022504
                   db022604da022704d9022804d8022904d7022a04d6022b04d5022c04d402
@@ -2521,57 +2519,57 @@
          names      ('__name__', '__module__', '__qualname__', 'secrets', 'access_secret_version', 'HEADERS', 'str', 'models', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', 'pd', 'DataFrame', 'enrich_targets_async', '_get_api_filter')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GrataWrapper'
          firstlineno 173
-         lnotab 0x0a021e0102fe06051e161a0b100b1a0f
+         lnotab 0x0a021e0102fe06051e161a0b100b1a0d
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
-         345           0 RESUME                   0
+         343           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SourceScrubWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         346          10 LOAD_CONST               1 ('domain')
+         344          10 LOAD_CONST               1 ('domain')
                       12 LOAD_NAME                3 (str)
                       14 LOAD_CONST               2 ('search')
                       16 LOAD_NAME                4 (Search)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (dict)
                       22 BUILD_TUPLE              6
-                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 346>)
+                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 344>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               6 (find_similar)
          
-         349          30 LOAD_CONST               2 ('search')
+         347          30 LOAD_CONST               2 ('search')
                       32 LOAD_NAME                4 (Search)
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                5 (dict)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 349>)
+                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 347>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (find_by_criteria)
          
-         352          46 LOAD_CONST               1 ('domain')
+         350          46 LOAD_CONST               1 ('domain')
                       48 LOAD_NAME                3 (str)
                       50 LOAD_CONST               3 ('return')
                       52 LOAD_NAME                5 (dict)
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 352>)
+                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 350>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (enrich)
                       62 LOAD_CONST               7 (None)
                       64 RETURN_VALUE
          consts
             'SourceScrubWrapper'
             'domain'
@@ -2579,81 +2577,81 @@
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               346           0 RESUME                   0
+               344           0 RESUME                   0
                
-               347           2 LOAD_CONST               0 (None)
+               345           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain', 'search')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 346
+               firstlineno 344
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               349           0 RESUME                   0
+               347           0 RESUME                   0
                
-               350           2 LOAD_CONST               0 (None)
+               348           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('search',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 349
+               firstlineno 347
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               352           0 RESUME                   0
+               350           0 RESUME                   0
                
-               353           2 LOAD_CONST               0 (None)
+               351           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 352
+               firstlineno 350
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'Search', 'dict', 'find_similar', 'find_by_criteria', 'enrich')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'SourceScrubWrapper'
-         firstlineno 345
+         firstlineno 343
          lnotab 0x0a0114031003
       'SourceScrubWrapper'
-   names      ('time', 'pandas', 'pd', 'concurrent.futures', 'ThreadPoolExecutor', 'functools', 'partial', 'typing', 'List', 'googlemaps', 'requests', 'gandai', 'gpt', 'helpers', 'models', 'query', 'secrets', 'gandai.models', 'Search', 'Client', 'access_secret_version', 'gmaps', 'MAX_WORKERS', 'GoogleMapsWrapper', 'GrataWrapper', 'SourceScrubWrapper')
+   names      ('time', 'concurrent.futures', 'ThreadPoolExecutor', 'functools', 'partial', 'typing', 'List', 'googlemaps', 'pandas', 'pd', 'requests', 'gandai', 'gpt', 'helpers', 'models', 'query', 'secrets', 'gandai.models', 'Search', 'Client', 'access_secret_version', 'gmaps', 'MAX_WORKERS', 'GoogleMapsWrapper', 'GrataWrapper', 'SourceScrubWrapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c010c010c02080108021c010c023e0104031a7f00
-      1d1a7f002d
+      0x00ff020108010c010c010c020801080108021c010c023e0104031a7f00
+      1d1a7f002b
```

### Comparing `gandai-1.3.8/gandai/analytics.py` & `gandai-1.3.9/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/auth.py` & `gandai-1.3.9/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/db.py` & `gandai-1.3.9/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/gpt.py` & `gandai-1.3.9/gandai/gpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 import openai
 import plotly.express as px
 
-from gandai import secrets, query, models
+from gandai import models, query, secrets
 
 openai.api_key = secrets.access_secret_version("OPENAI_KEY")
 
 
 def ask_gpt(prompt: str, max_tokens: int = 60):
     response = openai.Completion.create(
         engine="text-davinci-003",  # or "text-curie-003" for a less expensive engine
         prompt=prompt,
         max_tokens=max_tokens,
     )
 
     return response.choices[0].text.strip()
 
+
 def get_suggested_search_phrase(search: models.Search) -> str:
-    accepted = query.search_target_by_last_event_type(search_uid=search.uid, last_event_type="accept")
-    accepted['description'].tolist()
+    accepted = query.search_target_by_last_event_type(
+        search_uid=search.uid, last_event_type="accept"
+    )
+    accepted["description"].tolist()
     resp = ask_gpt(
         f"What search phrase would you use to search Google Maps to find companies that look like this: {accepted['description'].tolist()}",
         max_tokens=60,
     )
     return resp
 
+
 def get_top_zip_codes(area: str, top_n: int = 25) -> list:
     resp = ask_gpt(
         f"As a python array List[str], the top {top_n} zip codes in {area} are:",
         max_tokens=1000,
     )
     return eval(resp)
 
 
 def summarize_search_by(targets):
-
     px.histogram(targets, x="employees", nbins=20, height=400, width=400).show()
 
-    print(targets['ownership'].value_counts())
+    print(targets["ownership"].value_counts())
 
     GPT_PROMPT = f"""
     The top three geographic areas, based on the {[desc for desc in targets['description'].dropna().sample(20)]} are:
     """
 
     print(ask_gpt(prompt=GPT_PROMPT))
 
     GPT_PROMPT = f"""
     Give me the company type, products and services, and end markets {[desc for desc in targets['description'].dropna().sample(20)]} are:
     """
 
-    print(ask_gpt(prompt=GPT_PROMPT, max_tokens=100))
+    print(ask_gpt(prompt=GPT_PROMPT, max_tokens=100))
```

### Comparing `gandai-1.3.8/gandai/main.py` & `gandai-1.3.9/gandai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         company = query.find_company_by_domain(e.domain)
 
         # adding this check to mitigate API usage
         if "company_uid" not in company.meta.keys():
             # company uid is a grata identifier
             # where our uid maps back to dealcloud_id
             # this could just tidied up
-            
-            
+
             resp = grata.enrich(company.domain)
             if resp.get("status") == 404:
                 print(f"{company} not found")  # are we charged for "not found"?
             else:
                 print(resp)
                 company.name = resp.get("name")
                 company.description = resp.get("description")
```

### Comparing `gandai-1.3.8/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.3.9/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/migrations/db_seed.py` & `gandai-1.3.9/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/migrations/dealcloud.py` & `gandai-1.3.9/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/migrations/sql/schema.sql` & `gandai-1.3.9/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/models.py` & `gandai-1.3.9/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/query.py` & `gandai-1.3.9/gandai/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             "validate",
             "send",
             "accept",
             "reject",
             "conflict",
         ]
 
-        protected_stages = tuple(STAGES[STAGES.index(last_event_type): :])
+        protected_stages = tuple(STAGES[STAGES.index(last_event_type) : :])
 
         with db.connect() as conn:
             statement = f"""
                     SELECT distinct(domain)
                     FROM event
                     WHERE search_uid = :search_uid 
                     AND type IN {protected_stages}
```

### Comparing `gandai-1.3.8/gandai/secrets.py` & `gandai-1.3.9/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.8/gandai/sources.py` & `gandai-1.3.9/gandai/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
-import pandas as pd
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
 import googlemaps
+import pandas as pd
 import requests
 
 from gandai import gpt, helpers, models, query, secrets
 from gandai.models import Search
 
 gmaps = googlemaps.Client(key=secrets.access_secret_version("GOOLE_MAPS_KEY"))
 MAX_WORKERS = 25
@@ -175,21 +175,21 @@
         "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),
         "Content-Type": "application/json",
     }
 
     def find_similar(domain: str, search: models.Search) -> list:
         api_filters = GrataWrapper._get_api_filter(search)
         similiar_filters = {
-                "domain": domain,
-                "grata_employees_estimates_range": api_filters[
-                    "grata_employees_estimates_range"
-                ],
-                "headquarters": api_filters["headquarters"],
-                "ownership": api_filters["ownership"]
-            }
+            "domain": domain,
+            "grata_employees_estimates_range": api_filters[
+                "grata_employees_estimates_range"
+            ],
+            "headquarters": api_filters["headquarters"],
+            "ownership": api_filters["ownership"],
+        }
         print(similiar_filters)
         response = requests.post(
             "https://search.grata.com/api/v1.2/search-similar/",
             headers=GrataWrapper.HEADERS,
             json=similiar_filters,
         )
         data = response.json()
@@ -227,17 +227,15 @@
                 # print(company.name)
                 resp = GrataWrapper.enrich(domain)
                 company.description = resp.get("description")
                 company.meta = {**company.meta, **resp}  # merge 3.5+
                 query.update_company(company)
 
             with ThreadPoolExecutor(max_workers=5) as executor:
-                executor.map(
-                    enrich_company_by_domain, targets["domain"].tolist()
-                )
+                executor.map(enrich_company_by_domain, targets["domain"].tolist())
 
     def _get_api_filter(search: models.Search) -> dict:
         STATES = {
             "AL": "Alabama",
             "AK": "Alaska",
             "AZ": "Arizona",
             "AR": "Arkansas",
```

### Comparing `gandai-1.3.8/gandai.egg-info/SOURCES.txt` & `gandai-1.3.9/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

