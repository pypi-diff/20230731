# Comparing `tmp/ardoqpy-0.7.7.tar.gz` & `tmp/ardoqpy-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardoqpy-0.7.7.tar", last modified: Tue Jul 25 19:28:59 2023, max compression
+gzip compressed data, was "ardoqpy-0.7.8.tar", last modified: Mon Jul 31 12:58:26 2023, max compression
```

## Comparing `ardoqpy-0.7.7.tar` & `ardoqpy-0.7.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-25 19:28:59.520706 ardoqpy-0.7.7/
--rw-r--r--   0 jason      (501) staff       (20)     1119 2016-04-11 06:32:09.000000 ardoqpy-0.7.7/LICENSE.txt
--rw-r--r--   0 jason      (501) staff       (20)       57 2021-05-01 13:21:49.000000 ardoqpy-0.7.7/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     6229 2023-07-25 19:28:59.520796 ardoqpy-0.7.7/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     5165 2023-07-25 19:20:25.000000 ardoqpy-0.7.7/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-25 19:28:59.518845 ardoqpy-0.7.7/ardoqpy/
--rw-r--r--   0 jason      (501) staff       (20)       51 2021-05-11 18:42:19.000000 ardoqpy-0.7.7/ardoqpy/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)      304 2022-02-12 20:17:55.000000 ardoqpy-0.7.7/ardoqpy/ardoqpy.cfg
--rw-r--r--   0 jason      (501) staff       (20)    17453 2023-07-25 19:11:58.000000 ardoqpy-0.7.7/ardoqpy/ardoqpy.py
--rw-r--r--   0 jason      (501) staff       (20)    11264 2023-03-31 06:55:34.000000 ardoqpy-0.7.7/ardoqpy/ardoqpy_sync.py
--rw-r--r--   0 jason      (501) staff       (20)     1128 2022-08-10 09:44:52.000000 ardoqpy-0.7.7/ardoqpy/test_ardoqpy.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-25 19:28:59.520491 ardoqpy-0.7.7/ardoqpy.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     6229 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      313 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       32 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        8 2023-07-25 19:28:59.000000 ardoqpy-0.7.7/ardoqpy.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       79 2023-07-25 19:28:59.521157 ardoqpy-0.7.7/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1862 2023-07-25 19:20:25.000000 ardoqpy-0.7.7/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-31 12:58:26.517872 ardoqpy-0.7.8/
+-rw-r--r--   0 jason      (501) staff       (20)     1119 2016-04-11 06:32:09.000000 ardoqpy-0.7.8/LICENSE.txt
+-rw-r--r--   0 jason      (501) staff       (20)       57 2021-05-01 13:21:49.000000 ardoqpy-0.7.8/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     6297 2023-07-31 12:58:26.517955 ardoqpy-0.7.8/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     5233 2023-07-31 12:43:34.000000 ardoqpy-0.7.8/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-31 12:58:26.516717 ardoqpy-0.7.8/ardoqpy/
+-rw-r--r--   0 jason      (501) staff       (20)       51 2021-05-11 18:42:19.000000 ardoqpy-0.7.8/ardoqpy/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)      304 2022-02-12 20:17:55.000000 ardoqpy-0.7.8/ardoqpy/ardoqpy.cfg
+-rw-r--r--   0 jason      (501) staff       (20)    17694 2023-07-31 12:40:43.000000 ardoqpy-0.7.8/ardoqpy/ardoqpy.py
+-rw-r--r--   0 jason      (501) staff       (20)    11264 2023-03-31 06:55:34.000000 ardoqpy-0.7.8/ardoqpy/ardoqpy_sync.py
+-rw-r--r--   0 jason      (501) staff       (20)     1128 2022-08-10 09:44:52.000000 ardoqpy-0.7.8/ardoqpy/test_ardoqpy.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-07-31 12:58:26.517719 ardoqpy-0.7.8/ardoqpy.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     6297 2023-07-31 12:58:26.000000 ardoqpy-0.7.8/ardoqpy.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      313 2023-07-31 12:58:26.000000 ardoqpy-0.7.8/ardoqpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2023-07-31 12:58:26.000000 ardoqpy-0.7.8/ardoqpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       32 2023-07-31 12:58:26.000000 ardoqpy-0.7.8/ardoqpy.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        8 2023-07-31 12:58:26.000000 ardoqpy-0.7.8/ardoqpy.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       79 2023-07-31 12:58:26.518238 ardoqpy-0.7.8/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1862 2023-07-31 12:57:29.000000 ardoqpy-0.7.8/setup.py
```

### Comparing `ardoqpy-0.7.7/LICENSE.txt` & `ardoqpy-0.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ardoqpy-0.7.7/PKG-INFO` & `ardoqpy-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardoqpy
-Version: 0.7.7
+Version: 0.7.8
 Summary: A python REST API wrapper for Ardoq - https://ardoq.com.
 Home-page: https://github.com/jbaragry/ardoq-python-client
 Author: Jason Baragry
 Author-email: jason.baragry@gmail.com
 License: MIT
 Keywords: architecture ardoq REST API wrapper tool
 Classifier: Development Status :: 3 - Alpha
@@ -145,14 +145,16 @@
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN')
     # to use v2 API
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN', version='v2')
     ardoq.get_workspaces()
 
 ## Changelog
 - 202307
+  - added workspace and workspaces endpoints for v2 client
+- 202307
   - added del and update tag
 - 202303
   - added audit log for support for components created, updated, deleted, and skipped due to cache_hit
 - 202211
   - added support for Ardoq v2 REST API. Only for the ArdoqClient (not SyncClient)
 - 202207
   - add find_reference_type to return reftype definition from the metamodel for a workspace
```

### Comparing `ardoqpy-0.7.7/README.md` & `ardoqpy-0.7.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN')
     # to use v2 API
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN', version='v2')
     ardoq.get_workspaces()
 
 ## Changelog
 - 202307
+  - added workspace and workspaces endpoints for v2 client
+- 202307
   - added del and update tag
 - 202303
   - added audit log for support for components created, updated, deleted, and skipped due to cache_hit
 - 202211
   - added support for Ardoq v2 REST API. Only for the ArdoqClient (not SyncClient)
 - 202207
   - add find_reference_type to return reftype definition from the metamodel for a workspace
```

### Comparing `ardoqpy-0.7.7/ardoqpy/ardoqpy.py` & `ardoqpy-0.7.8/ardoqpy/ardoqpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,28 +140,34 @@
 
     '''
     functions for workspaces
     '''
 
     # get all workspaces
     def get_workspaces(self, summary=False):
-        self.workspaces = self._get('workspace' if not summary else 'workspace/summary')
+        if self.version == 'v1':
+            self.workspaces = self._get('workspace' if not summary else 'workspace/summary')
+        else: # v2
+            self.workspaces = self._get('workspaces')
         return self.workspaces
 
     # gets the workspace using either the workspace ID or name
     # TODO need to check if the ID or name is in the existing workspaces...
     # TODO: change this to only get the workspace by ID.
     #       need a different function to find the id by name
     def get_workspace(self, ws_id=None, aggregated=False):
         if ws_id is None:
             raise ArdoqClientException("need an id for get_workspace")
-        endpoint = 'workspace' + '/' + ws_id
-        if aggregated:
-            endpoint += '/aggregated'
-        self.workspace = self._get(endpoint)
+        if self.version == 'v1':
+            endpoint = 'workspace' + '/' + ws_id
+            if aggregated:
+                endpoint += '/aggregated'
+            self.workspace = self._get(endpoint)
+        else:  # v2
+            self.workspace = self._get('workspaces/' + ws_id)
         return self.workspace
 
     def create_workspace(self, ws=None):
         if ws is None:
             raise ArdoqClientException('must provide a workspace')
         res = self._post('workspace', ws)
         return res
```

### Comparing `ardoqpy-0.7.7/ardoqpy/ardoqpy_sync.py` & `ardoqpy-0.7.8/ardoqpy/ardoqpy_sync.py`

 * *Files identical despite different names*

### Comparing `ardoqpy-0.7.7/ardoqpy/test_ardoqpy.py` & `ardoqpy-0.7.8/ardoqpy/test_ardoqpy.py`

 * *Files identical despite different names*

### Comparing `ardoqpy-0.7.7/ardoqpy.egg-info/PKG-INFO` & `ardoqpy-0.7.8/ardoqpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardoqpy
-Version: 0.7.7
+Version: 0.7.8
 Summary: A python REST API wrapper for Ardoq - https://ardoq.com.
 Home-page: https://github.com/jbaragry/ardoq-python-client
 Author: Jason Baragry
 Author-email: jason.baragry@gmail.com
 License: MIT
 Keywords: architecture ardoq REST API wrapper tool
 Classifier: Development Status :: 3 - Alpha
@@ -145,14 +145,16 @@
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN')
     # to use v2 API
     ardoq = ardoqpy.ArdoqClient(hosturl='https://YOURORG.ardoq.com', token='YOURTOKEN', version='v2')
     ardoq.get_workspaces()
 
 ## Changelog
 - 202307
+  - added workspace and workspaces endpoints for v2 client
+- 202307
   - added del and update tag
 - 202303
   - added audit log for support for components created, updated, deleted, and skipped due to cache_hit
 - 202211
   - added support for Ardoq v2 REST API. Only for the ArdoqClient (not SyncClient)
 - 202207
   - add find_reference_type to return reftype definition from the metamodel for a workspace
```

### Comparing `ardoqpy-0.7.7/setup.py` & `ardoqpy-0.7.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from distutils.core import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='ardoqpy',
-    version='0.7.7',
+    version='0.7.8',
     description='A python REST API wrapper for Ardoq - https://ardoq.com.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/jbaragry/ardoq-python-client',
     author='Jason Baragry',
     author_email='jason.baragry@gmail.com',
     license='MIT',
```

