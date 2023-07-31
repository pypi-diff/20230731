# Comparing `tmp/somacore-1.0.3.tar.gz` & `tmp/somacore-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somacore-1.0.3.tar", last modified: Tue May 30 16:36:36 2023, max compression
+gzip compressed data, was "somacore-1.0.4.tar", last modified: Mon Jul 31 16:31:51 2023, max compression
```

## Comparing `somacore-1.0.3.tar` & `somacore-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-30 16:36:16.000000 somacore-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-30 16:36:16.000000 somacore-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 16:36:36.585210 somacore-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-30 16:36:16.000000 somacore-1.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.581210 somacore-1.0.3/python-spec/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 16:36:36.000000 somacore-1.0.3/python-spec/src/somacore/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/ephemeral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/ephemeral/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/_eager_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/_fast_csr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-30 16:36:16.000000 somacore-1.0.3/python-spec/src/somacore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:36.585210 somacore-1.0.3/python-spec/src/somacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-30 16:36:36.000000 somacore-1.0.3/python-spec/src/somacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:36:36.585210 somacore-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:31:51.528369 somacore-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-31 16:31:17.000000 somacore-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-31 16:31:17.000000 somacore-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 16:31:51.528369 somacore-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-31 16:31:17.000000 somacore-1.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:31:51.524369 somacore-1.0.4/python-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:31:51.524369 somacore-1.0.4/python-spec/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:31:51.524369 somacore-1.0.4/python-spec/src/somacore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 16:31:51.000000 somacore-1.0.4/python-spec/src/somacore/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:31:51.524369 somacore-1.0.4/python-spec/src/somacore/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/ephemeral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/ephemeral/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:31:51.528369 somacore-1.0.4/python-spec/src/somacore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/query/_eager_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/query/_fast_csr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/query/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19857 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-31 16:31:17.000000 somacore-1.0.4/python-spec/src/somacore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:31:51.528369 somacore-1.0.4/python-spec/src/somacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-31 16:31:51.000000 somacore-1.0.4/python-spec/src/somacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:31:51.528369 somacore-1.0.4/setup.cfg
```

### Comparing `somacore-1.0.3/LICENSE` & `somacore-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/PKG-INFO` & `somacore-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somacore
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python-language API specification and base utilities for implementation of the SOMA system.
 Project-URL: repository, https://github.com/single-cell-data/SOMA.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `somacore-1.0.3/pyproject.toml` & `somacore-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/README.md` & `somacore-1.0.4/python-spec/README.md`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/__init__.py` & `somacore-1.0.4/python-spec/src/somacore/__init__.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/_mixin.py` & `somacore-1.0.4/python-spec/src/somacore/_mixin.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/base.py` & `somacore-1.0.4/python-spec/src/somacore/base.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/collection.py` & `somacore-1.0.4/python-spec/src/somacore/collection.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/data.py` & `somacore-1.0.4/python-spec/src/somacore/data.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/ephemeral/collections.py` & `somacore-1.0.4/python-spec/src/somacore/ephemeral/collections.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/experiment.py` & `somacore-1.0.4/python-spec/src/somacore/experiment.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/measurement.py` & `somacore-1.0.4/python-spec/src/somacore/measurement.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/options.py` & `somacore-1.0.4/python-spec/src/somacore/options.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/query/_eager_iter.py` & `somacore-1.0.4/python-spec/src/somacore/query/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/query/_fast_csr.py` & `somacore-1.0.4/python-spec/src/somacore/query/_fast_csr.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/query/axis.py` & `somacore-1.0.4/python-spec/src/somacore/query/axis.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore/query/query.py` & `somacore-1.0.4/python-spec/src/somacore/query/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,17 +19,20 @@
 import pandas as pd
 import pyarrow as pa
 from scipy import sparse
 from typing_extensions import Literal, Protocol, Self, TypedDict, assert_never
 
 from .. import data
 from .. import measurement
+from .. import options
 from . import _fast_csr
 from . import axis
 
+_RO_AUTO = options.ResultOrder.AUTO
+
 
 class AxisColumnNames(TypedDict, total=False):
     """
     Specifies column names for experiment axis query read operations.
 
     Lifecycle: maturing
     """
@@ -93,43 +96,63 @@
 
         self._matrix_axis_query = _MatrixAxisQuery(obs=obs_query, var=var_query)
         self._joinids = _JoinIDCache(self)
         self._indexer = AxisIndexer(self)
         self._threadpool_: Optional[futures.ThreadPoolExecutor] = None
 
     def obs(
-        self, *, column_names: Optional[Sequence[str]] = None
+        self,
+        *,
+        column_names: Optional[Sequence[str]] = None,
+        batch_size: options.BatchSize = options.BatchSize(),
+        partitions: Optional[options.ReadPartitions] = None,
+        result_order: options.ResultOrderStr = _RO_AUTO,
+        platform_config: Optional[options.PlatformConfig] = None,
     ) -> data.ReadIter[pa.Table]:
         """Returns ``obs`` as an `Arrow table
         <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
         iterator.
 
         Lifecycle: maturing
         """
         obs_query = self._matrix_axis_query.obs
         return self._obs_df.read(
             obs_query.coords,
             value_filter=obs_query.value_filter,
             column_names=column_names,
+            batch_size=batch_size,
+            partitions=partitions,
+            result_order=result_order,
+            platform_config=platform_config,
         )
 
     def var(
-        self, *, column_names: Optional[Sequence[str]] = None
+        self,
+        *,
+        column_names: Optional[Sequence[str]] = None,
+        batch_size: options.BatchSize = options.BatchSize(),
+        partitions: Optional[options.ReadPartitions] = None,
+        result_order: options.ResultOrderStr = _RO_AUTO,
+        platform_config: Optional[options.PlatformConfig] = None,
     ) -> data.ReadIter[pa.Table]:
         """Returns ``var`` as an `Arrow table
         <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
         iterator.
 
         Lifecycle: maturing
         """
         var_query = self._matrix_axis_query.var
         return self._var_df.read(
             var_query.coords,
             value_filter=var_query.value_filter,
             column_names=column_names,
+            batch_size=batch_size,
+            partitions=partitions,
+            result_order=result_order,
+            platform_config=platform_config,
         )
 
     def obs_joinids(self) -> pa.Array:
         """Returns ``obs`` ``soma_joinids`` as an Arrow array.
 
         Lifecycle: maturing
         """
@@ -162,31 +185,51 @@
     def indexer(self) -> "AxisIndexer":
         """A ``soma_joinid`` indexer for both ``obs`` and ``var`` axes.
 
         Lifecycle: maturing
         """
         return self._indexer
 
-    def X(self, layer_name: str) -> data.SparseRead:
+    def X(
+        self,
+        layer_name: str,
+        *,
+        batch_size: options.BatchSize = options.BatchSize(),
+        partitions: Optional[options.ReadPartitions] = None,
+        result_order: options.ResultOrderStr = _RO_AUTO,
+        platform_config: Optional[options.PlatformConfig] = None,
+    ) -> data.SparseRead:
         """Returns an ``X`` layer as a sparse read.
 
         Args:
             layer_name: The X layer name to return.
+            batch_size: The size of batches that should be returned from a read.
+                See :class:`options.BatchSize` for details.
+            partitions: Specifies that this is part of a partitioned read,
+                and which partition to include, if present.
+            result_order: the order to return results, specified as a
+                :class:`~options.ResultOrder` or its string value.
 
         Lifecycle: maturing
         """
         try:
             x_layer = self._ms.X[layer_name]
         except KeyError as ke:
             raise KeyError(f"{layer_name} is not present in X") from ke
         if not isinstance(x_layer, data.SparseNDArray):
             raise TypeError("X layers may only be sparse arrays")
 
         self._joinids.preload(self._threadpool)
-        return x_layer.read((self._joinids.obs, self._joinids.var))
+        return x_layer.read(
+            (self._joinids.obs, self._joinids.var),
+            batch_size=batch_size,
+            partitions=partitions,
+            result_order=result_order,
+            platform_config=platform_config,
+        )
 
     def obsp(self, layer: str) -> data.SparseRead:
         """Returns an ``obsp`` layer as a sparse read.
 
         Lifecycle: maturing
         """
         return self._axisp_inner(_Axis.OBS, layer)
```

### Comparing `somacore-1.0.3/python-spec/src/somacore/types.py` & `somacore-1.0.4/python-spec/src/somacore/types.py`

 * *Files identical despite different names*

### Comparing `somacore-1.0.3/python-spec/src/somacore.egg-info/SOURCES.txt` & `somacore-1.0.4/python-spec/src/somacore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

