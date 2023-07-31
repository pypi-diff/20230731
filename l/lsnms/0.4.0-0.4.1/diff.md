# Comparing `tmp/lsnms-0.4.0.tar.gz` & `tmp/lsnms-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsnms-0.4.0.tar", max compression
+gzip compressed data, was "lsnms-0.4.1.tar", max compression
```

## Comparing `lsnms-0.4.0.tar` & `lsnms-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    10940 2023-07-16 16:25:36.000000 lsnms-0.4.0/README.md
--rw-r--r--   0        0        0       80 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/__init__.py
--rw-r--r--   0        0        0     7135 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/nms.py
--rw-r--r--   0        0        0    10147 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/rtree.py
--rw-r--r--   0        0        0    13403 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/util.py
--rw-r--r--   0        0        0     6255 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/wbc.py
--rw-r--r--   0        0        0      814 2023-07-16 16:53:36.000000 lsnms-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11738 1970-01-01 00:00:00.000000 lsnms-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10940 2023-07-16 16:25:36.000000 lsnms-0.4.1/README.md
+-rw-r--r--   0        0        0       80 2023-07-16 16:25:36.000000 lsnms-0.4.1/lsnms/__init__.py
+-rw-r--r--   0        0        0     7182 2023-07-31 20:51:49.000000 lsnms-0.4.1/lsnms/nms.py
+-rw-r--r--   0        0        0    10147 2023-07-16 16:25:36.000000 lsnms-0.4.1/lsnms/rtree.py
+-rw-r--r--   0        0        0    13403 2023-07-16 16:25:36.000000 lsnms-0.4.1/lsnms/util.py
+-rw-r--r--   0        0        0     6255 2023-07-16 16:25:36.000000 lsnms-0.4.1/lsnms/wbc.py
+-rw-r--r--   0        0        0      814 2023-07-31 21:04:10.000000 lsnms-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    11738 1970-01-01 00:00:00.000000 lsnms-0.4.1/PKG-INFO
```

### Comparing `lsnms-0.4.0/README.md` & `lsnms-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lsnms-0.4.0/lsnms/nms.py` & `lsnms-0.4.1/lsnms/nms.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     rtree.build()
 
     # Compute the areas once and for all: avoid recomputing it at each step
     areas = area(boxes)
 
     # Order by decreasing confidence
     order = np.argsort(scores)[::-1]
-    # Create a mask to keep track of boxes which have alread been visited
+    # Create a mask to keep track of boxes which have already been visited
     to_consider = np.full(len(boxes), True)
     for current_idx in order:
         # If already visited or discarded
         if not to_consider[current_idx]:
             continue
 
         # If score is already below threshold then break
@@ -67,15 +67,16 @@
             sc = overlap / (areas[current_idx] + areas[query_idx] - overlap)
             to_consider[query_idx] = sc < iou_threshold
 
         # Add the current box
         keep.append(current_idx)
         to_consider[current_idx] = False
 
-    return np.array(keep)
+    keep = np.array(keep)
+    return np.argwhere(score_mask)[:,0][keep]
 
 
 def nms(
     boxes: np.array,
     scores: np.array,
     iou_threshold: float = 0.5,
     score_threshold: float = 0.0,
```

### Comparing `lsnms-0.4.0/lsnms/rtree.py` & `lsnms-0.4.1/lsnms/rtree.py`

 * *Files identical despite different names*

### Comparing `lsnms-0.4.0/lsnms/util.py` & `lsnms-0.4.1/lsnms/util.py`

 * *Files identical despite different names*

### Comparing `lsnms-0.4.0/lsnms/wbc.py` & `lsnms-0.4.1/lsnms/wbc.py`

 * *Files identical despite different names*

### Comparing `lsnms-0.4.0/pyproject.toml` & `lsnms-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lsnms"
-version = "0.4.0"
+version = "0.4.1"
 description = "Large Scale Non Maximum Suppression"
 authors = ["Rémy Dubois <remydubois14@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/remydubois/lsnms"
 keywords = ["NMS", "Non Maximum Suppression", "Histology image", "Satellite images", "Object detection"]
 classifiers=["Programming Language :: Python :: 3", "Topic :: Scientific/Engineering"]
```

### Comparing `lsnms-0.4.0/PKG-INFO` & `lsnms-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsnms
-Version: 0.4.0
+Version: 0.4.1
 Summary: Large Scale Non Maximum Suppression
 Home-page: https://github.com/remydubois/lsnms
 License: MIT
 Keywords: NMS,Non Maximum Suppression,Histology image,Satellite images,Object detection
 Author: Rémy Dubois
 Author-email: remydubois14@gmail.com
 Requires-Python: >=3.8,<3.11
```

