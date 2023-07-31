# Comparing `tmp/easyecs-0.1.2.tar.gz` & `tmp/easyecs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.1.2.tar", max compression
+gzip compressed data, was "easyecs-0.1.3.tar", max compression
```

## Comparing `easyecs-0.1.2.tar` & `easyecs-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2230 2023-07-31 19:57:56.318579 easyecs-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8375 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0     3390 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0     3511 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     7949 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0      468 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/cloudformation/template/verify.py
--rw-r--r--   0        0        0    12418 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1459 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2043 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2360 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/helpers/signal.py
--rw-r--r--   0        0        0     1672 2023-07-31 19:57:56.342580 easyecs-0.1.2/easyecs/model/ecs.py
--rw-r--r--   0        0        0      505 2023-07-31 19:57:56.346580 easyecs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-07-31 20:04:45.575575 easyecs-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     8375 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0     3390 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0     3511 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     7949 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/cloudformation/template/verify.py
+-rw-r--r--   0        0        0    12418 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1459 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2043 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     2360 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0     1666 2023-07-31 20:04:45.599577 easyecs-0.1.3/easyecs/model/ecs.py
+-rw-r--r--   0        0        0      505 2023-07-31 20:04:45.599577 easyecs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 easyecs-0.1.3/PKG-INFO
```

### Comparing `easyecs-0.1.2/README.md` & `easyecs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/cli.py` & `easyecs-0.1.3/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/cloudformation/fetch.py` & `easyecs-0.1.3/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/cloudformation/stack/__init__.py` & `easyecs-0.1.3/easyecs/cloudformation/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/cloudformation/template/__init__.py` & `easyecs-0.1.3/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/command/__init__.py` & `easyecs-0.1.3/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/docker/__init__.py` & `easyecs-0.1.3/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/helpers/common.py` & `easyecs-0.1.3/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/helpers/loader.py` & `easyecs-0.1.3/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/helpers/selector.py` & `easyecs-0.1.3/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/helpers/settings.py` & `easyecs-0.1.3/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.2/easyecs/model/ecs.py` & `easyecs-0.1.3/easyecs/model/ecs.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     root: str
     exclude: List[str]
 
 
 class EcsFileBuildModel(BaseModel):
     dockerfile: str = "Dockerfile"
     target: Optional[str] = None
-    args: List[Dict[str, str]] = []
+    args: Dict[str, str] = {}
 
 
 class EcsFileEnvModel(BaseModel):
     name: str
     value: str
     active: bool = True
```

### Comparing `easyecs-0.1.2/PKG-INFO` & `easyecs-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

