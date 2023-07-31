# Comparing `tmp/KolejkaWorker-0.1.202301191731-py3-none-any.whl.zip` & `tmp/KolejkaWorker-0.1.202307311426-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 13061 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      544 b- defN 23-Jan-19 17:33 KolejkaWorker-0.1.202301191731-nspkg.pth
+Zip file size: 13649 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      544 b- defN 23-Jul-31 14:29 KolejkaWorker-0.1.202307311426-nspkg.pth
 -rw-rw-r--  2.0 unx     1514 b- defN 23-Jan-19 17:32 kolejka/worker/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 18:28 kolejka/worker/__nonpath__.py
 -rw-r--r--  2.0 unx     1831 b- defN 19-May-27 12:49 kolejka/worker/create_alpine_python3_volume.sh
--rw-rw-r--  2.0 unx    13752 b- defN 22-Nov-13 18:28 kolejka/worker/stage0.py
+-rw-rw-r--  2.0 unx    14308 b- defN 23-Jul-31 14:28 kolejka/worker/stage0.py
 -rwxr-xr-x  2.0 unx      342 b- defN 19-May-27 12:49 kolejka/worker/stage1.sh
--rw-rw-r--  2.0 unx    15754 b- defN 22-Nov-13 18:28 kolejka/worker/stage2.py
+-rw-rw-r--  2.0 unx    19285 b- defN 23-Jul-31 14:28 kolejka/worker/stage2.py
 -rw-rw-r--  2.0 unx     1730 b- defN 23-Jan-19 17:32 kolejka/worker/volume.py
--rw-rw-r--  2.0 unx      550 b- defN 23-Jan-19 17:33 KolejkaWorker-0.1.202301191731.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-19 17:33 KolejkaWorker-0.1.202301191731.dist-info/WHEEL
--rw-rw-r--  2.0 unx       56 b- defN 23-Jan-19 17:33 KolejkaWorker-0.1.202301191731.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaWorker-0.1.202301191731.dist-info/namespace_packages.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jan-19 17:33 KolejkaWorker-0.1.202301191731.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1283 b- defN 23-Jan-19 17:33 KolejkaWorker-0.1.202301191731.dist-info/RECORD
-14 files, 37464 bytes uncompressed, 10869 bytes compressed:  71.0%
+-rw-rw-r--  2.0 unx      550 b- defN 23-Jul-31 14:29 KolejkaWorker-0.1.202307311426.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 14:29 KolejkaWorker-0.1.202307311426.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jul-31 14:29 KolejkaWorker-0.1.202307311426.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaWorker-0.1.202307311426.dist-info/namespace_packages.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaWorker-0.1.202307311426.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1283 b- defN 23-Jul-31 14:29 KolejkaWorker-0.1.202307311426.dist-info/RECORD
+14 files, 41551 bytes uncompressed, 11457 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: KolejkaWorker-0.1.202301191731-nspkg.pth
+Filename: KolejkaWorker-0.1.202307311426-nspkg.pth
 Comment: 
 
 Filename: kolejka/worker/__init__.py
 Comment: 
 
 Filename: kolejka/worker/__nonpath__.py
 Comment: 
@@ -18,26 +18,26 @@
 
 Filename: kolejka/worker/stage2.py
 Comment: 
 
 Filename: kolejka/worker/volume.py
 Comment: 
 
-Filename: KolejkaWorker-0.1.202301191731.dist-info/METADATA
+Filename: KolejkaWorker-0.1.202307311426.dist-info/METADATA
 Comment: 
 
-Filename: KolejkaWorker-0.1.202301191731.dist-info/WHEEL
+Filename: KolejkaWorker-0.1.202307311426.dist-info/WHEEL
 Comment: 
 
-Filename: KolejkaWorker-0.1.202301191731.dist-info/entry_points.txt
+Filename: KolejkaWorker-0.1.202307311426.dist-info/entry_points.txt
 Comment: 
 
-Filename: KolejkaWorker-0.1.202301191731.dist-info/namespace_packages.txt
+Filename: KolejkaWorker-0.1.202307311426.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: KolejkaWorker-0.1.202301191731.dist-info/top_level.txt
+Filename: KolejkaWorker-0.1.202307311426.dist-info/top_level.txt
 Comment: 
 
-Filename: KolejkaWorker-0.1.202301191731.dist-info/RECORD
+Filename: KolejkaWorker-0.1.202307311426.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolejka/worker/stage0.py

```diff
@@ -56,14 +56,18 @@
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
         limits.gpus = len(gpu_stats().gpus)
     task.limits.update(limits)
 
     docker_task = f'kolejka_worker_{task.id}'
 
     docker_cleanup  = [
@@ -290,12 +294,16 @@
     parser.add_argument('--pids', type=int, help='pids limit')
     parser.add_argument('--storage', action=MemoryAction, help='storage limit')
     parser.add_argument('--image', action=MemoryAction, help='image size limit')
     parser.add_argument('--workspace', action=MemoryAction, help='workspace size limit')
     parser.add_argument('--time', action=TimeAction, help='time limit')
     parser.add_argument('--network', type=bool, help='allow netowrking')
     parser.add_argument('--gpus', type=int, help='gpus limit')
+    parser.add_argument('--perf-instructions', type=BigIntAction, help='CPU instructions limit')
+    parser.add_argument('--perf-cycles', type=BigIntAction, help='CPU cycles limit')
+    parser.add_argument('--cgroup-depth', type=int, help='Cgroup depth limit')
+    parser.add_argument('--cgroup-descendants', type=int, help='Cgroup descendants limit')
     def execute(args):
         kolejka_config(args=args)
         config = worker_config()
         stage0(args.task, args.result, temp_path=config.temp_path, consume_task_folder=args.consume)
     parser.set_defaults(execute=execute)
```

## kolejka/worker/stage2.py

```diff
@@ -71,14 +71,29 @@
             'M' : 60,
             's' : 1,
             'm' : 10**-3,
             'µ' : 10**-6,
             'n' : 10**-9,
         }))
 
+def parse_bigint(x):
+    if x is not None:
+        return int(round(parse_float_with_modifiers(x, {
+            'k' : 1000,
+            'K' : 1000,
+            'm' : 1000**2,
+            'M' : 1000**2,
+            'g' : 1000**3,
+            'G' : 1000**3,
+            't' : 1000**4,
+            'T' : 1000**4,
+            'p' : 1000**5,
+            'P' : 1000**5,
+        })))
+
 class MemoryAction(argparse.Action):
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         self.type = int
         if nargs is not None:
             raise ValueError("nargs not allowed")
         super().__init__(option_strings, dest, **kwargs)
     def __call__(self, parser, namespace, values, option_string=None):
@@ -89,53 +104,70 @@
         self.type = datetime.timedelta
         if nargs is not None:
             raise ValueError("nargs not allowed")
         super().__init__(option_strings, dest, **kwargs)
     def __call__(self, parser, namespace, values, option_string=None):
         setattr(namespace, self.dest, parse_time(values))
 
+class BigIntAction(argparse.Action):
+    def __init__(self, option_strings, dest, nargs=None, **kwargs):
+        self.type = int
+        if nargs is not None:
+            raise ValueError('nargs not allowed')
+        super().__init__(option_strings, dest, **kwargs)
+    def __call__(self, parser, namespace, values, option_string=None):
+        setattr(namespace, self.dest, parse_bigint(values))
+
 class HTTPUnixConnection(http.client.HTTPConnection):
     def _get_hostport(self, host, port):
         return (self.socket_path, None)
     def __init__(self, socket_path):
         self.socket_path = socket_path
         super().__init__(self, socket_path)
     def connect(self):
         self.sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         self.sock.connect(self.socket_path)
         if self._tunnel_host:
             self._tunnel()
 
-def observer_start(cpus, cpus_offset, memory, swap, pids, time):
+def observer_start(cpus, cpus_offset, memory, swap, pids, time, perf_instructions, perf_cycles, cgroup_depth, cgroup_descendants):
     if not os.path.exists(OBSERVER_SOCKET):
         logging.error('Limits enabled with no kolejka-observer socket present')
         sys.exit(0)
     conn = HTTPUnixConnection(OBSERVER_SOCKET)
     headers = dict()
     headers['Content-Type'] = 'application/json; charset=utf-8'
     headers['Content-Length'] = '2'
     conn.request('POST', 'attach', '{}', headers)
     with conn.getresponse() as response:
         response_body = json.loads(response.read().decode('utf-8'))
     session_id = response_body['session_id']
     secret = response_body['secret']
-    if cpus is not None or memory is not None or swap is not None or pids is not None: 
+    if cpus is not None or memory is not None or swap is not None or pids is not None or perf_instructions is not None or perf_cycles is not None or cgroup_depth is not None or cgroup_descendants is not None:
         limits = dict()
         if cpus is not None:
             limits['cpus'] = int(cpus)
         if cpus_offset is not None:
             limits['cpus_offset'] = int(cpus_offset)
         if memory is not None:
             limits['memory'] = int(memory)
         if swap is not None:
             limits['swap'] = int(swap)
         if pids is not None:
             limits['pids'] = int(pids)
         if time is not None:
             limits['time'] = float(time.total_seconds()) 
+        if perf_instructions is not None:
+            limits['perf_instructions'] = int(perf_instructions)
+        if perf_cycles is not None:
+            limits['perf_cycles'] = int(perf_cycles)
+        if cgroup_depth is not None:
+            limits['cgroup_depth'] = int(cgroup_depth)
+        if cgroup_descendants is not None:
+            limits['cgroup_descendants'] = int(cgroup_descendants)
         params = dict()
         params['limits'] = limits
         params['session_id'] = session_id
         params['secret'] = secret
         body = bytes(json.dumps(params), 'utf-8')
         headers['Content-Length'] = str(len(body))
         conn.request('POST', 'limits', body, headers)
@@ -162,15 +194,15 @@
     conn.request('POST', 'detach', body, headers)
     conn.getresponse()
     conn.request('POST', 'close', body, headers)
     conn.getresponse()
     conn.close()
     return response_body
 
-def stage2(task_path, result_path, consume, cpus=None, cpus_offset=None, memory=None, swap=None, pids=None, time=None):
+def stage2(task_path, result_path, consume, cpus=None, cpus_offset=None, memory=None, swap=None, pids=None, time=None, perf_instructions=None, perf_cycles=None, cgroup_depth=None, cgroup_descendants=None):
     if not os.path.isdir(task_path):
         logging.error('Provided task path is not a directory')
         sys.exit(1)
     if not os.path.isdir(result_path):
         logging.error('Provided result path is not a directory')
         sys.exit(1)
     if os.listdir(result_path):
@@ -206,28 +238,40 @@
     task_args = task.get('args', [ 'true' ])
     task_cpus = parse_int(task.get('limits', dict()).get('cpus', None))
     task_cpus_offset = parse_int(task.get('limits', dict()).get('cpus_offset', None))
     task_memory = parse_memory(task.get('limits', dict()).get('memory', None))
     task_swap = parse_memory(task.get('limits', dict()).get('swap', None))
     task_pids = parse_int(task.get('limits', dict()).get('pids', None))
     task_time = parse_time(task.get('limits', dict()).get('time', None))
+    task_perf_instructions = parse_bigint(task.get('limits', dict()).get('perf_instructions', None))
+    task_perf_cycles = parse_bigint(task.get('limits', dict()).get('perf_cycles', None))
+    task_cgroup_depth = parse_int(task.get('limits', dict()).get('cgroup_depth', None))
+    task_cgroup_descendants = parse_int(task.get('limits', dict()).get('cgroup_descendants', None))
     task_env = task.get('environment', dict())
 
     if task_cpus is not None and (cpus is None or task_cpus < cpus):
         cpus = task_cpus
     if task_cpus_offset is not None and (cpus_offset is None):
         cpus_offset = task_cpus_offset
     if task_memory is not None and (memory is None or task_memory < memory):
         memory = task_memory
     if task_swap is not None and (swap is None or task_swap < swap):
         swap = task_swap
     if task_pids is not None and (pids is None or task_pids < pids):
         pids = task_pids
     if task_time is not None and (time is None or task_time.total_seconds() < time.total_seconds()):
         time = task_time
+    if task_perf_instructions is not None and (perf_instructions is None or task_perf_instructions < perf_instructions):
+        perf_instructions = task_perf_instructions
+    if task_perf_cycles is not None and (perf_cycles is None or task_perf_cycles < perf_cycles):
+        perf_cycles = task_perf_cycles
+    if task_cgroup_depth is not None and (cgroup_depth is None or task_cgroup_depth < cgroup_depth):
+        cgroup_depth = task_cgroup_depth
+    if task_cgroup_descendants is not None and (cgroup_descendants is None or task_cgroup_descendants < cgroup_descendants):
+        cgroup_descendants = task_cgroup_descendants
     
     summary = dict()
     summary['files'] = dict()
     summary_spec_path = os.path.join(result_path, RESULT_SPEC)
     for field in [ 'id', 'stdout', 'stderr' ]:
         if field in task:
             summary[field] = task[field]
@@ -240,21 +284,29 @@
         summary['limits']['memory'] = memory
     if swap is not None:
         summary['limits']['swap'] = swap
     if pids is not None:
         summary['limits']['pids'] = pids
     if time is not None:
         summary['limits']['time'] = time.total_seconds()
+    if perf_instructions is not None:
+        summary['limits']['perf_instructions'] = perf_instructions
+    if perf_cycles is not None:
+        summary['limits']['perf_cycles'] = perf_cycles
+    if cgroup_depth is not None:
+        summary['limits']['cgroup_depth'] = cgroup_depth
+    if cgroup_descendants is not None:
+        summary['limits']['cgroup_descendants'] = cgroup_descendants
 
     observer = None
     if os.path.exists(OBSERVER_SOCKET):
-        observer = observer_start(cpus, cpus_offset, memory, swap, pids, time)
+        observer = observer_start(cpus, cpus_offset, memory, swap, pids, time, perf_instructions, perf_cycles, cgroup_depth, cgroup_descendants)
         logging.info('Using Kolejka Observer to limit task and collect stats.')
     else:
-        if cpus is not None or memory is not None or swap is not None or pids is not None or time is not None:
+        if cpus is not None or memory is not None or swap is not None or pids is not None or time is not None or perf_instructions is not None or perf_cycles is not None or cgroup_depth is not None or cgroup_descendants is not None:
             logging.error('Can\'t limit task without Kolejka Observer running.')
             sys.exit(1)
 
     stdin_path = '/dev/null'
     stdout_path = '/dev/stdout'
     stderr_path = '/dev/stderr'
     if task_stdin is not None:
@@ -378,16 +430,20 @@
     parser.add_argument("--consume", action="store_true", default=False, help='consume task folder') 
     parser.add_argument('--cpus', type=int, help='cpus limit')
     parser.add_argument('--cpus-offset', type=int, help='cpus limit')
     parser.add_argument('--memory', action=MemoryAction, help='memory limit')
     parser.add_argument('--swap', action=MemoryAction, help='swap limit')
     parser.add_argument('--pids', type=int, help='pids limit')
     parser.add_argument('--time', action=TimeAction, help='time limit')
+    parser.add_argument('--perf-instructions', type=BigIntAction, help='CPU instructions limit')
+    parser.add_argument('--perf-cycles', type=BigIntAction, help='CPU cycles limit')
+    parser.add_argument('--cgroup-depth', type=int, help='Cgroup depth limit')
+    parser.add_argument('--cgroup-descendants', type=int, help='Cgroup descendants limit')
     def execute(args):
-        stage2(args.task, args.result, args.consume, cpus=args.cpus, cpus_offset=args.cpus_offset, memory=args.memory, swap=args.swap, pids=args.pids, time=args.time)
+        stage2(args.task, args.result, args.consume, cpus=args.cpus, cpus_offset=args.cpus_offset, memory=args.memory, swap=args.swap, pids=args.pids, time=args.time, perf_instructions=args.perf_instructions, perf_cycles=args.perf_cycles, cgroup_depth=args.cgroup_depth, cgroup_descendants=args.cgroup_descendants)
     parser.set_defaults(execute=execute)
 
 def main():
     import argparse
     import logging
 
     parser = argparse.ArgumentParser(description='KOLEJKA worker')
```

## Comparing `KolejkaWorker-0.1.202301191731-nspkg.pth` & `KolejkaWorker-0.1.202307311426-nspkg.pth`

 * *Files identical despite different names*

## Comparing `KolejkaWorker-0.1.202301191731.dist-info/METADATA` & `KolejkaWorker-0.1.202307311426.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KolejkaWorker
-Version: 0.1.202301191731
+Version: 0.1.202307311426
 Summary: Kolejka Worker
 Home-page: https://github.com/kolejka/kolejka
 Author: KOLEJKA
 Author-email: kolejka@matinf.uj.edu.pl
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `KolejkaWorker-0.1.202301191731.dist-info/RECORD` & `KolejkaWorker-0.1.202307311426.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-KolejkaWorker-0.1.202301191731-nspkg.pth,sha256=ymghxcR0SaoJPJNC5JQSPrO2foeCxLaTaJ0CvL2Q_H4,544
+KolejkaWorker-0.1.202307311426-nspkg.pth,sha256=ymghxcR0SaoJPJNC5JQSPrO2foeCxLaTaJ0CvL2Q_H4,544
 kolejka/worker/__init__.py,sha256=Zp5v0DuTMpiHBGkIgT6uEocQb6chlfSwApEBQ9gkWqY,1514
 kolejka/worker/__nonpath__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolejka/worker/create_alpine_python3_volume.sh,sha256=tHOSlO4om5maEG-soqrxalwCHQ0QYvWQEYx8BdgclXQ,1831
-kolejka/worker/stage0.py,sha256=bPaJf-u3cPr6xxVl1sZEvV1Y5cd5fWA933ho_VDa7hk,13752
+kolejka/worker/stage0.py,sha256=BXecU5IQgsXmeqEBEioMY-xYIzjh8hORZoLOZ_NcYFA,14308
 kolejka/worker/stage1.sh,sha256=Byk9fsAiREsU5Wd7b1uL61S9Xbc6ogPXb-9tXfKKoC4,342
-kolejka/worker/stage2.py,sha256=ZZu63T1DtWDMrX4wIcd30DBQ1EOGv2PRKT4I-36WA4c,15754
+kolejka/worker/stage2.py,sha256=ynkA7Juj722JklEhocjhfEUH5cMHvwCDLPsY6z1mXXM,19285
 kolejka/worker/volume.py,sha256=T4V9AvwQZyIVtideuJWkngVstgXTgXHuJem4P1Qfb6k,1730
-KolejkaWorker-0.1.202301191731.dist-info/METADATA,sha256=IoMyHoLTDRH7xkJsivlk8Bz8xSEYY6006vH01MEU3zw,550
-KolejkaWorker-0.1.202301191731.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-KolejkaWorker-0.1.202301191731.dist-info/entry_points.txt,sha256=swtFIgFxghZFPsnkh53oN-BonHUw5yyHl8sl1IGvl3U,56
-KolejkaWorker-0.1.202301191731.dist-info/namespace_packages.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
-KolejkaWorker-0.1.202301191731.dist-info/top_level.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
-KolejkaWorker-0.1.202301191731.dist-info/RECORD,,
+KolejkaWorker-0.1.202307311426.dist-info/METADATA,sha256=h1T4AsrGJhq4vt-OHl8DVXe-CrhpHSNHrtX0rjkerp4,550
+KolejkaWorker-0.1.202307311426.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+KolejkaWorker-0.1.202307311426.dist-info/entry_points.txt,sha256=swtFIgFxghZFPsnkh53oN-BonHUw5yyHl8sl1IGvl3U,56
+KolejkaWorker-0.1.202307311426.dist-info/namespace_packages.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
+KolejkaWorker-0.1.202307311426.dist-info/top_level.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
+KolejkaWorker-0.1.202307311426.dist-info/RECORD,,
```

