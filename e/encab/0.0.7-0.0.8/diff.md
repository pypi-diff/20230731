# Comparing `tmp/encab-0.0.7.tar.gz` & `tmp/encab-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encab-0.0.7.tar", last modified: Mon Jul 17 16:06:24 2023, max compression
+gzip compressed data, was "encab-0.0.8.tar", last modified: Mon Jul 31 13:02:33 2023, max compression
```

## Comparing `encab-0.0.7.tar` & `encab-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.729121 encab-0.0.7/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.7/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-17 16:06:24.729121 encab-0.0.7/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4406 2023-07-17 15:56:26.000000 encab-0.0.7/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-07-17 15:56:18.000000 encab-0.0.7/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-17 16:06:24.729121 encab-0.0.7/setup.cfg
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.717121 encab-0.0.7/src/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.725121 encab-0.0.7/src/encab/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.7/src/encab/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.7/src/encab/__main__.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.729121 encab-0.0.7/src/encab/common/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1909 2023-07-16 12:17:22.000000 encab-0.0.7/src/encab/common/log_stream.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4069 2023-07-16 12:33:40.000000 encab-0.0.7/src/encab/common/process.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11826 2023-07-16 12:12:13.000000 encab-0.0.7/src/encab/config.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8260 2023-07-17 15:56:44.000000 encab-0.0.7/src/encab/encab.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.729121 encab-0.0.7/src/encab/ext/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.7/src/encab/ext/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.7/src/encab/ext/log_sanitizer.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9609 2023-07-17 15:35:23.000000 encab-0.0.7/src/encab/ext/startup_script.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.7/src/encab/ext/validation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.7/src/encab/extensions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5512 2023-07-17 15:17:13.000000 encab-0.0.7/src/encab/program.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10183 2023-07-17 15:18:53.000000 encab-0.0.7/src/encab/program_state.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3203 2023-07-16 12:24:46.000000 encab-0.0.7/src/encab/programs.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-17 16:06:24.725121 encab-0.0.7/src/encab.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4965 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      585 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-17 16:06:24.000000 encab-0.0.7/src/encab.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.557084 encab-0.0.8/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.8/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5048 2023-07-31 13:02:33.557084 encab-0.0.8/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4489 2023-07-31 13:00:37.000000 encab-0.0.8/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      961 2023-07-31 11:48:15.000000 encab-0.0.8/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-31 13:02:33.557084 encab-0.0.8/setup.cfg
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.545084 encab-0.0.8/src/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.549084 encab-0.0.8/src/encab/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.8/src/encab/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.8/src/encab/__main__.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.553084 encab-0.0.8/src/encab/common/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1935 2023-07-31 12:19:35.000000 encab-0.0.8/src/encab/common/log_stream.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4168 2023-07-31 12:20:55.000000 encab-0.0.8/src/encab/common/process.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11911 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/config.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8252 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/encab.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.557084 encab-0.0.8/src/encab/ext/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.8/src/encab/ext/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5995 2023-07-31 12:27:13.000000 encab-0.0.8/src/encab/ext/log_sanitizer.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     9694 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/ext/startup_script.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.8/src/encab/ext/validation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.8/src/encab/extensions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5574 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/program.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10172 2023-07-31 12:31:36.000000 encab-0.0.8/src/encab/program_state.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3203 2023-07-16 12:24:46.000000 encab-0.0.8/src/encab/programs.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-31 13:02:33.553084 encab-0.0.8/src/encab.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5048 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      585 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-31 13:02:33.000000 encab-0.0.8/src/encab.egg-info/top_level.txt
```

### Comparing `encab-0.0.7/LICENSE` & `encab-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `encab-0.0.7/PKG-INFO` & `encab-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.7
+Version: 0.0.8
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.7
+   INFO  encab: encab 0.0.8
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -75,16 +75,16 @@
 
 ## Installation
 
 ### Install locally
 
 #### Prerequisites
 
-- [Python](https://www.python.org/) Version >= 3.9
-- activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
+- [Python](https://www.python.org/) Version >= 3.7
+- activated Python virtual environment such as [miniconda](https://docs.conda.io/en/latest/miniconda.html) or [virtualenv](https://virtualenv.pypa.io/en/latest/)
 
 ```sh
    pip install -U encab
 ```
 
 #### Run locally
 
@@ -104,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.7
+INFO  encab: encab 0.0.8
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -121,20 +121,22 @@
 - [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
 
 #### Run in Container
 
 1. Create sample encab file `encab.yml`
 
 ```yml
+
    encab:
       dry_run: false
    programs:
       main:
          sh:
             - echo "Hello Encab!"
+
 ```
 
 2. Add Encab to your [Docker file][4].
 
    ```dockerfile
 
    FROM python:3.10.8-slim-bullseye
@@ -160,30 +162,30 @@
    # set encab as entrypoint
    ENTRYPOINT ["encab"]
 
    ```
 
    [4]: https://docs.docker.com/engine/reference/builder/
 
-2. Build container
+3. Build container
 
    ```sh
    docker build -t encab_minimum .
    ```
 
-3. Run container
+4. Run container
 
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.7
+   INFO  encab: encab 0.0.8
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.7/README.md` & `encab-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.7
+   INFO  encab: encab 0.0.8
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -60,16 +60,16 @@
 
 ## Installation
 
 ### Install locally
 
 #### Prerequisites
 
-- [Python](https://www.python.org/) Version >= 3.9
-- activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
+- [Python](https://www.python.org/) Version >= 3.7
+- activated Python virtual environment such as [miniconda](https://docs.conda.io/en/latest/miniconda.html) or [virtualenv](https://virtualenv.pypa.io/en/latest/)
 
 ```sh
    pip install -U encab
 ```
 
 #### Run locally
 
@@ -89,15 +89,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.7
+INFO  encab: encab 0.0.8
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -106,20 +106,22 @@
 - [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
 
 #### Run in Container
 
 1. Create sample encab file `encab.yml`
 
 ```yml
+
    encab:
       dry_run: false
    programs:
       main:
          sh:
             - echo "Hello Encab!"
+
 ```
 
 2. Add Encab to your [Docker file][4].
 
    ```dockerfile
 
    FROM python:3.10.8-slim-bullseye
@@ -145,30 +147,30 @@
    # set encab as entrypoint
    ENTRYPOINT ["encab"]
 
    ```
 
    [4]: https://docs.docker.com/engine/reference/builder/
 
-2. Build container
+3. Build container
 
    ```sh
    docker build -t encab_minimum .
    ```
 
-3. Run container
+4. Run container
 
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.7
+   INFO  encab: encab 0.0.8
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.7/pyproject.toml` & `encab-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encab"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Sebastian Kuebeck", email="sebastian.kuebeck@encab.io" },
 ]
 description = "Process manager"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `encab-0.0.7/src/encab/common/log_stream.py` & `encab-0.0.8/src/encab/common/log_stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         """starts reading and logging"""
         program = self.extra.get("program", "")
         name = f"{program}:{self.log_level}"
         thread = Thread(target=lambda: self._run(), name=name)
         thread.daemon = True
         self.thread = thread
         thread.start()
+        thread.join(0.01)
         return self
 
     def close(self):
         try:
             self.stream.flush()
         except IOError:
             pass
```

### Comparing `encab-0.0.7/src/encab/common/process.py` & `encab-0.0.8/src/encab/common/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,25 @@
     def __init__(self, 
                  args:Union[str, List[str]], 
                  environment: Dict[str, str], 
                  user: Optional[int] = None, 
                  group: Optional[int] = None, 
                  umask: Optional[int] = None, 
                  shell: bool=False,
-                 start_new_session: bool=True) -> None:
+                 start_new_session: bool=True,
+                 cwd: Optional[str] = None) -> None:
         self._args = args
         self._env = environment
         self._user = user
         self._group = group
         self._umask = umask
         self._shell = shell
         self._start_new_session = start_new_session
-        self._process: Optional[Popen] = None 
+        self._process: Optional[Popen] = None
+        self._cwd = cwd
         
     def execute(self, 
                 exec: Callable[[Popen], Any], 
                 stdin: Optional[int] = None, 
                 stdout: Optional[int] = None, 
                 stderr: Optional[int] = None) -> int:
         uid = self._user
@@ -89,15 +91,16 @@
                 self._args,
                 stdin=stdin,
                 stdout=stdout,
                 stderr=stderr,
                 env=self._env,
                 preexec_fn=preexec_fn,
                 shell=self._shell,
-                start_new_session=self._start_new_session
+                start_new_session=self._start_new_session,
+                cwd=self._cwd
             )
         exec(self._process)
         self._process.wait()
         return self._process.returncode
 
     def execute_and_log(self, 
                 exec: Callable[[Popen], Any], 
@@ -111,14 +114,15 @@
             assert process.stdout
             assert process.stderr
             
             streams.append(LogStream(logger, ERROR, process.stderr, extra).start())
             
             if log_stdout:
                 streams.append(LogStream(logger, INFO, process.stdout, extra).start())
+
             exec(process)
 
         try:
             return self.execute(outer_exec, None, PIPE, PIPE)
         finally:
             for stream in streams:
                 stream.close()
```

### Comparing `encab-0.0.7/src/encab/config.py` & `encab-0.0.8/src/encab/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from dataclasses import dataclass, fields
 from marshmallow.exceptions import MarshmallowError, ValidationError
 from logging import DEBUG, INFO
 from abc import ABC
 
 from .common.process import getUserId, getGroupId
 
+
 class ConfigError(ValueError):
     """
     Configuration error
     """
 
     pass
 
@@ -321,14 +322,17 @@
                     sh:     
                         - echo "Test1" 
                         - echo "Test2"
     """
     startup_delay: Optional[float]
     """The startup delay for this program in seconds. Default: 0 seconds"""
 
+    directory: Optional[str]
+    """the directory where the program is executed"""
+
     def __post_init__(self):
         """
         validates fields and sets default values
 
         :raises ConfigError: if fields have invalid values
         """
         super().__post_init__()
```

### Comparing `encab-0.0.7/src/encab/encab.py` & `encab-0.0.8/src/encab/encab.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 import os
 import io
 
 from logging import (
-    Logger,
     getLogger,
     StreamHandler,
     Formatter,
 )
 
 from signal import SIGTERM, SIGINT, signal, getsignal
 from typing import Optional, List, Tuple, Dict
@@ -95,15 +94,15 @@
     assert config.encab
     if dry_run is not None:
         config.encab.dry_run = dry_run
 
     return (config, f"file {encab_file}, source: {source}.")
 
 
-def set_up_logger(config: Config) -> Logger:
+def set_up_logger(config: Config):
     """
     Sets up the encab logger
 
     :param config: the encab configuraion
     :type config: Config
     :return: the logger
     :rtype: Logger
@@ -124,15 +123,15 @@
         root_logger.addHandler(handler)
 
     logger = getLogger(ENCAB)
     extensions.update_logger(ENCAB, logger)
     return logger
 
 
-def set_up_extensions(config: Config, logger: Logger, extra: Dict[str, str]):
+def set_up_extensions(config: Config, logger, extra: Dict[str, str]):
     """
     sets up and configures the extensions.
     In case of dry run, `encab.extensions.Extensions.validate_extension` instead of
     `encab.extensions.Extensions.configure_extension` is run for each plugin.
 
     :param config: the encab config
     :type config: Config
@@ -184,15 +183,15 @@
     try:
         config, location = load_config(encab_stream)
 
         logger = set_up_logger(config)
 
         extra = {"program": ENCAB}
 
-        logger.info("encab 0.0.7", extra=extra)
+        logger.info("encab 0.0.8", extra=extra)
         logger.info("Using configuration %s", location, extra=extra)
 
         logger.debug(
             "Encab config: %s",
             shorten(str(config), width=127, placeholder="..."),
             extra=extra,
         )
@@ -212,15 +211,17 @@
         config.encab.set_user()
         config.encab.set_group()
 
         assert config.encab.user is None or isinstance(config.encab.user, int)
         assert config.encab.group is None or isinstance(config.encab.group, int)
         assert config.encab.umask is None or isinstance(config.encab.umask, int)
 
-        Process.update_current(config.encab.user, config.encab.group, config.encab.umask)
+        Process.update_current(
+            config.encab.user, config.encab.group, config.encab.umask
+        )
 
         program_config = config.programs or {}
 
         if program_config:
             logger.debug("Starting program(s)...", extra=extra)
 
         observer = LoggingProgramObserver(ENCAB, logger, extra)
```

### Comparing `encab-0.0.7/src/encab/ext/log_sanitizer.py` & `encab-0.0.8/src/encab/ext/log_sanitizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
     certain patterns and replaces them with asterics.
 
     Predefined patterns are:
 
     - ``*KEY*``
     - ``*SECRET*``
     - ``*PASSWORD*``
-    - ``*PWD*``
 
     For patterns, UNIX file pattern rules are used (see https://docs.python.org/3/library/fnmatch.html#module-fnmatch)
     They can be extended or overriden in the extension settings.
 
     Example:
 
     Suppose you have the variable MY_PASSWORD set like this:
@@ -126,15 +125,15 @@
     so if you run a program like ``echo $MY_PASSWORD``,
     the output will be raplaced by ``******``.
 
     This extension is enabled by default and can be disabled in the extension settings.
 
     """
 
-    PATTERNS = ["*KEY*", "*SECRET*", "*PASSWORD", "*PWD*"]
+    PATTERNS = ["*KEY*", "*SECRET*", "*PASSWORD"]
 
     def __init__(self) -> None:
         self.sensitive_strings: Set[str] = set()
         self.settings = LogSanitizerSettings(patterns=self.PATTERNS, override=False)
         self.enabled = True
 
     @extension_impl
```

### Comparing `encab-0.0.7/src/encab/ext/startup_script.py` & `encab-0.0.8/src/encab/ext/startup_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,24 +260,29 @@
 
         extra = {"program": "startup_script/buildenv"}
 
         mylogger.info("Running buildenv script", extra={"program": ENCAB})
 
         lines: List[str] = list()
         try:
+
             def read_lines(process: Popen):
                 assert process.stdout
                 with process.stdout as stdout:
                     for line in stdout:
-                        strline = line.decode(sys.getdefaultencoding()).rstrip("\r\n\t ")
+                        strline = line.decode(sys.getdefaultencoding()).rstrip(
+                            "\r\n\t "
+                        )
                         lines.append(strline)
 
             process = Process(script, environment, shell=True)
 
-            exit_code = process.execute_and_log(read_lines, mylogger, extra, log_stdout=False)
+            exit_code = process.execute_and_log(
+                read_lines, mylogger, extra, log_stdout=False
+            )
 
             if exit_code != 0:
                 raise IOError(f"Buildenv script failed with exit code: {exit_code}")
 
         except BaseException as e:
             raise IOError(f"{STARTUP_SCRIPT}: Failed to execute buildenv script: {e}")
```

### Comparing `encab-0.0.7/src/encab/ext/validation.py` & `encab-0.0.8/src/encab/ext/validation.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.7/src/encab/extensions.py` & `encab-0.0.8/src/encab/extensions.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.7/src/encab/program.py` & `encab-0.0.8/src/encab/program.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 
-from typing import Dict, Optional,Union, List
+from typing import Dict, Optional, Union, List
 
 from subprocess import Popen
 from threading import Thread
 from signal import SIGINT, SIGTERM
 
 from logging import Logger, getLogger
 
@@ -112,14 +112,15 @@
         observer = self._observer
 
         startup_delay = self.config.startup_delay
 
         umask = self.config.umask
         user = self.config.user
         group = self.config.group
+        cwd = self.config.directory
 
         assert user is None or isinstance(user, int)
         assert group is None or isinstance(group, int)
 
         try:
             assert isinstance(startup_delay, float) or isinstance(startup_delay, int)
             assert isinstance(umask, int)
@@ -143,14 +144,15 @@
                 args,
                 env,
                 user=user,
                 group=group,
                 umask=umask,
                 shell=shell,
                 start_new_session=True,
+                cwd=cwd,
             )
             exit_code = self._process.execute_and_log(on_run, logger, extra)
             state.handle_exit(exit_code, self.command)
         except ProgramCanceledException:
             observer.on_cancel()
             state.set(ProgramState.CANCELED)
         except BaseException as e:
```

### Comparing `encab-0.0.7/src/encab/program_state.py` & `encab-0.0.8/src/encab/program_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
             extra=self.extra,
         )
 
         self.logger.debug("Config: %s", str(config), extra=self.extra)
 
         if config.user:
             self.logger.debug("User id: %d", config.user, extra=self.extra)
-            
-        if config.user:
+
+        if config.group:
             self.logger.debug("Group id: %d", config.group, extra=self.extra)
 
         if config.umask:
             self.logger.debug(
                 "umask: 0o%s", format(config.umask, "o"), extra=self.extra
             )
```

### Comparing `encab-0.0.7/src/encab/programs.py` & `encab-0.0.8/src/encab/programs.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.7/src/encab.egg-info/PKG-INFO` & `encab-0.0.8/src/encab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.7
+Version: 0.0.8
 Summary: Process manager
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.7
+   INFO  encab: encab 0.0.8
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -75,16 +75,16 @@
 
 ## Installation
 
 ### Install locally
 
 #### Prerequisites
 
-- [Python](https://www.python.org/) Version >= 3.9
-- activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
+- [Python](https://www.python.org/) Version >= 3.7
+- activated Python virtual environment such as [miniconda](https://docs.conda.io/en/latest/miniconda.html) or [virtualenv](https://virtualenv.pypa.io/en/latest/)
 
 ```sh
    pip install -U encab
 ```
 
 #### Run locally
 
@@ -104,15 +104,15 @@
 ```sh
    encab
 ```
 
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.7
+INFO  encab: encab 0.0.8
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
 INFO  main: Hello Encab!
 INFO  main: Exited with rc: 0
    ```
 
 ### Install in Container
 
@@ -121,20 +121,22 @@
 - [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
 
 #### Run in Container
 
 1. Create sample encab file `encab.yml`
 
 ```yml
+
    encab:
       dry_run: false
    programs:
       main:
          sh:
             - echo "Hello Encab!"
+
 ```
 
 2. Add Encab to your [Docker file][4].
 
    ```dockerfile
 
    FROM python:3.10.8-slim-bullseye
@@ -160,30 +162,30 @@
    # set encab as entrypoint
    ENTRYPOINT ["encab"]
 
    ```
 
    [4]: https://docs.docker.com/engine/reference/builder/
 
-2. Build container
+3. Build container
 
    ```sh
    docker build -t encab_minimum .
    ```
 
-3. Run container
+4. Run container
 
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.7
+   INFO  encab: encab 0.0.8
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.7/src/encab.egg-info/SOURCES.txt` & `encab-0.0.8/src/encab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

