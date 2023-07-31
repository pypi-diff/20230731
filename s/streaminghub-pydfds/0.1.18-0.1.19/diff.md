# Comparing `tmp/streaminghub-pydfds-0.1.18.tar.gz` & `tmp/streaminghub-pydfds-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaminghub-pydfds-0.1.18.tar", last modified: Fri Jul 28 21:25:56 2023, max compression
+gzip compressed data, was "streaminghub-pydfds-0.1.19.tar", last modified: Mon Jul 31 20:58:25 2023, max compression
```

## Comparing `streaminghub-pydfds-0.1.18.tar` & `streaminghub-pydfds-0.1.19.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pjaya001 (506721) users    (14514)        0 2023-07-28 21:25:56.055939 streaminghub-pydfds-0.1.18/
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)     1918 2023-07-28 21:25:56.053489 streaminghub-pydfds-0.1.18/PKG-INFO
--rw-r--r--   0 pjaya001 (506721) users    (14514)     1392 2023-07-28 21:23:37.000000 streaminghub-pydfds-0.1.18/README.md
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)     1203 2023-07-28 21:25:33.000000 streaminghub-pydfds-0.1.18/pyproject.toml
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)       38 2023-07-28 21:25:56.057687 streaminghub-pydfds-0.1.18/setup.cfg
-drwxr-xr-x   0 pjaya001 (506721) users    (14514)        0 2023-07-28 21:25:55.986671 streaminghub-pydfds-0.1.18/src/
-drwxr-xr-x   0 pjaya001 (506721) users    (14514)        0 2023-07-28 21:25:56.017000 streaminghub-pydfds-0.1.18/src/dfds/
--rw-r--r--   0 pjaya001 (506721) users    (14514)       58 2023-04-14 06:01:39.000000 streaminghub-pydfds-0.1.18/src/dfds/__init__.py
--rw-r--r--   0 pjaya001 (506721) users    (14514)     2692 2023-06-28 04:30:00.000000 streaminghub-pydfds-0.1.18/src/dfds/lsl.py
--rw-r--r--   0 pjaya001 (506721) users    (14514)     5752 2023-07-06 18:02:23.000000 streaminghub-pydfds-0.1.18/src/dfds/parser.py
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)     4670 2023-07-28 20:08:52.000000 streaminghub-pydfds-0.1.18/src/dfds/typing.py
-drwxr-xr-x   0 pjaya001 (506721) users    (14514)        0 2023-07-28 21:25:56.042013 streaminghub-pydfds-0.1.18/src/streaminghub_pydfds.egg-info/
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)     1918 2023-07-28 21:25:55.000000 streaminghub-pydfds-0.1.18/src/streaminghub_pydfds.egg-info/PKG-INFO
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)      354 2023-07-28 21:25:55.000000 streaminghub-pydfds-0.1.18/src/streaminghub_pydfds.egg-info/SOURCES.txt
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)        1 2023-07-28 21:25:55.000000 streaminghub-pydfds-0.1.18/src/streaminghub_pydfds.egg-info/dependency_links.txt
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)      145 2023-07-28 21:25:55.000000 streaminghub-pydfds-0.1.18/src/streaminghub_pydfds.egg-info/requires.txt
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)        5 2023-07-28 21:25:55.000000 streaminghub-pydfds-0.1.18/src/streaminghub_pydfds.egg-info/top_level.txt
-drwxr-xr-x   0 pjaya001 (506721) users    (14514)        0 2023-07-28 21:25:56.047264 streaminghub-pydfds-0.1.18/tests/
--rwxr-xr-x   0 pjaya001 (506721) users    (14514)      596 2023-06-29 19:50:14.000000 streaminghub-pydfds-0.1.18/tests/test_parser.py
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.658470 streaminghub-pydfds-0.1.19/
+-rw-r--r--   0 yasith     (501) staff       (20)     2110 2023-07-31 20:58:25.658335 streaminghub-pydfds-0.1.19/PKG-INFO
+-rw-r--r--   0 yasith     (501) staff       (20)     1583 2023-07-31 20:58:11.000000 streaminghub-pydfds-0.1.19/README.md
+-rwxr-xr-x   0 yasith     (501) staff       (20)     1258 2023-07-31 20:58:11.000000 streaminghub-pydfds-0.1.19/pyproject.toml
+-rw-r--r--   0 yasith     (501) staff       (20)       38 2023-07-31 20:58:25.658509 streaminghub-pydfds-0.1.19/setup.cfg
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.656634 streaminghub-pydfds-0.1.19/src/
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.657391 streaminghub-pydfds-0.1.19/src/dfds/
+-rw-r--r--   0 yasith     (501) staff       (20)       58 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/__init__.py
+-rw-r--r--   0 yasith     (501) staff       (20)     2692 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/lsl.py
+-rw-r--r--   0 yasith     (501) staff       (20)     5752 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/parser.py
+-rwxr-xr-x   0 yasith     (501) staff       (20)     4670 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/src/dfds/typing.py
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.658003 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/
+-rw-r--r--   0 yasith     (501) staff       (20)     2110 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/PKG-INFO
+-rw-r--r--   0 yasith     (501) staff       (20)      354 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/SOURCES.txt
+-rw-r--r--   0 yasith     (501) staff       (20)        1 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/dependency_links.txt
+-rw-r--r--   0 yasith     (501) staff       (20)      145 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/requires.txt
+-rw-r--r--   0 yasith     (501) staff       (20)        5 2023-07-31 20:58:25.000000 streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/top_level.txt
+drwxr-xr-x   0 yasith     (501) staff       (20)        0 2023-07-31 20:58:25.658145 streaminghub-pydfds-0.1.19/tests/
+-rwxr-xr-x   0 yasith     (501) staff       (20)      596 2023-07-31 20:19:49.000000 streaminghub-pydfds-0.1.19/tests/test_parser.py
```

### Comparing `streaminghub-pydfds-0.1.18/PKG-INFO` & `streaminghub-pydfds-0.1.19/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaminghub-pydfds
-Version: 0.1.18
+Version: 0.1.19
 Summary: Parser for Data Flow Description Schema (DFDS) metadata
 Author-email: Yasith Jayawardana <yasith@cs.odu.edu>
 Project-URL: homepage, https://github.com/nirdslab/streaminghub/tree/master/pydfds
 Keywords: dfds,metadata,parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,33 +18,46 @@
 
 PyDFDS is a parser for Data Flow Description Schema (DFDS) metadata, written using Python.
 
 ## Installation
 
 ```bash
 
-python -m pip install -U -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ streaminghub-pydfds
+pip install streaminghub-pydfds==0.1.19
 
 ```
 
 ## Usage
 
 ```python
 
-import dfds
+from dfds import Parser
+from dfds.typing import Collection, Stream
+from util import restream_data
+
+# define a DFDS parser
+parser = Parser()
+
+# open a DFDS collection
+fp = "/path/to/collection.json"
+collection = parser.get_collection_metadata(fp)
+dataloader = collection.dataloader()
+
+# list all items in the collection
+for attrs in dataloader.ls():
+  for stream_id, stream in collection.streams.items():
+      pass
 
-datasource_spec = dfds.get_datasource_spec("name_of_datasource")
-dataset_spec = dfds.get_dataset_spec("name_of_dataset")
-analytic_spec = dfds.get_analytic_spec("name_of_analytic")
-
-dfds.create_outlet_for_stream(
-  "some_unique_id",
-  "device_info_from_datasource_metadata",
-  "stream_info_from_datasource_metadata"
-)
+# read an entire recording at once
+attrs, data = dataloader.read(stream.attrs)
+
+# or replay the recording as a stream
+asyncio.create_task(replay_data(collection, stream))
+
+return streams
 
 ```
 
 ## Developer Guide
 
 ```bash
```

### Comparing `streaminghub-pydfds-0.1.18/README.md` & `streaminghub-pydfds-0.1.19/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,33 +4,46 @@
 
 PyDFDS is a parser for Data Flow Description Schema (DFDS) metadata, written using Python.
 
 ## Installation
 
 ```bash
 
-python -m pip install -U -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ streaminghub-pydfds
+pip install streaminghub-pydfds==0.1.19
 
 ```
 
 ## Usage
 
 ```python
 
-import dfds
+from dfds import Parser
+from dfds.typing import Collection, Stream
+from util import restream_data
+
+# define a DFDS parser
+parser = Parser()
+
+# open a DFDS collection
+fp = "/path/to/collection.json"
+collection = parser.get_collection_metadata(fp)
+dataloader = collection.dataloader()
+
+# list all items in the collection
+for attrs in dataloader.ls():
+  for stream_id, stream in collection.streams.items():
+      pass
 
-datasource_spec = dfds.get_datasource_spec("name_of_datasource")
-dataset_spec = dfds.get_dataset_spec("name_of_dataset")
-analytic_spec = dfds.get_analytic_spec("name_of_analytic")
-
-dfds.create_outlet_for_stream(
-  "some_unique_id",
-  "device_info_from_datasource_metadata",
-  "stream_info_from_datasource_metadata"
-)
+# read an entire recording at once
+attrs, data = dataloader.read(stream.attrs)
+
+# or replay the recording as a stream
+asyncio.create_task(replay_data(collection, stream))
+
+return streams
 
 ```
 
 ## Developer Guide
 
 ```bash
 
@@ -52,8 +65,8 @@
 # check package
 python -m twine check dist/*
 # publish package (testpypi)
 python -m twine upload -r testpypi dist/*
 # publish package (pypi)
 python -m twine upload dist/*
 
-```
+```
```

### Comparing `streaminghub-pydfds-0.1.18/pyproject.toml` & `streaminghub-pydfds-0.1.19/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streaminghub-pydfds"
-version = "0.1.18"
+version = "0.1.19"
 authors = [{ name = "Yasith Jayawardana", email = "yasith@cs.odu.edu" }]
 description = "Parser for Data Flow Description Schema (DFDS) metadata"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["dfds", "metadata", "parser"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy>=1.25.1",
+    "numpy>=1.25.2",
     "pylsl>=1.16.1",
     "jsonschema>=4.18.4",
     "pydantic>=2.1.1",
     "h5py>=3.9.0",
-    "parse>=1.19.1"
+    "parse>=1.19.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/nirdslab/streaminghub/tree/master/pydfds"
 
 [project.optional-dependencies]
 dev = ["black", "build", "twine", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.1.18"
+current_version = "0.1.19"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump pydfds version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
-"pyproject.toml" = [
-    'version = "{version}"',
-]
+"pyproject.toml" = ['version = "{version}"']
+"README.md" = ['pip install streaminghub-pydfds=={version}']
```

### Comparing `streaminghub-pydfds-0.1.18/src/dfds/lsl.py` & `streaminghub-pydfds-0.1.19/src/dfds/lsl.py`

 * *Files identical despite different names*

### Comparing `streaminghub-pydfds-0.1.18/src/dfds/parser.py` & `streaminghub-pydfds-0.1.19/src/dfds/parser.py`

 * *Files identical despite different names*

### Comparing `streaminghub-pydfds-0.1.18/src/dfds/typing.py` & `streaminghub-pydfds-0.1.19/src/dfds/typing.py`

 * *Files identical despite different names*

### Comparing `streaminghub-pydfds-0.1.18/src/streaminghub_pydfds.egg-info/PKG-INFO` & `streaminghub-pydfds-0.1.19/src/streaminghub_pydfds.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaminghub-pydfds
-Version: 0.1.18
+Version: 0.1.19
 Summary: Parser for Data Flow Description Schema (DFDS) metadata
 Author-email: Yasith Jayawardana <yasith@cs.odu.edu>
 Project-URL: homepage, https://github.com/nirdslab/streaminghub/tree/master/pydfds
 Keywords: dfds,metadata,parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,33 +18,46 @@
 
 PyDFDS is a parser for Data Flow Description Schema (DFDS) metadata, written using Python.
 
 ## Installation
 
 ```bash
 
-python -m pip install -U -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ streaminghub-pydfds
+pip install streaminghub-pydfds==0.1.19
 
 ```
 
 ## Usage
 
 ```python
 
-import dfds
+from dfds import Parser
+from dfds.typing import Collection, Stream
+from util import restream_data
+
+# define a DFDS parser
+parser = Parser()
+
+# open a DFDS collection
+fp = "/path/to/collection.json"
+collection = parser.get_collection_metadata(fp)
+dataloader = collection.dataloader()
+
+# list all items in the collection
+for attrs in dataloader.ls():
+  for stream_id, stream in collection.streams.items():
+      pass
 
-datasource_spec = dfds.get_datasource_spec("name_of_datasource")
-dataset_spec = dfds.get_dataset_spec("name_of_dataset")
-analytic_spec = dfds.get_analytic_spec("name_of_analytic")
-
-dfds.create_outlet_for_stream(
-  "some_unique_id",
-  "device_info_from_datasource_metadata",
-  "stream_info_from_datasource_metadata"
-)
+# read an entire recording at once
+attrs, data = dataloader.read(stream.attrs)
+
+# or replay the recording as a stream
+asyncio.create_task(replay_data(collection, stream))
+
+return streams
 
 ```
 
 ## Developer Guide
 
 ```bash
```

### Comparing `streaminghub-pydfds-0.1.18/tests/test_parser.py` & `streaminghub-pydfds-0.1.19/tests/test_parser.py`

 * *Files identical despite different names*

