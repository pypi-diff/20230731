# Comparing `tmp/useq_schema-0.3.2.tar.gz` & `tmp/useq_schema-0.4.0.tar.gz`

## Comparing `useq_schema-0.3.2.tar` & `useq_schema-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 useq_schema-0.3.2/mkdocs.yml
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.2/setup.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/api.md
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/index.md
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/images/favicon.ico
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/axes.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/event.md
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/hardware_autofocus.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/schema/sequence.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.3.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_actions.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_base_model.py
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_channel.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_grid.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_hardware_autofocus.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_mda_event.py
--rw-r--r--   0        0        0    21704 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_mda_sequence.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_position.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_time.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_utils.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/_z.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.3.2/src/useq/py.typed
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_autofocus.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_grid.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_misc.py
--rw-r--r--   0        0        0    18536 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_position_sequence.py
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_sequence.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/test_serialization.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/fixtures/mda.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.3.2/tests/fixtures/mda.yaml
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.3.2/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.3.2/LICENSE
--rw-r--r--   0        0        0     7977 2020-02-02 00:00:00.000000 useq_schema-0.3.2/README.md
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 useq_schema-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 useq_schema-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 useq_schema-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/api.md
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/index.md
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/images/favicon.ico
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/axes.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/event.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/hardware_autofocus.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/schema/sequence.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useq_schema-0.4.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/__init__.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_actions.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_base_model.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_channel.py
+-rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_grid.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_hardware_autofocus.py
+-rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_iter_sequence.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_mda_event.py
+-rw-r--r--   0        0        0    16227 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_mda_sequence.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_position.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_pydantic_compat.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_time.py
+-rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_utils.py
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/_z.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/py.typed
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 useq_schema-0.4.0/src/useq/pycromanager.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_autofocus.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_grid.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_misc.py
+-rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_position_sequence.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_pycromanager.py
+-rw-r--r--   0        0        0    13596 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_sequence.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/test_serialization.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/fixtures/mda.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 useq_schema-0.4.0/tests/fixtures/mda.yaml
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 useq_schema-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 useq_schema-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 useq_schema-0.4.0/README.md
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 useq_schema-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 useq_schema-0.4.0/PKG-INFO
```

### Comparing `useq_schema-0.3.2/.pre-commit-config.yaml` & `useq_schema-0.4.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -31,9 +31,9 @@
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
           - types-PyYAML
-          - pydantic<2.0.0
+          - pydantic>=2
         files: "^src/"
```

### Comparing `useq_schema-0.3.2/mkdocs.yml` & `useq_schema-0.4.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
           import:
             - https://docs.python.org/3/objects.inv
           options:
             heading_level: 3 # default is 2
             show_root_heading: true # default is false
             show_root_full_path: false # default is true
             docstring_style: 'numpy'
-            show_if_no_docstring: true  # default is false
             show_signature: false  # default is true
             annotations_path: 'source' # default is 'brief'
             show_bases: false # default is true
             show_source: false # default is true
 
 extra_css:
   - stylesheets/extra.css
```

### Comparing `useq_schema-0.3.2/.github/workflows/test_and_deploy.yml` & `useq_schema-0.4.0/.github/workflows/test_and_deploy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 name: tests
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 on:
   push:
     branches:
       - main
     tags:
       - "v*"
   pull_request: {}
@@ -14,39 +18,47 @@
     name: Check Manifest
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - run: pip3 install check-manifest && check-manifest
 
   test:
-    name: ${{ matrix.platform }} (${{ matrix.python-version }})
+    name: ${{ matrix.platform }} (${{ matrix.python-version }}) ${{ matrix.pydantic }}
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.8, 3.9, "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
         platform: [ubuntu-latest, macos-latest, windows-latest]
-    steps:
-      - name: Cancel Previous Runs
-        uses: styfle/cancel-workflow-action@0.11.0
-        with:
-          access_token: ${{ github.token }}
+        pydantic: [""]
+        include:
+          - python-version: "3.11"
+            platform: ubuntu-latest
+            pydantic: "'pydantic<2'"
+          - python-version: "3.8"
+            platform: ubuntu-latest
+            pydantic: "'pydantic<2'"
 
+    steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -e .[test]
 
+      - name: Downgrade pydantic
+        if: ${{ matrix.pydantic }}
+        run: pip install ${{ matrix.pydantic }}
+
       - name: Test
         run: pytest -v --color=yes --cov-report=xml --cov=useq
 
       - name: Coverage
         uses: codecov/codecov-action@v3
 
   test_pymmcore:
@@ -70,15 +82,15 @@
           pip install -e pymmcore-plus-from-github[testing]
           pip install -e .[test]
 
       - name: Install Micro-Manager
         run: mmcore install
 
       - name: Test
-        run: pytest -v --color=yes
+        run: pytest -v --color=yes -W default
         working-directory: pymmcore-plus-from-github
 
   test_pymmcore_widgets:
     name: Test pymmcore-widgets
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v3
@@ -98,37 +110,37 @@
           pip install -e pymmcore-widgets-from-github[test,image,pyqt6]
           pip install -e .[test]
 
       - name: Install Micro-Manager
         run: mmcore install
 
       - name: Test
-        run: pytest -v --color=yes -W ignore
+        run: pytest -v --color=yes -W default
         working-directory: pymmcore-widgets-from-github
 
   deploy:
     needs: test
     runs-on: ubuntu-latest
     if: ${{ github.repository == 'pymmcore-plus/useq-schema' && contains(github.ref, 'tags') }}
     steps:
       - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
 
       - name: install
         run: |
-          git tag
           pip install -U pip
           pip install -U build twine
           python -m build
           twine check dist/*
-          ls -lh dist
 
       - name: Build and publish
         run: twine upload dist/*
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
```

### Comparing `useq_schema-0.3.2/docs/index.md` & `useq_schema-0.4.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,16 @@
   in the clojure acquisition engine that drives Micro-Managers multi-dimensional
   acquisitions.
 - For [Pycro-manager](https://github.com/micro-manager/pycro-manager), this
   object is similar to an individual [acquisition event
   `dict`](https://pycro-manager.readthedocs.io/en/latest/apis.html#acquisition-event-specification)
   generated by
   [`multi_d_acquisition_events`](https://github.com/micro-manager/pycro-manager/blob/63cf209a8907fd23932ee9f8016cb6a2b61b45aa/pycromanager/acquire.py#L605),
-  (and, `MDAEvent` provides a `to_pycromanager` method
-  that returns a single dict following the pycro-manager event spec)
+  (and, `useq.pycromanager` provides a `to_pycromanager` method
+  that returns a dict following the pycro-manager event spec)
 - *your object here?...*
 
 ### `MDASequence`
 
 [`useq.MDASequence`][] represents a **sequence** of events – as might be
 generated by the multidimensional acquisition GUI in most microscope software.
 The Python `MDASequence` object is itself
@@ -56,28 +56,28 @@
   object is most similar to
   [`org.micromanager.acquisition.SequenceSettings`](https://github.com/micro-manager/micro-manager/blob/2b0f51a2f916112d39c6135ad35a112065f8d58d/mmstudio/src/main/java/org/micromanager/acquisition/SequenceSettings.java#L39),
   (generated by clicking the `Acquire!` button in the [Multi-D Acquisition
   GUI](https://micro-manager.org/Version_2.0_Users_Guide#multi-dimensional-acquisition))
 - For [Pycro-manager](https://github.com/micro-manager/pycro-manager), this
   object is similar to the
   [`multi_d_acquisition_events`](https://github.com/micro-manager/pycro-manager/blob/63cf209a8907fd23932ee9f8016cb6a2b61b45aa/pycromanager/acquire.py#L605)
-  convenience function, (and the Python `MDASequence` object provides a
-  [`to_pycromanager`][useq._mda_sequence.MDASequence.to_pycromanager] method
-  that returns a list of pycro-manager events)
+  convenience function, (and `useq.pycromanager` provides a
+  `to_pycromanager` method that returns a list of pycro-manager event dicts)
 - *your object here?...*
 
 ## Executing an MDASequence
 
 This library is just a schema, and does not provide any built-in functionality
 for executing an `MDASequence`.  However,
 [`pymmcore-plus`](https://github.com/pymmcore-plus/pymmcore-plus) implements an
 acquisition engine that can execute an `MDASequence` object with
 [micro-manager](https://micro-manager.org) (via the
 [`pymmcore`](https://github.com/micro-manager/pymmcore) python wrapper around
-the C++ MMCore).  See the `pymmcore_plus.CMMCorePlus.run_mda` method for more.
+the C++ MMCore).  See the [pymmcore-plus documentation for
+details](https://pymmcore-plus.github.io/pymmcore-plus/examples/mda/).
 `napari-micromanager` also creates a `useq.MDASequence` object from user input
 and passes it to `pymmcore-plus` for execution.
 
 !!! tip "hi! :wave:"
 
     Have you implemented an acquisition engine that can execute a `useq.MDASequence`?
     Let us know so we can add it here!
@@ -86,15 +86,15 @@
 
 `MDASequence` and `MDAEvent` objects are designed to be serialized and deserialized,
 allowing you to define an entire multi-dimensional acquisition in human-readable
 YAML (or JSON) file, and then load that file into your acquisition engine.
 
 For example, the following file defines an experiment with:
 
-- 3 channels (`DAPI`, `FITC`, and `Cy5`), specifying exposure times for each channel
+- 3 channels (`DAPI`, `FITC`, and `Cy5`), specifying exposure times in ms for each channel
 - a two-phase time-lapse: 3 frames in the first phase, followed by a frame every 10 seconds
 for 40 minutes
 - a Z-stack at each timepoint, with a range of 4 microns and a step size of 0.5 micron
 - two stage positions, specifying a unique Z-stack for the second position
 
 !!! example
```

### Comparing `useq_schema-0.3.2/docs/images/favicon.ico` & `useq_schema-0.4.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/docs/schema/axes.md` & `useq_schema-0.4.0/docs/schema/axes.md`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/docs/stylesheets/extra.css` & `useq_schema-0.4.0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/src/useq/__init__.py` & `useq_schema-0.4.0/src/useq/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,8 +41,12 @@
     "ZAboveBelow",
     "ZAbsolutePositions",
     "ZRangeAround",
     "ZRelativePositions",
     "ZTopBottom",
 ]
 
-MDAEvent.update_forward_refs(MDASequence=MDASequence)
+from useq._pydantic_compat import model_rebuild
+
+model_rebuild(MDAEvent, MDASequence=MDASequence)
+model_rebuild(Position, MDASequence=MDASequence)
+del model_rebuild
```

### Comparing `useq_schema-0.3.2/src/useq/_actions.py` & `useq_schema-0.4.0/src/useq/_actions.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/src/useq/_base_model.py` & `useq_schema-0.4.0/src/useq/_base_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,152 @@
 from __future__ import annotations
 
 import warnings
 from pathlib import Path
+from types import MappingProxyType
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     ClassVar,
-    Dict,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import numpy as np
-from pydantic import BaseModel, root_validator
-from pydantic.error_wrappers import ErrorWrapper, ValidationError
-from pydantic.utils import ROOT_KEY
+from pydantic import BaseModel
 
-from useq._utils import ReadOnlyDict
+from useq._pydantic_compat import PYDANTIC2, model_dump, model_fields
 
 if TYPE_CHECKING:
-    from pydantic.types import StrBytes
-
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
-
+    IncEx = set[int] | set[str] | dict[int, Any] | dict[str, Any] | None
 
 __all__ = ["UseqModel", "FrozenModel"]
 
 _T = TypeVar("_T", bound="FrozenModel")
 _Y = TypeVar("_Y", bound="UseqModel")
 
 
 class FrozenModel(BaseModel):
-    class Config:
-        allow_population_by_field_name = True
-        extra = "allow"
-        frozen = True
-        json_encoders: ClassVar[dict] = {"ReadOnlyDict": dict}
-
-    @root_validator(pre=False, skip_on_failure=True)
-    def _validate_kwargs(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """Validate kwargs for MDASequence."""
-        extra_kwargs = set(values) - set(cls.__fields__)
-        if extra_kwargs:
-            name = getattr(cls, "__name__", "")
-            warnings.warn(
-                f"{name} got unknown keyword arguments: {extra_kwargs}", stacklevel=2
-            )
-            for k in extra_kwargs:
-                values.pop(k)
-        return values
+    if PYDANTIC2:
+        model_config = {
+            "populate_by_name": True,
+            "extra": "ignore",
+            "frozen": True,
+        }
+
+    else:
+
+        class Config:
+            allow_population_by_field_name = True
+            extra = "ignore"
+            frozen = True
+            json_encoders: ClassVar[dict] = {MappingProxyType: dict}
 
     def replace(self: _T, **kwargs: Any) -> _T:
         """Return a new instance replacing specified kwargs with new values.
 
         This model is immutable, so this method is useful for creating a new
         sequence with only a few fields changed.  The uid of the new sequence will
         be different from the original.
 
         The difference between this and `self.copy(update={...})` is that this method
         will perform validation and casting on the new values, whereas `copy` assumes
         that all objects are valid and will not perform any validation or casting.
         """
-        state = self.dict(exclude={"uid"})
+        state = model_dump(self, exclude={"uid"})
         return type(self)(**{**state, **kwargs})
 
+    if PYDANTIC2:
+        # retain pydantic1's json method
+        def json(
+            self,
+            *,
+            indent: int | None = None,  # type: ignore
+            include: IncEx = None,
+            exclude: IncEx = None,  # type: ignore
+            by_alias: bool = False,
+            exclude_unset: bool = False,
+            exclude_defaults: bool = False,
+            exclude_none: bool = False,  # type: ignore
+            round_trip: bool = False,
+            warnings: bool = True,
+        ) -> str:
+            return super().model_dump_json(
+                indent=indent,
+                include=include,
+                exclude=exclude,
+                by_alias=by_alias,
+                exclude_unset=exclude_unset,
+                exclude_defaults=exclude_defaults,
+                exclude_none=exclude_none,
+                round_trip=round_trip,
+                warnings=warnings,
+            )
+
+        # we let this one be deprecated
+        # def dict()
+
+    elif not TYPE_CHECKING:
+        # Backport pydantic2 methods so that useq-0.1.0 can be used with pydantic1
+
+        def model_dump_json(self, **kwargs: Any) -> str:
+            """Backport of pydantic2's model_dump_json method."""
+            return self.json(**kwargs)
+
+        def model_dump(self, **kwargs: Any) -> dict[str, Any]:
+            """Backport of pydantic2's model_dump_json method."""
+            return self.dict(**kwargs)
+
 
 class UseqModel(FrozenModel):
     def __repr_args__(self) -> ReprArgs:
+        """Only show fields that are not None or equal to their default value."""
         return [
             (k, val)
             for k, val in super().__repr_args__()
-            if k in self.__fields__
+            if k in model_fields(self)
             and val
             != (
-                self.__fields__[k].default_factory()  # type: ignore
-                if self.__fields__[k].default_factory is not None
-                else self.__fields__[k].default
+                factory()
+                if (factory := model_fields(self)[k].default_factory) is not None
+                else model_fields(self)[k].default
             )
         ]
 
-    def __repr__(self) -> str:
-        """Repr, that only shows values that are changed form the defaults."""
-        from textwrap import indent
-
-        lines = []
-        for k, current in sorted(self.__repr_args__()):
-            if not k:
-                continue
-            f = self.__fields__[k]
-            default = (
-                self.__fields__[k].default_factory()  # type: ignore
-                if self.__fields__[k].default_factory is not None
-                else self.__fields__[k].default
-            )
-            if current != default:
-                lines.append(f"{f.name}={current!r},")
-        if len(lines) == 1:
-            body = lines[-1].rstrip(",")
-        elif lines:
-            body = "\n" + indent("\n".join(lines), "   ") + "\n"
-        else:
-            body = ""
-        return f"{self.__class__.__qualname__}({body})"
-
     @classmethod
-    def parse_raw(
-        cls: Type[_Y],
-        b: StrBytes,
-        *,
-        content_type: Optional[str] = None,
-        encoding: str = "utf8",
-        proto: Optional[str] = None,
-        allow_pickle: bool = False,
-    ) -> _Y:
-        if content_type is None:
-            assume_yaml = False
-        else:
-            assume_yaml = ("yaml" in content_type) or ("yml" in content_type)
-
-        if proto == "yaml" or assume_yaml:
+    def from_file(cls: Type[_Y], path: Union[str, Path]) -> _Y:
+        """Return an instance of this class from a file.  Supports JSON and YAML."""
+        path = Path(path)
+        if path.suffix in {".yaml", ".yml"}:
             import yaml
 
-            try:
-                obj = yaml.safe_load(b)
-            except Exception as e:
-                raise ValidationError([ErrorWrapper(e, loc=ROOT_KEY)], cls) from e
-            return cls.parse_obj(obj)
-        return super().parse_raw(
-            b,
-            content_type=content_type,  # type: ignore
-            encoding=encoding,
-            proto=proto,  # type: ignore
-            allow_pickle=allow_pickle,
-        )
+            obj = yaml.safe_load(path.read_bytes())
+        elif path.suffix == ".json":
+            import json
+
+            obj = json.loads(path.read_bytes())
+        else:  # pragma: no cover
+            raise ValueError(f"Unknown file type: {path.suffix}")
 
-    @classmethod
-    def parse_file(
-        cls: Type[_Y],
-        path: Union[str, Path],
-        *,
-        content_type: Optional[str] = None,
-        encoding: str = "utf8",
-        proto: Optional[str] = None,
-        allow_pickle: bool = False,
-    ) -> _Y:
-        if encoding is None:
-            assume_yaml = False
-        elif content_type:
-            assume_yaml = ("yaml" in content_type) or ("yml" in content_type)
-        else:
-            assume_yaml = str(path).endswith((".yml", ".yaml"))
-
-        if proto == "yaml" or assume_yaml:
-            return cls.parse_raw(
-                Path(path).read_bytes(),
-                content_type=content_type or "application/yaml",
-                encoding=encoding,
-                proto="yaml",
-                allow_pickle=allow_pickle,
-            )
+        return cls.model_validate(obj) if PYDANTIC2 else cls.parse_obj(obj)
 
-        return super().parse_file(
-            path,
-            content_type=content_type,  # type: ignore
-            encoding=encoding,
-            proto=proto,  # type: ignore
-            allow_pickle=allow_pickle,
+    @classmethod
+    def parse_file(cls: Type[_Y], path: Union[str, Path], **kwargs: Any) -> _Y:
+        warnings.warn(  # pragma: no cover
+            "parse_file is deprecated. Use from_file instead.",
+            DeprecationWarning,
+            stacklevel=2,
         )
+        return cls.from_file(path)  # pragma: no cover
 
     def yaml(
         self,
         *,
         include: Optional[Union[set, dict]] = None,
         exclude: Optional[Union[set, dict]] = None,
         by_alias: bool = False,
@@ -199,21 +170,22 @@
         yaml.SafeDumper.add_multi_representer(
             timedelta, lambda dumper, data: dumper.represent_str(str(data))
         )
         yaml.SafeDumper.add_multi_representer(
             Enum, lambda dumper, data: dumper.represent_str(str(data.value))
         )
         yaml.SafeDumper.add_multi_representer(
-            ReadOnlyDict, lambda dumper, data: dumper.represent_dict(data)
+            MappingProxyType, lambda dumper, data: dumper.represent_dict(data)
         )
         yaml.SafeDumper.add_multi_representer(
-            np.floating, lambda dumper, data: dumper.represent_float(float(data))
+            np.floating, lambda dumper, d: dumper.represent_float(float(d))
         )
 
-        data = self.dict(
+        data = model_dump(
+            self,
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
```

### Comparing `useq_schema-0.3.2/src/useq/_grid.py` & `useq_schema-0.4.0/src/useq/_grid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
+import contextlib
 import math
 from enum import Enum
 from functools import partial
-from typing import Any, Callable, Iterator, NamedTuple, Sequence, Tuple, Union
+from typing import Any, Callable, Iterator, NamedTuple, Optional, Sequence, Tuple, Union
 
 import numpy as np
-from pydantic import validator
+from pydantic import Field
 
 from useq._base_model import FrozenModel
+from useq._pydantic_compat import FROZEN, PYDANTIC2, field_validator
 
 
 class RelativeTo(Enum):
     center = "center"
     top_left = "top_left"
 
 
@@ -106,21 +108,42 @@
         Overlap between grid positions in percent. If a single value is provided, it is
         used for both x and y. If a tuple is provided, the first value is used
         for x and the second for y.
     mode : OrderMode
         Define the ways of ordering the grid positions. Options are
         row_wise, column_wise, row_wise_snake, column_wise_snake and spiral.
         By default, row_wise_snake.
+    fov_width : Optional[float]
+        Width of the field of view in microns.  If not provided, acquisition engines
+        should use current width of the FOV based on the current objective and camera.
+        Engines MAY override this even if provided.
+    fov_height : Optional[float]
+        Height of the field of view in microns. If not provided, acquisition engines
+        should use current height of the FOV based on the current objective and camera.
+        Engines MAY override this even if provided.
     """
 
-    overlap: Tuple[float, float] = (0.0, 0.0)
-    mode: OrderMode = OrderMode.row_wise_snake
+    # Overriding FrozenModel to make fov_width and fov_height mutable.
+    if PYDANTIC2:
+        model_config = {"validate_assignment": True, "frozen": False}
+    else:
+
+        class Config:
+            validate_assignment = True
+            frozen = False
+
+    overlap: Tuple[float, float] = Field((0.0, 0.0), **FROZEN)  # type: ignore
+    mode: OrderMode = Field(OrderMode.row_wise_snake, **FROZEN)  # type: ignore
+    fov_width: Optional[float] = Field(None)
+    fov_height: Optional[float] = Field(None)
 
-    @validator("overlap", pre=True)
+    @field_validator("overlap", mode="before")
     def _validate_overlap(cls, v: Any) -> Tuple[float, float]:
+        with contextlib.suppress(TypeError, ValueError):
+            v = float(v)
         if isinstance(v, float):
             return (v,) * 2
         if isinstance(v, Sequence) and len(v) == 2:
             return float(v[0]), float(v[1])
         raise ValueError(  # pragma: no cover
             "overlap must be a float or a tuple of two floats"
         )
@@ -139,57 +162,84 @@
         """Return the number of rows, given a grid step size."""
         raise NotImplementedError
 
     def _ncolumns(self, dx: float) -> int:
         """Return the number of columns, given a grid step size."""
         raise NotImplementedError
 
+    def num_positions(self) -> int:
+        """Return the number of individual positions in the grid.
+
+        Note: For GridFromEdges, this will depend on field of view size.  If no
+        field of view size is provided, the number of positions will be 1.
+        """
+        if not self.is_relative and (self.fov_width is None or self.fov_height is None):
+            raise ValueError(
+                "Retrieving the number of positions in a GridFromEdges plan requires "
+                "that the field of view size be set."
+            )
+
+        dx, dy = self._step_size(self.fov_width or 1, self.fov_height or 1)
+        rows = self._nrows(dy)
+        cols = self._ncolumns(dx)
+        return rows * cols
+
     def iter_grid_positions(
-        self, fov_width: float, fov_height: float
+        self,
+        fov_width: float | None = None,
+        fov_height: float | None = None,
+        *,
+        mode: OrderMode | None = None,
     ) -> Iterator[GridPosition]:
         """Iterate over all grid positions, given a field of view size."""
-        dx, dy = self._step_size(fov_width, fov_height)
+        _fov_width = fov_width or self.fov_width or 1.0
+        _fov_height = fov_height or self.fov_height or 1.0
+        mode = self.mode if mode is None else OrderMode(mode)
+
+        dx, dy = self._step_size(_fov_width, _fov_height)
         rows = self._nrows(dy)
         cols = self._ncolumns(dx)
         x0 = self._offset_x(dx)
         y0 = self._offset_y(dy)
-        for r, c in _INDEX_GENERATORS[self.mode](rows, cols):
+
+        for r, c in _INDEX_GENERATORS[mode](rows, cols):
             yield GridPosition(x0 + c * dx, y0 - r * dy, r, c, self.is_relative)
 
-    def __len__(self) -> int:
-        return len(list(self.iter_grid_positions(1, 1)))
+    def __iter__(self) -> Iterator[GridPosition]:  # type: ignore
+        yield from self.iter_grid_positions()
 
     def _step_size(self, fov_width: float, fov_height: float) -> Tuple[float, float]:
         dx = fov_width - (fov_width * self.overlap[0]) / 100
         dy = fov_height - (fov_height * self.overlap[1]) / 100
         return dx, dy
 
 
 class GridFromEdges(_GridPlan):
-    """Yield absolute stage positions to cover a bounded area...
+    """Yield absolute stage positions to cover a bounded area.
 
-    ...defined by setting the stage coordinates of the top, left,
-    bottom and right edges.
+    The bounded area is defined by top, left, bottom and right edges in
+    stage coordinates.
 
     Attributes
     ----------
     top : float
-        top stage position of the bounding area
+        Top stage position of the bounding area
     left : float
-        left stage position of the bounding area
+        Left stage position of the bounding area
     bottom : float
-        bottom stage position of the bounding area
+        Bottom stage position of the bounding area
     right : float
-        right stage position of the bounding area
+        Right stage position of the bounding area
     """
 
-    top: float
-    left: float
-    bottom: float
-    right: float
+    # everything but fov_width and fov_height is immutable
+    top: float = Field(..., **FROZEN)  # type: ignore
+    left: float = Field(..., **FROZEN)  # type: ignore
+    bottom: float = Field(..., **FROZEN)  # type: ignore
+    right: float = Field(..., **FROZEN)  # type: ignore
 
     def _nrows(self, dy: float) -> int:
         total_height = abs(self.top - self.bottom) + dy
         return math.ceil(total_height / dy)
 
     def _ncolumns(self, dx: float) -> int:
         total_width = abs(self.right - self.left) + dx
@@ -213,17 +263,18 @@
         Number of columns.
     relative_to : RelativeTo
         Point in the grid to which the coordinates are relative. If "center", the grid
         is centered around the origin. If "top_left", the grid is positioned such that
         the top left corner is at the origin.
     """
 
-    rows: int
-    columns: int
-    relative_to: RelativeTo = RelativeTo.center
+    # everything but fov_width and fov_height is immutable
+    rows: int = Field(..., **FROZEN)  # type: ignore
+    columns: int = Field(..., **FROZEN)  # type: ignore
+    relative_to: RelativeTo = Field(RelativeTo.center, **FROZEN)  # type: ignore
 
     @property
     def is_relative(self) -> bool:
         return True
 
     def _nrows(self, dy: float) -> int:
         return self.rows
```

### Comparing `useq_schema-0.3.2/src/useq/_hardware_autofocus.py` & `useq_schema-0.4.0/src/useq/_hardware_autofocus.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Optional, Tuple
 
 from pydantic import PrivateAttr
 
 from useq._actions import HardwareAutofocus
 from useq._base_model import FrozenModel
 from useq._mda_event import MDAEvent
+from useq._pydantic_compat import model_copy
 
 
 class AutoFocusPlan(FrozenModel):
     """Base class for hardware autofocus plans.
 
     Attributes
     ----------
@@ -41,15 +42,15 @@
 
         updates: dict[str, Any] = {"action": self.as_action()}
         if event.z_pos is not None and event.sequence is not None:
             zplan = event.sequence.z_plan
             if zplan and zplan.is_relative and "z" in event.index:
                 updates["z_pos"] = event.z_pos - list(zplan)[event.index["z"]]
 
-        return event.copy(update=updates)
+        return model_copy(event, update=updates)
 
     def should_autofocus(self, event: MDAEvent) -> bool:
         """Method that must be implemented by a subclass.
 
         Should return True if autofocus should be performed (see
         [`useq.AxesBasedAF`][]).
         """
```

### Comparing `useq_schema-0.3.2/src/useq/_mda_event.py` & `useq_schema-0.4.0/src/useq/_mda_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from __future__ import annotations
+# don't add __future__.annotations here
+# pydantic2 isn't rebuilding the model correctly
 
 import warnings
+from types import MappingProxyType
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
+    Mapping,
     NamedTuple,
-    NoReturn,
     Optional,
     Sequence,
     Tuple,
 )
 
-from pydantic import Field, validator
+from pydantic import Field
 
 from useq._actions import AcquireImage, AnyAction
 from useq._base_model import UseqModel
-from useq._utils import ReadOnlyDict
+from useq._pydantic_compat import PYDANTIC2, field_serializer
 
 if TYPE_CHECKING:
     from useq._mda_sequence import MDASequence
+    from useq.pycromanager import PycroManagerEvent
 
     ReprArgs = Sequence[Tuple[Optional[str], Any]]
 
 
 class Channel(UseqModel):
     """Channel in a MDA event.
 
@@ -61,16 +64,16 @@
     """
 
     device_name: str
     property_name: str
     property_value: Any
 
 
-def _readonly(self: object, *_: Any, **__: Any) -> NoReturn:
-    raise RuntimeError(f"Cannot modify {type(self).__name__}")
+def _float_or_none(v: Any) -> Optional[float]:
+    return float(v) if v is not None else v
 
 
 class MDAEvent(UseqModel):
     """Define a single event in a [`MDASequence`][useq.MDASequence].
 
     Usually, this object will be generator by iterating over a
     [`MDASequence`][useq.MDASequence] (see [`useq.MDASequence.iter_events`][]).
@@ -83,16 +86,16 @@
     channel : Channel | None
         Channel to use for this event. If `None`, implies use current channel.
         By default, `None`.  `Channel` is a simple pydantic object with two attributes:
         `config` and `group`.  `config` is the name of the configuration to use for this
         channel, (e.g. `"488nm"`, `"DAPI"`, `"FITC"`).  `group` is the name of the group
         to which this channel belongs. By default, `"Channel"`.
     exposure : float | None
-        Exposure time in seconds. If not provided, implies use current exposure time.
-        By default, `None`.
+        Exposure time in milliseconds. If not provided, implies use current exposure
+        time. By default, `None`.
     min_start_time : float | None
         Minimum start time of this event, in seconds.  If provided, the engine will
         pause until this time has elapsed (relative to the start of the sequence)
         before starting this event. By default, `None`.
     pos_name : str | None
         The name assigned to the position. By default, `None`.
     x_pos : float | None
@@ -123,68 +126,48 @@
         If True, the illumination shutter should be left open after the event has
         been executed, otherwise it should be closed. By default, `False`."
         This is useful when the sequence of events being executed use the same
         illumination scheme (such as a z-stack in a single channel), and closing and
         opening the shutter between events would be slow.
     """
 
-    index: ReadOnlyDict[str, int] = Field(default_factory=ReadOnlyDict)
+    # MappingProxyType is not subscriptable on Python 3.8
+    index: Mapping[str, int] = Field(default_factory=lambda: MappingProxyType({}))
     channel: Optional[Channel] = None
     exposure: Optional[float] = Field(default=None, gt=0.0)
     min_start_time: Optional[float] = None  # time in sec
     pos_name: Optional[str] = None
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
     z_pos: Optional[float] = None
-    sequence: Optional[MDASequence] = Field(default=None, repr=False)
+    sequence: Optional["MDASequence"] = Field(default=None, repr=False)
     properties: Optional[List[PropertyTuple]] = None
     metadata: Dict[str, Any] = Field(default_factory=dict)
     action: AnyAction = Field(default_factory=AcquireImage)
     keep_shutter_open: bool = False
 
-    # action
-    # keep shutter open between channels/steps
     @property
     def global_index(self) -> int:
         warnings.warn(
             "global_index is no longer functional.  Use `enumerate()` "
             "on an iterable of events instead.",
             stacklevel=2,
         )
         return 0
 
-    @validator("index", pre=True)
-    def validate_index(cls, v: dict) -> ReadOnlyDict[str, int]:
-        return ReadOnlyDict(v)
-
-    def __repr_args__(self) -> ReprArgs:
-        d = self.__dict__.copy()
-        d.pop("sequence")
-        return list(d.items())
-
-    def to_pycromanager(self) -> dict:
-        """Convenience method to convert this event to a pycro-manager events.
-
-        See: <https://pycro-manager.readthedocs.io/en/latest/apis.html>
-        """
-        d: Dict[str, Any] = {
-            "exposure": self.exposure,
-            "axes": {},
-            "z": self.z_pos,
-            "x": self.x_pos,
-            "y": self.y_pos,
-            "min_start_time": self.min_start_time,
-            "channel": self.channel and self.channel.dict(),
-        }
-        if "p" in self.index:
-            d["axes"]["position"] = self.index["p"]
-        if "t" in self.index:
-            d["axes"]["time"] = self.index["t"]
-        if "z" in self.index:
-            d["axes"]["z"] = self.index["z"]
-        if self.properties:
-            d["properties"] = [list(p) for p in self.properties]
-
-        for key, value in list(d.items()):
-            if value is None:
-                d.pop(key)
-        return d
+    def to_pycromanager(self) -> "PycroManagerEvent":
+        from useq.pycromanager import to_pycromanager
+
+        warnings.warn(
+            "useq.MDAEvent.to_pycromanager() is deprecated and will be removed in a "
+            "future version. Useq useq.pycromanager.to_pycromanager(event) instead.",
+            FutureWarning,
+            stacklevel=2,
+        )
+
+        return to_pycromanager(self)
+
+    if PYDANTIC2:
+        _si = field_serializer("index", mode="plain")(lambda v: dict(v))
+        _sx = field_serializer("x_pos", mode="plain")(_float_or_none)
+        _sy = field_serializer("y_pos", mode="plain")(_float_or_none)
+        _sz = field_serializer("z_pos", mode="plain")(_float_or_none)
```

### Comparing `useq_schema-0.3.2/tests/conftest.py` & `useq_schema-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/tests/test_autofocus.py` & `useq_schema-0.4.0/tests/test_autofocus.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 
 from typing import Iterable
 
 import pytest
 
 import useq
 from useq import AxesBasedAF, HardwareAutofocus, MDASequence
+from useq._pydantic_compat import model_copy
 
 ZRANGE2 = useq.ZRangeAround(range=2, step=1)
 ZPOS_30 = useq.Position(z=30.0)
 ZPOS_200 = useq.Position(z=200.0)
 GRID_PLAN = useq.GridRelative(rows=2, columns=1)
 TWO_CH = MDASequence(stage_positions=[ZPOS_30], channels=["DAPI", "FITC"])
 TWO_CH_TWO_P = TWO_CH.replace(stage_positions=[ZPOS_30, ZPOS_200])
 TWO_CH_TWO_P_GRID = TWO_CH_TWO_P.replace(grid_plan=GRID_PLAN)
 TWO_CH_TWO_P_T = TWO_CH_TWO_P.replace(time_plan={"interval": 1, "loops": 2})
 NO_CH_ZSTACK = MDASequence(stage_positions=[ZPOS_30], z_plan=ZRANGE2)
 TWO_CH_ZSTACK = NO_CH_ZSTACK.replace(channels=["DAPI", "FITC"])
 AF = AxesBasedAF(autofocus_device_name="Z", autofocus_motor_offset=40, axes=())
-AF_C = AF.copy(update={"axes": ("c",)})
-AF_G = AF.copy(update={"axes": ("g",)})
-AF_P = AF.copy(update={"axes": ("p",)})
-AF_Z = AF.copy(update={"axes": ("z",)})
+AF_C = model_copy(AF, update={"axes": ("c",)})
+AF_G = model_copy(AF, update={"axes": ("g",)})
+AF_P = model_copy(AF, update={"axes": ("p",)})
+AF_Z = model_copy(AF, update={"axes": ("z",)})
 AF_SEQ_C = MDASequence(autofocus_plan=AF_C)
 SUB_P_AF_C = useq.Position(z=10, sequence=AF_SEQ_C)
 SUB_P_AF_G = useq.Position(z=10, sequence=MDASequence(autofocus_plan=AF_G))
 SUB_P_AF_P = useq.Position(z=10, sequence=MDASequence(autofocus_plan=AF_P))
 SUB_P_AF_Z = useq.Position(z=10, sequence=MDASequence(autofocus_plan=AF_Z))
 TWO_CH_SUBPAF_C = TWO_CH.replace(stage_positions=[ZPOS_30, SUB_P_AF_C])
 TWO_CH_SUBPAF_Z = TWO_CH.replace(stage_positions=[ZPOS_30, SUB_P_AF_Z])
@@ -65,22 +66,21 @@
 @pytest.mark.parametrize("mda, af_axes, expected_af_indices", AF_TESTS)
 def test_autofocus(
     mda: MDASequence,
     af_axes: tuple[str, ...],
     expected_af_indices: Iterable[int],
 ) -> None:
     if af_axes:
-        mda = mda.replace(autofocus_plan=AF.copy(update={"axes": af_axes}))
+        mda = mda.replace(autofocus_plan=model_copy(AF, update={"axes": af_axes}))
         assert isinstance(mda.autofocus_plan, AxesBasedAF)
         assert mda.autofocus_plan.axes == af_axes
 
     actual = [i for i, e in enumerate(mda) if isinstance(e.action, HardwareAutofocus)]
     expected = list(expected_af_indices)
-    if expected != actual:
-        raise AssertionError(f"Expected AF indices at {expected} but got {actual}")
+    assert expected == actual, "Unexpected AF indices"
 
 
 def test_autofocus_z_pos() -> None:
     mda = TWO_CH.replace(
         stage_positions=[ZPOS_200], z_plan=ZRANGE2, autofocus_plan=AF_C
     )
     assert all(e.z_pos == 200 for e in mda if isinstance(e.action, HardwareAutofocus))
```

### Comparing `useq_schema-0.3.2/tests/test_grid.py` & `useq_schema-0.4.0/tests/test_grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,7 +78,12 @@
         (0.0, 0.0),
         (-1.0, 0.0),
         (-1.0, -1.0),
         (0.0, -1.0),
         (1.0, -1.0),
         (2.0, -1.0),
     ]
+
+
+def test_num_position_error() -> None:
+    with pytest.raises(ValueError, match="the field of view size be set"):
+        GridFromEdges(top=1, left=-1, bottom=-1, right=2).num_positions()
```

### Comparing `useq_schema-0.3.2/tests/test_position_sequence.py` & `useq_schema-0.4.0/tests/test_position_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,15 @@
 def expect_mda(mda: MDASequence, **expectations: Sequence[Any]) -> None:
     results: dict[str, list[Any]] = {}
     for event in mda:
         for attr_name in expectations:
             results.setdefault(attr_name, []).append(getattr(event, attr_name))
 
     for attr_name, actual_value in results.items():
-        expect = expectations[attr_name]
-        if actual_value != expect:
-            raise AssertionError(
-                f"Expected {attr_name} to be {expect}, but got {actual_value}"
-            )
+        assert actual_value == expectations[attr_name]
 
 
 # test channels
 def test_channel_only_in_position_sub_sequence() -> None:
     # test that a sub-position with a sequence has a channel, but not the main sequence
     expect_mda(
         MDASequence(stage_positions=[EMPTY, useq.Position(sequence=SEQ_1_CH)]),
```

### Comparing `useq_schema-0.3.2/tests/test_sequence.py` & `useq_schema-0.4.0/tests/test_sequence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+import json
 from typing import Any, List, Sequence, Tuple
 
 import numpy as np
 import pytest
 from pydantic import BaseModel
 
 from useq import (
@@ -16,15 +17,16 @@
     TIntervalDuration,
     TIntervalLoops,
     ZAboveBelow,
     ZAbsolutePositions,
     ZRangeAround,
     ZRelativePositions,
 )
-from useq._grid import OrderMode, RelativeTo
+from useq._grid import GridPosition
+from useq._pydantic_compat import PYDANTIC2
 
 _T = List[Tuple[Any, Sequence[float]]]
 
 z_as_class: _T = [
     (ZAboveBelow(above=8, below=4, step=2), [-4, -2, 0, 2, 4, 6, 8]),
     (ZAbsolutePositions(absolute=[0, 0.5, 5]), [0, 0.5, 5]),
     (ZRelativePositions(relative=[0, 0.5, 5]), [0, 0.5, 5]),
@@ -63,41 +65,50 @@
         [0, 0.25, 0.50, 0.75, 1, 2, 3, 4, 5],
     ),
     ({"loops": 5, "duration": {"milliseconds": 8}}, [0, 0.002, 0.004, 0.006, 0.008]),
     ({"loops": 5, "duration": {"seconds": 8}}, [0, 2, 4, 6, 8]),
 ]
 t_inputs = t_as_class + t_as_dict
 
-g_as_dict = [
+g_inputs = [
     (
-        {"overlap": 10.0, "rows": 1, "columns": 2, "relative_to": "center"},
-        [(10.0, 10.0), OrderMode.row_wise_snake, 1, 2, RelativeTo.center],
-    ),
-    (
-        {"overlap": 10.0, "rows": 1, "columns": 2, "relative_to": "top_left"},
-        [(10.0, 10.0), OrderMode.row_wise_snake, 1, 2, RelativeTo.top_left],
+        GridRelative(overlap=10, rows=1, columns=2, relative_to="center"),
+        [
+            GridPosition(x=-0.45, y=0.0, row=0, col=0, is_relative=True),
+            GridPosition(x=0.45, y=0.0, row=0, col=1, is_relative=True),
+        ],
     ),
     (
-        {"overlap": 10.0, "top": 0.0, "left": 0.0, "bottom": 2.0, "right": 2.0},
-        [(10.0, 10.0), OrderMode.row_wise_snake, 0.0, 0.0, 2.0, 2.0],
+        GridRelative(overlap=0, rows=1, columns=2, relative_to="top_left"),
+        [
+            GridPosition(x=0.0, y=0.0, row=0, col=0, is_relative=True),
+            GridPosition(x=1.0, y=0.0, row=0, col=1, is_relative=True),
+        ],
     ),
-]
-
-g_as_class = [
     (
-        GridRelative(overlap=10.0, rows=1, columns=2, relative_to="center"),
-        [(10.0, 10.0), OrderMode.row_wise_snake, 1, 2, RelativeTo.center],
+        GridRelative(overlap=(20, 40), rows=2, columns=2),
+        [
+            GridPosition(x=-0.4, y=0.3, row=0, col=0, is_relative=True),
+            GridPosition(x=0.4, y=0.3, row=0, col=1, is_relative=True),
+            GridPosition(x=0.4, y=-0.3, row=1, col=1, is_relative=True),
+            GridPosition(x=-0.4, y=-0.3, row=1, col=0, is_relative=True),
+        ],
     ),
     (
-        GridFromEdges(overlap=10.0, top=0.0, left=0, bottom=2, right=2),
-        [(10.0, 10.0), OrderMode.row_wise_snake, 0.0, 0.0, 2.0, 2.0],
+        GridFromEdges(
+            overlap=0, top=0, left=0, bottom=20, right=20, fov_height=20, fov_width=20
+        ),
+        [
+            GridPosition(x=0.0, y=20.0, row=0, col=0, is_relative=False),
+            GridPosition(x=20.0, y=20.0, row=0, col=1, is_relative=False),
+            GridPosition(x=20.0, y=0.0, row=1, col=1, is_relative=False),
+            GridPosition(x=0.0, y=0.0, row=1, col=0, is_relative=False),
+        ],
     ),
 ]
-g_inputs = g_as_class + g_as_dict
-
 
 all_orders = ["".join(i) for i in itertools.permutations("tpgcz")]
 
 c_inputs = [
     ("DAPI", ("Channel", "DAPI")),
     ({"config": "DAPI"}, ("Channel", "DAPI")),
     ({"config": "DAPI", "group": "Group", "acquire_every": 3}, ("Group", "DAPI")),
@@ -125,27 +136,31 @@
     (np.array([0, 0]), (0, 0, None)),
     ([Position(x=100, y=200, z=300)], (100, 200, 300)),
 ]
 
 
 @pytest.mark.parametrize("zplan, zexpectation", z_inputs)
 def test_z_plan(zplan: Any, zexpectation: Sequence[float]) -> None:
-    assert list(MDASequence(z_plan=zplan).z_plan) == zexpectation
+    z_plan = MDASequence(z_plan=zplan).z_plan
+    assert z_plan and list(z_plan) == zexpectation
+    assert z_plan.num_positions() == len(zexpectation)
 
 
 @pytest.mark.parametrize("gridplan, gridexpectation", g_inputs)
 def test_g_plan(gridplan: Any, gridexpectation: Sequence[Any]) -> None:
-    assert [
-        i[1] for i in list(MDASequence(grid_plan=gridplan).grid_plan)
-    ] == gridexpectation
+    g_plan = MDASequence(grid_plan=gridplan).grid_plan
+    assert g_plan and list(g_plan) == gridexpectation
+    assert g_plan.num_positions() == len(gridexpectation)
 
 
 @pytest.mark.parametrize("tplan, texpectation", t_inputs)
 def test_time_plan(tplan: Any, texpectation: Sequence[float]) -> None:
-    assert list(MDASequence(time_plan=tplan).time_plan) == texpectation
+    time_plan = MDASequence(time_plan=tplan).time_plan
+    assert time_plan and list(time_plan) == texpectation
+    assert time_plan.num_timepoints() == len(texpectation)
 
 
 @pytest.mark.parametrize("channel, cexpectation", c_inputs)
 def test_channel(channel: Any, cexpectation: Sequence[float]) -> None:
     channel = MDASequence(channels=[channel]).channels[0]
     assert (channel.group, channel.config) == cexpectation
 
@@ -257,21 +272,24 @@
 
     assert list(mda.z_plan) == zexpectation
     assert list(mda.time_plan) == texpectation
     assert (mda.channels[0].group, mda.channels[0].config) == cexpectation
     position = mda.stage_positions[0]
     assert (position.x, position.y, position.z) == pexpectation
 
-    assert mda.to_pycromanager()
-
 
 @pytest.mark.parametrize("cls", [MDASequence, MDAEvent])
 def test_schema(cls: BaseModel) -> None:
-    assert cls.schema()
-    assert cls.schema_json()
+    if PYDANTIC2:
+        schema = cls.model_json_schema()
+        assert schema
+        assert json.dumps(schema)
+    else:
+        assert cls.schema()
+        assert cls.schema_json()
 
 
 def test_z_position() -> None:
     mda = MDASequence(axis_order="tpcz", stage_positions=[(222, 1, 10), (111, 1, 20)])
     assert not mda.z_plan
     for event in mda:
         assert event.z_pos
@@ -305,24 +323,83 @@
 
 
 def test_mda_str_repr(mda1: MDASequence) -> None:
     assert str(mda1)
     assert repr(mda1)
 
 
-def test_mda_warns_extra() -> None:
-    with pytest.warns(UserWarning, match="got unknown keyword arguments"):
-        seq = MDASequence(random_key="random_value")
-    assert not hasattr(seq, "random_key")
-
-    with pytest.warns(UserWarning, match="got unknown keyword arguments"):
-        Position(random_key="random_value")
-
-
-def test_skip_channel_do_stack_no_zplan():
+def test_skip_channel_do_stack_no_zplan() -> None:
     mda = MDASequence(channels=[{"config": "DAPI", "do_stack": False}])
     assert len(list(mda)) == 1
 
 
 def test_event_action_union() -> None:
     # test that action unions work
     MDAEvent(action={"autofocus_device_name": "Z", "autofocus_motor_offset": 25})
+
+
+def test_set_fov_deprecation() -> None:
+    seq = MDASequence(grid_plan=GridRelative(overlap=10, rows=1, columns=2))
+    assert seq.grid_plan
+    assert list(seq.grid_plan) == [(-0.45, 0.0, 0, 0, True), (0.45, 0.0, 0, 1, True)]
+    with pytest.warns(match="deprecated"):
+        seq.set_fov_size((20, 20))
+    assert seq.grid_plan.fov_width == 20
+    assert list(seq.grid_plan) == [(-9, 0.0, 0, 0, True), (9, 0.0, 0, 1, True)]
+
+
+def test_keep_shutter_open() -> None:
+    # with z as the last axis, the shutter will be left open
+    # whenever z is the first index (since there are only 2 z planes)
+    mda1 = MDASequence(
+        axis_order="tcz",
+        channels=["DAPI", "FITC"],
+        time_plan=TIntervalLoops(loops=2, interval=0),
+        z_plan=ZRangeAround(range=1, step=1),
+        keep_shutter_open_across="z",
+    )
+    assert all(e.keep_shutter_open for e in mda1 if e.index["z"] == 0)
+
+    # with c as the last axis, the shutter will never be left open
+    mda2 = MDASequence(
+        axis_order="tzc",
+        channels=["DAPI", "FITC"],
+        time_plan=TIntervalLoops(loops=2, interval=0),
+        z_plan=ZRangeAround(range=1, step=1),
+        keep_shutter_open_across="z",
+    )
+    assert not any(e.keep_shutter_open for e in mda2)
+
+    # because t is changing faster than z, the shutter will never be left open
+    mda3 = MDASequence(
+        axis_order="czt",
+        channels=["DAPI", "FITC"],
+        time_plan=TIntervalLoops(loops=2, interval=0),
+        z_plan=ZRangeAround(range=1, step=1),
+        keep_shutter_open_across="z",
+    )
+    assert not any(e.keep_shutter_open for e in mda3)
+
+    # but, if we include 't' in the keep_shutter_open_across,
+    # it will be left open except when it's the last t and last z
+    mda4 = MDASequence(
+        axis_order="czt",
+        channels=["DAPI", "FITC"],
+        time_plan=TIntervalLoops(loops=2, interval=0),
+        z_plan=ZRangeAround(range=1, step=1),
+        keep_shutter_open_across=("z", "t"),
+    )
+    for event in mda4:
+        is_last_zt = bool(event.index["t"] == 1 and event.index["z"] == 1)
+        assert event.keep_shutter_open != is_last_zt
+
+    # even though c is the last axis, and comes after g, because the grid happens
+    # on a subsequence shutter will be open across the grid for each position
+    subseq = MDASequence(grid_plan=GridRelative(rows=2, columns=2))
+    mda5 = MDASequence(
+        axis_order="pgc",
+        channels=["DAPI", "FITC"],
+        stage_positions=[Position(sequence=subseq)],
+        keep_shutter_open_across="g",
+    )
+    for event in mda5:
+        assert event.keep_shutter_open != (event.index["g"] == 3)
```

### Comparing `useq_schema-0.3.2/tests/test_serialization.py` & `useq_schema-0.4.0/tests/test_serialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 from useq import MDASequence
 
 
 @pytest.mark.parametrize("ext", ["json", "yaml"])
 def test_serialization(mda1: MDASequence, ext: str) -> None:
     FILE = Path(__file__).parent / "fixtures" / f"mda.{ext}"
     text = FILE.read_text()
-    mda = MDASequence.parse_file(str(FILE))
+    mda = MDASequence.from_file(str(FILE))
     assert mda == mda1
     if ext == "json":
         assert json.loads(mda.json(exclude={"uid"})) == json.loads(text)
     else:
         assert mda.yaml() == text
 
     it = iter(mda)
     for _ in range(20):
-        assert getattr(next(it), ext)()
+        if ext == "json":
+            assert next(it).json()
+        else:
+            assert next(it).yaml()
```

### Comparing `useq_schema-0.3.2/tests/fixtures/mda.json` & `useq_schema-0.4.0/tests/fixtures/mda.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8726631393298061%*

 * *Differences: {"'grid_plan'": "{'fov_height': None, 'fov_width': None}",*

 * * "'keep_shutter_open_across'": '[]',*

 * * "'stage_positions'": "{1: {'sequence': {'grid_plan': {'fov_height': None, 'fov_width': None}, "*

 * *                      "'keep_shutter_open_across': []}}}"}*

```diff
@@ -34,22 +34,25 @@
             "exposure": null,
             "group": "Channel",
             "z_offset": 0.0
         }
     ],
     "grid_plan": {
         "columns": 1,
+        "fov_height": null,
+        "fov_width": null,
         "mode": "row_wise_snake",
         "overlap": [
             0.0,
             0.0
         ],
         "relative_to": "center",
         "rows": 2
     },
+    "keep_shutter_open_across": [],
     "metadata": {
         "some info": "something"
     },
     "stage_positions": [
         {
             "name": null,
             "sequence": null,
@@ -61,22 +64,25 @@
             "name": "test_name",
             "sequence": {
                 "autofocus_plan": null,
                 "axis_order": "tpgcz",
                 "channels": [],
                 "grid_plan": {
                     "columns": 3,
+                    "fov_height": null,
+                    "fov_width": null,
                     "mode": "row_wise_snake",
                     "overlap": [
                         0.0,
                         0.0
                     ],
                     "relative_to": "center",
                     "rows": 2
                 },
+                "keep_shutter_open_across": [],
                 "metadata": {},
                 "stage_positions": [],
                 "time_plan": null,
                 "z_plan": {
                     "above": 10.0,
                     "below": 0.0,
                     "go_up": true,
```

### Comparing `useq_schema-0.3.2/tests/fixtures/mda.yaml` & `useq_schema-0.4.0/tests/fixtures/mda.yaml`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/.gitignore` & `useq_schema-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/LICENSE` & `useq_schema-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `useq_schema-0.3.2/README.md` & `useq_schema-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,179 +11,161 @@
 *An implementation agnostic schema for describing a sequence of events during a
 multi-dimensional imaging acquisition.*
 
 **Documentation: <https://pymmcore-plus.github.io/useq-schema/>**
 
 The goal of this repo is to provide a specification (and some python utilities)
 for generating event objects that can be consumed by microscope acquisition
-engines.  The *hope* is that this will encourage inter-operability between
+engines.  The *hope* is that this will encourage interoperability between
 various efforts to drive automated image acquisition.
 
 The schema *tries* to remain agnostic to the specific acquisition engine, though
-it was designed based on the Micro-Manager acquisition engine. One hope is to
-solicit feedback from interested parties regarding limitations and/or potential
+it was designed around the needs of Micro-Manager. One hope is to solicit
+feedback from interested parties regarding limitations and/or potential
 extensions to the schema.  Similarly, while the "ideal" schema will support
 arbitrary dimensions (i.e. more than the conventional position, time, channel,
 z, ...), it also hard to avoid hard-coding some assumptions about dimensionality
-in certain places.  Any and all feedback (even minor stuff, such as parameter
-naming, etc...) is welcome!
+in certain places.  
+
+Any and all feedback is welcome!  Please get in touch if you have any thoughts.
 
 ## `MDAEvent`
 
-The primary "event" object is `useq.MDAEvent`.  This captures a single event
+The primary "event" object is `useq.MDAEvent`.  This represents a single event
 that a microscope should perform, including preparation of the hardware, and
-execution of the event (such as an image acquisition).
+execution of the event (such as an image acquisition).  This is the simpler,
+but more important of the two objects.  Downstream libraries that aim to support
+useq schema should support driving hardware based on an `Iterable[MDAEvent]`.
 
 - For [micro-manager](https://github.com/micro-manager/micro-manager), this
   object is most similar (though not *that* similar) to the events generated by
   [`generate-acq-sequence`](https://github.com/micro-manager/micro-manager/blob/2b0f51a2f916112d39c6135ad35a112065f8d58d/acqEngine/src/main/clj/org/micromanager/sequence_generator.clj#L410)
   in the clojure acquisition engine.
 - For [pycro-manager](https://github.com/micro-manager/pycro-manager), this
   object is similar to an individual [acquisition event
   `dict`](https://pycro-manager.readthedocs.io/en/latest/apis.html#acquisition-event-specification)
   generated by
   [`multi_d_acquisition_events`](https://github.com/micro-manager/pycro-manager/blob/63cf209a8907fd23932ee9f8016cb6a2b61b45aa/pycromanager/acquire.py#L605),
   (and, `useq.MDAEvent` provides a `to_pycromanager()` method that returns a
   single pycro-manager event dict)
 - *your object here?...*
 
-```python
-# simplified, and possibly outdated.  See useq.MDAEvent in codebase
-
-# where `None` generally means "make no change"
-class MDAEvent:
-    metadata: Dict[str, Any] = {}  # user-specific data
-    index: Dict[str, int] = {}  # {'axis'->index} for this event
-    channel: Optional[Channel]  # optical config
-    exposure: Optional[PositiveFloat]  # will likely expand for camera
-    min_start_time: Optional[int]  # min time delta for beginning event
-    x_pos: Optional[float]  # stage x
-    y_pos: Optional[float]  # stage y
-    z_pos: Optional[float]  # stage z
-    properties: Optional[Sequence[PropertyTuple]]  # set arbitrary device props
-    # TBD
-    # action: Action ... such as "acquire", etc...
-
-class Channel:
-    config: str
-    group: str = "Channel"
-
-class PropertyTuple(NamedTuple):
-    device_name: str
-    property_name: str
-    property_value: Any
-```
+See [`useq.MDAEvent` documentation](https://pymmcore-plus.github.io/useq-schema/schema/event/)
+for more details.
 
-> `useq-schema` uses [`pydantic`](https://pydantic-docs.helpmanual.io/) to
+> **Note:** `useq-schema` uses [`pydantic`](https://pydantic-docs.helpmanual.io/) to
 > define models, so you can retrieve the [json schema](https://json-schema.org/)
 > for the `MDAEvent` object with `MDAEvent.schema_json()`
 
 ## `MDASequence`
 
-`useq.MDASequence` represents a sequence of events (as might be generated by the
-multidimensional acquisition GUI in most microscope software).  A
+`useq.MDASequence` is a declarative representation of an entire experiment.  It
+represents a sequence of events (as might be generated by the multidimensional
+acquisition GUI in most microscope software).  It is composed of ["plans" for
+each axis in the
+experiment](https://pymmcore-plus.github.io/useq-schema/schema/axes/) (such as a
+Time Plan, a Z Plan, a list of channels and positions, etc.).  A
 `useq.MDASequence` object is itself iterable, and yields `MDAEvent` objects.
 
 - For [micro-manager](https://github.com/micro-manager/micro-manager), this
   object is most similar to
   [`org.micromanager.acquisition.SequenceSettings`](https://github.com/micro-manager/micro-manager/blob/2b0f51a2f916112d39c6135ad35a112065f8d58d/mmstudio/src/main/java/org/micromanager/acquisition/SequenceSettings.java#L39),
   (generated by clicking the "Acquire!" button in the Multi-D Acquisition GUI)
 - For [pycro-manager](https://github.com/micro-manager/pycro-manager), this
   object is similar to the
   [`multi_d_acquisition_events`](https://github.com/micro-manager/pycro-manager/blob/63cf209a8907fd23932ee9f8016cb6a2b61b45aa/pycromanager/acquire.py#L605)
   convenience function, (and `useq.MDASequence` provides a `to_pycromanager()`
   method that returns a list of pycro-manager events)
 - *your object here?...*
 
-```python
-# simplified, and possibly outdated.  See useq.MDASequence in codebase
+See [`useq.MDASequence` documentation](https://pymmcore-plus.github.io/useq-schema/schema/sequence/)
+for more details.
 
-class MDASequence(BaseModel):
-    metadata: Dict[str, Any] = {}  # user-specific data
-    axis_order: str  # e.g. 'tpcz'
-    stage_positions: Tuple[Position]
-    channels: Tuple[Channel, ...]
-    time_plan: AnyTimePlan  # see details below
-    z_plan: AnyZPlan  # see details below
-
-class Position(BaseModel):
-    # if None, implies 'do not move this axis'
-    x: Optional[float]
-    y: Optional[float]
-    z: Optional[float]
-    name: Optional[str]
-    z_plan: Optional[AnyZPlan]
-
-
-class Channel(BaseModel):
-    config: str
-    group: str
-    exposure: Optional[PositiveFloat]
-    do_stack: bool = True
-    z_offset: float = 0.0
-    acquire_every: PositiveInt = 1  # acquire every n frames
-    camera: Optional[str]
-```
+### example `MDASequence` usage:
 
-> `useq-schema` uses [`pydantic`](https://pydantic-docs.helpmanual.io/) to
-> define models, so you can retrieve the [json schema](https://json-schema.org/)
-> for the `MDASequence` object with `MDASequence.schema_json()`
+```python
+from useq import MDASequence
 
+mda_seq = MDASequence(
+    stage_positions=[(100, 100, 30), (200, 150, 35)],
+    channels=["DAPI", "FITC"],
+    time_plan={'interval': 1, 'loops': 20},
+    z_plan={"range": 4, "step": 0.5},
+    axis_order='tpcz',
+)
+events = list(mda_seq)
 
-`TimePlan` and `ZPlan` are each iterable objects that allow for various ways to
-describe time and Z series.  These are each rather configurable and will be documented more later.
+print(len(events))  # 720
 
-`TimePlans`:
+print(events[:3])
 
-- `TIntervalDuration` - specify *interval* and *duration*
-- `TIntervalLoops` - specify *interval* and *number of timepoints*
-- `TDurationLoops` - specify *duration* and *number of timepoints*
+# [MDAEvent(
+#     channel=Channel(config='DAPI'),
+#     index=mappingproxy({'t': 0, 'p': 0, 'c': 0, 'z': 0}),
+#     min_start_time=0.0,
+#     x_pos=100.0,
+#     y_pos=100.0,
+#     z_pos=28.0,
+#  ),
+#  MDAEvent(
+#     channel=Channel(config='DAPI'),
+#     index=mappingproxy({'t': 0, 'p': 0, 'c': 0, 'z': 1}),
+#     min_start_time=0.0,
+#     x_pos=100.0,
+#     y_pos=100.0,
+#     z_pos=28.5,
+#  ),
+#  MDAEvent(
+#     channel=Channel(config='DAPI'),
+#     index=mappingproxy({'t': 0, 'p': 0, 'c': 0, 'z': 2}),
+#     min_start_time=0.0,
+#     x_pos=100.0,
+#     y_pos=100.0,
+#     z_pos=29.0,
+#  )]
+```
 
-`ZPlans`:
+serialize to yaml or json
 
-- `ZTopBottom` - specify absolute *top*, *bottom*, and *step*
-- `ZRangeAround` - specify symmetric *range* and *step*
-- `ZAboveBelow` - specify asymmetric range *above* and *below* reference, with *step*
-- `ZRelativePositions` - directly specify a sequence of relative z positions
-- `ZAbsolutePositions` - directly specify a sequence of absolute z positions
+```py
+print(mda_seq.yaml())
+```
 
-#### example `MDASequence` usage:
+```yaml
+axis_order: tpcz
+channels:
+- config: DAPI
+- config: FITC
+stage_positions:
+- x: 100.0
+  y: 100.0
+  z: 30.0
+- x: 200.0
+  y: 150.0
+  z: 35.0
+time_plan:
+  interval: 0:00:01
+  loops: 20
+z_plan:
+  range: 4.0
+  step: 0.5
+```
+## Executing useq-schema experiments with pymmcore-plus
+
+[pymmcore-plus](https://github.com/pymmcore-plus/pymmcore-plus) implements an
+acquisition engine that can execute an `MDASequence` using
+micro-manager in a pure python environment (no Java required).
 
 ```python
-from useq import MDASequence
+from pymmcore_plus import CMMCorePlus
 
-mda = MDASequence(
-    stage_positions=[(100, 100, 30), (200, 150, 35)],
-    channels=["DAPI", "FITC"],
-    time_plan={'interval': 1, 'loops': 20},
-    z_plan={"range": 4, "step": 0.5},
-    axis_order='tpcz',
-)
+core = CMMCorePlus()
+core.loadSystemConfiguration()  # loads demo by default
 
-len(mda)
-# 720
+core.mda.run(mda_seq)  # run the experiment
 
-list(mda)
-# [
-#     MDAEvent(index={'t': 0, 'p': 0, 'c': 0, 'z': 0}, ... z_pos=28.0),
-#     MDAEvent(index={'t': 0, 'p': 0, 'c': 0, 'z': 1}, ... z_pos=28.5),
-#     ...
-# ]
-
-mda.to_pycromanager()
-
-# [
-#  {'axes': {'position': 0, 'time': 0, 'z': 0},
-#   'z': 28.0,
-#   'x': 100.0,
-#   'y': 100.0,
-#   'min_start_time': 0,
-#   'channel': {'config': 'DAPI', 'group': 'Channel'}},
-#  {'axes': {'position': 0, 'time': 0, 'z': 1},
-#   'z': 28.5,
-#   'x': 100.0,
-#   'y': 100.0,
-#   'min_start_time': 0,
-#   'channel': {'config': 'DAPI', 'group': 'Channel'}},
-#   ...
-# ]
+# or, construct a sequence of MDAEvents anyway you like
+events = [MDAEvent(...), MDAEvent(...), ...]
+core.mda.run(events)
 ```
+
+See [pymmcore-plus documentation](https://pymmcore-plus.github.io/pymmcore-plus/examples/mda/) for details
```

### Comparing `useq_schema-0.3.2/pyproject.toml` & `useq_schema-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Software Development",
     "Topic :: System :: Hardware",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic<2.0", "numpy"]
+dependencies = ["pydantic >=1.7", "numpy"]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 yaml = ["PyYAML"]
 test = ["pytest>=6.0", "pytest-cov", "PyYAML"]
 dev = [
@@ -46,14 +46,15 @@
     "pdbpp",
     "pre-commit",
     "pytest-cov",
     "pytest",
     "rich",
     "ruff",
     "PyYaml",
+    "types-PyYAML",
 ]
 docs = ["mkdocs >=1.4", "mkdocs-material", "mkdocstrings-python"]
 
 [project.urls]
 Source = "https://github.com/pymmcore-plus/useq-schema"
 Tracker = "https://github.com/pymmcore-plus/useq-schema/issues"
```

### Comparing `useq_schema-0.3.2/PKG-INFO` & `useq_schema-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useq-schema
-Version: 0.3.2
+Version: 0.4.0
 Summary: Schema for multi-dimensional microscopy experiments
 Project-URL: Source, https://github.com/pymmcore-plus/useq-schema
 Project-URL: Tracker, https://github.com/pymmcore-plus/useq-schema/issues
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Keywords: microscopy,schema
@@ -23,26 +23,27 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Hardware
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: numpy
-Requires-Dist: pydantic<2.0
+Requires-Dist: pydantic>=1.7
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pyyaml; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: types-pyyaml; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocs>=1.4; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
@@ -64,179 +65,161 @@
 *An implementation agnostic schema for describing a sequence of events during a
 multi-dimensional imaging acquisition.*
 
 **Documentation: <https://pymmcore-plus.github.io/useq-schema/>**
 
 The goal of this repo is to provide a specification (and some python utilities)
 for generating event objects that can be consumed by microscope acquisition
-engines.  The *hope* is that this will encourage inter-operability between
+engines.  The *hope* is that this will encourage interoperability between
 various efforts to drive automated image acquisition.
 
 The schema *tries* to remain agnostic to the specific acquisition engine, though
-it was designed based on the Micro-Manager acquisition engine. One hope is to
-solicit feedback from interested parties regarding limitations and/or potential
+it was designed around the needs of Micro-Manager. One hope is to solicit
+feedback from interested parties regarding limitations and/or potential
 extensions to the schema.  Similarly, while the "ideal" schema will support
 arbitrary dimensions (i.e. more than the conventional position, time, channel,
 z, ...), it also hard to avoid hard-coding some assumptions about dimensionality
-in certain places.  Any and all feedback (even minor stuff, such as parameter
-naming, etc...) is welcome!
+in certain places.  
+
+Any and all feedback is welcome!  Please get in touch if you have any thoughts.
 
 ## `MDAEvent`
 
-The primary "event" object is `useq.MDAEvent`.  This captures a single event
+The primary "event" object is `useq.MDAEvent`.  This represents a single event
 that a microscope should perform, including preparation of the hardware, and
-execution of the event (such as an image acquisition).
+execution of the event (such as an image acquisition).  This is the simpler,
+but more important of the two objects.  Downstream libraries that aim to support
+useq schema should support driving hardware based on an `Iterable[MDAEvent]`.
 
 - For [micro-manager](https://github.com/micro-manager/micro-manager), this
   object is most similar (though not *that* similar) to the events generated by
   [`generate-acq-sequence`](https://github.com/micro-manager/micro-manager/blob/2b0f51a2f916112d39c6135ad35a112065f8d58d/acqEngine/src/main/clj/org/micromanager/sequence_generator.clj#L410)
   in the clojure acquisition engine.
 - For [pycro-manager](https://github.com/micro-manager/pycro-manager), this
   object is similar to an individual [acquisition event
   `dict`](https://pycro-manager.readthedocs.io/en/latest/apis.html#acquisition-event-specification)
   generated by
   [`multi_d_acquisition_events`](https://github.com/micro-manager/pycro-manager/blob/63cf209a8907fd23932ee9f8016cb6a2b61b45aa/pycromanager/acquire.py#L605),
   (and, `useq.MDAEvent` provides a `to_pycromanager()` method that returns a
   single pycro-manager event dict)
 - *your object here?...*
 
-```python
-# simplified, and possibly outdated.  See useq.MDAEvent in codebase
-
-# where `None` generally means "make no change"
-class MDAEvent:
-    metadata: Dict[str, Any] = {}  # user-specific data
-    index: Dict[str, int] = {}  # {'axis'->index} for this event
-    channel: Optional[Channel]  # optical config
-    exposure: Optional[PositiveFloat]  # will likely expand for camera
-    min_start_time: Optional[int]  # min time delta for beginning event
-    x_pos: Optional[float]  # stage x
-    y_pos: Optional[float]  # stage y
-    z_pos: Optional[float]  # stage z
-    properties: Optional[Sequence[PropertyTuple]]  # set arbitrary device props
-    # TBD
-    # action: Action ... such as "acquire", etc...
-
-class Channel:
-    config: str
-    group: str = "Channel"
-
-class PropertyTuple(NamedTuple):
-    device_name: str
-    property_name: str
-    property_value: Any
-```
+See [`useq.MDAEvent` documentation](https://pymmcore-plus.github.io/useq-schema/schema/event/)
+for more details.
 
-> `useq-schema` uses [`pydantic`](https://pydantic-docs.helpmanual.io/) to
+> **Note:** `useq-schema` uses [`pydantic`](https://pydantic-docs.helpmanual.io/) to
 > define models, so you can retrieve the [json schema](https://json-schema.org/)
 > for the `MDAEvent` object with `MDAEvent.schema_json()`
 
 ## `MDASequence`
 
-`useq.MDASequence` represents a sequence of events (as might be generated by the
-multidimensional acquisition GUI in most microscope software).  A
+`useq.MDASequence` is a declarative representation of an entire experiment.  It
+represents a sequence of events (as might be generated by the multidimensional
+acquisition GUI in most microscope software).  It is composed of ["plans" for
+each axis in the
+experiment](https://pymmcore-plus.github.io/useq-schema/schema/axes/) (such as a
+Time Plan, a Z Plan, a list of channels and positions, etc.).  A
 `useq.MDASequence` object is itself iterable, and yields `MDAEvent` objects.
 
 - For [micro-manager](https://github.com/micro-manager/micro-manager), this
   object is most similar to
   [`org.micromanager.acquisition.SequenceSettings`](https://github.com/micro-manager/micro-manager/blob/2b0f51a2f916112d39c6135ad35a112065f8d58d/mmstudio/src/main/java/org/micromanager/acquisition/SequenceSettings.java#L39),
   (generated by clicking the "Acquire!" button in the Multi-D Acquisition GUI)
 - For [pycro-manager](https://github.com/micro-manager/pycro-manager), this
   object is similar to the
   [`multi_d_acquisition_events`](https://github.com/micro-manager/pycro-manager/blob/63cf209a8907fd23932ee9f8016cb6a2b61b45aa/pycromanager/acquire.py#L605)
   convenience function, (and `useq.MDASequence` provides a `to_pycromanager()`
   method that returns a list of pycro-manager events)
 - *your object here?...*
 
-```python
-# simplified, and possibly outdated.  See useq.MDASequence in codebase
+See [`useq.MDASequence` documentation](https://pymmcore-plus.github.io/useq-schema/schema/sequence/)
+for more details.
 
-class MDASequence(BaseModel):
-    metadata: Dict[str, Any] = {}  # user-specific data
-    axis_order: str  # e.g. 'tpcz'
-    stage_positions: Tuple[Position]
-    channels: Tuple[Channel, ...]
-    time_plan: AnyTimePlan  # see details below
-    z_plan: AnyZPlan  # see details below
-
-class Position(BaseModel):
-    # if None, implies 'do not move this axis'
-    x: Optional[float]
-    y: Optional[float]
-    z: Optional[float]
-    name: Optional[str]
-    z_plan: Optional[AnyZPlan]
-
-
-class Channel(BaseModel):
-    config: str
-    group: str
-    exposure: Optional[PositiveFloat]
-    do_stack: bool = True
-    z_offset: float = 0.0
-    acquire_every: PositiveInt = 1  # acquire every n frames
-    camera: Optional[str]
-```
+### example `MDASequence` usage:
 
-> `useq-schema` uses [`pydantic`](https://pydantic-docs.helpmanual.io/) to
-> define models, so you can retrieve the [json schema](https://json-schema.org/)
-> for the `MDASequence` object with `MDASequence.schema_json()`
+```python
+from useq import MDASequence
 
+mda_seq = MDASequence(
+    stage_positions=[(100, 100, 30), (200, 150, 35)],
+    channels=["DAPI", "FITC"],
+    time_plan={'interval': 1, 'loops': 20},
+    z_plan={"range": 4, "step": 0.5},
+    axis_order='tpcz',
+)
+events = list(mda_seq)
 
-`TimePlan` and `ZPlan` are each iterable objects that allow for various ways to
-describe time and Z series.  These are each rather configurable and will be documented more later.
+print(len(events))  # 720
 
-`TimePlans`:
+print(events[:3])
 
-- `TIntervalDuration` - specify *interval* and *duration*
-- `TIntervalLoops` - specify *interval* and *number of timepoints*
-- `TDurationLoops` - specify *duration* and *number of timepoints*
+# [MDAEvent(
+#     channel=Channel(config='DAPI'),
+#     index=mappingproxy({'t': 0, 'p': 0, 'c': 0, 'z': 0}),
+#     min_start_time=0.0,
+#     x_pos=100.0,
+#     y_pos=100.0,
+#     z_pos=28.0,
+#  ),
+#  MDAEvent(
+#     channel=Channel(config='DAPI'),
+#     index=mappingproxy({'t': 0, 'p': 0, 'c': 0, 'z': 1}),
+#     min_start_time=0.0,
+#     x_pos=100.0,
+#     y_pos=100.0,
+#     z_pos=28.5,
+#  ),
+#  MDAEvent(
+#     channel=Channel(config='DAPI'),
+#     index=mappingproxy({'t': 0, 'p': 0, 'c': 0, 'z': 2}),
+#     min_start_time=0.0,
+#     x_pos=100.0,
+#     y_pos=100.0,
+#     z_pos=29.0,
+#  )]
+```
 
-`ZPlans`:
+serialize to yaml or json
 
-- `ZTopBottom` - specify absolute *top*, *bottom*, and *step*
-- `ZRangeAround` - specify symmetric *range* and *step*
-- `ZAboveBelow` - specify asymmetric range *above* and *below* reference, with *step*
-- `ZRelativePositions` - directly specify a sequence of relative z positions
-- `ZAbsolutePositions` - directly specify a sequence of absolute z positions
+```py
+print(mda_seq.yaml())
+```
 
-#### example `MDASequence` usage:
+```yaml
+axis_order: tpcz
+channels:
+- config: DAPI
+- config: FITC
+stage_positions:
+- x: 100.0
+  y: 100.0
+  z: 30.0
+- x: 200.0
+  y: 150.0
+  z: 35.0
+time_plan:
+  interval: 0:00:01
+  loops: 20
+z_plan:
+  range: 4.0
+  step: 0.5
+```
+## Executing useq-schema experiments with pymmcore-plus
+
+[pymmcore-plus](https://github.com/pymmcore-plus/pymmcore-plus) implements an
+acquisition engine that can execute an `MDASequence` using
+micro-manager in a pure python environment (no Java required).
 
 ```python
-from useq import MDASequence
+from pymmcore_plus import CMMCorePlus
 
-mda = MDASequence(
-    stage_positions=[(100, 100, 30), (200, 150, 35)],
-    channels=["DAPI", "FITC"],
-    time_plan={'interval': 1, 'loops': 20},
-    z_plan={"range": 4, "step": 0.5},
-    axis_order='tpcz',
-)
+core = CMMCorePlus()
+core.loadSystemConfiguration()  # loads demo by default
 
-len(mda)
-# 720
+core.mda.run(mda_seq)  # run the experiment
 
-list(mda)
-# [
-#     MDAEvent(index={'t': 0, 'p': 0, 'c': 0, 'z': 0}, ... z_pos=28.0),
-#     MDAEvent(index={'t': 0, 'p': 0, 'c': 0, 'z': 1}, ... z_pos=28.5),
-#     ...
-# ]
-
-mda.to_pycromanager()
-
-# [
-#  {'axes': {'position': 0, 'time': 0, 'z': 0},
-#   'z': 28.0,
-#   'x': 100.0,
-#   'y': 100.0,
-#   'min_start_time': 0,
-#   'channel': {'config': 'DAPI', 'group': 'Channel'}},
-#  {'axes': {'position': 0, 'time': 0, 'z': 1},
-#   'z': 28.5,
-#   'x': 100.0,
-#   'y': 100.0,
-#   'min_start_time': 0,
-#   'channel': {'config': 'DAPI', 'group': 'Channel'}},
-#   ...
-# ]
+# or, construct a sequence of MDAEvents anyway you like
+events = [MDAEvent(...), MDAEvent(...), ...]
+core.mda.run(events)
 ```
+
+See [pymmcore-plus documentation](https://pymmcore-plus.github.io/pymmcore-plus/examples/mda/) for details
```

