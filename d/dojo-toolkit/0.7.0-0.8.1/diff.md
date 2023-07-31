# Comparing `tmp/dojo-toolkit-0.7.0.tar.gz` & `tmp/dojo_toolkit-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo-toolkit-0.7.0.tar", max compression
+gzip compressed data, was "dojo_toolkit-0.8.1.tar", max compression
```

## Comparing `dojo-toolkit-0.7.0.tar` & `dojo_toolkit-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    35141 2022-06-28 18:08:37.045622 dojo-toolkit-0.7.0/LICENSE
--rw-r--r--   0        0        0     1321 2022-09-16 11:05:10.204114 dojo-toolkit-0.7.0/README.rst
--rw-r--r--   0        0        0        0 2022-06-28 18:08:37.045622 dojo-toolkit-0.7.0/dojo_toolkit/__init__.py
--rw-r--r--   0        0        0    12143 2022-06-28 18:08:37.045622 dojo-toolkit-0.7.0/dojo_toolkit/assets/g.jpg
--rw-r--r--   0        0        0    17415 2022-06-28 18:08:37.045622 dojo-toolkit-0.7.0/dojo_toolkit/assets/r.jpg
--rw-r--r--   0        0        0   885748 2022-06-28 18:08:37.052288 dojo-toolkit-0.7.0/dojo_toolkit/assets/sounds/pass.wav
--rw-r--r--   0        0        0  2281720 2022-06-28 18:08:37.065622 dojo-toolkit-0.7.0/dojo_toolkit/assets/sounds/start.wav
--rw-r--r--   0        0        0   879114 2022-06-28 18:08:37.068955 dojo-toolkit-0.7.0/dojo_toolkit/assets/sounds/timeup.wav
--rw-r--r--   0        0        0     1080 2022-09-16 11:05:10.204114 dojo-toolkit-0.7.0/dojo_toolkit/code_handler.py
--rw-r--r--   0        0        0     1505 2022-09-16 11:05:10.207448 dojo-toolkit-0.7.0/dojo_toolkit/dojo.py
--rw-r--r--   0        0        0     1558 2022-09-16 11:05:10.207448 dojo-toolkit-0.7.0/dojo_toolkit/dojo_thread.py
--rw-r--r--   0        0        0     1126 2022-09-02 14:31:22.853014 dojo-toolkit-0.7.0/dojo_toolkit/main.py
--rw-r--r--   0        0        0     1429 2022-06-28 18:08:37.068955 dojo-toolkit-0.7.0/dojo_toolkit/notifier.py
--rw-r--r--   0        0        0      161 2022-06-28 18:08:37.068955 dojo-toolkit-0.7.0/dojo_toolkit/settings.py
--rw-r--r--   0        0        0     1023 2022-06-28 18:08:37.068955 dojo-toolkit-0.7.0/dojo_toolkit/sound_handler.py
--rw-r--r--   0        0        0     2294 2022-06-28 18:08:37.068955 dojo-toolkit-0.7.0/dojo_toolkit/test_runner.py
--rw-r--r--   0        0        0      698 2022-09-16 11:05:10.207448 dojo-toolkit-0.7.0/dojo_toolkit/timer.py
--rw-r--r--   0        0        0      994 2022-09-16 11:05:10.207448 dojo-toolkit-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2329 2022-09-16 11:05:29.314164 dojo-toolkit-0.7.0/setup.py
--rw-r--r--   0        0        0     1880 2022-09-16 11:05:29.314413 dojo-toolkit-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-07-27 00:29:47.944332 dojo_toolkit-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1321 2023-07-27 00:29:47.944332 dojo_toolkit-0.8.1/README.rst
+-rw-r--r--   0        0        0        0 2023-07-27 00:29:47.944332 dojo_toolkit-0.8.1/dojo_toolkit/__init__.py
+-rw-r--r--   0        0        0    12143 2023-07-27 00:29:47.944332 dojo_toolkit-0.8.1/dojo_toolkit/assets/g.jpg
+-rw-r--r--   0        0        0    17415 2023-07-27 00:29:47.944332 dojo_toolkit-0.8.1/dojo_toolkit/assets/r.jpg
+-rw-r--r--   0        0        0   885748 2023-07-27 00:29:47.950999 dojo_toolkit-0.8.1/dojo_toolkit/assets/sounds/pass.wav
+-rw-r--r--   0        0        0  2281720 2023-07-27 00:29:47.957666 dojo_toolkit-0.8.1/dojo_toolkit/assets/sounds/start.wav
+-rw-r--r--   0        0        0   879114 2023-07-27 00:29:47.960999 dojo_toolkit-0.8.1/dojo_toolkit/assets/sounds/timeup.wav
+-rw-r--r--   0        0        0     1059 2023-07-28 17:36:23.029941 dojo_toolkit-0.8.1/dojo_toolkit/code_handler.py
+-rw-r--r--   0        0        0     1497 2023-07-28 17:36:23.029941 dojo_toolkit-0.8.1/dojo_toolkit/dojo.py
+-rw-r--r--   0        0        0     1558 2023-07-27 00:29:47.960999 dojo_toolkit-0.8.1/dojo_toolkit/dojo_thread.py
+-rw-r--r--   0        0        0     1402 2023-07-31 13:10:03.686320 dojo_toolkit-0.8.1/dojo_toolkit/main.py
+-rw-r--r--   0        0        0     1410 2023-07-28 17:36:23.029941 dojo_toolkit-0.8.1/dojo_toolkit/notifier.py
+-rw-r--r--   0        0        0      161 2023-07-27 00:29:47.960999 dojo_toolkit-0.8.1/dojo_toolkit/settings.py
+-rw-r--r--   0        0        0     1023 2023-07-27 00:29:47.960999 dojo_toolkit-0.8.1/dojo_toolkit/sound_handler.py
+-rw-r--r--   0        0        0     2294 2023-07-27 00:29:47.960999 dojo_toolkit-0.8.1/dojo_toolkit/test_runner.py
+-rw-r--r--   0        0        0      698 2023-07-27 00:29:47.960999 dojo_toolkit-0.8.1/dojo_toolkit/timer.py
+-rw-r--r--   0        0        0     1385 2023-07-31 13:26:25.221861 dojo_toolkit-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 dojo_toolkit-0.8.1/PKG-INFO
```

### Comparing `dojo-toolkit-0.7.0/LICENSE` & `dojo_toolkit-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/README.rst` & `dojo_toolkit-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/assets/g.jpg` & `dojo_toolkit-0.8.1/dojo_toolkit/assets/g.jpg`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/assets/r.jpg` & `dojo_toolkit-0.8.1/dojo_toolkit/assets/r.jpg`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/assets/sounds/pass.wav` & `dojo_toolkit-0.8.1/dojo_toolkit/assets/sounds/pass.wav`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/assets/sounds/start.wav` & `dojo_toolkit-0.8.1/dojo_toolkit/assets/sounds/start.wav`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/assets/sounds/timeup.wav` & `dojo_toolkit-0.8.1/dojo_toolkit/assets/sounds/timeup.wav`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/code_handler.py` & `dojo_toolkit-0.8.1/dojo_toolkit/code_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ignore_directories = True
     min_test_time_interval = 2
 
     def __init__(self, *args, **kwargs):
         self.dojo = kwargs.pop("dojo")
         self.test_runner = kwargs.pop("test_runner")
 
-        super(DojoCodeHandler, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         self.last_test_run_time = time.time()
 
     def get_last_test_run_interval(self):
         return time.time() - self.last_test_run_time
 
     def on_modified(self, event):
```

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/dojo.py` & `dojo_toolkit-0.8.1/dojo_toolkit/dojo.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         event_handler = DojoCodeHandler(dojo=self.controller, test_runner=test_runner)
 
         self.observer = Observer()
         self.observer.schedule(event_handler, self.code_path, recursive=False)
 
     def start(self):
         self.observer.start()
-        print("\nWatching: {} folder".format(self.code_path))
+        print(f"\nWatching: {self.code_path} folder")
 
         self.is_running = True
         print("Dojo toolkit started!")
         self.thread = Thread(target=dojo_thread.main, args=(self.controller,))
         self.thread.daemon = True
         self.thread.start()
```

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/dojo_thread.py` & `dojo_toolkit-0.8.1/dojo_toolkit/dojo_thread.py`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/main.py` & `dojo_toolkit-0.8.1/dojo_toolkit/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,63 @@
+import os
 from enum import Enum
 from pathlib import Path
-from typing import Optional
+from typing import Annotated, Optional
 
 import typer
 
 from dojo_toolkit.dojo import Dojo
 
 
 class Runners(str, Enum):
     doctest = "doctest"
     pytest = "pytest"
 
 
 def main(
-    path: Optional[Path] = typer.Argument(
-        Path("."),
-        exists=True,
-        file_okay=False,
-        dir_okay=True,
-        readable=True,
-        help="The path to the folder containing the code used during the dojo",
-    ),
-    time: Optional[float] = typer.Option(
-        Dojo.ROUND_TIME,
-        "--time",
-        "-t",
-        help="The amount of time a dojo round lasts",
-    ),
-    mute: Optional[bool] = typer.Option(
-        False,
-        help="Mute all sounds, note: this only works in Linux",
-    ),
-    runner: Optional[Runners] = typer.Option(
-        Runners.doctest.value,
-        "--runner",
-        help="Name of the runner",
-    ),
+    path: Annotated[
+        Optional[Path],
+        typer.Argument(
+            exists=True,
+            file_okay=False,
+            dir_okay=True,
+            readable=True,
+            help="The path to the folder containing the code used during the dojo",
+        ),
+    ] = Path("."),
+    time: Annotated[
+        Optional[float],
+        typer.Option(
+            "--time",
+            "-t",
+            help="The amount of time a dojo round lasts, in minutes",
+        ),
+    ] = Dojo.ROUND_TIME,
+    mute: Annotated[
+        Optional[bool],
+        typer.Option(
+            help="Mute all sounds, note: this only works in Linux",
+        ),
+    ] = False,
+    runner: Annotated[
+        Optional[Runners],
+        typer.Option(
+            "--runner",
+            help="Name of the runner",
+        ),
+    ] = Runners.doctest,
 ):
     dojo = Dojo(
         code_path=path.as_posix(),  # type: ignore
         round_time=time,  # type: ignore
         mute=mute,  # type: ignore
         runner=runner.value,  # type: ignore
     )
-    dojo.start()
+    os.system("stty -ixon")
+    try:
+        dojo.start()
+    finally:
+        os.system("stty ixon")
 
 
 def run():
     typer.run(main)
```

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/notifier.py` & `dojo_toolkit-0.8.1/dojo_toolkit/notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def notify(self, message, image=None):
         raise NotImplementedError()
 
 
 class GnomeNotifier(BaseNotifier):
     def __init__(self):
-        super(GnomeNotifier, self).__init__()
+        super().__init__()
 
         self.fail_img = GdkPixbuf.Pixbuf.new_from_file(self.fail_img_path)
         self.success_img = GdkPixbuf.Pixbuf.new_from_file(self.success_img_path)
 
         self._notifier = self.get_notifier()
 
     def get_notifier(self):
```

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/sound_handler.py` & `dojo_toolkit-0.8.1/dojo_toolkit/sound_handler.py`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/test_runner.py` & `dojo_toolkit-0.8.1/dojo_toolkit/test_runner.py`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/dojo_toolkit/timer.py` & `dojo_toolkit-0.8.1/dojo_toolkit/timer.py`

 * *Files identical despite different names*

### Comparing `dojo-toolkit-0.7.0/PKG-INFO` & `dojo_toolkit-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dojo-toolkit
-Version: 0.7.0
+Version: 0.8.1
 Summary: Toolkit for Python Coding Dojos.
 Author: grupy-sanca
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clint (>=0.5.1,<0.6.0)
-Requires-Dist: pgi (>=0.0.11,<0.0.12); sys_platform == "linux"
+Requires-Dist: pgi (>=0.0.11,<0.0.12) ; sys_platform == "linux"
 Requires-Dist: pyglet (>=1.5.21,<2.0.0)
-Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: watchdog (>=2.1.6,<3.0.0)
 Description-Content-Type: text/x-rst
 
 Dojo Toolkit
 ============
 
 .. image:: https://github.com/grupy-sanca/dojo-toolkit/actions/workflows/test_push.yaml/badge.svg?branch=main
```

