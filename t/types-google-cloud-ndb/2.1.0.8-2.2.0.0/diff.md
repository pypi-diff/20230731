# Comparing `tmp/types-google-cloud-ndb-2.1.0.8.tar.gz` & `tmp/types-google-cloud-ndb-2.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-google-cloud-ndb-2.1.0.8.tar", last modified: Thu Jul 20 15:20:25 2023, max compression
+gzip compressed data, was "types-google-cloud-ndb-2.2.0.0.tar", last modified: Mon Jul 31 09:15:34 2023, max compression
```

## Comparing `types-google-cloud-ndb-2.1.0.8.tar` & `types-google-cloud-ndb-2.2.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.708238 types-google-cloud-ndb-2.1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 15:20:25.708238 types-google-cloud-ndb-2.1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.700237 types-google-cloud-ndb-2.1.0.8/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.700237 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.704238 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_batch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_datastore_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_datastore_query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_eventloop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_options.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/blobstore.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/context.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/django_middleware.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/global_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/msgprop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/polymodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/stats.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/tasklets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 15:15:13.000000 types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:25.708238 types-google-cloud-ndb-2.1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-20 15:20:24.000000 types-google-cloud-ndb-2.1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:25.704238 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:20:25.000000 types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:34.796199 types-google-cloud-ndb-2.2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-31 09:15:32.000000 types-google-cloud-ndb-2.2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 09:15:32.000000 types-google-cloud-ndb-2.2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-31 09:15:34.796199 types-google-cloud-ndb-2.2.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:34.792199 types-google-cloud-ndb-2.2.0.0/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-31 09:15:32.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:34.792199 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:34.796199 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_datastore_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_datastore_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_eventloop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/blobstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/django_middleware.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/global_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/msgprop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/polymodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/tasklets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-31 09:15:19.000000 types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:15:34.796199 types-google-cloud-ndb-2.2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-31 09:15:32.000000 types-google-cloud-ndb-2.2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:15:34.796199 types-google-cloud-ndb-2.2.0.0/types_google_cloud_ndb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-31 09:15:34.000000 types-google-cloud-ndb-2.2.0.0/types_google_cloud_ndb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 09:15:34.000000 types-google-cloud-ndb-2.2.0.0/types_google_cloud_ndb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:15:34.000000 types-google-cloud-ndb-2.2.0.0/types_google_cloud_ndb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 09:15:34.000000 types-google-cloud-ndb-2.2.0.0/types_google_cloud_ndb.egg-info/top_level.txt
```

### Comparing `types-google-cloud-ndb-2.1.0.8/CHANGELOG.md` & `types-google-cloud-ndb-2.2.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.2.0.0 (2023-07-31)
+
+Bump google-cloud-ndb to 2.2.* (#10521)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 2.1.0.8 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 2.1.0.7 (2023-05-10)
```

### Comparing `types-google-cloud-ndb-2.1.0.8/PKG-INFO` & `types-google-cloud-ndb-2.2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-google-cloud-ndb
-Version: 2.1.0.8
+Version: 2.2.0.0
 Summary: Typing stubs for google-cloud-ndb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `fe2ebd69af14d376825f21182d415223bd037485` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
```

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/__init__.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_cache.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_cache.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_datastore_query.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_datastore_query.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_eventloop.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_eventloop.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/_transaction.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/_transaction.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/blobstore.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/blobstore.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/context.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/context.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/exceptions.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/global_cache.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/global_cache.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/key.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/key.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     def __ge__(self, other): ...
     def __getnewargs__(self): ...
     def parent(self): ...
     def root(self): ...
     def namespace(self): ...
     def project(self): ...
     app: Any
+    def database(self) -> str | None: ...
     def id(self): ...
     def string_id(self): ...
     def integer_id(self): ...
     def pairs(self): ...
     def flat(self): ...
     def kind(self): ...
     def reference(self): ...
```

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/metadata.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/metadata.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/model.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/model.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -316,14 +316,15 @@
         global_cache_timeout: int | None = ...,
         use_datastore: bool | None = ...,
         use_memcache: bool | None = ...,
         memcache_timeout: int | None = ...,
         max_memcache_items: int | None = ...,
         force_writes: bool | None = ...,
         _options=...,
+        database: str | None = None,
     ) -> Model | None: ...
     @classmethod
     def get_by_id_async(
         cls: type[Model],
         id: int | str,
         parent: key_module.Key | None = ...,
         namespace: str | None = ...,
@@ -340,14 +341,15 @@
         global_cache_timeout: int | None = ...,
         use_datastore: bool | None = ...,
         use_memcache: bool | None = ...,
         memcache_timeout: int | None = ...,
         max_memcache_items: int | None = ...,
         force_writes: bool | None = ...,
         _options=...,
+        database: str | None = None,
     ) -> tasklets_module.Future: ...
     @classmethod
     def get_or_insert(
         cls: type[Model],
         _name: str,
         parent: key_module.Key | None = ...,
         namespace: str | None = ...,
```

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/query.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/query.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
 AND = ConjunctionNode
 OR = DisjunctionNode
 
 class QueryOptions(_options.ReadOptions):
     project: Any
     namespace: Any
+    database: str | None
     def __init__(self, config: Incomplete | None = ..., context: Incomplete | None = ..., **kwargs) -> None: ...
 
 class Query:
     default_options: Any
     kind: Any
     ancestor: Any
     filters: Any
@@ -102,14 +103,15 @@
     project: Any
     namespace: Any
     limit: Any
     offset: Any
     keys_only: Any
     projection: Any
     distinct_on: Any
+    database: str | None
     def __init__(
         self,
         kind: Incomplete | None = ...,
         filters: Incomplete | None = ...,
         ancestor: Incomplete | None = ...,
         order_by: Incomplete | None = ...,
         orders: Incomplete | None = ...,
```

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/stats.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/stats.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/tasklets.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/tasklets.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/google-stubs/cloud/ndb/utils.pyi` & `types-google-cloud-ndb-2.2.0.0/google-stubs/cloud/ndb/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.8/setup.py` & `types-google-cloud-ndb-2.2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `fe2ebd69af14d376825f21182d415223bd037485` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.0.8",
+      version="2.2.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md",
```

### Comparing `types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/PKG-INFO` & `types-google-cloud-ndb-2.2.0.0/types_google_cloud_ndb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-google-cloud-ndb
-Version: 2.1.0.8
+Version: 2.2.0.0
 Summary: Typing stubs for google-cloud-ndb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `fe2ebd69af14d376825f21182d415223bd037485` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
```

### Comparing `types-google-cloud-ndb-2.1.0.8/types_google_cloud_ndb.egg-info/SOURCES.txt` & `types-google-cloud-ndb-2.2.0.0/types_google_cloud_ndb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

