# Comparing `tmp/tortoise-api-0.2.3.tar.gz` & `tmp/tortoise-api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.2.3.tar", last modified: Fri Jul 28 19:32:32 2023, max compression
+gzip compressed data, was "tortoise-api-0.2.4.tar", last modified: Mon Jul 31 11:51:37 2023, max compression
```

## Comparing `tortoise-api-0.2.3.tar` & `tortoise-api-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:32:32.330144 tortoise-api-0.2.3/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.3/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 19:32:32.329777 tortoise-api-0.2.3/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.3/README.md
--rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-28 19:32:07.000000 tortoise-api-0.2.3/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 19:32:32.330228 tortoise-api-0.2.3/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:32:32.327515 tortoise-api-0.2.3/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.3/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     3186 2023-07-27 10:21:50.000000 tortoise-api-0.2.3/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)     2768 2023-07-28 19:32:07.000000 tortoise-api-0.2.3/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 19:32:32.329301 tortoise-api-0.2.3/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-28 19:32:32.000000 tortoise-api-0.2.3/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:51:37.040105 tortoise-api-0.2.4/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.4/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-31 11:51:37.039869 tortoise-api-0.2.4/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.4/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-31 11:50:56.000000 tortoise-api-0.2.4/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 11:51:37.040166 tortoise-api-0.2.4/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:51:37.038347 tortoise-api-0.2.4/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.4/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     3527 2023-07-31 11:49:15.000000 tortoise-api-0.2.4/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)     3069 2023-07-31 11:44:47.000000 tortoise-api-0.2.4/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:51:37.039592 tortoise-api-0.2.4/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-31 11:51:37.000000 tortoise-api-0.2.4/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.2.3/LICENSE` & `tortoise-api-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.3/PKG-INFO` & `tortoise-api-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `tortoise-api-0.2.3/README.md` & `tortoise-api-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.3/pyproject.toml` & `tortoise-api-0.2.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 description = "Simplest fastest minimal REST API CRUD generator for Tortoise ORM models"
 readme = "README.md"
 license = {text = "MIT"}
 dependencies = [
     "asyncpg",
     "python-dotenv",
     "starlette",
-    "tortoise-api-model>=0.0.5",
+    "tortoise-api-model>=0.1.0",
     "uvicorn"
 ]
-version = "0.2.3"
+version = "0.2.4"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.2.3/tortoise_api/api.py` & `tortoise-api-0.2.4/tortoise_api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dotenv import load_dotenv
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response, RedirectResponse
 from starlette.routing import Route
 from starlette.templating import Jinja2Templates
 from tortoise.contrib.starlette import register_tortoise
+from tortoise.fields import ManyToManyRelation
 from tortoise_api_model import Model
 
 from tortoise_api.util import jsonify, update, delete, parse_qs
 
 
 class Api:
     app: Starlette
@@ -48,15 +49,20 @@
     async def api_menu(self, _: Request):
         return JSONResponse(list(self.models))
 
     async def all_create(self, request: Request):
         model: type[Model] = self._get_model(request)
         if request.method == 'POST':
             data = parse_qs(await request.body())
-            await model.create(**data)
+            m2ms = {k: data.pop(k) for k in model._meta.m2m_fields}
+            obj: Model = await model.create(**data)
+            for k, ids in m2ms.items():
+                m2m_rel: ManyToManyRelation = getattr(obj, k)
+                items = [await m2m_rel.remote_model[i] for i in ids]
+                await m2m_rel.add(*items)
             return RedirectResponse('/'+model.__name__, 303) # create # {True: 201, False: 202}[res[1]]
         objects: [Model] = await model.all().prefetch_related(*model._meta.fetch_fields)
         data = [jsonify(obj) for obj in objects]
         return JSONResponse({'data': data}) # show all
 
     async def one_update(self, request: Request):
         model: type[Model] = self._get_model(request)
```

### Comparing `tortoise-api-0.2.3/tortoise_api/util.py` & `tortoise-api-0.2.4/tortoise_api/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,28 +32,37 @@
 
     return {key: check(field, key) for key, field in obj._meta.fields_map.items() if not key.endswith('_id')}
 
 def parse_qs(s: str) -> dict:
     data = {}
     for k, v in parse_qsl(unquote(s)):
         # for collection-like fields (1d tuples): multiple the same name params merges to tuple
-        if k in data:
-            if isinstance(data[k], tuple):
-                data[k] += (v,)
+        if k.endswith('[]'):
+            k = k[:-2]
+            # for list-like fields(2d lists: (1d list of 1d tuples)): '.'-separated param names splits to {key}.{index}
+            if '.' in k:
+                k, i = k.split('.')
+                i = int(i)
+                data[k] = data.get(k, [()])
+                if len(data[k]) > i:
+                    data[k][i] += (v,)
+                else:
+                    data[k].append((v,))
             else:
-                data[k] = data[k], float(v)
-        # for list-like fields(2d lists: (1d list of 1d tuples)): '.'-separated param names splits to {key}.{index}
-        elif '.' in k:
-            bk, i = k.split('.')
-            i = int(i)
-            data[bk] = data.get(bk, [()])
-            if len(data[bk]) > i:
-                data[bk][i] += (v,)
-            else:
-                data[bk].append((v,))
+                data[k] = data.get(k, ()) + (v,)
+        # todo: make list with no collections ablility
+        # elif '.' in k:
+        #     k, i = k.split('.')
+        #     i = int(i)
+        #     data[k] = data.get(k, [()])
+        #     if len(data[k]) > i:
+        #         data[k][i] += (v,)
+        #     else:
+        #         data[k].append((v,))
+
         else: # if v is IntEnum - it requires explicit convert to int
             data[k] = int(v) if v.isnumeric() else v
     return data
 
 # async def upsert(model: type[Model], dct: dict):
 #     meta: MetaInfo = model._meta
 #     if pk := meta.pk_attr in dct.keys():
```

### Comparing `tortoise-api-0.2.3/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.2.4/tortoise_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

