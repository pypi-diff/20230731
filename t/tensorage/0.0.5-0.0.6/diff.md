# Comparing `tmp/tensorage-0.0.5.tar.gz` & `tmp/tensorage-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.5.tar", last modified: Sun Jul 30 18:30:06 2023, max compression
+gzip compressed data, was "tensorage-0.0.6.tar", last modified: Mon Jul 31 05:26:22 2023, max compression
```

## Comparing `tensorage-0.0.5.tar` & `tensorage-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 18:30:06.980695 tensorage-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-30 18:29:56.000000 tensorage-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 18:29:56.000000 tensorage-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 18:30:06.980695 tensorage-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 18:29:56.000000 tensorage-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-30 18:29:56.000000 tensorage-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-30 18:30:06.980695 tensorage-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-30 18:29:56.000000 tensorage-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 18:30:06.980695 tensorage-0.0.5/tensorage/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/db_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     7325 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-30 18:29:56.000000 tensorage-0.0.5/tensorage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 18:30:06.980695 tensorage-0.0.5/tensorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-30 18:30:06.000000 tensorage-0.0.5/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 05:26:22.053734 tensorage-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-31 05:26:07.000000 tensorage-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 05:26:07.000000 tensorage-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 05:26:22.053734 tensorage-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 05:26:07.000000 tensorage-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-31 05:26:07.000000 tensorage-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 05:26:22.053734 tensorage-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-31 05:26:07.000000 tensorage-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 05:26:22.053734 tensorage-0.0.6/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7351 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 05:26:22.053734 tensorage-0.0.6/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.5/LICENSE` & `tensorage-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.5/setup.py` & `tensorage-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.5/tensorage/db_init.py` & `tensorage-0.0.6/tensorage/db_init.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.5/tensorage/session.py` & `tensorage-0.0.6/tensorage/session.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.5/tensorage/store.py` & `tensorage-0.0.6/tensorage/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,21 +142,21 @@
         response = self.backend.client.table('datasets').insert({'key': key, 'shape': shape, 'ndim': dim, 'user_id': self.user_id}).execute()
         self.__restore_auth()
 
         # return an instance of Dataset
         data = response.data[0]
         return Dataset(id=data['id'], key=data['key'], shape=data['shape'], ndim=data['ndim'])
     
-    def insert_tensor(self, data_id: int, data: List[np.ndarray]) -> bool:
+    def insert_tensor(self, data_id: int, data: List[np.ndarray], offset: int = 0) -> bool:
         # setup auth token
         self.__setup_auth()
         
         # run the insert
         try:
-            response = self.backend.client.table('tensors_float4').insert([{'data_id': data_id, 'index': i + 1, 'user_id': self.user_id, 'tensor': chunk.tolist()} for i, chunk in enumerate(data)]).execute()
+            response = self.backend.client.table('tensors_float4').insert([{'data_id': data_id, 'index': i + 1 + offset, 'user_id': self.user_id, 'tensor': chunk.tolist()} for i, chunk in enumerate(data)]).execute()
         except Exception as e:
             print(response.data)
             raise e
         
         # restore old token
         self.__restore_auth()
```

