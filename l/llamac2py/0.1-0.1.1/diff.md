# Comparing `tmp/llamac2py-0.1.tar.gz` & `tmp/llamac2py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamac2py-0.1.tar", last modified: Mon Jul 31 04:00:28 2023, max compression
+gzip compressed data, was "llamac2py-0.1.1.tar", last modified: Mon Jul 31 05:54:46 2023, max compression
```

## Comparing `llamac2py-0.1.tar` & `llamac2py-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 04:00:28.718313 llamac2py-0.1/
--rw-rw-rw-   0        0        0     1084 2023-07-30 17:40:42.000000 llamac2py-0.1/LICENSE
--rw-rw-rw-   0        0        0      422 2023-07-31 04:00:28.718313 llamac2py-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2023-07-30 18:29:59.000000 llamac2py-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 04:00:28.717367 llamac2py-0.1/llamac2py.egg-info/
--rw-rw-rw-   0        0        0      422 2023-07-31 04:00:28.000000 llamac2py-0.1/llamac2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-07-31 04:00:28.000000 llamac2py-0.1/llamac2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:00:28.000000 llamac2py-0.1/llamac2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 04:00:28.000000 llamac2py-0.1/llamac2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 04:00:28.719263 llamac2py-0.1/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-07-30 16:52:20.000000 llamac2py-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:46.089161 llamac2py-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-30 17:40:42.000000 llamac2py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-31 05:54:46.089161 llamac2py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2023-07-31 04:11:20.000000 llamac2py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:46.073419 llamac2py-0.1.1/llamac2py/
+-rw-rw-rw-   0        0        0        0 2023-07-30 16:41:01.000000 llamac2py-0.1.1/llamac2py/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-07-30 18:50:11.000000 llamac2py-0.1.1/llamac2py/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:46.089161 llamac2py-0.1.1/llamac2py.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-31 05:54:45.000000 llamac2py-0.1.1/llamac2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-07-31 05:54:45.000000 llamac2py-0.1.1/llamac2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:54:45.000000 llamac2py-0.1.1/llamac2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 05:54:45.000000 llamac2py-0.1.1/llamac2py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22107 2023-07-30 17:40:42.000000 llamac2py-0.1.1/run.c
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:54:46.089161 llamac2py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1191 2023-07-31 05:54:40.000000 llamac2py-0.1.1/setup.py
```

### Comparing `llamac2py-0.1/LICENSE` & `llamac2py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llamac2py-0.1/README.md` & `llamac2py-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # llamac2py
 
 llamac2py is a Python package that provides a wrapper for running inference using the Llama-2 Transformer model. The package includes a C executable (run.c) from [Karpathy's llama2.c](https://github.com/karpathy/llama2.c) that performs the inference, and the package allows easy inference for the same.
 ---
-download model: 
+## Get Started:
 
-`wget https://huggingface.co/karpathy/tinyllamas/resolve/main/stories15M.bin` # Will add support for more models
+Clone the Repository: `git clone https://github.com/adarshxs/llamac2py`
 
-`git clone https://github.com/adarshxs/llamac2py`
+cd into the Repository: `cd llamac2py`
 
-Compile the C code using the following command to generate the executable "run" using:
+download the Model (Will add support for more models): 
 
-`cd llamac2py && gcc -O3 -o run run.c -lm`
+`wget https://huggingface.co/karpathy/tinyllamas/resolve/main/stories15M.bin`
 
+Compile the C file: `run make`
 
-`cd .. ` # Go back to the root
-
-Then in a notebook or a python script, run:
+Then in a notebook or a Python script, run:
 
 ```
 from llamac2py.wrapper import generate_short_story
 
 # Load your Llama-2 model checkpoint (model.bin) here
 checkpoint_file = 'path/to/your/model.bin'
```

