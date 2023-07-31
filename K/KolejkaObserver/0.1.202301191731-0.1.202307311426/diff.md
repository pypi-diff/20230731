# Comparing `tmp/KolejkaObserver-0.1.202301191731-py3-none-any.whl.zip` & `tmp/KolejkaObserver-0.1.202307311426-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11703 bytes, number of entries: 12
--rw-rw-r--  2.0 unx      544 b- defN 23-Jan-19 17:33 KolejkaObserver-0.1.202301191731-nspkg.pth
+Zip file size: 11763 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx      544 b- defN 23-Jul-31 14:29 KolejkaObserver-0.1.202307311426-nspkg.pth
 -rw-rw-r--  2.0 unx      191 b- defN 22-Nov-13 18:28 kolejka/observer/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 18:28 kolejka/observer/__nonpath__.py
 -rw-rw-r--  2.0 unx     2572 b- defN 22-Nov-13 18:28 kolejka/observer/client.py
--rw-rw-r--  2.0 unx     9621 b- defN 22-Nov-13 18:28 kolejka/observer/runner.py
+-rw-rw-r--  2.0 unx     9899 b- defN 23-Jul-31 14:28 kolejka/observer/runner.py
 -rw-rw-r--  2.0 unx    23389 b- defN 23-Jan-19 17:32 kolejka/observer/server.py
--rw-rw-r--  2.0 unx      528 b- defN 23-Jan-19 17:33 KolejkaObserver-0.1.202301191731.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-19 17:33 KolejkaObserver-0.1.202301191731.dist-info/WHEEL
--rw-rw-r--  2.0 unx      113 b- defN 23-Jan-19 17:33 KolejkaObserver-0.1.202301191731.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaObserver-0.1.202301191731.dist-info/namespace_packages.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaObserver-0.1.202301191731.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1123 b- defN 23-Jan-19 17:33 KolejkaObserver-0.1.202301191731.dist-info/RECORD
-12 files, 38189 bytes uncompressed, 9755 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx      528 b- defN 23-Jul-31 14:29 KolejkaObserver-0.1.202307311426.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 14:29 KolejkaObserver-0.1.202307311426.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      113 b- defN 23-Jul-31 14:29 KolejkaObserver-0.1.202307311426.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaObserver-0.1.202307311426.dist-info/namespace_packages.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaObserver-0.1.202307311426.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1123 b- defN 23-Jul-31 14:29 KolejkaObserver-0.1.202307311426.dist-info/RECORD
+12 files, 38467 bytes uncompressed, 9815 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: KolejkaObserver-0.1.202301191731-nspkg.pth
+Filename: KolejkaObserver-0.1.202307311426-nspkg.pth
 Comment: 
 
 Filename: kolejka/observer/__init__.py
 Comment: 
 
 Filename: kolejka/observer/__nonpath__.py
 Comment: 
@@ -12,26 +12,26 @@
 
 Filename: kolejka/observer/runner.py
 Comment: 
 
 Filename: kolejka/observer/server.py
 Comment: 
 
-Filename: KolejkaObserver-0.1.202301191731.dist-info/METADATA
+Filename: KolejkaObserver-0.1.202307311426.dist-info/METADATA
 Comment: 
 
-Filename: KolejkaObserver-0.1.202301191731.dist-info/WHEEL
+Filename: KolejkaObserver-0.1.202307311426.dist-info/WHEEL
 Comment: 
 
-Filename: KolejkaObserver-0.1.202301191731.dist-info/entry_points.txt
+Filename: KolejkaObserver-0.1.202307311426.dist-info/entry_points.txt
 Comment: 
 
-Filename: KolejkaObserver-0.1.202301191731.dist-info/namespace_packages.txt
+Filename: KolejkaObserver-0.1.202307311426.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: KolejkaObserver-0.1.202301191731.dist-info/top_level.txt
+Filename: KolejkaObserver-0.1.202307311426.dist-info/top_level.txt
 Comment: 
 
-Filename: KolejkaObserver-0.1.202301191731.dist-info/RECORD
+Filename: KolejkaObserver-0.1.202307311426.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolejka/observer/runner.py

```diff
@@ -142,14 +142,16 @@
 
     parser.add_argument('--cpus', type=int, help='cpus limit')
     parser.add_argument('--cpus-offset', type=int, help='cpus limit')
     parser.add_argument('--memory', action=MemoryAction, help='memory limit')
     parser.add_argument('--swap', action=MemoryAction, help='swap limit')
     parser.add_argument('--pids', type=int, help='pids limit')
     parser.add_argument('--time', action=TimeAction, help='time limit')
+    parser.add_argument('--perf-instructions', type=BigIntAction, help='CPU instructions limit')
+    parser.add_argument('--perf-cycles', type=BigIntAction, help='CPU cycles limit')
     parser.add_argument('args', nargs=argparse.REMAINDER, help='command line to run')
     args = parser.parse_args()
     level=logging.WARNING
     if args.verbose:
         level=logging.INFO
     if args.debug:
         level=logging.DEBUG
@@ -164,14 +166,16 @@
     limits = KolejkaLimits()
     limits.cpus = args.cpus
     limits.cpus_offset = args.cpus_offset
     limits.memory = args.memory
     limits.swap = args.swap
     limits.pids = args.pids
     limits.time = args.time
+    limits.perf_instructions = args.perf_instructions
+    limits.perf_cycles = args.perf_cycles
 
     env = dict(os.environ)
     kwargs = dict()
     uid = None
     user = None
     gid = None
     group = None
```

## Comparing `KolejkaObserver-0.1.202301191731-nspkg.pth` & `KolejkaObserver-0.1.202307311426-nspkg.pth`

 * *Files identical despite different names*

## Comparing `KolejkaObserver-0.1.202301191731.dist-info/METADATA` & `KolejkaObserver-0.1.202307311426.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KolejkaObserver
-Version: 0.1.202301191731
+Version: 0.1.202307311426
 Summary: Kolejka Observer Daemon
 Home-page: https://github.com/kolejka/kolejka
 Author: KOLEJKA
 Author-email: kolejka@matinf.uj.edu.pl
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

