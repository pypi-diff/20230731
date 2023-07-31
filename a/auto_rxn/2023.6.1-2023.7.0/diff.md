# Comparing `tmp/auto_rxn-2023.6.1.tar.gz` & `tmp/auto_rxn-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_rxn-2023.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "auto_rxn-2023.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `auto_rxn-2023.6.1.tar` & `auto_rxn-2023.7.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
--rw-r--r--   0        0        0      764 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/.github/workflows/python-mypy.yml
--rw-r--r--   0        0        0     1033 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      797 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/.github/workflows/python-pytest.yml
--rw-r--r--   0        0        0      827 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/.github/workflows/run-entry-points.yml
--rw-r--r--   0        0        0      448 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/.gitignore
--rw-r--r--   0        0        0      359 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      754 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/LICENSE
--rw-r--r--   0        0        0     1247 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/README.md
--rw-r--r--   0        0        0       76 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/__init__.py
--rw-r--r--   0        0        0      197 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/__init__.py
--rw-r--r--   0        0        0      550 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/__main__.py
--rw-r--r--   0        0        0      419 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/__version__.py
--rw-r--r--   0        0        0        0 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/_config.py
--rw-r--r--   0        0        0     1098 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/_exceptions.py
--rw-r--r--   0        0        0      263 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/_happi.py
--rw-r--r--   0        0        0     1520 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/_recipe.py
--rw-r--r--   0        0        0     1202 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/_run.py
--rw-r--r--   0        0        0      752 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/_testing.py
--rw-r--r--   0        0        0       54 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/devices/__init__.py
--rw-r--r--   0        0        0     1156 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/devices/_fake_furnace.py
--rw-r--r--   0        0        0     1285 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/devices/_fake_mfc.py
--rw-r--r--   0        0        0      160 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/devices/_reading.py
--rw-r--r--   0        0        0    19275 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/auto_rxn/devices/_status.py
--rw-r--r--   0        0        0     1595 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0      859 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/tests/minimal_csv/db.json
--rw-r--r--   0        0        0      119 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/tests/minimal_csv/recipe.csv
--rw-r--r--   0        0        0      308 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/tests/minimal_csv/test_minimal_csv.py
--rw-r--r--   0        0        0       56 2023-06-20 19:24:10.863236 auto_rxn-2023.6.1/tests/test_smoke.py
--rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 auto_rxn-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0      764 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/python-mypy.yml
+-rw-r--r--   0        0        0     1033 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      790 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/python-pytest.yml
+-rw-r--r--   0        0        0      828 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.github/workflows/run-entry-points.yml
+-rw-r--r--   0        0        0      448 2023-07-31 12:05:29.506278 auto_rxn-2023.7.0/.gitignore
+-rw-r--r--   0        0        0      359 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1245 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/LICENSE
+-rw-r--r--   0        0        0     1247 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/README.md
+-rw-r--r--   0        0        0       76 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/__init__.py
+-rw-r--r--   0        0        0     1098 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/__main__.py
+-rw-r--r--   0        0        0      419 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_config.py
+-rw-r--r--   0        0        0     2795 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_device.py
+-rw-r--r--   0        0        0     1098 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_exceptions.py
+-rw-r--r--   0        0        0     2156 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_recipe.py
+-rw-r--r--   0        0        0     3103 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_run.py
+-rw-r--r--   0        0        0     1248 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_safety.py
+-rw-r--r--   0        0        0      949 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/_testing.py
+-rw-r--r--   0        0        0       77 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/__init__.py
+-rw-r--r--   0        0        0     2418 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_fake_furnace.py
+-rw-r--r--   0        0        0     1285 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_fake_mfc.py
+-rw-r--r--   0        0        0      160 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_reading.py
+-rw-r--r--   0        0        0    19275 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/auto_rxn/devices/_status.py
+-rw-r--r--   0        0        0     1505 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1126 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/children/db.json
+-rw-r--r--   0        0        0      159 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/children/recipe.csv
+-rw-r--r--   0        0        0      796 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/children/test_children.py
+-rw-r--r--   0        0        0     1127 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/fallback_position/db.json
+-rw-r--r--   0        0        0      165 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/fallback_position/recipe.csv
+-rw-r--r--   0        0        0      516 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/fallback_position/test_fallback.py
+-rw-r--r--   0        0        0     1126 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/minimal_csv/db.json
+-rw-r--r--   0        0        0      125 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/minimal_csv/recipe.csv
+-rw-r--r--   0        0        0      308 2023-07-31 12:05:29.510278 auto_rxn-2023.7.0/tests/minimal_csv/test_minimal_csv.py
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 auto_rxn-2023.7.0/PKG-INFO
```

### Comparing `auto_rxn-2023.6.1/.github/workflows/python-mypy.yml` & `auto_rxn-2023.7.0/.github/workflows/python-mypy.yml`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.6.1/.github/workflows/python-publish.yml` & `auto_rxn-2023.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.6.1/.github/workflows/python-pytest.yml` & `auto_rxn-2023.7.0/.github/workflows/python-pytest.yml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `auto_rxn-2023.6.1/.github/workflows/run-entry-points.yml` & `auto_rxn-2023.7.0/.github/workflows/run-entry-points.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `auto_rxn-2023.6.1/LICENSE` & `auto_rxn-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.6.1/README.md` & `auto_rxn-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.6.1/auto_rxn/_exceptions.py` & `auto_rxn-2023.7.0/auto_rxn/_exceptions.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.6.1/auto_rxn/_recipe.py` & `auto_rxn-2023.7.0/auto_rxn/_recipe.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,37 +13,52 @@
     length: Union[int, float]
     setpoints: Dict[str, Union[int, float]]
 
 
 class Recipe:
     def __init__(self, filepath):
         self._df = pd.read_csv(filepath)
-        self.control_point_ids = list(self._df.keys()[1:])
+        self.control_point_ids = [
+            k for k in self._df.keys()[1:] if not k.endswith("fallback_position")
+        ]
+        self.fallback_position_ids = [
+            k for k in self._df.keys()[1:] if k.endswith("fallback_position")
+        ]
         # read in metadata row by row, until see recipe start
         self.metadata: Dict[str, Dict[str, str]] = {k: {} for k in self.control_point_ids}
         row_index = 0
         while True:
             row = self._df.loc[row_index]
             if row["Control Point ID"] == "RECIPE_STARTS_BELOW":
                 break
             else:
                 key = row["Control Point ID"]
                 for id in self.control_point_ids:
                     self.metadata[id][key] = row[id]
             row_index += 1
         # now the rest of the dataframe contains recipe steps
         self.steps: List[Step] = []
+        self.fallback_positions: List[Step] = []
         row_index += 1
         while True:
             try:
                 row = self._df.loc[row_index]
+                # setpoints
                 length = row["Control Point ID"]
                 setpoints = {k: row[k] for k in self.control_point_ids}
                 step = Step(length=length, setpoints=setpoints)
                 self.steps.append(step)
+                # fallback positions
+                setpoints = {
+                    k.removesuffix(".fallback_position"): row[k]
+                    for k in self.fallback_position_ids
+                }
+                step = Step(length=length, setpoints=setpoints)
+                self.fallback_positions.append(step)
                 row_index += 1
             except KeyError:
                 break
-        print(self.steps)
 
     def save(self, filepath) -> pathlib.Path:
-        raise NotImplementedError
+        path = pathlib.Path(filepath)
+        self._df.to_csv(path, index=False)
+        return path
```

### Comparing `auto_rxn-2023.6.1/auto_rxn/devices/_fake_furnace.py` & `auto_rxn-2023.7.0/auto_rxn/devices/_fake_mfc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,50 @@
-__all__ = ["FakeFurnace", "FakeFurnaceItem"]
+__all__ = ["FakeMFC", "FakeMFCItem"]
 
 
 import copy
 import time
+import threading
+from typing import Dict
 
 from happi.item import HappiItem, EntryInfo  # type: ignore
 
 from ._reading import Reading
 from ._status import Status
 
 
-class FakeFurnace:
+class FakeMFC:
     def __init__(self, name: str):
         self.name = name
         self.parent = None
         self.value = 0.0
 
     def describe(self) -> dict:
         out = dict()
-        out[f"{self.name}_setpoint"] = {"source": "FakeFurnace", "dtype": "number", "shape": []}
-        out[f"{self.name}_readback"] = {"source": "FakeFurnace", "dtype": "number", "shape": []}
+        out[f"{self.name}_setpoint"] = {"source": "FakeMFC", "dtype": "number", "shape": []}
+        out[f"{self.name}_readback"] = {"source": "FakeMFC", "dtype": "number", "shape": []}
         return out
 
     def read(self) -> dict:
         ts = time.time()
         out = dict()
         out[f"{self.name}_setpoint"] = {"value": self.value, "timestamp": ts}
         out[f"{self.name}_readback"] = {"value": self.value, "timestamp": ts}
         return out
 
     def set(self, value) -> Status:
         self.value = value
-        s = Status()
-        s.set_finished()
-        return s
+        st = Status()
 
+        def done_later():
+            time.sleep(0.1)
+            st.set_finished()
 
-class FakeFurnaceItem(HappiItem):
+        threading.Thread(target=done_later).start()
+
+        return st
+
+
+class FakeMFCItem(HappiItem):
     kwargs = copy.copy(HappiItem.kwargs)
     kwargs.default = {"name": "{{name}}"}
-    device_class = EntryInfo(default="auto_rxn.devices.FakeFurnace")
+    device_class = EntryInfo(default="auto_rxn.devices.FakeMFC")
```

### Comparing `auto_rxn-2023.6.1/auto_rxn/devices/_fake_mfc.py` & `auto_rxn-2023.7.0/auto_rxn/devices/_fake_furnace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,87 @@
-__all__ = ["FakeMFC", "FakeMFCItem"]
+__all__ = ["FakeFurnace", "FakeFurnaceItem"]
 
 
 import copy
 import time
-import threading
-from typing import Dict
 
 from happi.item import HappiItem, EntryInfo  # type: ignore
 
 from ._reading import Reading
 from ._status import Status
 
 
-class FakeMFC:
+class PropertyDevice(object):
+    def __init__(self, parent, name):
+        self.parent = parent
+        self.name = name
+        self._setpoint = float("nan")
+        self._readback = float("nan")
+
+    def set(self, value) -> Status:
+        self._setpoint = float(value)
+        self._readback = float(value)
+        st = Status()
+        st.set_finished()
+        st.wait()
+        return st
+
+    def describe(self) -> dict:
+        out = dict()
+        out[f"{self.parent.name}_{self.name}_readback"] = {
+            "source": "FakeFurnace",
+            "dtype": "number",
+            "shape": [],
+        }
+        out[f"{self.parent.name}_{self.name}_setpoint"] = {
+            "source": "FakeFurnace",
+            "dtype": "number",
+            "shape": [],
+        }
+        return out
+
+    def read(self) -> dict:
+        ts = time.time()
+        out = dict()
+        out[f"{self.parent.name}_{self.name}_readback"] = {
+            "value": self._readback,
+            "timestamp": ts,
+        }
+        out[f"{self.parent.name}_{self.name}_setpoint"] = {
+            "value": self._setpoint,
+            "timestamp": ts,
+        }
+        return out
+
+
+class FakeFurnace:
     def __init__(self, name: str):
         self.name = name
         self.parent = None
         self.value = 0.0
+        self.ramp_time = PropertyDevice(self, "ramp_time")
+        self.children = [self.ramp_time]
 
     def describe(self) -> dict:
         out = dict()
-        out[f"{self.name}_setpoint"] = {"source": "FakeMFC", "dtype": "number", "shape": []}
-        out[f"{self.name}_readback"] = {"source": "FakeMFC", "dtype": "number", "shape": []}
+        out[f"{self.name}_setpoint"] = {"source": "FakeFurnace", "dtype": "number", "shape": []}
+        out[f"{self.name}_readback"] = {"source": "FakeFurnace", "dtype": "number", "shape": []}
         return out
 
     def read(self) -> dict:
         ts = time.time()
         out = dict()
         out[f"{self.name}_setpoint"] = {"value": self.value, "timestamp": ts}
         out[f"{self.name}_readback"] = {"value": self.value, "timestamp": ts}
         return out
 
     def set(self, value) -> Status:
         self.value = value
-        st = Status()
-
-        def done_later():
-            time.sleep(0.1)
-            st.set_finished()
-
-        threading.Thread(target=done_later).start()
-
-        return st
+        s = Status()
+        s.set_finished()
+        return s
 
 
-class FakeMFCItem(HappiItem):
+class FakeFurnaceItem(HappiItem):
     kwargs = copy.copy(HappiItem.kwargs)
     kwargs.default = {"name": "{{name}}"}
-    device_class = EntryInfo(default="auto_rxn.devices.FakeMFC")
+    device_class = EntryInfo(default="auto_rxn.devices.FakeFurnace")
```

### Comparing `auto_rxn-2023.6.1/auto_rxn/devices/_status.py` & `auto_rxn-2023.7.0/auto_rxn/devices/_status.py`

 * *Files identical despite different names*

### Comparing `auto_rxn-2023.6.1/pyproject.toml` & `auto_rxn-2023.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 
 [tool.flit.metadata]
 module = "auto_rxn"
 dist-name = "auto_rxn"
 author = "auto_rxn developers"
 home-page = "https://github.com/uw-madison-chem-shops/auto_rxn"
 description-file = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 requires = ["appdirs",
             "click",
             "happi",
             "pandas",
             "bluesky",
             "suitcase-csv",
             ]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.flit.metadata.urls]
```

### Comparing `auto_rxn-2023.6.1/PKG-INFO` & `auto_rxn-2023.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: auto_rxn
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: Python package for running chemical reactions as defined by recipe files.
 Home-page: https://github.com/uw-madison-chem-shops/auto_rxn
 Author: auto_rxn developers
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: happi
```

