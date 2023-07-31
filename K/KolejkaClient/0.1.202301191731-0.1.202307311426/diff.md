# Comparing `tmp/KolejkaClient-0.1.202301191731-py3-none-any.whl.zip` & `tmp/KolejkaClient-0.1.202307311426-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6413 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      544 b- defN 23-Jan-19 17:33 KolejkaClient-0.1.202301191731-nspkg.pth
+Zip file size: 6536 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      544 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426-nspkg.pth
 -rw-rw-r--  2.0 unx     1032 b- defN 23-Jan-19 17:32 kolejka/client/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 18:28 kolejka/client/__nonpath__.py
--rw-rw-r--  2.0 unx    17718 b- defN 22-Nov-13 18:28 kolejka/client/client.py
--rw-rw-r--  2.0 unx      535 b- defN 23-Jan-19 17:33 KolejkaClient-0.1.202301191731.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-19 17:33 KolejkaClient-0.1.202301191731.dist-info/WHEEL
--rw-rw-r--  2.0 unx       56 b- defN 23-Jan-19 17:33 KolejkaClient-0.1.202301191731.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaClient-0.1.202301191731.dist-info/namespace_packages.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaClient-0.1.202301191731.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      937 b- defN 23-Jan-19 17:33 KolejkaClient-0.1.202301191731.dist-info/RECORD
-10 files, 20930 bytes uncompressed, 4761 bytes compressed:  77.3%
+-rw-rw-r--  2.0 unx    18662 b- defN 23-Jul-31 14:28 kolejka/client/client.py
+-rw-rw-r--  2.0 unx      535 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/namespace_packages.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      937 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/RECORD
+10 files, 21874 bytes uncompressed, 4884 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: KolejkaClient-0.1.202301191731-nspkg.pth
+Filename: KolejkaClient-0.1.202307311426-nspkg.pth
 Comment: 
 
 Filename: kolejka/client/__init__.py
 Comment: 
 
 Filename: kolejka/client/__nonpath__.py
 Comment: 
 
 Filename: kolejka/client/client.py
 Comment: 
 
-Filename: KolejkaClient-0.1.202301191731.dist-info/METADATA
+Filename: KolejkaClient-0.1.202307311426.dist-info/METADATA
 Comment: 
 
-Filename: KolejkaClient-0.1.202301191731.dist-info/WHEEL
+Filename: KolejkaClient-0.1.202307311426.dist-info/WHEEL
 Comment: 
 
-Filename: KolejkaClient-0.1.202301191731.dist-info/entry_points.txt
+Filename: KolejkaClient-0.1.202307311426.dist-info/entry_points.txt
 Comment: 
 
-Filename: KolejkaClient-0.1.202301191731.dist-info/namespace_packages.txt
+Filename: KolejkaClient-0.1.202307311426.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: KolejkaClient-0.1.202301191731.dist-info/top_level.txt
+Filename: KolejkaClient-0.1.202307311426.dist-info/top_level.txt
 Comment: 
 
-Filename: KolejkaClient-0.1.202301191731.dist-info/RECORD
+Filename: KolejkaClient-0.1.202307311426.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolejka/client/client.py

```diff
@@ -196,14 +196,18 @@
         limits.pids = self.config.pids
         limits.storage = self.config.storage
         limits.image = self.config.image
         limits.workspace = self.config.workspace
         limits.time = self.config.time
         limits.network = self.config.network
         limits.gpus = self.config.gpus
+        limits.perf_instructions = self.config.perf_instructions
+        limits.perf_cycles = self.config.perf_cycles
+        limits.cgroup_depth = self.config.cgroup_depth
+        limits.cgroup_descendants = self.config.cgroup_descendants
         if limits.gpus is None:
             limits.gpus = task.limits.gpus
         limits.gpu_memory = self.config.gpu_memory
         task.limits.update(limits)
         if not self.instance_session:
             self.login() 
         for f in task.files.values():
@@ -331,14 +335,18 @@
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
         client = KolejkaClient()
         task = KolejkaTask(args.task)
         response = client.task_put(task)
         print(response.id)
     parser.set_defaults(execute=execute)
@@ -418,14 +426,18 @@
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
         client = KolejkaClient()
         task = KolejkaTask(args.task)
         response = client.task_put(task)
         while True:
             client.session.close()
```

## Comparing `KolejkaClient-0.1.202301191731-nspkg.pth` & `KolejkaClient-0.1.202307311426-nspkg.pth`

 * *Files identical despite different names*

## Comparing `KolejkaClient-0.1.202301191731.dist-info/METADATA` & `KolejkaClient-0.1.202307311426.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KolejkaClient
-Version: 0.1.202301191731
+Version: 0.1.202307311426
 Summary: Kolejka Client
 Home-page: https://github.com/kolejka/kolejka
 Author: KOLEJKA
 Author-email: kolejka@matinf.uj.edu.pl
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

