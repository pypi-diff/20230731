# Comparing `tmp/mc_trimmer-0.1.0.tar.gz` & `tmp/mc_trimmer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc_trimmer-0.1.0.tar", last modified: Mon Jul 31 09:19:26 2023, max compression
+gzip compressed data, was "mc_trimmer-0.1.1.tar", last modified: Mon Jul 31 11:09:10 2023, max compression
```

## Comparing `mc_trimmer-0.1.0.tar` & `mc_trimmer-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 09:19:26.030845 mc_trimmer-0.1.0/
--rw-rw-rw-   0        0        0     1069 2023-07-22 16:39:55.000000 mc_trimmer-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2177 2023-07-31 09:19:26.029846 mc_trimmer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1947 2023-07-31 09:09:52.000000 mc_trimmer-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 09:19:25.964344 mc_trimmer-0.1.0/mc_trimmer/
--rw-rw-rw-   0        0        0      189 2023-07-30 10:41:28.000000 mc_trimmer-0.1.0/mc_trimmer/__init__.py
--rw-rw-rw-   0        0        0      122 2023-07-27 21:56:00.000000 mc_trimmer-0.1.0/mc_trimmer/__main__.py
--rw-rw-rw-   0        0        0       22 2023-07-25 17:48:13.000000 mc_trimmer-0.1.0/mc_trimmer/__version__.py
--rw-rw-rw-   0        0        0     2388 2023-07-31 08:37:24.000000 mc_trimmer-0.1.0/mc_trimmer/cli.py
--rw-rw-rw-   0        0        0     3552 2023-07-30 15:37:16.000000 mc_trimmer-0.1.0/mc_trimmer/entities.py
--rw-rw-rw-   0        0        0     5532 2023-07-31 08:25:48.000000 mc_trimmer-0.1.0/mc_trimmer/main.py
--rw-rw-rw-   0        0        0     9063 2023-07-30 16:30:41.000000 mc_trimmer-0.1.0/mc_trimmer/primitives.py
--rw-rw-rw-   0        0        0     4265 2023-07-30 15:37:02.000000 mc_trimmer-0.1.0/mc_trimmer/regions.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:19:26.020844 mc_trimmer-0.1.0/mc_trimmer/submodule/
--rw-rw-rw-   0        0        0       43 2023-07-25 17:43:02.000000 mc_trimmer-0.1.0/mc_trimmer/submodule/__init__.py
--rw-rw-rw-   0        0        0       56 2023-07-25 17:43:02.000000 mc_trimmer-0.1.0/mc_trimmer/submodule/subcomponent.py
-drwxrwxrwx   0        0        0        0 2023-07-31 09:19:26.005844 mc_trimmer-0.1.0/mc_trimmer.egg-info/
--rw-rw-rw-   0        0        0     2177 2023-07-31 09:19:25.000000 mc_trimmer-0.1.0/mc_trimmer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-07-31 09:19:25.000000 mc_trimmer-0.1.0/mc_trimmer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 09:19:25.000000 mc_trimmer-0.1.0/mc_trimmer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-31 09:19:25.000000 mc_trimmer-0.1.0/mc_trimmer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-07-31 09:19:25.000000 mc_trimmer-0.1.0/mc_trimmer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 09:19:25.000000 mc_trimmer-0.1.0/mc_trimmer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      984 2023-07-31 09:18:44.000000 mc_trimmer-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 09:19:26.030845 mc_trimmer-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 09:19:26.028843 mc_trimmer-0.1.0/tests/
--rw-rw-rw-   0        0        0     3081 2023-07-30 15:14:06.000000 mc_trimmer-0.1.0/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:09:10.570171 mc_trimmer-0.1.1/
+-rw-rw-rw-   0        0        0     1069 2023-07-22 16:39:55.000000 mc_trimmer-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2177 2023-07-31 11:09:10.569172 mc_trimmer-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1947 2023-07-31 09:09:52.000000 mc_trimmer-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 11:09:10.510670 mc_trimmer-0.1.1/mc_trimmer/
+-rw-rw-rw-   0        0        0      189 2023-07-30 10:41:28.000000 mc_trimmer-0.1.1/mc_trimmer/__init__.py
+-rw-rw-rw-   0        0        0      122 2023-07-27 21:56:00.000000 mc_trimmer-0.1.1/mc_trimmer/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-07-31 11:07:59.000000 mc_trimmer-0.1.1/mc_trimmer/__version__.py
+-rw-rw-rw-   0        0        0     2388 2023-07-31 08:37:24.000000 mc_trimmer-0.1.1/mc_trimmer/cli.py
+-rw-rw-rw-   0        0        0     3552 2023-07-30 15:37:16.000000 mc_trimmer-0.1.1/mc_trimmer/entities.py
+-rw-rw-rw-   0        0        0     6286 2023-07-31 11:06:48.000000 mc_trimmer-0.1.1/mc_trimmer/main.py
+-rw-rw-rw-   0        0        0     9061 2023-07-31 11:07:43.000000 mc_trimmer-0.1.1/mc_trimmer/primitives.py
+-rw-rw-rw-   0        0        0     4265 2023-07-30 15:37:02.000000 mc_trimmer-0.1.1/mc_trimmer/regions.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:09:10.560672 mc_trimmer-0.1.1/mc_trimmer/submodule/
+-rw-rw-rw-   0        0        0       43 2023-07-25 17:43:02.000000 mc_trimmer-0.1.1/mc_trimmer/submodule/__init__.py
+-rw-rw-rw-   0        0        0       56 2023-07-25 17:43:02.000000 mc_trimmer-0.1.1/mc_trimmer/submodule/subcomponent.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:09:10.545671 mc_trimmer-0.1.1/mc_trimmer.egg-info/
+-rw-rw-rw-   0        0        0     2177 2023-07-31 11:09:10.000000 mc_trimmer-0.1.1/mc_trimmer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-07-31 11:09:10.000000 mc_trimmer-0.1.1/mc_trimmer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:09:10.000000 mc_trimmer-0.1.1/mc_trimmer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-31 11:09:10.000000 mc_trimmer-0.1.1/mc_trimmer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-07-31 11:09:10.000000 mc_trimmer-0.1.1/mc_trimmer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 11:09:10.000000 mc_trimmer-0.1.1/mc_trimmer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      984 2023-07-31 09:18:44.000000 mc_trimmer-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:09:10.570171 mc_trimmer-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 11:09:10.568169 mc_trimmer-0.1.1/tests/
+-rw-rw-rw-   0        0        0     3081 2023-07-30 15:14:06.000000 mc_trimmer-0.1.1/tests/test_all.py
```

### Comparing `mc_trimmer-0.1.0/LICENSE` & `mc_trimmer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mc_trimmer-0.1.0/PKG-INFO` & `mc_trimmer-0.1.1/mc_trimmer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mc_trimmer
-Version: 0.1.0
+Name: mc-trimmer
+Version: 0.1.1
 Author: Thaodan
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MC-Trimmer
```

### Comparing `mc_trimmer-0.1.0/README.md` & `mc_trimmer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mc_trimmer-0.1.0/mc_trimmer/cli.py` & `mc_trimmer-0.1.1/mc_trimmer/cli.py`

 * *Files identical despite different names*

### Comparing `mc_trimmer-0.1.0/mc_trimmer/entities.py` & `mc_trimmer-0.1.1/mc_trimmer/entities.py`

 * *Files identical despite different names*

### Comparing `mc_trimmer-0.1.0/mc_trimmer/main.py` & `mc_trimmer-0.1.1/mc_trimmer/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import shutil
 from dataclasses import dataclass
 from functools import partial
+import sys
+import traceback
 from typing import Callable, Iterable
 
 from multiprocess.pool import Pool
 
 from mc_trimmer.entities import EntitiesFile, Entity
 from mc_trimmer.primitives import Paths, RegionLike
 from mc_trimmer.regions import Chunk, RegionFile
@@ -106,34 +108,49 @@
 
 def process_region(manager: RegionManager, criteria: Callable[[Chunk, Entity], bool], file_name: str):
     region: Region = manager.open_file(file_name=file_name)
     manager.trim(region=region, condition=criteria)
     manager.save_to_file(region=region, file_name=file_name)
 
 
-def process_batch(manager: RegionManager, criteria: str, file_names: list[str]):
+def process_batch(manager: RegionManager, criteria: str, file_names: list[str]) -> list[tuple[Exception, str]]:
     l = len(file_names)
+    exceptions: list[tuple[Exception, str]] = []
     for i, r in enumerate(file_names, start=1):
         print(f"Processing region {r} ({i}/{l})")
-        process_region(manager, CRITERIA_MAPPING[criteria], r)
+        try:
+            process_region(manager, CRITERIA_MAPPING[criteria], r)
+        except AssertionError as e:
+            e.add_note(f"[E]: AssertionError while processing {r}")
+            tb = str(traceback.extract_tb(sys.exc_info()[2]))
+            exceptions.append((e, tb))
+        except Exception as e:
+            e.add_note(f"[E]: Exception while processing {r}")
+            tb = str(traceback.extract_tb(sys.exc_info()[2]))
+            exceptions.append((e, tb))
+    return exceptions
 
 
 def main(*, threads: int | None, paths: Paths, trimming_criteria: str) -> None:
     rm = RegionManager(paths=paths)
     region_file_names: Iterable[str] = RegionLike.get_regions(paths.inp_region)
 
     if threads is None:
-        process_batch(
+        res = process_batch(
             manager=rm,
             criteria=trimming_criteria,
             file_names=list(region_file_names),
         )
+        for e, traceback in res:
+            print("\n".join(e.__notes__), e, traceback)
     else:
         work: list[list[str]] = [[] for _ in range(threads)]
         for i, r in enumerate(region_file_names):
             work[i % threads].append(r)
 
         foo = partial(process_batch, rm, trimming_criteria)
         with Pool(threads) as p:
             res = p.map(func=foo, iterable=work)
             pass
-        pass
+        for combo in res:
+            for e, traceback in combo:
+                print("\n".join(e.__notes__), e, traceback)
```

### Comparing `mc_trimmer-0.1.0/mc_trimmer/primitives.py` & `mc_trimmer-0.1.1/mc_trimmer/primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,18 +257,18 @@
             previous = cd.index
         bytes_to_add = bytearray(b"\x00\x00\x00\x00") * (1024 - previous - 1)
         locations += bytes_to_add
         timestamps += bytes_to_add
 
         l1 = len(timestamps)
         if l1 != 4096:
-            raise Exception(f"WTF: {l1} != 4096")
+            raise Exception(f"len {l1} != 4096")
         l2 = len(locations)
         if l2 != 4096:
-            raise Exception(f"WTF: {l1} != 4096")
+            raise Exception(f"len {l2} != 4096")
 
         return bytes(locations + timestamps + chunks)
 
 
 def fast_get_property(decompressed_data: bytes, name: bytes, strategy: Strategy[T]) -> T:
     """Quick-fetch property by seeking through the byte-stream.
```

### Comparing `mc_trimmer-0.1.0/mc_trimmer/regions.py` & `mc_trimmer-0.1.1/mc_trimmer/regions.py`

 * *Files identical despite different names*

### Comparing `mc_trimmer-0.1.0/mc_trimmer.egg-info/PKG-INFO` & `mc_trimmer-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mc-trimmer
-Version: 0.1.0
+Name: mc_trimmer
+Version: 0.1.1
 Author: Thaodan
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MC-Trimmer
```

### Comparing `mc_trimmer-0.1.0/pyproject.toml` & `mc_trimmer-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mc_trimmer-0.1.0/tests/test_all.py` & `mc_trimmer-0.1.1/tests/test_all.py`

 * *Files identical despite different names*

