# Comparing `tmp/kr8s-0.8.7.tar.gz` & `tmp/kr8s-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.8.7.tar", max compression
+gzip compressed data, was "kr8s-0.8.8.tar", max compression
```

## Comparing `kr8s-0.8.7.tar` & `kr8s-0.8.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1549 2023-07-27 15:57:43.772847 kr8s-0.8.7/LICENSE
--rw-r--r--   0        0        0     2587 2023-07-27 15:57:43.772847 kr8s-0.8.7/README.md
--rw-r--r--   0        0        0     1143 2023-07-27 15:58:16.827524 kr8s-0.8.7/kr8s/__init__.py
--rw-r--r--   0        0        0    14674 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_api.py
--rw-r--r--   0        0        0     6266 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4336 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_io.py
--rw-r--r--   0        0        0    36828 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_objects.py
--rw-r--r--   0        0        0     8074 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_testutils.py
--rw-r--r--   0        0        0      248 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0     1681 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/_helpers.py
--rw-r--r--   0        0        0      827 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0      168 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5503 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     5909 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3394 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     1710 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    21028 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2676 2023-07-27 15:58:16.827524 kr8s-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-31 14:09:28.616289 kr8s-0.8.8/LICENSE
+-rw-r--r--   0        0        0     2587 2023-07-31 14:09:28.616289 kr8s-0.8.8/README.md
+-rw-r--r--   0        0        0     1143 2023-07-31 14:09:54.796281 kr8s-0.8.8/kr8s/__init__.py
+-rw-r--r--   0        0        0    14674 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_api.py
+-rw-r--r--   0        0        0     6266 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4336 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_io.py
+-rw-r--r--   0        0        0    37029 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_objects.py
+-rw-r--r--   0        0        0     8074 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/_testutils.py
+-rw-r--r--   0        0        0      248 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     6090 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3394 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    21055 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-31 14:09:28.636289 kr8s-0.8.8/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2676 2023-07-31 14:09:54.796281 kr8s-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.8/PKG-INFO
```

### Comparing `kr8s-0.8.7/LICENSE` & `kr8s-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/README.md` & `kr8s-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/__init__.py` & `kr8s-0.8.8/kr8s/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .asyncio import (
     version as _version,
 )
 from .asyncio import (
     watch as _watch,
 )
 
-__version__ = "0.8.7"
+__version__ = "0.8.8"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.8.7/kr8s/_api.py` & `kr8s-0.8.8/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/_auth.py` & `kr8s-0.8.8/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/_data_utils.py` & `kr8s-0.8.8/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/_io.py` & `kr8s-0.8.8/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/_objects.py` & `kr8s-0.8.8/kr8s/_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,18 @@
     @raw.setter
     def raw(self, value: Any) -> None:
         self._raw = value
 
     @property
     def name(self) -> str:
         """Name of the Kubernetes resource."""
-        return self.raw["metadata"]["name"]
+        try:
+            return self.raw["metadata"]["name"]
+        except KeyError:
+            raise ValueError("Resource does not have a name")
 
     @property
     def namespace(self) -> str:
         """Namespace of the Kubernetes resource."""
         if self.namespaced:
             return self.raw.get("metadata", {}).get("namespace", self.api.namespace)
         return None
@@ -195,22 +198,25 @@
 
     async def exists(self, ensure=False) -> bool:
         """Check if this object exists in Kubernetes."""
         return await self._exists(ensure=ensure)
 
     async def _exists(self, ensure=False) -> bool:
         """Check if this object exists in Kubernetes."""
-        async with self.api.call_api(
-            "GET",
-            version=self.version,
-            url=f"{self.endpoint}/{self.name}",
-            namespace=self.namespace,
-            raise_for_status=False,
-        ) as resp:
-            status = resp.status_code
+        try:
+            async with self.api.call_api(
+                "GET",
+                version=self.version,
+                url=f"{self.endpoint}/{self.name}",
+                namespace=self.namespace,
+                raise_for_status=False,
+            ) as resp:
+                status = resp.status_code
+        except ValueError:
+            status = 400
         if status == 200:
             return True
         if ensure:
             raise NotFoundError(f"Object {self.name} does not exist")
         return False
 
     async def create(self) -> None:
```

### Comparing `kr8s-0.8.7/kr8s/_portforward.py` & `kr8s-0.8.8/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/_testutils.py` & `kr8s-0.8.8/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/asyncio/_api.py` & `kr8s-0.8.8/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/asyncio/_helpers.py` & `kr8s-0.8.8/kr8s/asyncio/_helpers.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/asyncio/objects.py` & `kr8s-0.8.8/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/conftest.py` & `kr8s-0.8.8/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/objects.py` & `kr8s-0.8.8/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/tests/scripts/envexec.py` & `kr8s-0.8.8/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/tests/test_api.py` & `kr8s-0.8.8/kr8s/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,34 +23,34 @@
     assert k1 is k2
 
     k3 = await kr8s.asyncio.api(serviceaccount=serviceaccount)
     k4 = await kr8s.asyncio.api(serviceaccount=serviceaccount)
     assert k1 is not k3
     assert k3 is k4
 
-    p = await Pod({})
+    p = await Pod({"metadata": {"name": "foo"}})
     assert p.api is k1
     assert p.api is not k3
 
 
 async def test_api_factory_with_kubeconfig(k8s_cluster, serviceaccount):
     k1 = await kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
     k2 = await kr8s.asyncio.api(serviceaccount=serviceaccount)
     k3 = await kr8s.asyncio.api()
     assert k1 is not k2
     assert k3 is k1
     assert k3 is not k2
 
-    p = await Pod({})
+    p = await Pod({"metadata": {"name": "foo"}})
     assert p.api is k1
 
-    p2 = await Pod({}, api=k2)
+    p2 = await Pod({"metadata": {"name": "bar"}}, api=k2)
     assert p2.api is k2
 
-    p3 = await Pod({}, api=k3)
+    p3 = await Pod({"metadata": {"name": "baz"}}, api=k3)
     assert p3.api is k3
     assert p3.api is not k2
 
 
 def test_version_sync():
     kubernetes = kr8s.api()
     version = kubernetes.version()
@@ -100,14 +100,15 @@
 
 
 async def test_get_pods_as_table():
     kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get("pods", namespace="kube-system", as_object=Table)
     assert isinstance(pods, Table)
     assert len(pods.rows) > 0
+    assert not await pods.exists()  # Cannot exist in the Kubernetes API
 
 
 async def test_watch_pods(example_pod_spec, ns):
     pod = await Pod(example_pod_spec)
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
```

### Comparing `kr8s-0.8.7/kr8s/tests/test_auth.py` & `kr8s-0.8.8/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/tests/test_data_utils.py` & `kr8s-0.8.8/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/tests/test_io.py` & `kr8s-0.8.8/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/kr8s/tests/test_objects.py` & `kr8s-0.8.8/kr8s/tests/test_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,15 +506,15 @@
         assert resp.status_code == 404
 
     await pf.stop()
     assert pf._bg_task is None
 
 
 async def test_unsupported_port_forward():
-    pv = await PersistentVolume({})
+    pv = await PersistentVolume({"metadata": {"name": "foo"}})
     with pytest.raises(AttributeError):
         await pv.portforward(80)
     with pytest.raises(ValueError):
         await PortForward(pv, 80).start()
 
 
 async def test_scalable_dot_notation():
```

### Comparing `kr8s-0.8.7/kr8s/tests/test_testutils.py` & `kr8s-0.8.8/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.7/pyproject.toml` & `kr8s-0.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.8.7"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.8.8"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `kr8s-0.8.7/PKG-INFO` & `kr8s-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.8.7
+Version: 0.8.8
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

