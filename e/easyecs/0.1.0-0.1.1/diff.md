# Comparing `tmp/easyecs-0.1.0.tar.gz` & `tmp/easyecs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyecs-0.1.0.tar", max compression
+gzip compressed data, was "easyecs-0.1.1.tar", max compression
```

## Comparing `easyecs-0.1.0.tar` & `easyecs-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2230 2023-07-31 07:36:37.752166 easyecs-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-27 12:28:14.648874 easyecs-0.1.0/easyecs/__init__.py
--rwxr-xr-x   0        0        0     8473 2023-07-31 07:36:36.912166 easyecs-0.1.0/easyecs/cli.py
--rw-r--r--   0        0        0        0 2023-07-27 12:17:09.308874 easyecs-0.1.0/easyecs/cloudformation/__init__.py
--rw-r--r--   0        0        0     3390 2023-07-31 07:36:31.412166 easyecs-0.1.0/easyecs/cloudformation/fetch.py
--rw-r--r--   0        0        0     3511 2023-07-31 07:36:31.412166 easyecs-0.1.0/easyecs/cloudformation/stack/__init__.py
--rw-r--r--   0        0        0     8098 2023-07-31 07:36:31.422166 easyecs-0.1.0/easyecs/cloudformation/template/__init__.py
--rw-r--r--   0        0        0      488 2023-07-31 07:36:31.422166 easyecs-0.1.0/easyecs/cloudformation/template/verify.py
--rw-r--r--   0        0        0    12565 2023-07-31 07:36:31.422166 easyecs-0.1.0/easyecs/command/__init__.py
--rw-r--r--   0        0        0     1530 2023-07-31 07:36:33.182166 easyecs-0.1.0/easyecs/docker/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 12:17:27.718874 easyecs-0.1.0/easyecs/helpers/__init__.py
--rw-r--r--   0        0        0      264 2023-07-31 07:36:31.422166 easyecs-0.1.0/easyecs/helpers/color.py
--rw-r--r--   0        0        0     2043 2023-07-31 07:36:31.422166 easyecs-0.1.0/easyecs/helpers/common.py
--rw-r--r--   0        0        0     1895 2023-07-31 07:36:31.422166 easyecs-0.1.0/easyecs/helpers/loader.py
--rw-r--r--   0        0        0      531 2023-07-31 07:36:38.162166 easyecs-0.1.0/easyecs/helpers/selector.py
--rw-r--r--   0        0        0     2285 2023-07-31 07:36:31.422166 easyecs-0.1.0/easyecs/helpers/settings.py
--rw-r--r--   0        0        0       42 2023-07-31 07:36:31.862167 easyecs-0.1.0/easyecs/helpers/signal.py
--rw-r--r--   0        0        0      485 2023-07-31 07:45:08.852167 easyecs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 easyecs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2230 2023-07-31 17:03:44.840777 easyecs-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/__init__.py
+-rwxr-xr-x   0        0        0     8473 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cli.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/__init__.py
+-rw-r--r--   0        0        0     3390 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/fetch.py
+-rw-r--r--   0        0        0     3511 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/stack/__init__.py
+-rw-r--r--   0        0        0     8098 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/template/__init__.py
+-rw-r--r--   0        0        0      488 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/cloudformation/template/verify.py
+-rw-r--r--   0        0        0    12565 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/command/__init__.py
+-rw-r--r--   0        0        0     1530 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/docker/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/__init__.py
+-rw-r--r--   0        0        0      264 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/color.py
+-rw-r--r--   0        0        0     2043 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/common.py
+-rw-r--r--   0        0        0     1895 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/loader.py
+-rw-r--r--   0        0        0      531 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/selector.py
+-rw-r--r--   0        0        0     2285 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/settings.py
+-rw-r--r--   0        0        0       42 2023-07-31 17:03:44.860777 easyecs-0.1.1/easyecs/helpers/signal.py
+-rw-r--r--   0        0        0      485 2023-07-31 17:03:44.860777 easyecs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 easyecs-0.1.1/PKG-INFO
```

### Comparing `easyecs-0.1.0/README.md` & `easyecs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/cli.py` & `easyecs-0.1.1/easyecs/cli.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/cloudformation/fetch.py` & `easyecs-0.1.1/easyecs/cloudformation/fetch.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/cloudformation/stack/__init__.py` & `easyecs-0.1.1/easyecs/cloudformation/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/cloudformation/template/__init__.py` & `easyecs-0.1.1/easyecs/cloudformation/template/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/command/__init__.py` & `easyecs-0.1.1/easyecs/command/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/docker/__init__.py` & `easyecs-0.1.1/easyecs/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/helpers/common.py` & `easyecs-0.1.1/easyecs/helpers/common.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/helpers/loader.py` & `easyecs-0.1.1/easyecs/helpers/loader.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/helpers/selector.py` & `easyecs-0.1.1/easyecs/helpers/selector.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/easyecs/helpers/settings.py` & `easyecs-0.1.1/easyecs/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `easyecs-0.1.0/PKG-INFO` & `easyecs-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyecs
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: BONVARLET Benjamin
 Author-email: benjaminbonvarlet96@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

