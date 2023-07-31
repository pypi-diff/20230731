# Comparing `tmp/contrastive_xai-0.1.0.tar.gz` & `tmp/contrastive_xai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrastive_xai-0.1.0.tar", last modified: Mon Jul 31 02:51:50 2023, max compression
+gzip compressed data, was "contrastive_xai-0.1.1.tar", last modified: Mon Jul 31 02:54:12 2023, max compression
```

## Comparing `contrastive_xai-0.1.0.tar` & `contrastive_xai-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:51:50.470887 contrastive_xai-0.1.0/
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:31:03.000000 contrastive_xai-0.1.0/Dockerfile
--rw-r--r--   0 samsonqian   (501) staff       (20)     1068 2023-07-31 02:29:28.000000 contrastive_xai-0.1.0/LICENSE
--rw-r--r--   0 samsonqian   (501) staff       (20)       61 2023-07-31 02:32:08.000000 contrastive_xai-0.1.0/MANIFEST.in
--rw-r--r--   0 samsonqian   (501) staff       (20)      408 2023-07-31 02:51:50.470973 contrastive_xai-0.1.0/PKG-INFO
--rw-r--r--   0 samsonqian   (501) staff       (20)       42 2023-07-31 02:29:28.000000 contrastive_xai-0.1.0/README.md
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:51:50.465674 contrastive_xai-0.1.0/contrastive_xai/
--rw-r--r--   0 samsonqian   (501) staff       (20)       60 2023-07-31 02:40:18.000000 contrastive_xai-0.1.0/contrastive_xai/__init__.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:51:50.466937 contrastive_xai-0.1.0/contrastive_xai/grad_cam/
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:39:52.000000 contrastive_xai-0.1.0/contrastive_xai/grad_cam/__init__.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     3986 2023-07-31 02:48:34.000000 contrastive_xai-0.1.0/contrastive_xai/grad_cam/contrastive_grad_cam.py
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:39:56.000000 contrastive_xai-0.1.0/contrastive_xai/grad_cam/grad_cam.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:51:50.468594 contrastive_xai-0.1.0/contrastive_xai/lime/
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:38:59.000000 contrastive_xai-0.1.0/contrastive_xai/lime/__init__.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     3306 2023-07-31 02:47:22.000000 contrastive_xai-0.1.0/contrastive_xai/lime/contrastive_lime.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     2487 2023-07-31 02:39:46.000000 contrastive_xai-0.1.0/contrastive_xai/lime/lime.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     3897 2023-07-31 02:28:35.000000 contrastive_xai-0.1.0/contrastive_xai/lime/lime_contrastive.py
--rw-r--r--   0 samsonqian   (501) staff       (20)    12315 2023-07-31 02:28:39.000000 contrastive_xai-0.1.0/contrastive_xai/lime/my_lime_exp.py
--rw-r--r--   0 samsonqian   (501) staff       (20)    49327 2023-07-31 02:28:41.000000 contrastive_xai-0.1.0/contrastive_xai/lime/utils.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:51:50.470778 contrastive_xai-0.1.0/contrastive_xai/shap/
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:40:00.000000 contrastive_xai-0.1.0/contrastive_xai/shap/__init__.py
--rw-r--r--   0 samsonqian   (501) staff       (20)     3313 2023-07-31 02:49:24.000000 contrastive_xai-0.1.0/contrastive_xai/shap/contrastive_shap.py
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:40:03.000000 contrastive_xai-0.1.0/contrastive_xai/shap/shap.py
--rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:31:38.000000 contrastive_xai-0.1.0/contrastive_xai/utils.py
-drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:51:50.466284 contrastive_xai-0.1.0/contrastive_xai.egg-info/
--rw-r--r--   0 samsonqian   (501) staff       (20)      408 2023-07-31 02:51:50.000000 contrastive_xai-0.1.0/contrastive_xai.egg-info/PKG-INFO
--rw-r--r--   0 samsonqian   (501) staff       (20)      721 2023-07-31 02:51:50.000000 contrastive_xai-0.1.0/contrastive_xai.egg-info/SOURCES.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)        1 2023-07-31 02:51:50.000000 contrastive_xai-0.1.0/contrastive_xai.egg-info/dependency_links.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)       16 2023-07-31 02:51:50.000000 contrastive_xai-0.1.0/contrastive_xai.egg-info/top_level.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)      203 2023-07-31 02:32:16.000000 contrastive_xai-0.1.0/requirements.txt
--rw-r--r--   0 samsonqian   (501) staff       (20)      141 2023-07-31 02:51:50.471318 contrastive_xai-0.1.0/setup.cfg
--rw-r--r--   0 samsonqian   (501) staff       (20)     1448 2023-07-31 02:42:35.000000 contrastive_xai-0.1.0/setup.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:54:12.021549 contrastive_xai-0.1.1/
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:31:03.000000 contrastive_xai-0.1.1/Dockerfile
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1068 2023-07-31 02:29:28.000000 contrastive_xai-0.1.1/LICENSE
+-rw-r--r--   0 samsonqian   (501) staff       (20)       61 2023-07-31 02:32:08.000000 contrastive_xai-0.1.1/MANIFEST.in
+-rw-r--r--   0 samsonqian   (501) staff       (20)      681 2023-07-31 02:54:12.021622 contrastive_xai-0.1.1/PKG-INFO
+-rw-r--r--   0 samsonqian   (501) staff       (20)      314 2023-07-31 02:53:40.000000 contrastive_xai-0.1.1/README.md
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:54:12.016820 contrastive_xai-0.1.1/contrastive_xai/
+-rw-r--r--   0 samsonqian   (501) staff       (20)       60 2023-07-31 02:40:18.000000 contrastive_xai-0.1.1/contrastive_xai/__init__.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:54:12.018015 contrastive_xai-0.1.1/contrastive_xai/grad_cam/
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:39:52.000000 contrastive_xai-0.1.1/contrastive_xai/grad_cam/__init__.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     3986 2023-07-31 02:48:34.000000 contrastive_xai-0.1.1/contrastive_xai/grad_cam/contrastive_grad_cam.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:39:56.000000 contrastive_xai-0.1.1/contrastive_xai/grad_cam/grad_cam.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:54:12.019538 contrastive_xai-0.1.1/contrastive_xai/lime/
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:38:59.000000 contrastive_xai-0.1.1/contrastive_xai/lime/__init__.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     3306 2023-07-31 02:47:22.000000 contrastive_xai-0.1.1/contrastive_xai/lime/contrastive_lime.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     2487 2023-07-31 02:39:46.000000 contrastive_xai-0.1.1/contrastive_xai/lime/lime.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     3897 2023-07-31 02:28:35.000000 contrastive_xai-0.1.1/contrastive_xai/lime/lime_contrastive.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)    12315 2023-07-31 02:28:39.000000 contrastive_xai-0.1.1/contrastive_xai/lime/my_lime_exp.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)    49327 2023-07-31 02:28:41.000000 contrastive_xai-0.1.1/contrastive_xai/lime/utils.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:54:12.021447 contrastive_xai-0.1.1/contrastive_xai/shap/
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:40:00.000000 contrastive_xai-0.1.1/contrastive_xai/shap/__init__.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)     3313 2023-07-31 02:49:24.000000 contrastive_xai-0.1.1/contrastive_xai/shap/contrastive_shap.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:40:03.000000 contrastive_xai-0.1.1/contrastive_xai/shap/shap.py
+-rw-r--r--   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:31:38.000000 contrastive_xai-0.1.1/contrastive_xai/utils.py
+drwxr-xr-x   0 samsonqian   (501) staff       (20)        0 2023-07-31 02:54:12.017399 contrastive_xai-0.1.1/contrastive_xai.egg-info/
+-rw-r--r--   0 samsonqian   (501) staff       (20)      681 2023-07-31 02:54:11.000000 contrastive_xai-0.1.1/contrastive_xai.egg-info/PKG-INFO
+-rw-r--r--   0 samsonqian   (501) staff       (20)      721 2023-07-31 02:54:11.000000 contrastive_xai-0.1.1/contrastive_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)        1 2023-07-31 02:54:11.000000 contrastive_xai-0.1.1/contrastive_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)       16 2023-07-31 02:54:11.000000 contrastive_xai-0.1.1/contrastive_xai.egg-info/top_level.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)      203 2023-07-31 02:32:16.000000 contrastive_xai-0.1.1/requirements.txt
+-rw-r--r--   0 samsonqian   (501) staff       (20)      141 2023-07-31 02:54:12.021902 contrastive_xai-0.1.1/setup.cfg
+-rw-r--r--   0 samsonqian   (501) staff       (20)     1448 2023-07-31 02:53:48.000000 contrastive_xai-0.1.1/setup.py
```

### Comparing `contrastive_xai-0.1.0/LICENSE` & `contrastive_xai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai/grad_cam/contrastive_grad_cam.py` & `contrastive_xai-0.1.1/contrastive_xai/grad_cam/contrastive_grad_cam.py`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai/lime/contrastive_lime.py` & `contrastive_xai-0.1.1/contrastive_xai/lime/contrastive_lime.py`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai/lime/lime.py` & `contrastive_xai-0.1.1/contrastive_xai/lime/lime.py`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai/lime/lime_contrastive.py` & `contrastive_xai-0.1.1/contrastive_xai/lime/lime_contrastive.py`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai/lime/my_lime_exp.py` & `contrastive_xai-0.1.1/contrastive_xai/lime/my_lime_exp.py`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai/lime/utils.py` & `contrastive_xai-0.1.1/contrastive_xai/lime/utils.py`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai/shap/contrastive_shap.py` & `contrastive_xai-0.1.1/contrastive_xai/shap/contrastive_shap.py`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/contrastive_xai.egg-info/SOURCES.txt` & `contrastive_xai-0.1.1/contrastive_xai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contrastive_xai-0.1.0/setup.py` & `contrastive_xai-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     install_reqs = _parse_requirements("requirements.txt")
 except Exception as e:
     logging.warning('Fail load requirements file, so using default ones.')
     install_reqs = []
 
 setup(
     name="contrastive_xai",
-    version="0.1.0",
+    version="0.1.1",
     author="Samson Qian",
     author_email="samsonqian@gmail.com",
     packages=["contrastive_xai", "contrastive_xai.grad_cam", "contrastive_xai.lime", "contrastive_xai.shap"],
     url="https://github.com/samsonq/contrastive-xai",
     license="MIT",
     description="Contrastive Explainable AI Algorithms",
     long_description=README,
```

