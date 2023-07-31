# Comparing `tmp/graphreduce-1.5.4.tar.gz` & `tmp/graphreduce-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.5.4.tar", last modified: Sun Jul 30 14:41:17 2023, max compression
+gzip compressed data, was "graphreduce-1.5.5.tar", last modified: Mon Jul 31 13:22:19 2023, max compression
```

## Comparing `graphreduce-1.5.4.tar` & `graphreduce-1.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-30 14:41:17.452883 graphreduce-1.5.4/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-30 14:41:17.452756 graphreduce-1.5.4/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5.4/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-30 14:41:17.452000 graphreduce-1.5.4/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5.4/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-26 01:15:17.000000 graphreduce-1.5.4/graphreduce/context.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-07-26 01:15:32.000000 graphreduce-1.5.4/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    16681 2023-07-29 18:41:49.000000 graphreduce-1.5.4/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15431 2023-07-26 12:48:40.000000 graphreduce-1.5.4/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-30 14:41:17.452600 graphreduce-1.5.4/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5.4/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      124 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-30 14:41:17.000000 graphreduce-1.5.4/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-30 14:41:17.452919 graphreduce-1.5.4/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1824 2023-07-30 14:40:55.000000 graphreduce-1.5.4/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-31 13:22:19.118687 graphreduce-1.5.5/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-31 13:22:19.118558 graphreduce-1.5.5/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.5.5/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-31 13:22:19.117793 graphreduce-1.5.5/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.5.5/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      868 2023-07-26 01:15:17.000000 graphreduce-1.5.5/graphreduce/context.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-07-26 01:15:32.000000 graphreduce-1.5.5/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    16748 2023-07-31 13:21:03.000000 graphreduce-1.5.5/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15434 2023-07-31 13:21:40.000000 graphreduce-1.5.5/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-31 13:22:19.118378 graphreduce-1.5.5/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7927 2023-07-31 13:22:19.000000 graphreduce-1.5.5/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-31 13:22:19.000000 graphreduce-1.5.5/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-31 13:22:19.000000 graphreduce-1.5.5/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.5.5/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      124 2023-07-31 13:22:19.000000 graphreduce-1.5.5/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-31 13:22:19.000000 graphreduce-1.5.5/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-31 13:22:19.118724 graphreduce-1.5.5/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1824 2023-07-31 13:21:52.000000 graphreduce-1.5.5/setup.py
```

### Comparing `graphreduce-1.5.4/PKG-INFO` & `graphreduce-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5.4
+Version: 1.5.5
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5.4/README.md` & `graphreduce-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5.4/graphreduce/context.py` & `graphreduce-1.5.5/graphreduce/context.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.5.4/graphreduce/graph_reduce.py` & `graphreduce-1.5.5/graphreduce/graph_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         logger.info("checking for prefix uniqueness")
         self.prefix_uniqueness()
     
         for node in self.nodes():
             logger.info(f"running filters, clip cols, and annotations for {node.__class__.__name__}")
             node.do_annotate()
-            node.do_filter()
+            node.do_filters()
             node.do_transpose()
 
         logger.info(f"depth-first traversal through the graph from source: {self.parent_node.__class__.__name__}")
         for edge in self.depth_first_generator():
             parent_node = edge[0]
             relation_node = edge[1]
             edge_data = self.get_edge_data(parent_node, relation_node)
@@ -437,8 +437,9 @@
                         relation_df=label_df
                     )
                     parent_node.df = joined_with_labels
 
             # post-join annotations (if any)
             parent_node.do_post_join_annotate()
             # post-join filters (if any)
-            parent_node.do_post_join_filter()
+            if hasattr(parent_node, 'do_post_join_filters'):
+                parent_node.do_post_join_filters()
```

### Comparing `graphreduce-1.5.4/graphreduce/node.py` & `graphreduce-1.5.5/graphreduce/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             pass
 
         elif self.compute_layer.value == 'redshift':
             pass
 
 
     @abc.abstractmethod
-    def do_filter (
+    def do_filters (
         self
     ):
         """
 do some filters on the data
         """
         pass
     
@@ -178,15 +178,15 @@
 
 
     @abc.abstractmethod
     def do_clip_cols(self):
         pass
 
 
-    def do_post_join_filter(self):
+    def do_post_join_filters(self):
         """
 Filter operations that require some
 additional relational data to perform.
         """
         pass
 
 
@@ -433,15 +433,15 @@
 
     def do_post_join_annotate(self):
         pass
 
     def do_clip_cols(self):
         pass
 
-    def do_post_join_filter(self):
+    def do_post_join_filters(self):
         pass
 
     def do_reduce(self):
         pass
 
     def do_labels(self):
         pass
```

### Comparing `graphreduce-1.5.4/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.5.5/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.5.4
+Version: 1.5.5
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.5.4/setup.py` & `graphreduce-1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = "1.5.4",
+        version = "1.5.5",
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask",
             "networkx>=2.6.3",
             "pandas>=1.3.4",
```

