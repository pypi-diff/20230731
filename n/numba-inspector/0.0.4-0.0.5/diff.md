# Comparing `tmp/numba_inspector-0.0.4.tar.gz` & `tmp/numba_inspector-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba_inspector-0.0.4.tar", max compression
+gzip compressed data, was "numba_inspector-0.0.5.tar", max compression
```

## Comparing `numba_inspector-0.0.4.tar` & `numba_inspector-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1428 2023-07-31 13:05:42.728827 numba_inspector-0.0.4/README.md
--rw-r--r--   0        0        0      265 2023-07-10 14:32:37.520531 numba_inspector-0.0.4/numba_inspector/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 14:24:29.660514 numba_inspector-0.0.4/numba_inspector/frontend/__init__.py
--rw-r--r--   0        0        0      159 2023-07-10 14:47:47.708513 numba_inspector-0.0.4/numba_inspector/frontend/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    33486 2023-07-10 17:43:41.334660 numba_inspector-0.0.4/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc
--rw-r--r--   0        0        0    36003 2023-07-10 17:43:35.494660 numba_inspector-0.0.4/numba_inspector/frontend/annotate.py
--rw-r--r--   0        0        0     8572 2023-07-31 12:49:16.065503 numba_inspector-0.0.4/numba_inspector/ipython_magic.py
--rw-r--r--   0        0        0      415 2023-07-31 13:10:16.958725 numba_inspector-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1913 1970-01-01 00:00:00.000000 numba_inspector-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1550 2023-07-31 13:14:24.056403 numba_inspector-0.0.5/README.md
+-rw-r--r--   0        0        0      265 2023-07-10 14:32:37.520531 numba_inspector-0.0.5/numba_inspector/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:24:29.660514 numba_inspector-0.0.5/numba_inspector/frontend/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-10 14:47:47.708513 numba_inspector-0.0.5/numba_inspector/frontend/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    33486 2023-07-10 17:43:41.334660 numba_inspector-0.0.5/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc
+-rw-r--r--   0        0        0    36003 2023-07-10 17:43:35.494660 numba_inspector-0.0.5/numba_inspector/frontend/annotate.py
+-rw-r--r--   0        0        0     8572 2023-07-31 12:49:16.065503 numba_inspector-0.0.5/numba_inspector/ipython_magic.py
+-rw-r--r--   0        0        0      415 2023-07-31 13:15:37.752197 numba_inspector-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 numba_inspector-0.0.5/PKG-INFO
```

### Comparing `numba_inspector-0.0.4/README.md` & `numba_inspector-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             y=y+1
         else:
             y=y-1
     return x+y
 
 func(1,2)
 ```
-![View the bytecode of a jitted function (CPUDispatcher object)](./examples/cpu_dispatcher_control_flow.png)
+![View the bytecode of a jitted function (CPUDispatcher object)](https://raw.githubusercontent.com/Matt711/numba-inspector/main/examples/cpu_dispatcher_control_flow.png)
 
 
 Install the cudatoolkit:
 ```console
 conda install cudatoolkit
 ```
 
@@ -70,8 +70,8 @@
 d_a = cuda.to_device(a)
 blocks = 32
 threads = 128
 increment_by_one[blocks, threads](d_a)
 cuda.synchronize()
 d_a.copy_to_host()
 ```
-![View the PTX of CUDA kernel (CPUDispatcher object example)](./examples/cuda_dispatcher.png)
+![View the PTX of CUDA kernel (CPUDispatcher object example)](https://raw.githubusercontent.com/Matt711/numba-inspector/main/examples/cuda_dispatcher.png)
```

### Comparing `numba_inspector-0.0.4/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc` & `numba_inspector-0.0.5/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.4/numba_inspector/frontend/annotate.py` & `numba_inspector-0.0.5/numba_inspector/frontend/annotate.py`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.4/numba_inspector/ipython_magic.py` & `numba_inspector-0.0.5/numba_inspector/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.4/PKG-INFO` & `numba_inspector-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-inspector
-Version: 0.0.4
+Version: 0.0.5
 Summary: Visualize and Debug Numba compiled code in Jupyter
 Author: Matthew Murray
 Author-email: matthewmurray711@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -49,15 +49,15 @@
             y=y+1
         else:
             y=y-1
     return x+y
 
 func(1,2)
 ```
-![View the bytecode of a jitted function (CPUDispatcher object)](./examples/cpu_dispatcher_control_flow.png)
+![View the bytecode of a jitted function (CPUDispatcher object)](https://raw.githubusercontent.com/Matt711/numba-inspector/main/examples/cpu_dispatcher_control_flow.png)
 
 
 Install the cudatoolkit:
 ```console
 conda install cudatoolkit
 ```
 
@@ -84,9 +84,9 @@
 d_a = cuda.to_device(a)
 blocks = 32
 threads = 128
 increment_by_one[blocks, threads](d_a)
 cuda.synchronize()
 d_a.copy_to_host()
 ```
-![View the PTX of CUDA kernel (CPUDispatcher object example)](./examples/cuda_dispatcher.png)
+![View the PTX of CUDA kernel (CPUDispatcher object example)](https://raw.githubusercontent.com/Matt711/numba-inspector/main/examples/cuda_dispatcher.png)
```

