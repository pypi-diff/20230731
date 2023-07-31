# Comparing `tmp/lc-checkpoint-0.5.0.tar.gz` & `tmp/lc-checkpoint-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lc-checkpoint-0.5.0.tar", last modified: Thu Jul 13 07:52:22 2023, max compression
+gzip compressed data, was "lc-checkpoint-0.5.1.tar", last modified: Mon Jul 31 11:53:22 2023, max compression
```

## Comparing `lc-checkpoint-0.5.0.tar` & `lc-checkpoint-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.162656 lc-checkpoint-0.5.0/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     1041 2023-06-06 16:13:52.000000 lc-checkpoint-0.5.0/LICENSE
--rw-r--r--   0 yeoshuheng   (501) staff       (20)     6044 2023-07-13 07:52:22.162727 lc-checkpoint-0.5.0/PKG-INFO
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     5698 2023-07-13 07:48:09.000000 lc-checkpoint-0.5.0/README.md
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      104 2023-06-06 16:07:14.000000 lc-checkpoint-0.5.0/pyproject.toml
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      608 2023-07-13 07:52:22.163004 lc-checkpoint-0.5.0/setup.cfg
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.160790 lc-checkpoint-0.5.0/src/
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.161676 lc-checkpoint-0.5.0/src/lc_checkpoint/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        0 2023-06-06 15:15:50.000000 lc-checkpoint-0.5.0/src/lc_checkpoint/__init__.py
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6081 2023-07-13 07:47:41.000000 lc-checkpoint-0.5.0/src/lc_checkpoint/main.py
-drwxr-xr-x   0 yeoshuheng   (501) staff       (20)        0 2023-07-13 07:52:22.162515 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)     6044 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/PKG-INFO
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)      262 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/SOURCES.txt
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)        1 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/dependency_links.txt
--rw-rw-rw-   0 yeoshuheng   (501) staff       (20)       14 2023-07-13 07:52:22.000000 lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5698 2023-07-31 11:31:00.000000 lc-checkpoint-0.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/src/lc_checkpoint/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 10:40:38.000000 lc-checkpoint-0.5.1/src/lc_checkpoint/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6091 2023-07-31 11:10:39.000000 lc-checkpoint-0.5.1/src/lc_checkpoint/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:53:22.516278 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-31 11:53:22.000000 lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/top_level.txt
```

### Comparing `lc-checkpoint-0.5.0/LICENSE` & `lc-checkpoint-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.5.0/PKG-INFO` & `lc-checkpoint-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lc-checkpoint-0.5.0/README.md` & `lc-checkpoint-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lc-checkpoint-0.5.0/setup.cfg` & `lc-checkpoint-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lc-checkpoint
-version = 0.5.0
+version = 0.5.1
 author = Dedy Van Hauten
 author_email = dedy.van@ui.ac.id
 description = A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pypi.org/project/lc-checkpoint/
 classifiers =
```

### Comparing `lc-checkpoint-0.5.0/src/lc_checkpoint/main.py` & `lc-checkpoint-0.5.1/src/lc_checkpoint/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     os.makedirs(checkpoint_dir, exist_ok=True)
     num_buckets = num_buckets
     num_bits = num_bits
     prev_state_dict = net.state_dict()
 
 def compress_data(δt, num_bits= 32, k = 5, treshold=True):
     sign = np.sign(δt)
-    x_abs = np.abs(δt)
+    x_abs = np.round(np.abs(δt))
     exponent = np.floor(np.log2(x_abs, where = (x_abs != 0)))
     mantissa = x_abs / (2 ** exponent)
     quantized = sign * mantissa * (2 ** exponent)
     smallest_value = 2 ** (-1 * num_bits)
     quantized = np.round(quantized / smallest_value) * smallest_value
 
     the_sign = np.zeros_like(δt)
```

### Comparing `lc-checkpoint-0.5.0/src/lc_checkpoint.egg-info/PKG-INFO` & `lc-checkpoint-0.5.1/src/lc_checkpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lc-checkpoint
-Version: 0.5.0
+Version: 0.5.1
 Summary: A package for compressing PyTorch model checkpoints using the LC-Checkpoint method
 Home-page: https://pypi.org/project/lc-checkpoint/
 Author: Dedy Van Hauten
 Author-email: dedy.van@ui.ac.id
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

