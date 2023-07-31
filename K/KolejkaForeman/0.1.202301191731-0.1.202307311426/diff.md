# Comparing `tmp/KolejkaForeman-0.1.202301191731-py3-none-any.whl.zip` & `tmp/KolejkaForeman-0.1.202307311426-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6015 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      544 b- defN 23-Jan-19 17:33 KolejkaForeman-0.1.202301191731-nspkg.pth
+Zip file size: 6235 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      544 b- defN 23-Jul-31 14:29 KolejkaForeman-0.1.202307311426-nspkg.pth
 -rw-rw-r--  2.0 unx     1012 b- defN 23-Jan-19 17:32 kolejka/foreman/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 18:28 kolejka/foreman/__nonpath__.py
--rw-rw-r--  2.0 unx    11842 b- defN 23-Jan-19 17:32 kolejka/foreman/foreman.py
--rw-rw-r--  2.0 unx      548 b- defN 23-Jan-19 17:33 KolejkaForeman-0.1.202301191731.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-19 17:33 KolejkaForeman-0.1.202301191731.dist-info/WHEEL
--rw-rw-r--  2.0 unx       58 b- defN 23-Jan-19 17:33 KolejkaForeman-0.1.202301191731.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaForeman-0.1.202301191731.dist-info/namespace_packages.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaForeman-0.1.202301191731.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      948 b- defN 23-Jan-19 17:33 KolejkaForeman-0.1.202301191731.dist-info/RECORD
-10 files, 15060 bytes uncompressed, 4341 bytes compressed:  71.2%
+-rw-rw-r--  2.0 unx    13532 b- defN 23-Jul-31 14:28 kolejka/foreman/foreman.py
+-rw-rw-r--  2.0 unx      548 b- defN 23-Jul-31 14:29 KolejkaForeman-0.1.202307311426.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 14:29 KolejkaForeman-0.1.202307311426.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       58 b- defN 23-Jul-31 14:29 KolejkaForeman-0.1.202307311426.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaForeman-0.1.202307311426.dist-info/namespace_packages.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaForeman-0.1.202307311426.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      948 b- defN 23-Jul-31 14:29 KolejkaForeman-0.1.202307311426.dist-info/RECORD
+10 files, 16750 bytes uncompressed, 4561 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: KolejkaForeman-0.1.202301191731-nspkg.pth
+Filename: KolejkaForeman-0.1.202307311426-nspkg.pth
 Comment: 
 
 Filename: kolejka/foreman/__init__.py
 Comment: 
 
 Filename: kolejka/foreman/__nonpath__.py
 Comment: 
 
 Filename: kolejka/foreman/foreman.py
 Comment: 
 
-Filename: KolejkaForeman-0.1.202301191731.dist-info/METADATA
+Filename: KolejkaForeman-0.1.202307311426.dist-info/METADATA
 Comment: 
 
-Filename: KolejkaForeman-0.1.202301191731.dist-info/WHEEL
+Filename: KolejkaForeman-0.1.202307311426.dist-info/WHEEL
 Comment: 
 
-Filename: KolejkaForeman-0.1.202301191731.dist-info/entry_points.txt
+Filename: KolejkaForeman-0.1.202307311426.dist-info/entry_points.txt
 Comment: 
 
-Filename: KolejkaForeman-0.1.202301191731.dist-info/namespace_packages.txt
+Filename: KolejkaForeman-0.1.202307311426.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: KolejkaForeman-0.1.202301191731.dist-info/top_level.txt
+Filename: KolejkaForeman-0.1.202307311426.dist-info/top_level.txt
 Comment: 
 
-Filename: KolejkaForeman-0.1.202301191731.dist-info/RECORD
+Filename: KolejkaForeman-0.1.202307311426.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolejka/foreman/foreman.py

```diff
@@ -20,15 +20,15 @@
 import traceback
 from threading import Thread
 import time
 import uuid
 
 from kolejka.common import kolejka_config, foreman_config
 from kolejka.common import KolejkaTask, KolejkaResult, KolejkaLimits
-from kolejka.common import MemoryAction, TimeAction, parse_memory
+from kolejka.common import MemoryAction, TimeAction, BigIntAction
 from kolejka.client import KolejkaClient
 from kolejka.common.gpu import gpu_stats
 from kolejka.common.images import (
     pull_docker_image,
     get_docker_image_size,
     check_docker_image_existance,
     list_docker_images,
@@ -123,14 +123,18 @@
     limits.pids = config.pids
     limits.storage = config.storage
     limits.image = config.image
     limits.workspace = config.workspace
     limits.time = config.time
     limits.network = config.network
     limits.gpus = config.gpus
+    limits.perf_instructions = config.perf_instructions
+    limits.perf_cycles = config.perf_cycles
+    limits.cgroup_depth = config.cgroup_depth
+    limits.cgroup_descendants = config.cgroup_descendants
     if limits.gpus is None:
         limits.gpus = len(gstats)
     limits.gpu_memory = config.gpu_memory
     for k,v in gstats.items():
         if limits.gpu_memory is None:
             limits.gpu_memory = v.memory_total
         elif v.memory_total is not None:
@@ -179,14 +183,22 @@
                             ok = False
                         if resources.image is not None:
                             image_usage_add = max(image_usage.get(task.image, 0), task.limits.image) - image_usage.get(task.image, 0)
                             if image_usage_add > resources.image:
                                 ok = False
                         if resources.workspace is not None and task.limits.workspace > resources.workspace:
                             ok = False
+                        if resources.perf_instructions is not None and task.limits.perf_instructions > resources.perf_instructions:
+                            ok = False
+                        if resources.perf_cycles is not None and task.limits.perf_cycles > resources.perf_cycles:
+                            ok = False
+                        if resources.cgroup_depth is not None and task.limits.cgroup_depth > resources.cgroup_depth:
+                            ok = False
+                        if resources.cgroup_descendants is not None and task.limits.cgroup_descendants > resources.cgroup_descendants:
+                            ok = False
                         if ok:
                             children_args.append([config.temp_path, task])
                             cpus_offset += task.limits.cpus
                             if resources.cpus is not None:
                                 resources.cpus -= task.limits.cpus
                             if resources.gpus is not None and task.limits.gpus is not None:
                                 resources.gpus -= task.limits.gpus
@@ -200,14 +212,20 @@
                             if resources.storage is not None:
                                 resources.storage -= task.limits.storage
                             if resources.image is not None:
                                 resources.image -= image_usage_add
                                 image_usage[task.image] = max(image_usage.get(task.image, 0), task.limits.image)
                             if resources.workspace is not None:
                                 resources.workspace -= task.limits.workspace
+                            if resources.perf_instructions is not None:
+                                resources.perf_instructions -= task.limits.perf_instructions
+                            if resources.perf_cycles is not None:
+                                resources.perf_cycles -= task.limits.perf_cycles
+                            if resources.cgroup_descendants is not None:
+                                resources.cgroup_descendants -= task.limits.cgroup_descendants
                             if task.limits.time is None:
                                 tasks_timeout = -1
                             else:
                                 if tasks_timeout is None:
                                     tasks_timeout = task.limits.time.total_seconds()
                                 else:
                                     tasks_timeout = max(task.limits.time.total_seconds(), tasks_timeout)
@@ -253,11 +271,15 @@
     parser.add_argument('--storage', action=MemoryAction, help='storage limit')
     parser.add_argument('--image', action=MemoryAction, help='image size limit')
     parser.add_argument('--workspace', action=MemoryAction, help='workspace size limit')
     parser.add_argument('--time', action=TimeAction, help='time limit')
     parser.add_argument('--network', type=bool, help='allow netowrking')
     parser.add_argument('--gpus', type=int, help='gpus limit')
     parser.add_argument('--gpu-memory', type=MemoryAction, help='gpu memory limit')
+    parser.add_argument('--perf-instructions', type=BigIntAction, help='CPU instructions limit')
+    parser.add_argument('--perf-cycles', type=BigIntAction, help='CPU cycles limit')
+    parser.add_argument('--cgroup-depth', type=int, help='Cgroup depth limit')
+    parser.add_argument('--cgroup-descendants', type=int, help='Cgroup descendants limit')
     def execute(args):
         kolejka_config(args=args)
         foreman()
     parser.set_defaults(execute=execute)
```

## Comparing `KolejkaForeman-0.1.202301191731-nspkg.pth` & `KolejkaForeman-0.1.202307311426-nspkg.pth`

 * *Files identical despite different names*

## Comparing `KolejkaForeman-0.1.202301191731.dist-info/METADATA` & `KolejkaForeman-0.1.202307311426.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KolejkaForeman
-Version: 0.1.202301191731
+Version: 0.1.202307311426
 Summary: Kolejka Foreman
 Home-page: https://github.com/kolejka/kolejka
 Author: KOLEJKA
 Author-email: kolejka@matinf.uj.edu.pl
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

