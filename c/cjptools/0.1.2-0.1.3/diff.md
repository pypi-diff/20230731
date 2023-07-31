# Comparing `tmp/cjptools-0.1.2.tar.gz` & `tmp/cjptools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjptools-0.1.2.tar", last modified: Fri Jul 28 07:17:48 2023, max compression
+gzip compressed data, was "cjptools-0.1.3.tar", last modified: Mon Jul 31 13:37:23 2023, max compression
```

## Comparing `cjptools-0.1.2.tar` & `cjptools-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.330849 cjptools-0.1.2/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      276 2023-07-28 07:17:48.330849 cjptools-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.309327 cjptools-0.1.2/cjptools/
--rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.2/cjptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.319329 cjptools-0.1.2/cjptools/printModules/
--rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/__init__.py
--rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/absPrinter.py
--rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/printerCompose.py
--rw-rw-rw-   0        0        0      626 2022-10-13 16:20:01.000000 cjptools-0.1.2/cjptools/printModules/printers.py
-drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.329794 cjptools-0.1.2/cjptools/utils/
--rw-rw-rw-   0        0        0      167 2023-07-28 07:06:53.000000 cjptools-0.1.2/cjptools/utils/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.2/cjptools/utils/check.py
--rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.2/cjptools/utils/gpu_mem_track.py
--rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.2/cjptools/utils/modelsize_estimate.py
--rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.2/cjptools/utils/path.py
--rw-rw-rw-   0        0        0      768 2023-07-28 03:39:36.000000 cjptools-0.1.2/cjptools/utils/rnd.py
--rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.2/cjptools/utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-28 07:17:48.314342 cjptools-0.1.2/cjptools.egg-info/
--rw-rw-rw-   0        0        0      276 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 07:17:48.000000 cjptools-0.1.2/cjptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 07:17:48.331823 cjptools-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-07-28 07:17:44.000000 cjptools-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:37:23.477046 cjptools-0.1.3/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-07-31 13:37:23.477046 cjptools-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 13:37:23.433316 cjptools-0.1.3/cjptools/
+-rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.3/cjptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:37:23.440297 cjptools-0.1.3/cjptools/dptools/
+-rw-rw-rw-   0        0        0       25 2023-07-31 13:36:57.000000 cjptools-0.1.3/cjptools/dptools/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-07-31 13:36:34.000000 cjptools-0.1.3/cjptools/dptools/rdpAccount.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:37:23.445285 cjptools-0.1.3/cjptools/printModules/
+-rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.3/cjptools/printModules/__init__.py
+-rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.3/cjptools/printModules/absPrinter.py
+-rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.3/cjptools/printModules/printerCompose.py
+-rw-rw-rw-   0        0        0      626 2022-10-13 16:20:01.000000 cjptools-0.1.3/cjptools/printModules/printers.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:37:23.476047 cjptools-0.1.3/cjptools/utils/
+-rw-rw-rw-   0        0        0      167 2023-07-28 07:06:53.000000 cjptools-0.1.3/cjptools/utils/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.3/cjptools/utils/check.py
+-rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.3/cjptools/utils/gpu_mem_track.py
+-rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.3/cjptools/utils/modelsize_estimate.py
+-rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.3/cjptools/utils/path.py
+-rw-rw-rw-   0        0        0      741 2023-07-31 13:33:07.000000 cjptools-0.1.3/cjptools/utils/rnd.py
+-rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.3/cjptools/utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:37:23.438303 cjptools-0.1.3/cjptools.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-07-31 13:37:23.000000 cjptools-0.1.3/cjptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-07-31 13:37:23.000000 cjptools-0.1.3/cjptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 13:37:23.000000 cjptools-0.1.3/cjptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 13:37:23.000000 cjptools-0.1.3/cjptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 13:37:23.478043 cjptools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-07-31 13:37:14.000000 cjptools-0.1.3/setup.py
```

### Comparing `cjptools-0.1.2/LICENSE` & `cjptools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.2/cjptools/printModules/printers.py` & `cjptools-0.1.3/cjptools/printModules/printers.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.2/cjptools/utils/gpu_mem_track.py` & `cjptools-0.1.3/cjptools/utils/gpu_mem_track.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.2/cjptools/utils/modelsize_estimate.py` & `cjptools-0.1.3/cjptools/utils/modelsize_estimate.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.2/cjptools/utils/path.py` & `cjptools-0.1.3/cjptools/utils/path.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.2/cjptools/utils/rnd.py` & `cjptools-0.1.3/cjptools/utils/rnd.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 def torch_seed(seed=0):
     torch.manual_seed(seed)  # sets the seed for generating random numbers.
     torch.cuda.manual_seed(
         seed)  # Sets the seed for generating random numbers for the current GPU. It’s safe to call this function if CUDA is not available; in that case, it is silently ignored.
     torch.cuda.manual_seed_all(
         seed)  # Sets the seed for generating random numbers on all GPUs. It’s safe to call this function if CUDA is not available; in that case, it is silently ignored.
-    if seed == 0:
-        torch.backends.cudnn.deterministic = True
-        torch.backends.cudnn.benchmark = False
+    torch.backends.cudnn.deterministic = True
+    torch.backends.cudnn.benchmark = False
 
 
 def normal_seed(seed=0):
     random.seed(seed)
     np.random.seed(seed)
```

### Comparing `cjptools-0.1.2/setup.py` & `cjptools-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="cjptools",
-    version="0.1.2",
+    version="0.1.3",
     keywords=("database", "localServer"),
     description="My Personal Toolkit",
     long_description="My Personal Toolkit",
     license="MIT Licence",
     author="Cai Jianping",
     author_email="jpingcai@163.com",
```

