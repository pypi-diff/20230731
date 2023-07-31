# Comparing `tmp/slurm_gpustat-0.0.8.tar.gz` & `tmp/slurm_gpustat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slurm_gpustat-0.0.8.tar", last modified: Thu Oct 29 15:39:04 2020, max compression
+gzip compressed data, was "dist/slurm_gpustat-0.0.9.tar", last modified: Sun Dec 20 17:13:34 2020, max compression
```

## Comparing `slurm_gpustat-0.0.8.tar` & `slurm_gpustat-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 albanie   (1177) albanie  (11177)        0 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/
--rw-rw-r--   0 albanie   (1177) albanie  (11177)     4131 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/PKG-INFO
--rw-rw-r--   0 albanie   (1177) albanie  (11177)     2898 2020-09-25 06:30:43.000000 slurm_gpustat-0.0.8/README.md
--rw-rw-r--   0 albanie   (1177) albanie  (11177)       38 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/setup.cfg
--rw-rw-r--   0 albanie   (1177) albanie  (11177)      940 2020-10-29 15:38:45.000000 slurm_gpustat-0.0.8/setup.py
-drwxrwxr-x   0 albanie   (1177) albanie  (11177)        0 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat/
--rw-rw-r--   0 albanie   (1177) albanie  (11177)    25709 2020-10-29 15:38:14.000000 slurm_gpustat-0.0.8/slurm_gpustat/slurm_gpustat.py
-drwxrwxr-x   0 albanie   (1177) albanie  (11177)        0 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat.egg-info/
--rw-rw-r--   0 albanie   (1177) albanie  (11177)     4131 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat.egg-info/PKG-INFO
--rw-rw-r--   0 albanie   (1177) albanie  (11177)      273 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat.egg-info/SOURCES.txt
--rw-rw-r--   0 albanie   (1177) albanie  (11177)        1 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat.egg-info/dependency_links.txt
--rw-rw-r--   0 albanie   (1177) albanie  (11177)       68 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat.egg-info/entry_points.txt
--rw-rw-r--   0 albanie   (1177) albanie  (11177)       31 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat.egg-info/requires.txt
--rw-rw-r--   0 albanie   (1177) albanie  (11177)       14 2020-10-29 15:39:04.000000 slurm_gpustat-0.0.8/slurm_gpustat.egg-info/top_level.txt
+drwxrwxr-x   0 albanie   (1177) albanie  (11177)        0 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)     4331 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/PKG-INFO
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)     3066 2020-12-20 17:10:41.000000 slurm_gpustat-0.0.9/README.md
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)       38 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/setup.cfg
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)      940 2020-12-20 17:13:20.000000 slurm_gpustat-0.0.9/setup.py
+drwxrwxr-x   0 albanie   (1177) albanie  (11177)        0 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat/
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)    27348 2020-12-20 17:12:36.000000 slurm_gpustat-0.0.9/slurm_gpustat/slurm_gpustat.py
+drwxrwxr-x   0 albanie   (1177) albanie  (11177)        0 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat.egg-info/
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)     4331 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat.egg-info/PKG-INFO
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)      273 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat.egg-info/SOURCES.txt
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)        1 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat.egg-info/dependency_links.txt
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)       68 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat.egg-info/entry_points.txt
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)       31 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat.egg-info/requires.txt
+-rw-rw-r--   0 albanie   (1177) albanie  (11177)       14 2020-12-20 17:13:34.000000 slurm_gpustat-0.0.9/slurm_gpustat.egg-info/top_level.txt
```

### Comparing `slurm_gpustat-0.0.8/PKG-INFO` & `slurm_gpustat-0.0.9/slurm_gpustat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: slurm_gpustat
-Version: 0.0.8
+Name: slurm-gpustat
+Version: 0.0.9
 Summary: A simple SLURM gpu summary tool
 Home-page: https://github.com/albanie/slurm_gpustat
 Author: Samuel Albanie
 License: UNKNOWN
 Description: ## slurm_gpustat
         
         `slurm_gpustat` is a simple command line utility that produces a summary of GPU usage on a slurm cluster. The tool can be used in two ways:
@@ -18,14 +18,18 @@
         
         ### Usage
         
         To print a summary of current activity:
         
         `slurm_gpustat`
         
+        To print a summary of current activity on particular partitions, e.g. `debug` & `normal`:
+        
+        `slurm_gpustat -p debug,normal` or `slurm_gpustat --partition debug,normal`
+        
         To start the logging dameon:
         
         `slurm_gpustat --action daemon-start`
         
         To view a summary of logged data:
         
         `slurm_gpustat --action history`
```

### Comparing `slurm_gpustat-0.0.8/README.md` & `slurm_gpustat-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 ### Usage
 
 To print a summary of current activity:
 
 `slurm_gpustat`
 
+To print a summary of current activity on particular partitions, e.g. `debug` & `normal`:
+
+`slurm_gpustat -p debug,normal` or `slurm_gpustat --partition debug,normal`
+
 To start the logging dameon:
 
 `slurm_gpustat --action daemon-start`
 
 To view a summary of logged data:
 
 `slurm_gpustat --action history`
```

### Comparing `slurm_gpustat-0.0.8/setup.py` & `slurm_gpustat-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name="slurm_gpustat",
-    version="0.0.8",
+    version="0.0.9",
     entry_points={
         "console_scripts": [
             "slurm_gpustat=slurm_gpustat.slurm_gpustat:main",
         ],
     },
     author="Samuel Albanie",
     description="A simple SLURM gpu summary tool",
```

### Comparing `slurm_gpustat-0.0.8/slurm_gpustat/slurm_gpustat.py` & `slurm_gpustat-0.0.9/slurm_gpustat/slurm_gpustat.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
    to provide simple usage statistics.
 """
 import argparse
 import ast
 import atexit
 import os
 import random
+import re
 import signal
 import subprocess
 import sys
 import time
 from collections import defaultdict
 from datetime import datetime
 from pathlib import Path
@@ -21,14 +22,15 @@
 import functools
 
 import colored
 import numpy as np
 import seaborn as sns
 
 from beartype import beartype
+from beartype.cave import NoneType
 
 # SLURM states which indicate that the node is not available for submitting jobs
 INACCESSIBLE = {"drain*", "down*", "drng", "drain", "down"}
 INTERACTIVE_CMDS = {"bash", "zsh", "sh"}
 
 class Daemon:
     """A Generic linux daemon base class for python 3.x.
@@ -343,21 +345,27 @@
     output = subprocess.check_output(cmd, shell=True).decode("utf-8")
     if split:
         output = [x for x in output.split("\n") if x]
     return output
 
 
 @beartype
-def node_states() -> dict:
+def node_states(partition: (str, NoneType) = None) -> dict:
     """Query SLURM for the state of each managed node.
 
+    Args:
+        partition: the partition/queue (or multiple, comma separated) of interest.
+            By default None, which queries all available partitions.
+
     Returns:
         a mapping between node names and SLURM states.
     """
     cmd = "sinfo --noheader"
+    if partition:
+        cmd += f" --partition={partition}"
     rows = parse_cmd(cmd)
     states = {}
     for row in rows:
         tokens = row.split()
         state, names = tokens[4], tokens[5]
         node_names = parse_node_names(names)
         states.update({name: state for name in node_names})
@@ -395,37 +403,49 @@
     for metric, alloc_val in metrics["AllocTRES"].items():
         cfg_val = metrics["CfgTRES"][metric]
         occupancy[metric] = f"{alloc_val}/{cfg_val}"
     return occupancy
 
 
 @beartype
-def parse_all_gpus(default_gpus: int = 4) -> dict:
+def parse_all_gpus(partition: (str, NoneType) = None,
+                   default_gpus: int = 4,
+                   default_gpu_name: str = "NONAME_GPU") -> dict:
     """Query SLURM for the number and types of GPUs under management.
 
     Args:
+        partition: the partition/queue (or multiple, comma separated) of interest.
+            By default None, which queries all available partitions.
         default_gpus: The number of GPUs estimated for nodes that have incomplete SLURM
             meta data.
+        default_gpu_name: The name of the GPU for nodes that have incomplete SLURM meta
+        data.
 
     Returns:
         a mapping between node names and a list of the GPUs that they have available.
     """
-    cmd = "sinfo -o '%50N|%30G' --noheader"
+    cmd = "sinfo -o '%1000N|%1000G' --noheader"
+    if partition:
+        cmd += f" --partition={partition}"
     rows = parse_cmd(cmd)
     resources = defaultdict(list)
+
+    # Debug the regular expression below at
+    # https://regex101.com/r/RHYM8Z/3
+    p = re.compile(r'gpu:(?:(\w*):)?(\d*)(?:\(\S*\))?\s*')
+
     for row in rows:
         node_str, resource_strs = row.split("|")
         for resource_str in resource_strs.split(","):
             if not resource_str.startswith("gpu"):
                 continue
-            tokens = resource_str.strip().split(":")
+            match = p.search(resource_str)
+            gpu_type = match.group(1) if match.group(1) is not None else default_gpu_name
             # if the number of GPUs is not specified, we assume it is `default_gpus`
-            if tokens[2] == "":
-                tokens[2] = default_gpus
-            gpu_type, gpu_count = tokens[1], int(tokens[2])
+            gpu_count = int(match.group(2)) if match.group(2) != "" else default_gpus
             node_names = parse_node_names(node_str)
             for name in node_names:
                 resources[name].append({"type": gpu_type, "count": gpu_count})
     return resources
 
 
 @beartype
@@ -483,24 +503,26 @@
         res = resources
     else:
         raise ValueError(f"Unknown mode: {mode}")
     summary_by_type(res, tag=mode)
 
 
 @beartype
-def gpu_usage(resources: dict) -> dict:
+def gpu_usage(resources: dict, partition: (str, NoneType) = None) -> dict:
     """Build a data structure of the cluster resource usage, organised by user.
 
     Args:
         resources (dict :: None): a summary of cluster resources, organised by node name.
 
     Returns:
         (dict): a summary of resources organised by user (and also by node name).
     """
-    cmd = "squeue -O tres-per-node,nodelist,username,jobid --noheader"
+    cmd = "squeue -O tres-per-node:100,nodelist:100,username:100,jobid:100 --noheader"
+    if partition:
+        cmd += f" --partition={partition}"
     detailed_job_cmd = "scontrol show jobid -dd %s"
     rows = parse_cmd(cmd)
     usage = defaultdict(dict)
     for row in rows:
         tokens = row.split()
         # ignore pending jobs
         if len(tokens) < 4 or not tokens[0].startswith("gpu"):
@@ -521,17 +543,17 @@
             # If a node still has jobs running but is draining, it will not be present
             # in the "available" resources, so we ignore it
             if node_name not in resources:
                 continue
             node_gpu_types = [x["type"] for x in resources[node_name]]
             if gpu_type is None:
                 if len(node_gpu_types) != 1:
-                    gpu_type = random.choice(node_gpu_types)
+                    gpu_type = sorted(resources[node_name], key=lambda k: k['count'], reverse=True)[0]['type']
                     msg = (f"cannot determine node gpu type for {user} on {node_name}"
-                           f" (guesssing {gpu_type})")
+                           f" (guessing {gpu_type})")
                     print(f"WARNING >>> {msg}")
                 else:
                     gpu_type = node_gpu_types[0]
             if gpu_type in usage[user]:
                 usage[user][gpu_type][node_name]['n_gpu'] += num_gpus
                 usage[user][gpu_type][node_name]['bash_gpu'] += num_bash_gpus
 
@@ -540,23 +562,23 @@
                 usage[user][gpu_type][node_name]['n_gpu'] += num_gpus
                 usage[user][gpu_type][node_name]['bash_gpu'] += num_bash_gpus
 
     return usage
 
 
 @beartype
-def in_use(resources: dict = None):
+def in_use(resources: dict = None, partition: (str, NoneType) = None):
     """Print a short summary of the resources that are currently used by each user.
 
     Args:
         resources: a summary of cluster resources, organised by node name.
     """
     if not resources:
         resources = parse_all_gpus()
-    usage = gpu_usage(resources)
+    usage = gpu_usage(resources, partition=partition)
     aggregates = {}
     for user, subdict in usage.items():
         aggregates[user] = {}
         aggregates[user]['n_gpu'] = {key: sum([x['n_gpu'] for x in val.values()])
                                      for key, val in subdict.items()}
         aggregates[user]['bash_gpu'] = {key: sum([x['bash_gpu'] for x in val.values()])
                                         for key, val in subdict.items()}
@@ -619,62 +641,69 @@
                     details = f"[{', '.join(details)}] [{','.join(users)}]"
                     summary.append(f"\n -> {node}: {count} {key} {details}")
             tail = " ".join(summary)
         print(f"{key}: {gpu_count} available {tail}")
 
 
 @beartype
-def all_info(color: int, verbose: bool):
+def all_info(color: int, verbose: bool, partition: (str, NoneType) = None):
     """Print a collection of summaries about SLURM gpu usage, including: all nodes
     managed by the cluster, nodes that are currently accesible and gpu usage for each
     active user.
+
+    Args:
+        partition: the partition/queue (or multiple, comma separated) of interest.
+            By default None, which queries all available partitions.
     """
     divider, slurm_str = "---------------------------------", "SLURM"
     if color:
         colors = sns.color_palette("hls", 8).as_hex()
         divider = colored.stylize(divider, colored.fg(colors[7]))
         slurm_str = colored.stylize(slurm_str, colored.fg(colors[0]))
     print(divider)
     print(f"Under {slurm_str} management")
     print(divider)
-    resources = parse_all_gpus()
-    states = node_states()
+    resources = parse_all_gpus(partition=partition)
+    states = node_states(partition=partition)
     for mode in ("up", "accessible"):
         summary(mode=mode, resources=resources, states=states)
         print(divider)
-    in_use(resources)
+    in_use(resources, partition=partition)
     print(divider)
     available(resources=resources, states=states, verbose=verbose)
     print(divider)
 
 
 def main():
     parser = argparse.ArgumentParser(description="slurm_gpus tool")
     parser.add_argument("--action", default="current",
                         choices=["current", "history", "daemon-start", "daemon-stop"],
                         help=("The function performed by slurm_gpustat: `current` will"
                               " provide a summary of current usage, 'history' will "
                               "provide statistics from historical data (provided that the"
                               "logging daemon has been running). 'daemon-start' and"
                               "'daemon-stop' will start and stop the daemon, resp."))
+    parser.add_argument("-p", "--partition", default=None,
+                        help="the partition/queue (or multiple, comma separated) of interest. "
+                             "By default set to all available partitions.")
     parser.add_argument("--log_path",
                         default=Path.home() / "data/daemons/logs/slurm_gpustat.log",
                         help="the location where daemon log files will be stored")
     parser.add_argument("--gpustat_pid",
                         default=Path.home() / "data/daemons/pids/slurm_gpustat.pid",
                         help="the location where the daemon PID file will be stored")
     parser.add_argument("--daemon_log_interval", type=int, default=43200,
                         help="time interval (secs) between stat logging (default 12 hrs)")
     parser.add_argument("--color", type=int, default=1, help="color output")
     parser.add_argument("--verbose", action="store_true",
                         help="provide a more detailed breakdown of resources")
     args = parser.parse_args()
 
     if args.action == "current":
-        all_info(color=args.color, verbose=args.verbose)
+        all_info(color=args.color, verbose=args.verbose, partition=args.partition)
     elif args.action == "history":
         data = GPUStatDaemon.deserialize_usage(args.log_path)
         historical_summary(data)
     elif args.action.startswith("daemon"):
         daemon = GPUStatDaemon(
             log_path=args.log_path,
             pidfile=args.gpustat_pid,
```

### Comparing `slurm_gpustat-0.0.8/slurm_gpustat.egg-info/PKG-INFO` & `slurm_gpustat-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: slurm-gpustat
-Version: 0.0.8
+Name: slurm_gpustat
+Version: 0.0.9
 Summary: A simple SLURM gpu summary tool
 Home-page: https://github.com/albanie/slurm_gpustat
 Author: Samuel Albanie
 License: UNKNOWN
 Description: ## slurm_gpustat
         
         `slurm_gpustat` is a simple command line utility that produces a summary of GPU usage on a slurm cluster. The tool can be used in two ways:
@@ -18,14 +18,18 @@
         
         ### Usage
         
         To print a summary of current activity:
         
         `slurm_gpustat`
         
+        To print a summary of current activity on particular partitions, e.g. `debug` & `normal`:
+        
+        `slurm_gpustat -p debug,normal` or `slurm_gpustat --partition debug,normal`
+        
         To start the logging dameon:
         
         `slurm_gpustat --action daemon-start`
         
         To view a summary of logged data:
         
         `slurm_gpustat --action history`
```

