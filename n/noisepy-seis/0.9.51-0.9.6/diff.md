# Comparing `tmp/noisepy_seis-0.9.51.tar.gz` & `tmp/noisepy_seis-0.9.6.tar.gz`

## Comparing `noisepy_seis-0.9.51.tar` & `noisepy_seis-0.9.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12766 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0    10254 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    34841 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/pnwstore.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/scheduler.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/zarrstore.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/LICENSE
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/README.md
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/pyproject.toml
--rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/PKG-INFO
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    12766 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0    10254 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    34841 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/pnwstore.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/zarrstore.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/LICENSE
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/README.md
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/PKG-INFO
```

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.9.6/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.9.6/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.9.6/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.9.6/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.6/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.9.6/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.9.6/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.9.6/src/noisepy/seis/datatypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from __future__ import annotations
 
 import sys
+import typing
+from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
-from typing import List, Optional
+from typing import Any, DefaultDict, Dict, List, Optional
+from urllib.parse import urlparse
 
 import numpy as np
 import obspy
 from pydantic import BaseModel, ConfigDict, Field
 from pydantic.functional_validators import model_validator
 from pydantic_yaml import parse_yaml_raw_as, to_yaml_str
 
+from noisepy.seis.utils import get_filesystem
+
 INVALID_COORD = -sys.float_info.max
 
 
 @dataclass
 class ChannelType:
     """
     A type of channel, e.g. BHN, but not associated with a particular station
@@ -171,14 +176,24 @@
     keep_substack: bool = Field(default=False, description="keep all sub-stacks in final ASDF file")
     # new rotation para
     rotation: bool = Field(default=True, description="rotation from E-N-Z to R-T-Z")
     correction: bool = Field(default=False, description="angle correction due to mis-orientation")
     correction_csv: Optional[str] = Field(default=None, description="Path to e.g. meso_angles.csv")
     # 'RESP', or 'polozeros' to remove response
 
+    storage_options: DefaultDict[str, typing.MutableMapping] = Field(
+        default=defaultdict(dict),
+        description="Storage options to pass to fsspec, keyed by protocol (local files are ''))",
+    )
+
+    def get_storage_options(self, path: str) -> Dict[str, Any]:
+        """The storage options for the given path"""
+        url = urlparse(path)
+        return self.storage_options.get(url.scheme, {})
+
     @property
     def dt(self) -> float:
         return 1.0 / self.samp_freq
 
     @model_validator(mode="after")
     def validate(cls, m: ConfigParameters) -> ConfigParameters:
         if m.substack_len % m.cc_len != 0:
@@ -190,19 +205,21 @@
         # Hack since pydantic model properties are nor part of the object's __dict__
         if key == "dt":
             return self.dt
         return self.__dict__[key]
 
     def save_yaml(self, filename: str):
         yaml_str = to_yaml_str(self)
-        with open(filename, "w") as f:
+        fs = get_filesystem(filename, storage_options=self.storage_options)
+        with fs.open(filename, "w") as f:
             f.write(yaml_str)
 
-    def load_yaml(filename: str) -> ConfigParameters:
-        with open(filename, "r") as f:
+    def load_yaml(filename: str, storage_options={}) -> ConfigParameters:
+        fs = get_filesystem(filename, storage_options=storage_options)
+        with fs.open(filename, "r") as f:
             yaml_str = f.read()
             config = parse_yaml_raw_as(ConfigParameters, yaml_str)
             return config
 
 
 @dataclass
 class Channel:
```

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/main.py` & `noisepy_seis-0.9.6/src/noisepy/seis/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -154,41 +154,45 @@
     logger.setLevel(args.loglevel.upper())
 
     def run_download():
         params = initialize_params(args, None)
         download(args.raw_data_path, params)
         params.save_yaml(fs_join(args.raw_data_path, CONFIG_FILE))
 
-    def get_cc_store(args, mode="a"):
+    def get_cc_store(args, params: ConfigParameters, mode="a"):
         return (
-            ZarrCCStore(args.ccf_path, mode=mode)
+            ZarrCCStore(
+                args.ccf_path,
+                mode=mode,
+                storage_options=params.get_storage_options(args.ccf_path),
+            )
             if args.format == DataFormat.ZARR.value
             else ASDFCCStore(args.ccf_path, mode=mode)
         )
 
-    def get_stack_store(args):
+    def get_stack_store(args, params: ConfigParameters):
         return (
-            ZarrStackStore(args.stack_path, mode="a")
+            ZarrStackStore(args.stack_path, mode="a", storage_options=params.get_storage_options(args.stack_path))
             if args.format == DataFormat.ZARR.value
             else ASDFStackStore(args.stack_path, "a")
         )
 
     def run_cross_correlation():
         ccf_dir = args.ccf_path
-        cc_store = get_cc_store(args)
         params = initialize_params(args, args.raw_data_path)
+        cc_store = get_cc_store(args, params)
         raw_store = create_raw_store(args, params)
         scheduler = MPIScheduler(0) if args.mpi else SingleNodeScheduler()
         cross_correlate(raw_store, params, cc_store, scheduler)
         params.save_yaml(fs_join(ccf_dir, CONFIG_FILE))
 
     def run_stack():
-        cc_store = get_cc_store(args, mode="r")
-        stack_store = get_stack_store(args)
         params = initialize_params(args, args.ccf_path)
+        cc_store = get_cc_store(args, params, mode="r")
+        stack_store = get_stack_store(args, params)
         scheduler = MPIScheduler(0) if args.mpi else SingleNodeScheduler()
         stack(cc_store, stack_store, params, scheduler)
         params.save_yaml(fs_join(args.stack_path, CONFIG_FILE))
 
     if args.cmd == Command.DOWNLOAD:
         run_download()
     if args.cmd == Command.CROSS_CORRELATE:
```

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.6/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.9.6/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/pnwstore.py` & `noisepy_seis-0.9.6/src/noisepy/seis/pnwstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.9.6/src/noisepy/seis/scedc_s3store.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/scheduler.py` & `noisepy_seis-0.9.6/src/noisepy/seis/scheduler.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/stores.py` & `noisepy_seis-0.9.6/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/utils.py` & `noisepy_seis-0.9.6/src/noisepy/seis/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 ANON_ARG = "anon"
 utils_logger = logging.getLogger(__name__)
 
 
 def get_filesystem(path: str, storage_options: dict = {}) -> fsspec.AbstractFileSystem:
     """Construct an fsspec filesystem for the given path"""
     url = urlparse(path)
+    # The storage_options coming from the ConfigParameters is keyed by protocol
+    storage_options = storage_options.get(url.scheme, storage_options)
     # default to anonymous access for S3 if the this is not already specified
     if url.scheme == S3_SCHEME and ANON_ARG not in storage_options:
         storage_options = {ANON_ARG: True}
     return fsspec.filesystem(url.scheme, **storage_options)
 
 
 def fs_join(path1: str, path2: str) -> str:
```

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/zarrstore.py` & `noisepy_seis-0.9.6/src/noisepy/seis/zarrstore.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
 
 class ZarrStoreHelper:
     """
     Helper object for storing data and parameters into Zarr and track a "done" bit for subsets of the data
     'done' is a dummy array to track completed sets in its attribute dictionary.
     Args:
-        root_dir: Storage location
-        mode: "r" or "w" for read-only or writing mode
+        root_dir: Storage location, can be a local or S3 path
+        mode: "r" or "a" for read-only or writing mode
         dims: number dimensions of the data
-
+        storage_options: options to pass to fsspec
     """
 
-    def __init__(self, root_dir: str, mode: str, dims: int) -> None:
+    def __init__(self, root_dir: str, mode: str, dims: int, storage_options={}) -> None:
         super().__init__()
         self.dims = dims
-        self.root = zarr.open(root_dir, mode=mode)
+        self.root = zarr.open_group(root_dir, mode=mode, storage_options=storage_options)
         logger.info(f"store created at {root_dir}")
 
     def contains(self, path: str) -> bool:
         return path in self.root
 
     def append(
         self,
@@ -84,17 +84,17 @@
     CrossCorrelationDataStore that uses hierarchical Zarr files for storage. The directory organization is as follows:
     /                           (root)
         station_pair            (group)
             timestamp           (group)
                 channel_pair    (array)
     """
 
-    def __init__(self, root_dir: str, mode: str = "a") -> None:
+    def __init__(self, root_dir: str, mode: str = "a", storage_options={}) -> None:
         super().__init__()
-        self.helper = ZarrStoreHelper(root_dir, mode, dims=2)
+        self.helper = ZarrStoreHelper(root_dir, mode, dims=2, storage_options=storage_options)
 
     def contains(self, timespan: DateTimeRange, src_chan: Channel, rec_chan: Channel) -> bool:
         path = self._get_path(timespan, src_chan, rec_chan)
         return self.helper.contains(path)
 
     def append(
         self,
@@ -154,17 +154,17 @@
     A class for reading and writing stack data using Zarr format. Hierarchy is:
     /
         station_pair            (group)
             stack name          (group)
                 component       (array)
     """
 
-    def __init__(self, root_dir: str, mode: str = "a") -> None:
+    def __init__(self, root_dir: str, mode: str = "a", storage_options={}) -> None:
         super().__init__()
-        self.helper = ZarrStoreHelper(root_dir, mode, dims=1)
+        self.helper = ZarrStoreHelper(root_dir, mode, dims=1, storage_options=storage_options)
 
     def mark_done(self, src: Station, rec: Station):
         path = self._get_station_path(src, rec)
         return self.helper.mark_done(path)
 
     def is_done(self, src: Station, rec: Station):
         path = self._get_station_path(src, rec)
```

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/.gitignore` & `noisepy_seis-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/LICENSE` & `noisepy_seis-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/README.md` & `noisepy_seis-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/pyproject.toml` & `noisepy_seis-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.51/PKG-INFO` & `noisepy_seis-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.9.51
+Version: 0.9.6
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
```

