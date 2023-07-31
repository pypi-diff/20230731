# Comparing `tmp/pycis_cli-0.0.8.tar.gz` & `tmp/pycis_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycis_cli-0.0.8.tar", max compression
+gzip compressed data, was "pycis_cli-0.0.9.tar", max compression
```

## Comparing `pycis_cli-0.0.8.tar` & `pycis_cli-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1083 2023-07-12 18:00:09.011444 pycis_cli-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      394 2023-07-15 21:22:15.146910 pycis_cli-0.0.8/README.rst
--rw-r--r--   0        0        0      994 2023-07-19 22:37:40.450596 pycis_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 03:17:30.118993 pycis_cli-0.0.8/source/packages/pycis/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 04:12:29.753800 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      768 2023-07-15 21:02:15.428500 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/__init__.py
--rw-r--r--   0        0        0       43 2023-07-15 21:15:03.524375 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/constants.py
--rw-r--r--   0        0        0      802 2023-07-15 21:02:15.432500 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
--rw-r--r--   0        0        0     2948 2023-07-19 22:27:05.917177 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
--rw-r--r--   0        0        0     2616 2023-07-15 21:15:03.528375 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
--rw-r--r--   0        0        0      602 2023-07-15 21:02:15.432500 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
--rw-r--r--   0        0        0     2883 2023-07-15 21:15:03.528375 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
--rw-r--r--   0        0        0      713 2023-07-15 21:02:15.432500 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/__init__.py
--rw-r--r--   0        0        0     1367 2023-07-15 21:14:22.747367 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/__init__.py
--rw-r--r--   0        0        0     2611 2023-07-15 21:16:57.763186 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
--rw-r--r--   0        0        0     2189 2023-07-15 21:16:57.759186 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/addchange.py
--rw-r--r--   0        0        0     2748 2023-07-19 22:35:48.004906 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/initialize.py
--rw-r--r--   0        0        0     2487 2023-07-15 21:16:57.759186 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
--rw-r--r--   0        0        0     2703 2023-07-15 21:16:57.755186 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/update.py
--rw-r--r--   0        0        0      612 2023-07-15 21:02:15.432500 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
--rw-r--r--   0        0        0     1444 2023-07-19 22:35:25.850346 pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/testrun/create.py
--rw-r--r--   0        0        0     1273 2023-07-15 21:02:15.428500 pycis_cli-0.0.8/source/packages/pycis/cli/pycis_command.py
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 pycis_cli-0.0.8/setup.py
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 pycis_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-12 18:00:09.011444 pycis_cli-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      394 2023-07-15 21:22:15.146910 pycis_cli-0.0.9/README.rst
+-rw-r--r--   0        0        0      994 2023-07-27 15:17:35.911771 pycis_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 03:17:30.118993 pycis_cli-0.0.9/source/packages/pycis/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 04:12:29.753800 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      768 2023-07-15 21:02:15.428500 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-15 21:15:03.524375 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/constants.py
+-rw-r--r--   0        0        0      802 2023-07-15 21:02:15.432500 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
+-rw-r--r--   0        0        0     2948 2023-07-19 22:27:05.917177 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
+-rw-r--r--   0        0        0     2616 2023-07-15 21:15:03.528375 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
+-rw-r--r--   0        0        0      602 2023-07-15 21:02:15.432500 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
+-rw-r--r--   0        0        0     2883 2023-07-15 21:15:03.528375 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
+-rw-r--r--   0        0        0      713 2023-07-15 21:02:15.432500 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/__init__.py
+-rw-r--r--   0        0        0     1367 2023-07-15 21:14:22.747367 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/__init__.py
+-rw-r--r--   0        0        0     2611 2023-07-15 21:16:57.763186 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
+-rw-r--r--   0        0        0     2189 2023-07-15 21:16:57.759186 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/addchange.py
+-rw-r--r--   0        0        0     2748 2023-07-19 22:35:48.004906 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/initialize.py
+-rw-r--r--   0        0        0     2487 2023-07-15 21:16:57.759186 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
+-rw-r--r--   0        0        0     2703 2023-07-15 21:16:57.755186 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/update.py
+-rw-r--r--   0        0        0      612 2023-07-15 21:02:15.432500 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-27 15:14:11.333462 pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/testrun/create.py
+-rw-r--r--   0        0        0     1273 2023-07-15 21:02:15.428500 pycis_cli-0.0.9/source/packages/pycis/cli/pycis_command.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 pycis_cli-0.0.9/setup.py
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 pycis_cli-0.0.9/PKG-INFO
```

### Comparing `pycis_cli-0.0.8/LICENSE.txt` & `pycis_cli-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/pyproject.toml` & `pycis_cli-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pycis-cli"
 description = "Python Continuous Integration System (PyCIS) - CLI Tools"
-version = "0.0.8"
+version = "0.0.9"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/__init__.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/__init__.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/__init__.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/addchange.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/addchange.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/initialize.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/build/update.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/build/update.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/cmdtree/document/testrun/create.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/cmdtree/document/testrun/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 import json
 import os
 
 import click
 
 from mojo.xmods.jsos import load_jsos_stream_from_file
 
+from mojo.xmods.xclick import NORMALIZED_STRING
+
 HELP_RESULTS = "A folder containing test results to publish"
 HELP_EXPIRY = "A number of days to persist the up uploaded results."
+HELP_ARCHIVE = "An optional 'archive' value to set in the build document."
 
 @click.command("create")
 @click.option("--results", required=True, type=click.Path(exists=True, file_okay=False), help=HELP_RESULTS)
+@click.option("--archive", required=False, type=NORMALIZED_STRING, default=None, help=HELP_ARCHIVE)
 @click.argument('filename', metavar='<testrun document>', type=click.Path(dir_okay=False))
-def command_pycis_document_testrun_create(results: str, filename: str):
+def command_pycis_document_testrun_create(results: str, archive: str, filename: str):
 
     # Make sure the summary document and the tests document exists
     summary_file = os.path.join(results, "testrun_summary.json")
     testresults_file = os.path.join(results, "testrun_results.jsos")
 
     summary = None
     with open(summary_file, 'r') as sf:
@@ -35,17 +39,17 @@
     del summary["runid"]
 
     trstream = load_jsos_stream_from_file(testresults_file)
 
     document = {
         "dversion": "1.0",
         "dtype": "testrun",
-        "resultitems": trstream
+        "resultitems": trstream,
+        "archive": archive
     }
 
     document.update(summary)
 
-
     with open(filename, 'w') as of:
         json.dump(document, of, indent=4)
 
     return
```

### Comparing `pycis_cli-0.0.8/source/packages/pycis/cli/pycis_command.py` & `pycis_cli-0.0.9/source/packages/pycis/cli/pycis_command.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.0.8/setup.py` & `pycis_cli-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 {'couchdb': ['couchdb>=1.2,<2.0'], 'mongodb': ['pymongo[srv]>=4.0.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['pycis = pycis.cli.pycis_command:pycis_root_command']}
 
 setup_kwargs = {
     'name': 'pycis-cli',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Python Continuous Integration System (PyCIS) - CLI Tools',
     'long_description': '========================================================\nPython Continuous Integration System (PyCIS) - CLI Tools\n========================================================\n\nProvides a set of CLI tools for working with the PyCIS continuous integration system.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pycis_cli-0.0.8/PKG-INFO` & `pycis_cli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycis-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Continuous Integration System (PyCIS) - CLI Tools
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

