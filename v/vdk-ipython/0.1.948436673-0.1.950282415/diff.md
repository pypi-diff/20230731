# Comparing `tmp/vdk-ipython-0.1.948436673.tar.gz` & `tmp/vdk-ipython-0.1.950282415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-ipython-0.1.948436673.tar", last modified: Fri Jul 28 09:42:42 2023, max compression
+gzip compressed data, was "vdk-ipython-0.1.950282415.tar", last modified: Mon Jul 31 08:15:13 2023, max compression
```

## Comparing `vdk-ipython-0.1.948436673.tar` & `vdk-ipython-0.1.950282415.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-28 09:42:19.000000 vdk-ipython-0.1.948436673/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-07-28 09:42:29.000000 vdk-ipython-0.1.948436673/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/tests/
--rw-rw-rw-   0 root         (0) root         (0)     9998 2023-07-28 09:42:19.000000 vdk-ipython-0.1.948436673/tests/test_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-07-31 08:14:55.000000 vdk-ipython-0.1.950282415/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-07-31 08:15:00.000000 vdk-ipython-0.1.950282415/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/src/vdk/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2023-07-31 08:14:55.000000 vdk-ipython-0.1.950282415/src/vdk/plugin/ipython.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-07-31 08:15:13.000000 vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-31 08:15:13.000000 vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 08:15:13.000000 vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-31 08:15:13.000000 vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 08:15:13.000000 vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-31 08:15:13.000000 vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:15:13.729678 vdk-ipython-0.1.950282415/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    10012 2023-07-31 08:14:55.000000 vdk-ipython-0.1.950282415/tests/test_plugin.py
```

### Comparing `vdk-ipython-0.1.948436673/PKG-INFO` & `vdk-ipython-0.1.950282415/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-ipython
-Version: 0.1.948436673
+Version: 0.1.950282415
 Summary: Ipython extension for VDK
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,27 +23,27 @@
 See more about magic commands: https://ipython.readthedocs.io/en/stable/interactive/magics.html
 
 
 ## Usage
 To use the extension it must be firstly installed with pip as a python package.
 Then to load the extension in Jupyter the user should use:
 ```
-%reload_ext vdk_ipython
+%reload_ext vdk.plugin.ipython
 ```
 And to load the VDK (Job Control object):
 ```
 %reload_VDK
 ```
 The %reload_VDK magic can be used with arguments such as passing the job's path with --path
 or giving the job a new with --name, etc.
 
 ### Example
 The output of this example is "myjob"
 ```
-%reload_ext vdk_ipython
+%reload_ext vdk.plugin.ipython
 
 %reload_VDK --name=myjob
 
 job_input = VDK.get_initialized_job_input()
 
 job_input.get_name()
 ```
```

### Comparing `vdk-ipython-0.1.948436673/README.md` & `vdk-ipython-0.1.950282415/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 See more about magic commands: https://ipython.readthedocs.io/en/stable/interactive/magics.html
 
 
 ## Usage
 To use the extension it must be firstly installed with pip as a python package.
 Then to load the extension in Jupyter the user should use:
 ```
-%reload_ext vdk_ipython
+%reload_ext vdk.plugin.ipython
 ```
 And to load the VDK (Job Control object):
 ```
 %reload_VDK
 ```
 The %reload_VDK magic can be used with arguments such as passing the job's path with --path
 or giving the job a new with --name, etc.
 
 ### Example
 The output of this example is "myjob"
 ```
-%reload_ext vdk_ipython
+%reload_ext vdk.plugin.ipython
 
 %reload_VDK --name=myjob
 
 job_input = VDK.get_initialized_job_input()
 
 job_input.get_name()
 ```
```

### Comparing `vdk-ipython-0.1.948436673/setup.py` & `vdk-ipython-0.1.950282415/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.1.948436673"
+__version__ = "0.1.950282415"
 
 setuptools.setup(
     name="vdk-ipython",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Ipython extension for VDK",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=["vdk-core", "iPython"],
     package_dir={"": "src"},
     packages=setuptools.find_namespace_packages(where="src"),
-    entry_points={"vdk.plugin.run": ["ipython = vdk_ipython"]},
+    entry_points={"vdk.plugin.run": ["ipython = vdk.plugin.ipython"]},
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/PKG-INFO` & `vdk-ipython-0.1.950282415/src/vdk_ipython.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-ipython
-Version: 0.1.948436673
+Version: 0.1.950282415
 Summary: Ipython extension for VDK
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,27 +23,27 @@
 See more about magic commands: https://ipython.readthedocs.io/en/stable/interactive/magics.html
 
 
 ## Usage
 To use the extension it must be firstly installed with pip as a python package.
 Then to load the extension in Jupyter the user should use:
 ```
-%reload_ext vdk_ipython
+%reload_ext vdk.plugin.ipython
 ```
 And to load the VDK (Job Control object):
 ```
 %reload_VDK
 ```
 The %reload_VDK magic can be used with arguments such as passing the job's path with --path
 or giving the job a new with --name, etc.
 
 ### Example
 The output of this example is "myjob"
 ```
-%reload_ext vdk_ipython
+%reload_ext vdk.plugin.ipython
 
 %reload_VDK --name=myjob
 
 job_input = VDK.get_initialized_job_input()
 
 job_input.get_name()
 ```
```

### Comparing `vdk-ipython-0.1.948436673/tests/test_plugin.py` & `vdk-ipython-0.1.950282415/tests/test_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 import pytest
 from IPython.core.error import UsageError
 from IPython.testing.globalipapp import start_ipython
 from vdk.api.job_input import IJobInput
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.builtin_plugins.run.job_context import JobContext
-from vdk_ipython import JobControl
+from vdk.plugin.ipython import JobControl
 
 _log = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope="session")
 def session_ip():
     yield start_ipython()
 
 
 @pytest.fixture(scope="function")
 def ip(session_ip):
-    session_ip.run_line_magic(magic_name="load_ext", line="vdk_ipython")
+    session_ip.run_line_magic(magic_name="load_ext", line="vdk.plugin.ipython")
     session_ip.run_line_magic(magic_name="reload_VDK", line="")
     yield session_ip
     session_ip.run_line_magic(magic_name="reset", line="-f")
 
 
 def test_load_vdk_with_no_arguments(ip):
     assert ip.user_global_ns["VDK"] is not None
```

