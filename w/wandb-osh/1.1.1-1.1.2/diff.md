# Comparing `tmp/wandb_osh-1.1.1.tar.gz` & `tmp/wandb_osh-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wandb_osh-1.1.1.tar", last modified: Fri Jul 28 19:20:44 2023, max compression
+gzip compressed data, was "wandb_osh-1.1.2.tar", last modified: Mon Jul 31 19:36:16 2023, max compression
```

## Comparing `wandb_osh-1.1.1.tar` & `wandb_osh-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.107986 wandb_osh-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/src/wandb_osh/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/lightning_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/ray_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/syncer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/src/wandb_osh/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/util/hash_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/src/wandb_osh/util/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/src/wandb_osh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:20:43.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 19:20:44.000000 wandb_osh-1.1.1/src/wandb_osh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:20:44.111986 wandb_osh-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_lightning_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_ray_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-28 19:20:36.000000 wandb_osh-1.1.1/tests/test_syncer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:16.640865 wandb_osh-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-31 19:36:16.640865 wandb_osh-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-31 19:36:16.640865 wandb_osh-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:16.632865 wandb_osh-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:16.636865 wandb_osh-1.1.2/src/wandb_osh/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/lightning_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/ray_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/syncer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:16.636865 wandb_osh-1.1.2/src/wandb_osh/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/util/hash_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/src/wandb_osh/util/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:16.636865 wandb_osh-1.1.2/src/wandb_osh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-31 19:36:16.000000 wandb_osh-1.1.2/src/wandb_osh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-31 19:36:16.000000 wandb_osh-1.1.2/src/wandb_osh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:36:16.000000 wandb_osh-1.1.2/src/wandb_osh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 19:36:16.000000 wandb_osh-1.1.2/src/wandb_osh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:36:16.000000 wandb_osh-1.1.2/src/wandb_osh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 19:36:16.000000 wandb_osh-1.1.2/src/wandb_osh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 19:36:16.000000 wandb_osh-1.1.2/src/wandb_osh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:16.640865 wandb_osh-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/tests/test_lightning_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/tests/test_ray_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-31 19:36:07.000000 wandb_osh-1.1.2/tests/test_syncer.py
```

### Comparing `wandb_osh-1.1.1/LICENSE.txt` & `wandb_osh-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/PKG-INFO` & `wandb_osh-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: wandb_osh
-Version: 1.1.1
-Summary: Trigger wandb offline syncs from a compute node without internet
-Home-page: https://github.com/klieret/wandb-offline-sync-hook
-Author: Kilian Lieret
-Author-email: kilian.lieret@posteo.de
-Maintainer: Kilian Lieret
-Maintainer-email: kilian.lieret@posteo.de
-License: MIT
-Project-URL: Bug Tracker, https://github.com/klieret/wandb-offline-sync-hook/issues
-Project-URL: Documentation, https://wandb_osh.readthedocs.io/
-Project-URL: Source Code, https://github.com/klieret/wandb-offline-sync-hook
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: lightning
-Provides-Extra: ray
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
 <p></p>
 
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
@@ -82,22 +55,31 @@
 ### What alternatives are there?
 
 With [ray tune][ray-tune], you can use your ray head node as the place to synchronize from (rather than deploying it via the batch system as well, as the [current docs][ray-tune-slurm-docs] suggest). See the note below or my [demo repository][ray-tune-slurm-test].
 Similar strategies might be possible for `wandb` as well (let me know!).
 
 ## 📦 Installation
 
-```
+```bash
 pip3 install wandb-osh
 ```
 
-If you want to use this package with `ray`, use
+For completeness, the extra dependencies `lightning` and `ray` are given, but they only ensure that the corresponding package is installed.
+For example
 
+```bash
+pip3 install 'wandb-osh[lightning]'
 ```
-pip3 install 'wandb-osh[ray]'
+
+also installs pytorch lightning if it is not already present, but has no other effect.
+
+For development, make sure also to include the `testing` extra requirement.
+
+```bash
+pip3 install --editable '.[testing]'
 ```
 
 ## 🔥 Running it!
 
 Two steps: Set up the hook, then run the script from your head node.
 
 ### Step 1: Setting up the hook
@@ -129,14 +111,16 @@
     if batch_idx % args.log_interval == 0:
         wandb.log({"loss": loss})
         trigger_sync()  # <-- New!
 ```
 
 #### With pytorch lightning
 
+Simply add the `TriggerWandbSyncLightningCallback` to your list of callbacks and you're good to go!
+
 ```python
 from wandb_osh.lightning_hooks import TriggerWandbSyncLightningCallback  # <-- New!
 from pytorch_lightning.loggers import WandbLogger
 from pytorch_lightning import Trainer
 
 logger = WandbLogger(
     project="project",
```

### Comparing `wandb_osh-1.1.1/README.md` & `wandb_osh-1.1.2/src/wandb_osh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: wandb-osh
+Version: 1.1.2
+Summary: Trigger wandb offline syncs from a compute node without internet
+Home-page: https://github.com/klieret/wandb-offline-sync-hook
+Author: Kilian Lieret
+Author-email: kilian.lieret@posteo.de
+Maintainer: Kilian Lieret
+Maintainer-email: kilian.lieret@posteo.de
+License: MIT
+Project-URL: Bug Tracker, https://github.com/klieret/wandb-offline-sync-hook/issues
+Project-URL: Documentation, https://wandb_osh.readthedocs.io/
+Project-URL: Source Code, https://github.com/klieret/wandb-offline-sync-hook
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: lightning
+Provides-Extra: ray
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 <div align="center">
 <h1>Wandb Offline Sync Hook</h1>
 <em>A convenient way to trigger synchronizations to wandb if your compute nodes don't have internet!</em>
 <p></p>
 
 [![Documentation Status](https://readthedocs.org/projects/wandb-offline-sync-hook/badge/?version=latest)](https://wandb-offline-sync-hook.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/wandb-osh.svg)](https://pypi.org/project/wandb-osh)
@@ -55,22 +82,31 @@
 ### What alternatives are there?
 
 With [ray tune][ray-tune], you can use your ray head node as the place to synchronize from (rather than deploying it via the batch system as well, as the [current docs][ray-tune-slurm-docs] suggest). See the note below or my [demo repository][ray-tune-slurm-test].
 Similar strategies might be possible for `wandb` as well (let me know!).
 
 ## 📦 Installation
 
-```
+```bash
 pip3 install wandb-osh
 ```
 
-If you want to use this package with `ray`, use
+For completeness, the extra dependencies `lightning` and `ray` are given, but they only ensure that the corresponding package is installed.
+For example
 
+```bash
+pip3 install 'wandb-osh[lightning]'
 ```
-pip3 install 'wandb-osh[ray]'
+
+also installs pytorch lightning if it is not already present, but has no other effect.
+
+For development, make sure also to include the `testing` extra requirement.
+
+```bash
+pip3 install --editable '.[testing]'
 ```
 
 ## 🔥 Running it!
 
 Two steps: Set up the hook, then run the script from your head node.
 
 ### Step 1: Setting up the hook
@@ -102,14 +138,16 @@
     if batch_idx % args.log_interval == 0:
         wandb.log({"loss": loss})
         trigger_sync()  # <-- New!
 ```
 
 #### With pytorch lightning
 
+Simply add the `TriggerWandbSyncLightningCallback` to your list of callbacks and you're good to go!
+
 ```python
 from wandb_osh.lightning_hooks import TriggerWandbSyncLightningCallback  # <-- New!
 from pytorch_lightning.loggers import WandbLogger
 from pytorch_lightning import Trainer
 
 logger = WandbLogger(
     project="project",
```

### Comparing `wandb_osh-1.1.1/setup.cfg` & `wandb_osh-1.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wandb_osh
-version = 1.1.1
+version = 1.1.2
 description = Trigger wandb offline syncs from a compute node without internet
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klieret/wandb-offline-sync-hook
 author = Kilian Lieret
 author_email = kilian.lieret@posteo.de
 maintainer = Kilian Lieret
```

### Comparing `wandb_osh-1.1.1/setup.py` & `wandb_osh-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/src/wandb_osh/cli.py` & `wandb_osh-1.1.2/src/wandb_osh/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,20 @@
     parser.add_argument(
         "--wait",
         default=1,
         type=float,
         help="Minimal time that has to pass before checking the command dir again.",
     )
     parser.add_argument(
+        "--timeout",
+        default=120,
+        type=int,
+        help="Timeout for wandb sync. If <=0, no timeout.",
+    )
+    parser.add_argument(
         "wandb_options",
         nargs="*",
         help="Options to be passed on to `wandb sync`, e.g. `--sync-all`. When "
         "specifying a flag to wandb, please add a `--` before the option, "
         "e.g., `wandb-osh -- --sync-all`",
     )
     return parser
```

### Comparing `wandb_osh-1.1.1/src/wandb_osh/hooks.py` & `wandb_osh-1.1.2/src/wandb_osh/hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/src/wandb_osh/lightning_hooks.py` & `wandb_osh-1.1.2/src/wandb_osh/lightning_hooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import annotations
 
 from os import PathLike
 
+from pytorch_lightning import LightningModule, Trainer
 from pytorch_lightning.callbacks import Callback
 
 from wandb_osh.hooks import TriggerWandbSyncHook, _comm_default_dir
 
 
 class TriggerWandbSyncLightningCallback(Callback):
-    def __init__(self, communication_dir: PathLike = _comm_default_dir):
+    def __init__(
+        self,
+        communication_dir: PathLike = _comm_default_dir,
+    ):
         """Hook to be used when interfacing wandb with pytorch lightning.
 
         Args:
             communication_dir: Directory used for communication with wandb-osh.
 
         Usage
 
@@ -24,10 +28,13 @@
 
         """
         super().__init__()
         self._hook = TriggerWandbSyncHook(communication_dir=communication_dir)
 
     def on_validation_epoch_end(
         self,
-        *args,
-    ):
+        trainer: Trainer,
+        pl_module: LightningModule,
+    ) -> None:
+        if trainer.sanity_checking:
+            return
         self._hook()
```

### Comparing `wandb_osh-1.1.1/src/wandb_osh/ray_hooks.py` & `wandb_osh-1.1.2/src/wandb_osh/ray_hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/src/wandb_osh/syncer.py` & `wandb_osh-1.1.2/src/wandb_osh/syncer.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,36 +13,40 @@
 
 class WandbSyncer:
     def __init__(
         self,
         command_dir: PathLike = _command_dir_default,
         wait: int = 1,
         wandb_options: list[str] | None = None,
+        *,
+        timeout: int | float = 120,
     ):
         """Class for interpreting command files and triggering
         `wandb sync`.
 
         Args:
             command_dir: Directory used for communication
             wait: Minimal time to wait before scanning command dir again
             wandb_options: Options to pass on to wandb
+            timeout: Timeout for wandb sync. If <=0, no timeout.
         """
         if wandb_options is None:
             wandb_options = []
         self.command_dir = Path(command_dir)
         self.wait = wait
         self.wandb_options = wandb_options
+        self._timeout = timeout
 
     def sync(self, dir: PathLike) -> None:
         """Sync a directory. Thin wrapper around the `sync_dir` function.
 
         Args:
             dir: Directory with wandb files to be synced
         """
-        sync_dir(dir, options=self.wandb_options)
+        sync_dir(dir, options=self.wandb_options, timeout=self._timeout)
 
     def loop(self) -> None:
         """Read command files and trigger syncing"""
         logger.info(
             "wandb-osh v%s, starting to watch %s", __version__, self.command_dir
         )
         while True:
@@ -59,33 +63,44 @@
                         command_file,
                         target,
                     )
                     continue
                 targets.append(target)
             for target in set(targets):
                 logger.info("Syncing %s...", target)
-                self.sync(target)
+                try:
+                    self.sync(target)
+                except subprocess.TimeoutExpired:
+                    # try again later
+                    logger.warning("Syncing %s timed out. Trying later.", target)
+                    from wandb_osh.hooks import TriggerWandbSyncHook
+
+                    TriggerWandbSyncHook(self.command_dir)(target)
             time.sleep(0.25)
             for cf in command_files:
                 if cf.is_file():
                     cf.unlink()
             if "PYTEST_CURRENT_TEST" in os.environ:
                 break
             time.sleep(max(0.0, (time.time() - start_time) - self.wait))
 
 
-def sync_dir(dir: PathLike, options: list[str] | None = None) -> None:
+def sync_dir(
+    dir: PathLike, options: list[str] | None = None, *, timeout: int | float = 0
+) -> None:
     """Call wandb sync on a directory.
 
     Args:
         dir: Directory with wandb runs
         options: List of options to pass on to `wandb sync`
+        timeout: Timeout for wandb sync. If <=0: no timeout
     """
     if options is None:
         options = []
     dir = Path(dir)
     command = ["wandb", "sync", *options, "."]
     if "PYTEST_CURRENT_TEST" in os.environ:
         logger.debug("Testing mode enabled. Not actually calling wandb.")
         logger.debug("Command would be: %s in %s", " ".join(command), dir)
         return
-    subprocess.run(command, cwd=dir)
+    _timeout = None if timeout <= 0 else timeout
+    subprocess.run(command, cwd=dir, timeout=_timeout)
```

### Comparing `wandb_osh-1.1.1/src/wandb_osh/util/log.py` & `wandb_osh-1.1.2/src/wandb_osh/util/log.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/src/wandb_osh.egg-info/PKG-INFO` & `wandb_osh-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wandb-osh
-Version: 1.1.1
+Name: wandb_osh
+Version: 1.1.2
 Summary: Trigger wandb offline syncs from a compute node without internet
 Home-page: https://github.com/klieret/wandb-offline-sync-hook
 Author: Kilian Lieret
 Author-email: kilian.lieret@posteo.de
 Maintainer: Kilian Lieret
 Maintainer-email: kilian.lieret@posteo.de
 License: MIT
@@ -82,22 +82,31 @@
 ### What alternatives are there?
 
 With [ray tune][ray-tune], you can use your ray head node as the place to synchronize from (rather than deploying it via the batch system as well, as the [current docs][ray-tune-slurm-docs] suggest). See the note below or my [demo repository][ray-tune-slurm-test].
 Similar strategies might be possible for `wandb` as well (let me know!).
 
 ## 📦 Installation
 
-```
+```bash
 pip3 install wandb-osh
 ```
 
-If you want to use this package with `ray`, use
+For completeness, the extra dependencies `lightning` and `ray` are given, but they only ensure that the corresponding package is installed.
+For example
 
+```bash
+pip3 install 'wandb-osh[lightning]'
 ```
-pip3 install 'wandb-osh[ray]'
+
+also installs pytorch lightning if it is not already present, but has no other effect.
+
+For development, make sure also to include the `testing` extra requirement.
+
+```bash
+pip3 install --editable '.[testing]'
 ```
 
 ## 🔥 Running it!
 
 Two steps: Set up the hook, then run the script from your head node.
 
 ### Step 1: Setting up the hook
@@ -129,14 +138,16 @@
     if batch_idx % args.log_interval == 0:
         wandb.log({"loss": loss})
         trigger_sync()  # <-- New!
 ```
 
 #### With pytorch lightning
 
+Simply add the `TriggerWandbSyncLightningCallback` to your list of callbacks and you're good to go!
+
 ```python
 from wandb_osh.lightning_hooks import TriggerWandbSyncLightningCallback  # <-- New!
 from pytorch_lightning.loggers import WandbLogger
 from pytorch_lightning import Trainer
 
 logger = WandbLogger(
     project="project",
```

### Comparing `wandb_osh-1.1.1/src/wandb_osh.egg-info/SOURCES.txt` & `wandb_osh-1.1.2/src/wandb_osh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/tests/test_cli.py` & `wandb_osh-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/tests/test_ray_hooks.py` & `wandb_osh-1.1.2/tests/test_ray_hooks.py`

 * *Files identical despite different names*

### Comparing `wandb_osh-1.1.1/tests/test_syncer.py` & `wandb_osh-1.1.2/tests/test_syncer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
 import logging
+import subprocess
+import unittest
+import unittest.mock
 from pathlib import Path
 
 from wandb_osh.syncer import WandbSyncer
 
 
 def test_wandb_syncer(tmp_path, caplog):
     tmp_path = Path(tmp_path)
@@ -16,7 +19,21 @@
     assert "points to non-existing directory" in caplog.text
     caplog.clear()
     (tmp_path / "123.command").write_text(str(target.resolve()))
     target.mkdir(parents=True)
     with caplog.at_level(logging.DEBUG):
         ws.loop()
     assert f"Command would be: wandb sync . in {target.resolve()}" in caplog.text
+
+
+def test_wandb_sync_timeout(tmp_path, caplog):
+    with unittest.mock.patch(
+        "wandb_osh.syncer.sync_dir", side_effect=subprocess.TimeoutExpired("asdf", 123)
+    ):
+        tmp_path = Path(tmp_path)
+        ws = WandbSyncer(tmp_path)
+        target = tmp_path / "test" / "123"
+        (tmp_path / "123.command").write_text(str(target.resolve()))
+        target.mkdir(parents=True)
+        with caplog.at_level(logging.DEBUG):
+            ws.loop()
+        assert "timed out. Trying later." in caplog.text
```

