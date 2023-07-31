# Comparing `tmp/dauth-0.5.tar.gz` & `tmp/dauth-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauth-0.5.tar", last modified: Thu Jun 29 19:46:24 2023, max compression
+gzip compressed data, was "dauth-0.6.tar", last modified: Mon Jul 31 08:23:27 2023, max compression
```

## Comparing `dauth-0.5.tar` & `dauth-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 19:46:24.090052 dauth-0.5/PKG-INFO
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2569 2023-06-21 07:35:06.000000 dauth-0.5/README.md
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)       38 2023-06-29 19:46:24.090052 dauth-0.5/setup.cfg
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      570 2023-06-29 19:38:55.000000 dauth-0.5/setup.py
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/src/
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/src/dauth/
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      187 2023-06-21 07:35:08.000000 dauth-0.5/src/dauth/__init__.py
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      903 2023-06-29 19:38:49.000000 dauth-0.5/src/dauth/auth.py
-drwxr-xr-x   0 denvilk   (1000) denvilk   (1000)        0 2023-06-29 19:46:24.090052 dauth-0.5/src/dauth.egg-info/
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)     2705 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/PKG-INFO
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)      190 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/SOURCES.txt
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)        1 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/dependency_links.txt
--rw-r--r--   0 denvilk   (1000) denvilk   (1000)        6 2023-06-29 19:46:24.000000 dauth-0.5/src/dauth.egg-info/top_level.txt
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.401097 dauth-0.6/
+-rw-r--r--   0 denvilk    (501) staff       (20)     2541 2023-07-31 08:23:27.400995 dauth-0.6/PKG-INFO
+-rw-r--r--   0 denvilk    (501) staff       (20)     2405 2023-07-31 08:18:49.000000 dauth-0.6/README.md
+-rw-r--r--   0 denvilk    (501) staff       (20)       38 2023-07-31 08:23:27.401125 dauth-0.6/setup.cfg
+-rw-r--r--   0 denvilk    (501) staff       (20)      570 2023-07-31 08:23:14.000000 dauth-0.6/setup.py
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.399860 dauth-0.6/src/
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.400265 dauth-0.6/src/dauth/
+-rw-r--r--   0 denvilk    (501) staff       (20)      187 2023-07-31 08:12:43.000000 dauth-0.6/src/dauth/__init__.py
+-rw-r--r--   0 denvilk    (501) staff       (20)      770 2023-07-31 08:15:56.000000 dauth-0.6/src/dauth/auth.py
+drwxr-xr-x   0 denvilk    (501) staff       (20)        0 2023-07-31 08:23:27.400856 dauth-0.6/src/dauth.egg-info/
+-rw-r--r--   0 denvilk    (501) staff       (20)     2541 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/PKG-INFO
+-rw-r--r--   0 denvilk    (501) staff       (20)      190 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/SOURCES.txt
+-rw-r--r--   0 denvilk    (501) staff       (20)        1 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/dependency_links.txt
+-rw-r--r--   0 denvilk    (501) staff       (20)        6 2023-07-31 08:23:27.000000 dauth-0.6/src/dauth.egg-info/top_level.txt
```

### Comparing `dauth-0.5/PKG-INFO` & `dauth-0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: dauth
-Version: 0.5
-Summary: FastAPI ABAC authorization realization
-Description-Content-Type: text/markdown
-
 # DAuth 
 
 Python FastAPI ABAC Realization.
 
 ---
 ## Getting started
 Requirements:
@@ -29,34 +23,34 @@
 Library represents function 
 ```python
 def Policy(
     subject_call: Callable, 
     resource_type: Any, 
     method: str, 
     check_callback: Callable,
-    database_callback: Union[Callable, None] = None,
-    cache_callback: Union[Callable, None] = None
+    database: Optional[Database] = None,
+    cache: Optional[Redis] = None
 )
 ```
 
 - `subject_callback` - Is function that library put in FastAPI `Depends `. Usually function returns user which tries to work with `resource`
 - `resource_type` - Is `str` which on which User tries to get access
 - `method` - Is API method by which working endpoint
 - `check_callback` - Is function that realize Policy's check. Function take arguments:
     ```python
     check_callback(subject, resource_type, item_id, method, db, cache)
     ```
 - - `subject` is result of `Depends(subject_callback)`
 - - `resource_type` is argument of `Policy()`
 - - `item_id` __(by default '*')__ is providing by FastAPI decorator `@app.get(/test/{item_id})`
 - - `method` is argument of `Policy()`
-- - `db` is database connection, result of `Depends(database_callback)`
-- - `cache` is redis connection, result of `Depends(cache_callback)`
-- `database_callback` - Is a function for getting database connecion
-- `cache_callback` - Is a function for getting Redis connection
+- - `db` is database connection
+- - `cache` is redis connection
+- `database` - Is a database connecion
+- `cache` - Is a Redis connection
 ---
 ## Examples
 Simple usage
 ```python
 from fastapi import FastAPI, Depends
 from dauth import auth
 
@@ -83,28 +77,28 @@
 # function get_database returns Databases connection
 def test_db(
     user = Depends(auth.Policy(
         get_user_auth, 
         'test', 
         'get', 
         is_admin, 
-        database_callback=get_database
+        database=Depends(get_database)
     ))
 ):
     return {"message":"Good"}
 
 @app.get("/test_with_cache")
 # function get_cache returns Redis connection
 def test_cache(
     user = Depends(auth.Policy(
         get_user_auth, 
         'test', 
         'get', 
         is_admin, 
-        cache_callback=get_cache
+        cache=Depends(get_cache)
     ))
 ):
     return {"message":"Good"}
 ```
 
 ---
 Developed by [DenVilk](https://github.com/denvilk)
```

### Comparing `dauth-0.5/README.md` & `dauth-0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: dauth
+Version: 0.6
+Summary: FastAPI ABAC authorization realization
+Description-Content-Type: text/markdown
+
 # DAuth 
 
 Python FastAPI ABAC Realization.
 
 ---
 ## Getting started
 Requirements:
@@ -23,34 +29,34 @@
 Library represents function 
 ```python
 def Policy(
     subject_call: Callable, 
     resource_type: Any, 
     method: str, 
     check_callback: Callable,
-    database_callback: Union[Callable, None] = None,
-    cache_callback: Union[Callable, None] = None
+    database: Optional[Database] = None,
+    cache: Optional[Redis] = None
 )
 ```
 
 - `subject_callback` - Is function that library put in FastAPI `Depends `. Usually function returns user which tries to work with `resource`
 - `resource_type` - Is `str` which on which User tries to get access
 - `method` - Is API method by which working endpoint
 - `check_callback` - Is function that realize Policy's check. Function take arguments:
     ```python
     check_callback(subject, resource_type, item_id, method, db, cache)
     ```
 - - `subject` is result of `Depends(subject_callback)`
 - - `resource_type` is argument of `Policy()`
 - - `item_id` __(by default '*')__ is providing by FastAPI decorator `@app.get(/test/{item_id})`
 - - `method` is argument of `Policy()`
-- - `db` is database connection, result of `Depends(database_callback)`
-- - `cache` is redis connection, result of `Depends(cache_callback)`
-- `database_callback` - Is a function for getting database connecion
-- `cache_callback` - Is a function for getting Redis connection
+- - `db` is database connection
+- - `cache` is redis connection
+- `database` - Is a database connecion
+- `cache` - Is a Redis connection
 ---
 ## Examples
 Simple usage
 ```python
 from fastapi import FastAPI, Depends
 from dauth import auth
 
@@ -77,28 +83,28 @@
 # function get_database returns Databases connection
 def test_db(
     user = Depends(auth.Policy(
         get_user_auth, 
         'test', 
         'get', 
         is_admin, 
-        database_callback=get_database
+        database=Depends(get_database)
     ))
 ):
     return {"message":"Good"}
 
 @app.get("/test_with_cache")
 # function get_cache returns Redis connection
 def test_cache(
     user = Depends(auth.Policy(
         get_user_auth, 
         'test', 
         'get', 
         is_admin, 
-        cache_callback=get_cache
+        cache=Depends(get_cache)
     ))
 ):
     return {"message":"Good"}
 ```
 
 ---
 Developed by [DenVilk](https://github.com/denvilk)
```

### Comparing `dauth-0.5/setup.py` & `dauth-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 print(long_description)
 
 if __name__ == '__main__':
     setup(
         name='dauth',
-        version="0.5",
+        version="0.6",
         package_dir={'': 'src'},
         packages=find_packages('src', include=[
             'dauth*'
         ]),
         description='FastAPI ABAC authorization realization',
         long_description=long_description,
         long_description_content_type='text/markdown',
```

### Comparing `dauth-0.5/src/dauth/auth.py` & `dauth-0.6/src/dauth/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 
 
 def Policy(
     subject_callback: Callable, 
     resource_type: str, 
     method: str, 
     check_callback: Callable,
-    database_callback: Optional[Callable] = None,
-    cache_callback: Optional[Callable] = None
+    database: Optional[Database] = None,
+    cache: Optional[Redis] = None
 ):
     '''Function that give opportunity to work with Fastapi Depends'''
     def _check(
         subject: Any = Depends(subject_callback), 
         item_id: Union[str, int] = "*",
-        db: Optional[Database] = Depends(database_callback),
-        cache: Optional[Redis] = Depends(cache_callback)
     ) -> Any:
         '''Function that checks policy'''
-        check_callback(subject, resource_type, item_id, method, db, cache)
+        check_callback(subject, resource_type, item_id, method, database, cache)
         return subject
 
     return _check
```

### Comparing `dauth-0.5/src/dauth.egg-info/PKG-INFO` & `dauth-0.6/src/dauth.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dauth
-Version: 0.5
+Version: 0.6
 Summary: FastAPI ABAC authorization realization
 Description-Content-Type: text/markdown
 
 # DAuth 
 
 Python FastAPI ABAC Realization.
 
@@ -29,34 +29,34 @@
 Library represents function 
 ```python
 def Policy(
     subject_call: Callable, 
     resource_type: Any, 
     method: str, 
     check_callback: Callable,
-    database_callback: Union[Callable, None] = None,
-    cache_callback: Union[Callable, None] = None
+    database: Optional[Database] = None,
+    cache: Optional[Redis] = None
 )
 ```
 
 - `subject_callback` - Is function that library put in FastAPI `Depends `. Usually function returns user which tries to work with `resource`
 - `resource_type` - Is `str` which on which User tries to get access
 - `method` - Is API method by which working endpoint
 - `check_callback` - Is function that realize Policy's check. Function take arguments:
     ```python
     check_callback(subject, resource_type, item_id, method, db, cache)
     ```
 - - `subject` is result of `Depends(subject_callback)`
 - - `resource_type` is argument of `Policy()`
 - - `item_id` __(by default '*')__ is providing by FastAPI decorator `@app.get(/test/{item_id})`
 - - `method` is argument of `Policy()`
-- - `db` is database connection, result of `Depends(database_callback)`
-- - `cache` is redis connection, result of `Depends(cache_callback)`
-- `database_callback` - Is a function for getting database connecion
-- `cache_callback` - Is a function for getting Redis connection
+- - `db` is database connection
+- - `cache` is redis connection
+- `database` - Is a database connecion
+- `cache` - Is a Redis connection
 ---
 ## Examples
 Simple usage
 ```python
 from fastapi import FastAPI, Depends
 from dauth import auth
 
@@ -83,28 +83,28 @@
 # function get_database returns Databases connection
 def test_db(
     user = Depends(auth.Policy(
         get_user_auth, 
         'test', 
         'get', 
         is_admin, 
-        database_callback=get_database
+        database=Depends(get_database)
     ))
 ):
     return {"message":"Good"}
 
 @app.get("/test_with_cache")
 # function get_cache returns Redis connection
 def test_cache(
     user = Depends(auth.Policy(
         get_user_auth, 
         'test', 
         'get', 
         is_admin, 
-        cache_callback=get_cache
+        cache=Depends(get_cache)
     ))
 ):
     return {"message":"Good"}
 ```
 
 ---
 Developed by [DenVilk](https://github.com/denvilk)
```

