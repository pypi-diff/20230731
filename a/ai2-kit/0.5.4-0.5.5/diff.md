# Comparing `tmp/ai2_kit-0.5.4.tar.gz` & `tmp/ai2_kit-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.5.4.tar", max compression
+gzip compressed data, was "ai2_kit-0.5.5.tar", max compression
```

## Comparing `ai2_kit-0.5.4.tar` & `ai2_kit-0.5.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.4/LICENSE
--rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.4/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.4/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.4/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.4/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.4/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     8127 2023-07-25 07:20:18.077054 ai2_kit-0.5.4/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.4/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.4/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.4/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2363 2023-07-25 08:15:29.956291 ai2_kit-0.5.4/ai2_kit/core/script.py
--rw-r--r--   0        0        0     5894 2023-07-26 03:27:15.718128 ai2_kit-0.5.4/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.4/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.4/ai2_kit/domain/asap.py
--rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.4/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/domain/data.py
--rw-r--r--   0        0        0     7895 2023-07-25 02:20:46.132275 ai2_kit-0.5.4/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.4/ai2_kit/domain/iface.py
--rw-r--r--   0        0        0    17292 2023-07-25 01:07:27.943305 ai2_kit-0.5.4/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/domain/lasp.py
--rw-r--r--   0        0        0    13433 2023-07-26 03:43:28.387903 ai2_kit-0.5.4/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.4/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.4/ai2_kit/domain/util.py
--rw-r--r--   0        0        0     7678 2023-07-25 03:06:53.751626 ai2_kit-0.5.4/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.4/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.4/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      953 2023-07-26 03:46:11.947863 ai2_kit-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2081 2023-07-26 13:52:05.868290 ai2_kit-0.5.5/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.5/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.5/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.5/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.5/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8127 2023-07-25 07:20:18.077054 ai2_kit-0.5.5/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.5/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.5/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9721 2023-07-26 07:51:36.614431 ai2_kit-0.5.5/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2391 2023-07-26 09:20:42.973178 ai2_kit-0.5.5/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     6704 2023-07-27 04:45:11.760090 ai2_kit-0.5.5/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.5/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.5/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     1773 2023-07-28 10:17:35.722445 ai2_kit-0.5.5/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.5/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.5/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0     7895 2023-07-25 02:20:46.132275 ai2_kit-0.5.5/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.5/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    17292 2023-07-27 01:48:54.442571 ai2_kit-0.5.5/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.5/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0    13433 2023-07-26 03:43:28.387903 ai2_kit-0.5.5/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      191 2023-07-31 01:35:39.925006 ai2_kit-0.5.5/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.5/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7678 2023-07-25 03:06:53.751626 ai2_kit-0.5.5/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.5/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.5/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.5/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-07-27 03:31:46.483603 ai2_kit-0.5.5/ai2_kit/tool/misc.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.5/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0    10063 2023-07-31 01:28:49.995095 ai2_kit-0.5.5/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.5/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      953 2023-07-31 02:15:55.574445 ai2_kit-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 ai2_kit-0.5.5/PKG-INFO
```

### Comparing `ai2_kit-0.5.4/LICENSE` & `ai2_kit-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/README.md` & `ai2_kit-0.5.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 ### Domain Specific Tools
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
 * CLL MLP Training Workflow: [English](doc/manual/cll-workflow.md), [中文](doc/manual/cll-workflow.zh.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ### Build-in Functionalities
 * [Checkpoint Mechanism](doc/manual/checkpoint.md)
+* HPC Executor Introduction: [中文](doc/manual/hpc-executor.zh.md)
 * [ASE Toolkit](doc/manual/ase.md)
 * [Tips](doc/manual/tips.md)
 
 
 ## Acknowledgement
 This project is inspired by and built upon the following projects:
 * [dpgen](https://github.com/deepmodeling/dpgen/tree/master/dpgen): A concurrent learning platform for the generation of reliable deep learning based potential energy models.
```

### Comparing `ai2_kit-0.5.4/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.5.5/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/core/artifact.py` & `ai2_kit-0.5.5/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/core/checkpoint.py` & `ai2_kit-0.5.5/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/core/connector.py` & `ai2_kit-0.5.5/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/core/executor.py` & `ai2_kit-0.5.5/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/core/job.py` & `ai2_kit-0.5.5/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/core/queue_system.py` & `ai2_kit-0.5.5/ai2_kit/core/queue_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,30 +175,29 @@
         self._last_states = None
 
     def _translate_state(self, slurm_state: str) -> JobState:
         return self.translate_table.get(slurm_state, JobState.UNKNOWN)
 
     def _get_all_states(self) -> Dict[str, JobState]:
         current_ts = time.time()
+        # cache the states for 10 seconds to reduce the number of squeue calls
         if self._last_states is not None and current_ts - self._last_update_at < self.config.polling_interval:
             return self._last_states
-
-        cmd = "{} --noheader --format='%i %t' -u $(whoami)".format(
+        # call squeue to get all states
+        cmd = "{} --noheader --format='%i %t' -u $USER".format(
             self.config.squeue_bin)
         r = self.connector.run(cmd, hide=True)
-
         states: Dict[str, JobState] = dict()
-
         for line in r.stdout.split('\n'):
             if not line:  # skip empty line
                 continue
             job_id, slurm_state = line.split()
-
             state = self._translate_state(slurm_state)
             states[job_id] = state
+        # update cache
         self._last_update_at = current_ts
         self._last_states = states
         return states
 
 
 class Lsf(BaseQueueSystem):
```

### Comparing `ai2_kit-0.5.4/ai2_kit/core/resource_manager.py` & `ai2_kit-0.5.5/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/core/script.py` & `ai2_kit-0.5.5/ai2_kit/core/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from typing import Optional, List, Union
+from typing import Optional, List, Union, Sequence
 import shlex
 
 
 def exit_on_error_statment(v='__EXITCODE__'):
     return f"{v}=$?; if [ ${v} -ne 0 ]; then exit ${v}; fi"
 
 
@@ -19,16 +19,16 @@
     header: str = ''
     setup: str = ''
     teardown: str = ''
 
 
 class BashStep(BaseModel):
     cmd: Union[str, List[str]]
-    cwd: Optional[str]
-    checkpoint: Optional[str]
+    cwd: Optional[str] = None
+    checkpoint: Optional[str] = None
     exit_on_error: bool = True
 
     def render(self):
         if isinstance(self.cmd, list):
             self.cmd = ' '.join(self.cmd)
 
         rendered_step = '\n'.join([
@@ -60,15 +60,15 @@
                 rendered_step,
                 'popd',
             ])
 
         return rendered_step
 
 
-BashSteps = List[Union[str, BashStep]]
+BashSteps = Sequence[Union[str, BashStep]]
 
 
 class BashScript(BaseModel):
     template: Optional[BashTemplate]
     steps: BashSteps
 
     def render(self):
```

### Comparing `ai2_kit-0.5.4/ai2_kit/core/util.py` & `ai2_kit-0.5.5/ai2_kit/core/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ruamel.yaml import YAML
+from ruamel.yaml import YAML, ScalarNode, SequenceNode
 from pathlib import Path
-from typing import Tuple, List, TypeVar
+from typing import Tuple, List, TypeVar, Union
 from dataclasses import field
 from itertools import zip_longest
 
 import shortuuid
 import hashlib
 import base64
 import copy
@@ -19,18 +19,26 @@
 EMPTY = object()
 
 
 def default_mutable_field(obj):
     return field(default_factory=lambda: copy.copy(obj))
 
 
-def load_yaml_file(path: Path):
+def get_yaml():
     yaml = YAML(typ='safe')
     JoinTag.register(yaml)
-    ReadTag.register(yaml)
+    LoadTextTag.register(yaml)
+    LoadYamlTag.register(yaml)
+    return yaml
+
+
+def load_yaml_file(path: Union[Path, str]):
+    if isinstance(path, str):
+        path = Path(path)
+    yaml = get_yaml()
     return yaml.load(path)
 
 
 def load_yaml_files(*paths: Tuple[Path]):
     d = {}
     for path in paths:
         print('load yaml file: ', path)
@@ -85,44 +93,71 @@
     @classmethod
     def from_yaml(cls, constructor, node):
         seq = constructor.construct_sequence(node)
         return ''.join([str(i) for i in seq])
 
     @classmethod
     def to_yaml(cls, dumper, data):
-        # do nothing
-        return dumper.represent_sequence(cls.yaml_tag, data)
+        ...
 
     @classmethod
     def register(cls, yaml: YAML):
         yaml.register_class(cls)
 
-
-class ReadTag:
+class LoadTextTag:
     """a tag to read string from file"""
 
-    yaml_tag = u'!read'
+    yaml_tag = u'!load_text'
 
     @classmethod
     def from_yaml(cls, constructor, node):
-        seq = constructor.construct_sequence(node)
-        path = os.path.join(*seq)
+        path = _yaml_get_path_node(node, constructor)
         with open(path, 'r') as f:
             return f.read()
 
     @classmethod
     def to_yaml(cls, dumper, data):
-        # do nothing
-        return dumper.represent_sequence(cls.yaml_tag, data)
+        ...
+
+    @classmethod
+    def register(cls, yaml: YAML):
+        yaml.register_class(cls)
+
+
+class LoadYamlTag:
+    """a tag to read string from file"""
+
+    yaml_tag = u'!load_yaml'
+
+    @classmethod
+    def from_yaml(cls, constructor, node):
+        path = _yaml_get_path_node(node, constructor)
+        yaml = get_yaml()
+        with open(path, 'r') as f:
+            return yaml.load(f)
+
+    @classmethod
+    def to_yaml(cls, dumper, data):
+        ...
 
     @classmethod
     def register(cls, yaml: YAML):
         yaml.register_class(cls)
 
 
+def _yaml_get_path_node(node, constructor):
+    if isinstance(node, ScalarNode):
+        return constructor.construct_scalar(node)
+    elif isinstance(node, SequenceNode):
+        seq = constructor.construct_sequence(node)
+        return os.path.join(*seq)
+    else:
+        raise ValueError(f'Unknown node type {type(node)}')
+
+
 def __export_remote_functions():
     """cloudpickle compatible: https://stackoverflow.com/questions/75292769"""
 
     def merge_dict(lo: dict, ro: dict, path=None):
         """
         Merge two dict, the left dict will be overridden.
         Note: list will be replaced instead of merged.
```

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/asap.py` & `ai2_kit-0.5.5/ai2_kit/domain/asap.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/constant.py` & `ai2_kit-0.5.5/ai2_kit/domain/constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,12 +75,12 @@
     'reducer_type': 'average',
     'element_wise': False,
     'zeta': 1,
 }
 
 DEFAULT_ASAP_PCA_REDUCER = {
     'type': 'PCA',
-            'parameter': {
-                'n_components': 3,
-                'scalecenter': True,
-            }
+    'parameter': {
+        'n_components': 3,
+        'scalecenter': True,
+    }
 }
```

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/cp2k.py` & `ai2_kit-0.5.5/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/data.py` & `ai2_kit-0.5.5/ai2_kit/domain/data.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/deepmd.py` & `ai2_kit-0.5.5/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/iface.py` & `ai2_kit-0.5.5/ai2_kit/domain/iface.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/lammps.py` & `ai2_kit-0.5.5/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/lasp.py` & `ai2_kit-0.5.5/ai2_kit/domain/lasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/selector.py` & `ai2_kit-0.5.5/ai2_kit/domain/selector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/util.py` & `ai2_kit-0.5.5/ai2_kit/domain/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/domain/vasp.py` & `ai2_kit-0.5.5/ai2_kit/domain/vasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/main.py` & `ai2_kit-0.5.5/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/tool/ase.py` & `ai2_kit-0.5.5/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.5.5/ai2_kit/workflow/cll_mlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     context: Context
 
 
 class WorkflowConfig(BaseModel):
     class General(BaseModel):
         type_map: List[str]
         mass_map: List[float]
-        max_iters: int = 10
+        max_iters: int = 1
 
     class Label(BaseModel):
         cp2k: Optional[cp2k.CllCp2kInputConfig]
         vasp: Optional[vasp.CllVaspInputConfig]
 
     class Train(BaseModel):
         deepmd: deepmd.CllDeepmdInputConfig
```

### Comparing `ai2_kit-0.5.4/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.5.5/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.4/pyproject.toml` & `ai2_kit-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.5.4"
+version = "0.5.5"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.5.4/PKG-INFO` & `ai2_kit-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.5.4
+Version: 0.5.5
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -69,14 +69,15 @@
 ### Domain Specific Tools
 * [Proton Transfer Analysis Toolkit](doc/manual/proton-transfer.md)
 * CLL MLP Training Workflow: [English](doc/manual/cll-workflow.md), [中文](doc/manual/cll-workflow.zh.md)
 * [FEP MLP Training Workflow](doc/manual/fep-workflow.md)
 
 ### Build-in Functionalities
 * [Checkpoint Mechanism](doc/manual/checkpoint.md)
+* HPC Executor Introduction: [中文](doc/manual/hpc-executor.zh.md)
 * [ASE Toolkit](doc/manual/ase.md)
 * [Tips](doc/manual/tips.md)
 
 
 ## Acknowledgement
 This project is inspired by and built upon the following projects:
 * [dpgen](https://github.com/deepmodeling/dpgen/tree/master/dpgen): A concurrent learning platform for the generation of reliable deep learning based potential energy models.
```

