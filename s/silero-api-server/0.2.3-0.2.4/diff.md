# Comparing `tmp/silero_api_server-0.2.3.tar.gz` & `tmp/silero_api_server-0.2.4.tar.gz`

## Comparing `silero_api_server-0.2.3.tar` & `silero_api_server-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/silero_api_server/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/silero_api_server/__main__.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/silero_api_server/server.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/silero_api_server/tts.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/LICENSE
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/README.md
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 silero_api_server-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/silero_api_server/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/silero_api_server/__main__.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/silero_api_server/server.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/silero_api_server/tts.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/README.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 silero_api_server-0.2.4/PKG-INFO
```

### Comparing `silero_api_server-0.2.3/.github/workflows/publish-to-test-pypi.yml` & `silero_api_server-0.2.4/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.2.3/silero_api_server/__main__.py` & `silero_api_server-0.2.4/silero_api_server/__main__.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.2.3/silero_api_server/server.py` & `silero_api_server-0.2.4/silero_api_server/server.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.2.3/silero_api_server/tts.py` & `silero_api_server-0.2.4/silero_api_server/tts.py`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.2.3/LICENSE` & `silero_api_server-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_api_server-0.2.3/README.md` & `silero_api_server-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 This is primarily to serve the TTS extension in [SillyTavern](https://github.com/Cohee1207/SillyTavern). The TTS module or server can be used any way you wish.
 
 ## Installation
 `pip install silero-api-server`
 
 ## Starting Server
-`py -m silero_api_server` will run on default ip and port (0.0.0.0:8001)
+`python -m silero_api_server` will run on default ip and port (0.0.0.0:8001)
 
 ```
 usage: silero_api_server [-h] [-o HOST] [-p PORT]
 
 Run Silero within a FastAPI application
 
 options:
```

### Comparing `silero_api_server-0.2.3/pyproject.toml` & `silero_api_server-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "fastapi==0.95.1",
+  "fastapi",
   "loguru==0.7.0",
   "pydantic==1.10.7",
   "python-dotenv==1.0.0",
   "torch==2.0.0",
   "torchaudio==2.0.1",
   "uvicorn",
   "soundfile",
@@ -33,8 +33,8 @@
 "Homepage" = "https://github.com/ouoertheo/silero-api-server"
 "Bug Tracker" = "https://github.com/ouoertheo/silero-api-server/issues"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.targets.wheel]
-only-include = ["silero_api_server"]
+only-include = ["silero_api_server"]
```

### Comparing `silero_api_server-0.2.3/PKG-INFO` & `silero_api_server-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: silero-api-server
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple FastAPI server to host Silero TTS
 Project-URL: Homepage, https://github.com/ouoertheo/silero-api-server
 Project-URL: Bug Tracker, https://github.com/ouoertheo/silero-api-server/issues
 Author-email: Ouoertheo <ouoertheo@tomeofjamin.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: fastapi==0.95.1
+Requires-Dist: fastapi
 Requires-Dist: loguru==0.7.0
 Requires-Dist: numpy
 Requires-Dist: pydantic==1.10.7
 Requires-Dist: pydub==0.25.1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: soundfile
 Requires-Dist: torch==2.0.0
@@ -29,15 +29,15 @@
 
 This is primarily to serve the TTS extension in [SillyTavern](https://github.com/Cohee1207/SillyTavern). The TTS module or server can be used any way you wish.
 
 ## Installation
 `pip install silero-api-server`
 
 ## Starting Server
-`py -m silero_api_server` will run on default ip and port (0.0.0.0:8001)
+`python -m silero_api_server` will run on default ip and port (0.0.0.0:8001)
 
 ```
 usage: silero_api_server [-h] [-o HOST] [-p PORT]
 
 Run Silero within a FastAPI application
 
 options:
```

