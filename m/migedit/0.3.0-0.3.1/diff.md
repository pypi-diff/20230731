# Comparing `tmp/migedit-0.3.0.tar.gz` & `tmp/migedit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migedit-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "migedit-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `migedit-0.3.0.tar` & `migedit-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1799 2023-07-27 10:46:05.001162 migedit-0.3.0/.gitignore
--rw-r--r--   0        0        0     1079 2023-07-27 10:46:05.001162 migedit-0.3.0/LICENSE
--rw-r--r--   0        0        0     1236 2023-07-31 12:11:36.103634 migedit-0.3.0/README.md
--rw-r--r--   0        0        0     8722 2023-07-31 12:08:09.846163 migedit-0.3.0/migedit.py
--rw-r--r--   0        0        0      459 2023-07-31 12:28:47.251569 migedit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 migedit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-27 10:46:05.001162 migedit-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1079 2023-07-27 10:46:05.001162 migedit-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1269 2023-07-31 13:51:42.491040 migedit-0.3.1/README.md
+-rw-r--r--   0        0        0     8902 2023-07-31 13:51:47.059074 migedit-0.3.1/migedit.py
+-rw-r--r--   0        0        0      459 2023-07-31 12:28:47.251569 migedit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 migedit-0.3.1/PKG-INFO
```

### Comparing `migedit-0.3.0/.gitignore` & `migedit-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `migedit-0.3.0/LICENSE` & `migedit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `migedit-0.3.0/README.md` & `migedit-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 `migedit.get_mig_profiles()`
 to get a list of all available MIG instance configurations.
 
 `migedit.make_mig_devices(0, ["1g.10gb"])`
 to remove old MIG instances and create new ones.
 
-# Changelog:
+# Changelog:'
+- 3.1: Added `remove_old` flag.
 - 3.0: Support for non-A100 devices (H100, A30, etc.) by dynamically grabbing available profiles.
 - 2.0: Support for Shared Memory Mig Mode (with 7g.40gb instances)
 - 1.1: Various bugfixes
 - 1.0: Initial
 
 ## Supported platforms
```

### Comparing `migedit-0.3.0/migedit.py` & `migedit-0.3.1/migedit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """MIG Editor. CLI/importable module to automatically delete and create MIG gpu/cpu instances."""
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 import argparse
 import os
 import re
 import time
 
 from subprocess import Popen, PIPE
@@ -100,23 +100,28 @@
     Returns:
         list: Transposed list
     """
     return [list(i) for i in zip(*input_list)]
 
 
 def make_mig_devices(
-    gpu: int, profiles: list, available_mig: list = [], available_smig: list = []
+    gpu: int,
+    profiles: list,
+    available_mig: list = [],
+    available_smig: list = [],
+    remove_old: bool = True,
 ) -> list:
     """Remove any old MIG instances and create MIG instances on gpu following profiles
 
     Args:
         gpu (int): GPU instance to create on
         profiles (list): List of profiles to use
         available_mig (list, optional): Available MIG profiles. Automatically retrieves profiles if empty
         available_smig (list, optional): Available shared MIG profiles. Automatically retrieves profiles if empty
+        remove_old (bool, optional): Whether to remove old MIG instances. Defaults to True.
 
     Raises:
         ValueError: Command failed
 
     Returns:
         list: Allocated MIG instances
 
@@ -128,23 +133,23 @@
 
         if not available_mig:
             available_mig = options_mig
         if not available_smig:
             available_smig = options_smig
 
     # Remove old instances
-    result = "".join(_execute_command(f"sudo nvidia-smi mig -dci")).lower()
-    if "failed" in result or "unable" in result:
-        raise ValueError(result)
-
-    result = "".join(_execute_command(f"sudo nvidia-smi mig -dgi")).lower()
-    if "failed" in result or "unable" in result:
-        raise ValueError(result)
-
-    time.sleep(1)
+    if remove_old:
+        result = "".join(_execute_command(f"sudo nvidia-smi mig -dci")).lower()
+        if "failed" in result or "unable" in result:
+            raise ValueError(result)
+
+        result = "".join(_execute_command(f"sudo nvidia-smi mig -dgi")).lower()
+        if "failed" in result or "unable" in result:
+            raise ValueError(result)
+        time.sleep(1)
 
     devicetemp = []
 
     # TODO: remove this temp code
     shared_mig_gpui = {}
 
     # This supports Multi-MIG, which doesn't actually work right now
```

### Comparing `migedit-0.3.0/PKG-INFO` & `migedit-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migedit
-Version: 0.3.0
+Version: 0.3.1
 Summary: MIG Editor. CLI/importable module to automatically delete and create MIG gpu/cpu instances.
 Author-email: Ties Robroek <migedit@trobroek.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/Sipondo/migedit
 
@@ -32,15 +32,16 @@
 
 `migedit.get_mig_profiles()`
 to get a list of all available MIG instance configurations.
 
 `migedit.make_mig_devices(0, ["1g.10gb"])`
 to remove old MIG instances and create new ones.
 
-# Changelog:
+# Changelog:'
+- 3.1: Added `remove_old` flag.
 - 3.0: Support for non-A100 devices (H100, A30, etc.) by dynamically grabbing available profiles.
 - 2.0: Support for Shared Memory Mig Mode (with 7g.40gb instances)
 - 1.1: Various bugfixes
 - 1.0: Initial
 
 ## Supported platforms
```

