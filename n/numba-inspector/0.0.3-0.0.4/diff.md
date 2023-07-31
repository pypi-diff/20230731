# Comparing `tmp/numba_inspector-0.0.3.tar.gz` & `tmp/numba_inspector-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba_inspector-0.0.3.tar", max compression
+gzip compressed data, was "numba_inspector-0.0.4.tar", max compression
```

## Comparing `numba_inspector-0.0.3.tar` & `numba_inspector-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1386 2023-07-10 20:00:21.880231 numba_inspector-0.0.3/README.md
--rw-r--r--   0        0        0      265 2023-07-10 14:32:37.520531 numba_inspector-0.0.3/numba_inspector/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 14:24:29.660514 numba_inspector-0.0.3/numba_inspector/frontend/__init__.py
--rw-r--r--   0        0        0      159 2023-07-10 14:47:47.708513 numba_inspector-0.0.3/numba_inspector/frontend/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    33486 2023-07-10 17:43:41.334660 numba_inspector-0.0.3/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc
--rw-r--r--   0        0        0    36003 2023-07-10 17:43:35.494660 numba_inspector-0.0.3/numba_inspector/frontend/annotate.py
--rw-r--r--   0        0        0     8969 2023-07-20 22:05:37.975821 numba_inspector-0.0.3/numba_inspector/ipython_magic.py
--rw-r--r--   0        0        0      415 2023-07-31 12:43:07.289551 numba_inspector-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 numba_inspector-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1428 2023-07-31 13:05:42.728827 numba_inspector-0.0.4/README.md
+-rw-r--r--   0        0        0      265 2023-07-10 14:32:37.520531 numba_inspector-0.0.4/numba_inspector/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:24:29.660514 numba_inspector-0.0.4/numba_inspector/frontend/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-10 14:47:47.708513 numba_inspector-0.0.4/numba_inspector/frontend/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    33486 2023-07-10 17:43:41.334660 numba_inspector-0.0.4/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc
+-rw-r--r--   0        0        0    36003 2023-07-10 17:43:35.494660 numba_inspector-0.0.4/numba_inspector/frontend/annotate.py
+-rw-r--r--   0        0        0     8572 2023-07-31 12:49:16.065503 numba_inspector-0.0.4/numba_inspector/ipython_magic.py
+-rw-r--r--   0        0        0      415 2023-07-31 13:10:16.958725 numba_inspector-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1913 1970-01-01 00:00:00.000000 numba_inspector-0.0.4/PKG-INFO
```

### Comparing `numba_inspector-0.0.3/README.md` & `numba_inspector-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # numba-inspector
-View Numba compiled code in Jupyter
+Visualize and Debug Numba compiled code in Jupyter
 
 ## Quickstart
 
 ### Installation
 
-Fork then clone the repository:
+Install the package:
 ```console
-$ git clone git@github.com:<username>/numba-inspector.git
+pip install numba-inspector
 ```
 
 ### %%numba magic command
 
 ```python
 %load_ext numba_inspector
 ```
@@ -37,14 +37,20 @@
             y=y-1
     return x+y
 
 func(1,2)
 ```
 ![View the bytecode of a jitted function (CPUDispatcher object)](./examples/cpu_dispatcher_control_flow.png)
 
+
+Install the cudatoolkit:
+```console
+conda install cudatoolkit
+```
+
 ```python
 %%numba --ptx
 
 from numba import cuda
 import numpy as np
 
 @cuda.jit(lineinfo=True)
```

### Comparing `numba_inspector-0.0.3/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc` & `numba_inspector-0.0.4/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.3/numba_inspector/frontend/annotate.py` & `numba_inspector-0.0.4/numba_inspector/frontend/annotate.py`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.3/numba_inspector/ipython_magic.py` & `numba_inspector-0.0.4/numba_inspector/ipython_magic.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from IPython.core import magic_arguments
 from IPython.core.magic import Magics, magics_class, cell_magic
 from IPython.paths import get_ipython_cache_dir
 from numba_inspector.frontend.annotate import Annotate, Annotate2, AnnotateBytecode, AnnotatePTX, AnnotatePTXGray
 from functools import cache
 from numba.cuda.dispatcher import CUDADispatcher
-from ipykernel.compiler import get_file_name
 
 @magics_class
 class NumbaMagics(Magics):
     """
     Numba magic commands
     """
 
@@ -33,22 +32,14 @@
         dest='annotate_ptx', help="Produce a colorized HTML version of the source."
     )
     @cell_magic
     def numba(self, line, cell):
         """Compile the jitted function and display the
         compiled code, control, flow graph, etc.
         """
-        # from numba.core.ir import Loc
-        # import linecache
-        # exec(cell, globals())
-        # # print(Loc(get_file_name(cell), 7).lines)
-        # print(get_file_name(cell))
-        # # print(linecache.getlines(get_file_name(cell)))
-        # with open(get_file_name(cell), "r", encoding="utf-8") as f:
-        #     print(f.getlines())
         args = magic_arguments.parse_argstring(self.numba, line)
         function_names = self._get_function_names(cell)
         cell = self._preprocess_cell(cell)
         code = cell
         spec = self._build_module_spec(line, code)
 
         # Import the module
```

### Comparing `numba_inspector-0.0.3/PKG-INFO` & `numba_inspector-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: numba-inspector
-Version: 0.0.3
+Version: 0.0.4
 Summary: Visualize and Debug Numba compiled code in Jupyter
 Author: Matthew Murray
 Author-email: matthewmurray711@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: notebook (>=6.5.4,<7.0.0)
 Requires-Dist: numba (>=0.57.1,<0.58.0)
 Description-Content-Type: text/markdown
 
 # numba-inspector
-View Numba compiled code in Jupyter
+Visualize and Debug Numba compiled code in Jupyter
 
 ## Quickstart
 
 ### Installation
 
-Fork then clone the repository:
+Install the package:
 ```console
-$ git clone git@github.com:<username>/numba-inspector.git
+pip install numba-inspector
 ```
 
 ### %%numba magic command
 
 ```python
 %load_ext numba_inspector
 ```
@@ -51,14 +51,20 @@
             y=y-1
     return x+y
 
 func(1,2)
 ```
 ![View the bytecode of a jitted function (CPUDispatcher object)](./examples/cpu_dispatcher_control_flow.png)
 
+
+Install the cudatoolkit:
+```console
+conda install cudatoolkit
+```
+
 ```python
 %%numba --ptx
 
 from numba import cuda
 import numpy as np
 
 @cuda.jit(lineinfo=True)
```

