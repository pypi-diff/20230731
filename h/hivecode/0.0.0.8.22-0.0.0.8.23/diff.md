# Comparing `tmp/hivecode-0.0.0.8.22.tar.gz` & `tmp/hivecode-0.0.0.8.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivecode-0.0.0.8.22.tar", last modified: Sat Jul 29 06:04:04 2023, max compression
+gzip compressed data, was "hivecode-0.0.0.8.23.tar", last modified: Mon Jul 31 00:24:26 2023, max compression
```

## Comparing `hivecode-0.0.0.8.22.tar` & `hivecode-0.0.0.8.23.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.443242 hivecode-0.0.0.8.22/
--rw-rw-rw-   0        0        0     3790 2023-07-29 06:04:04.443242 hivecode-0.0.0.8.22/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.22/README.rst
--rw-rw-rw-   0        0        0     1402 2023-07-29 06:03:23.000000 hivecode-0.0.0.8.22/pyproject.toml
--rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.22/requirements.txt
--rw-rw-rw-   0        0        0     1182 2023-07-29 06:04:04.447003 hivecode-0.0.0.8.22/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.339204 hivecode-0.0.0.8.22/src/
-drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.355309 hivecode-0.0.0.8.22/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.22/src/hiveadb/eda.py
--rw-rw-rw-   0        0        0    11930 2023-07-29 05:56:28.000000 hivecode-0.0.0.8.22/src/hiveadb/function.py
--rw-rw-rw-   0        0        0     3694 2023-07-26 06:36:39.000000 hivecode-0.0.0.8.22/src/hiveadb/functions.py
--rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.22/src/hiveadb/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.398388 hivecode-0.0.0.8.22/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     3790 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      314 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-29 06:04:04.000000 hivecode-0.0.0.8.22/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.432158 hivecode-0.0.0.8.22/src/hivecore/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.22/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.22/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.22/src/hivecore/eda.py
--rw-rw-rw-   0        0        0    10008 2023-07-29 05:36:22.000000 hivecode-0.0.0.8.22/src/hivecore/functions.py
--rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.22/src/hivecore/patterns.py
--rw-rw-rw-   0        0        0    28728 2023-07-20 03:05:40.000000 hivecode-0.0.0.8.22/src/hivecore/preprocess.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivecore/py.typed
--rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.22/src/hivecore/visual.py
-drwxrwxrwx   0        0        0        0 2023-07-29 06:04:04.441684 hivecode-0.0.0.8.22/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/eda.py
--rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.22/src/hivesignal/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.850968 hivecode-0.0.0.8.23/
+-rw-rw-rw-   0        0        0     3790 2023-07-31 00:24:26.851467 hivecode-0.0.0.8.23/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.23/README.rst
+-rw-rw-rw-   0        0        0     1402 2023-07-31 00:24:05.000000 hivecode-0.0.0.8.23/pyproject.toml
+-rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.23/requirements.txt
+-rw-rw-rw-   0        0        0     1182 2023-07-31 00:24:26.852973 hivecode-0.0.0.8.23/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.794349 hivecode-0.0.0.8.23/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.811809 hivecode-0.0.0.8.23/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.23/src/hiveadb/eda.py
+-rw-rw-rw-   0        0        0    11930 2023-07-29 05:56:28.000000 hivecode-0.0.0.8.23/src/hiveadb/function.py
+-rw-rw-rw-   0        0        0     3706 2023-07-30 23:57:54.000000 hivecode-0.0.0.8.23/src/hiveadb/functions.py
+-rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.23/src/hiveadb/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.828878 hivecode-0.0.0.8.23/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3790 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      314 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-31 00:24:26.000000 hivecode-0.0.0.8.23/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.845456 hivecode-0.0.0.8.23/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.23/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.23/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.23/src/hivecore/eda.py
+-rw-rw-rw-   0        0        0    11298 2023-07-30 23:04:15.000000 hivecode-0.0.0.8.23/src/hivecore/functions.py
+-rw-rw-rw-   0        0        0        0 2023-07-30 23:46:14.000000 hivecode-0.0.0.8.23/src/hivecore/legacy_preprocess.py
+-rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.23/src/hivecore/patterns.py
+-rw-rw-rw-   0        0        0    31989 2023-07-30 23:56:16.000000 hivecode-0.0.0.8.23/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivecore/py.typed
+-rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.23/src/hivecore/visual.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:24:26.850466 hivecode-0.0.0.8.23/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.23/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.22/PKG-INFO` & `hivecode-0.0.0.8.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.22
+Version: 0.0.0.8.23
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.22/README.rst` & `hivecode-0.0.0.8.23/README.rst`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/pyproject.toml` & `hivecode-0.0.0.8.23/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hivecode"
 description = "Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell."
-version = "0.0.0.8.22"
+version = "0.0.0.8.23"
 requires-python = ">=3.8.0"
 readme = "README.rst"
 authors = [
     {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
     {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
```

### Comparing `hivecode-0.0.0.8.22/setup.cfg` & `hivecode-0.0.0.8.23/setup.cfg`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hiveadb/eda.py` & `hivecode-0.0.0.8.23/src/hiveadb/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hiveadb/function.py` & `hivecode-0.0.0.8.23/src/hiveadb/function.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hiveadb/functions.py` & `hivecode-0.0.0.8.23/src/hiveadb/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union, Any
 
-from hivecore.functions import lib_required
+from hivecore.functions import lib_required, LazyImport
 
 from pyspark.context import SparkContext
 from pyspark.sql.session import SparkSession
 
 # DBUtils
 try:
     # up to DBR 8.2
```

### Comparing `hivecode-0.0.0.8.22/src/hiveadb/io.py` & `hivecode-0.0.0.8.23/src/hiveadb/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivecode.egg-info/PKG-INFO` & `hivecode-0.0.0.8.23/src/hivecode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.22
+Version: 0.0.0.8.23
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.22/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.23/src/hivecode.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/hivecode.egg-info/requires.txt
 src/hivecode.egg-info/top_level.txt
 src/hivecore/__init__.py
 src/hivecore/constant.py
 src/hivecore/decorator.py
 src/hivecore/eda.py
 src/hivecore/functions.py
+src/hivecore/legacy_preprocess.py
 src/hivecore/patterns.py
 src/hivecore/preprocess.py
 src/hivecore/py.typed
 src/hivecore/visual.py
 src/hivesignal/__init__.py
 src/hivesignal/analysis.py
 src/hivesignal/eda.py
```

### Comparing `hivecode-0.0.0.8.22/src/hivecore/constant.py` & `hivecode-0.0.0.8.23/src/hivecore/constant.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivecore/decorator.py` & `hivecode-0.0.0.8.23/src/hivecore/decorator.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivecore/eda.py` & `hivecode-0.0.0.8.23/src/hivecore/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivecore/functions.py` & `hivecode-0.0.0.8.23/src/hivecore/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import pydoc
 from os import system, getpid
 import hashlib
 import uuid
 from typing import Union, Optional, List, Any
 from pandas import Series
-from pyspark.sql.column import Column
 from psutil import Process
-from hivecore.patterns import singleton
 from importlib import import_module
 from warnings import warn
 
+from hivecore.patterns import singleton
+
+from pyspark.sql import SparkSession, DataFrame
+from pyspark.sql.column import Column
+from pyspark.sql.window import Window
+from pyspark.sql.functions import monotonically_increasing_id, row_number
 
 def get_memory_usage() -> float:
     """
     Get the current memory usage of the process.
     
     :return: The current memory usage in megabytes.
     :rtype: float
     """
     process = Process(getpid())
     megabytes = process.memory_info().rss / (1024 * 1024)
     return megabytes
 
 
-
-
 class ImportPromise:
     """
     A class that acts as a placeholder for an import.
     """
     def __init__(self, module: str, item: Optional[str] = None):
         """
         Initialize the ImportPromise with the module and item names.
@@ -279,8 +281,37 @@
     hash_bytes = hashlib.md5(seed_str).digest()
     
     # Generate UUID using the hash bytes and node value, then format and return the key
     namespace = uuid.UUID(int=uuid.getnode()).hex
     random_uuid = str(uuid.uuid5(uuid.UUID(bytes=hash_bytes), namespace)).replace('-', '')
     key = ''.join(c for c in random_uuid if c in chars)
     
-    return key
+    return key
+
+
+def pyspark_concat(left: DataFrame, right: DataFrame, axis: int = 0) -> DataFrame:
+    """
+    Concatenate two PySpark DataFrames along the specified axis.
+
+    :param left: The first PySpark DataFrame.
+    :type left: DataFrame
+    :param right: The second PySpark DataFrame to concatenate with `left`.
+    :type right: DataFrame
+    :param axis: The axis along which the DataFrames will be concatenated. Possible values: 0 or 1. Default is 0.
+    :type axis: int
+
+    :return: The concatenated PySpark DataFrame.
+    :rtype: DataFrame
+
+    :raises ValueError: If an invalid axis is provided.
+    """
+    if axis == 0:
+        return left.union(right)
+    elif axis == 1:
+        # Add a unique ID to each DataFrame to use for joining
+        left = left.withColumn("_row_id", row_number().over(Window.orderBy(monotonically_increasing_id())))
+        right = right.withColumn("_row_id", row_number().over(Window.orderBy(monotonically_increasing_id())))
+
+        # Join
+        return left.join(right, on="_row_id").drop("_row_id")
+    else:
+        raise ValueError("Invalid axis. Use 0 or 1.")
```

### Comparing `hivecode-0.0.0.8.22/src/hivecore/patterns.py` & `hivecode-0.0.0.8.23/src/hivecore/patterns.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivecore/visual.py` & `hivecode-0.0.0.8.23/src/hivecore/visual.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.23/src/hivesignal/analysis.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivesignal/io.py` & `hivecode-0.0.0.8.23/src/hivesignal/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.22/src/hivesignal/transform.py` & `hivecode-0.0.0.8.23/src/hivesignal/transform.py`

 * *Files identical despite different names*

