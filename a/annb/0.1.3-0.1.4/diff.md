# Comparing `tmp/annb-0.1.3.tar.gz` & `tmp/annb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annb-0.1.3.tar", last modified: Wed Jul 26 03:46:13 2023, max compression
+gzip compressed data, was "annb-0.1.4.tar", last modified: Mon Jul 31 02:06:21 2023, max compression
```

## Comparing `annb-0.1.3.tar` & `annb-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.727983 annb-0.1.3/
--rw-r--r--   0 jibin      (501) staff       (20)    11357 2023-06-23 11:24:40.000000 annb-0.1.3/LICENSE
--rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:46:13.728068 annb-0.1.3/PKG-INFO
--rw-r--r--   0 jibin      (501) staff       (20)      297 2023-07-25 03:49:16.000000 annb-0.1.3/README.md
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.724796 annb-0.1.3/annb/
--rw-r--r--   0 jibin      (501) staff       (20)      385 2023-07-26 03:45:48.000000 annb-0.1.3/annb/__init__.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.722423 annb-0.1.3/annb/anns/
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.726479 annb-0.1.3/annb/anns/faiss/
--rw-r--r--   0 jibin      (501) staff       (20)      489 2023-06-23 14:28:30.000000 annb-0.1.3/annb/anns/faiss/deploy.py
--rw-r--r--   0 jibin      (501) staff       (20)     3595 2023-07-26 03:41:08.000000 annb-0.1.3/annb/anns/faiss/indexes.py
--rw-r--r--   0 jibin      (501) staff       (20)     9433 2023-07-26 03:45:30.000000 annb-0.1.3/annb/cli.py
--rw-r--r--   0 jibin      (501) staff       (20)     1853 2023-07-25 03:08:09.000000 annb-0.1.3/annb/config.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.727729 annb-0.1.3/annb/dataset/
--rw-r--r--   0 jibin      (501) staff       (20)      213 2023-07-25 03:44:19.000000 annb-0.1.3/annb/dataset/__init__.py
--rw-r--r--   0 jibin      (501) staff       (20)     1267 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/base_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     6734 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/hdf5_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     1946 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/random_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     2416 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/utils.py
--rw-r--r--   0 jibin      (501) staff       (20)       75 2023-06-23 13:33:53.000000 annb-0.1.3/annb/envs.py
--rw-r--r--   0 jibin      (501) staff       (20)     7996 2023-07-26 03:37:36.000000 annb-0.1.3/annb/indexes.py
--rw-r--r--   0 jibin      (501) staff       (20)     1431 2023-07-25 03:07:57.000000 annb-0.1.3/annb/plot.py
--rw-r--r--   0 jibin      (501) staff       (20)     6405 2023-07-25 03:08:09.000000 annb-0.1.3/annb/result.py
--rw-r--r--   0 jibin      (501) staff       (20)     7718 2023-07-25 03:07:57.000000 annb-0.1.3/annb/runner.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.726091 annb-0.1.3/annb.egg-info/
--rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/PKG-INFO
--rw-r--r--   0 jibin      (501) staff       (20)      517 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/SOURCES.txt
--rw-r--r--   0 jibin      (501) staff       (20)        1 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/dependency_links.txt
--rw-r--r--   0 jibin      (501) staff       (20)       84 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/entry_points.txt
--rw-r--r--   0 jibin      (501) staff       (20)       49 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/requires.txt
--rw-r--r--   0 jibin      (501) staff       (20)        5 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/top_level.txt
--rw-r--r--   0 jibin      (501) staff       (20)       99 2023-07-25 03:07:57.000000 annb-0.1.3/pyproject.toml
--rw-r--r--   0 jibin      (501) staff       (20)      668 2023-07-26 03:46:13.728399 annb-0.1.3/setup.cfg
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-31 02:06:21.638687 annb-0.1.4/
+-rw-r--r--   0 jibin      (501) staff       (20)    11357 2023-06-23 11:24:40.000000 annb-0.1.4/LICENSE
+-rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-31 02:06:21.638755 annb-0.1.4/PKG-INFO
+-rw-r--r--   0 jibin      (501) staff       (20)      297 2023-07-25 03:49:16.000000 annb-0.1.4/README.md
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-31 02:06:21.636260 annb-0.1.4/annb/
+-rw-r--r--   0 jibin      (501) staff       (20)      385 2023-07-31 02:05:23.000000 annb-0.1.4/annb/__init__.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-31 02:06:21.633898 annb-0.1.4/annb/anns/
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-31 02:06:21.637390 annb-0.1.4/annb/anns/faiss/
+-rw-r--r--   0 jibin      (501) staff       (20)      489 2023-06-23 14:28:30.000000 annb-0.1.4/annb/anns/faiss/deploy.py
+-rw-r--r--   0 jibin      (501) staff       (20)     3538 2023-07-31 02:05:23.000000 annb-0.1.4/annb/anns/faiss/indexes.py
+-rw-r--r--   0 jibin      (501) staff       (20)     9797 2023-07-31 02:05:23.000000 annb-0.1.4/annb/cli.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1853 2023-07-25 03:08:09.000000 annb-0.1.4/annb/config.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-31 02:06:21.638475 annb-0.1.4/annb/dataset/
+-rw-r--r--   0 jibin      (501) staff       (20)      213 2023-07-25 03:44:19.000000 annb-0.1.4/annb/dataset/__init__.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1267 2023-07-25 03:08:09.000000 annb-0.1.4/annb/dataset/base_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     6734 2023-07-25 03:08:09.000000 annb-0.1.4/annb/dataset/hdf5_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1946 2023-07-25 03:08:09.000000 annb-0.1.4/annb/dataset/random_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     2416 2023-07-25 03:08:09.000000 annb-0.1.4/annb/dataset/utils.py
+-rw-r--r--   0 jibin      (501) staff       (20)       75 2023-06-23 13:33:53.000000 annb-0.1.4/annb/envs.py
+-rw-r--r--   0 jibin      (501) staff       (20)     7996 2023-07-26 03:37:36.000000 annb-0.1.4/annb/indexes.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1431 2023-07-25 03:07:57.000000 annb-0.1.4/annb/plot.py
+-rw-r--r--   0 jibin      (501) staff       (20)     6405 2023-07-25 03:08:09.000000 annb-0.1.4/annb/result.py
+-rw-r--r--   0 jibin      (501) staff       (20)     7668 2023-07-31 02:05:23.000000 annb-0.1.4/annb/runner.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-31 02:06:21.637042 annb-0.1.4/annb.egg-info/
+-rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-31 02:06:21.000000 annb-0.1.4/annb.egg-info/PKG-INFO
+-rw-r--r--   0 jibin      (501) staff       (20)      517 2023-07-31 02:06:21.000000 annb-0.1.4/annb.egg-info/SOURCES.txt
+-rw-r--r--   0 jibin      (501) staff       (20)        1 2023-07-31 02:06:21.000000 annb-0.1.4/annb.egg-info/dependency_links.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       84 2023-07-31 02:06:21.000000 annb-0.1.4/annb.egg-info/entry_points.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       49 2023-07-31 02:06:21.000000 annb-0.1.4/annb.egg-info/requires.txt
+-rw-r--r--   0 jibin      (501) staff       (20)        5 2023-07-31 02:06:21.000000 annb-0.1.4/annb.egg-info/top_level.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       99 2023-07-25 03:07:57.000000 annb-0.1.4/pyproject.toml
+-rw-r--r--   0 jibin      (501) staff       (20)      668 2023-07-31 02:06:21.639033 annb-0.1.4/setup.cfg
```

### Comparing `annb-0.1.3/LICENSE` & `annb-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/PKG-INFO` & `annb-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annb
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple ANN benchmark tools
 Home-page: https://github.com/matrixji/annb
 Author: Ji Bin
 Author-email: matrixji@live.com
 License: Apache-2.0
 Keywords: ANN benchmark,Test tools
 Requires-Python: >=3.6
```

### Comparing `annb-0.1.3/annb/anns/faiss/indexes.py` & `annb-0.1.4/annb/anns/faiss/indexes.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,30 +47,30 @@
                 quantizer,
                 self.dimension,
                 self.kwargs.get("nlist", 128),
                 faiss.ScalarQuantizer.QT_8bit,
             )
         else:
             index = faiss.index_factory(self.dimension, index_string, faiss_metric)
-        if (
-            using_gpu
-            and hasattr(faiss, "index_cpu_to_gpu")
-            and hasattr(faiss, "StandardGpuResources")
-        ):
+
+        self.log.debug(
+            "use cpu index, use gpu: %s, faiss has gpu support: %s",
+            using_gpu,
+            self.support_gpu(),
+        )
+        if using_gpu and self.support_gpu():
             self.log.debug("copy index to gpu")
-            index = faiss.index_cpu_to_gpu(faiss.StandardGpuResources(), 0, index)
-        else:
-            self.log.debug(
-                "use cpu index, gpu: %s, faiss has gpu support: %s",
-                using_gpu,
-                hasattr(faiss, "index_cpu_to_gpu")
-                and hasattr(faiss, "StandardGpuResources"),
-            )
+            res = faiss.StandardGpuResources()
+            index = faiss.index_cpu_to_gpu(res, 0, index)
         return index
 
+    @classmethod
+    def support_gpu(cls) -> bool:
+        return hasattr(faiss, "get_num_gpus") and faiss.get_num_gpus() > 0
+
     def train(self, data: np.ndarray) -> None:
         return self.index.train(data)
 
     def add(self, data: np.ndarray) -> None:
         return self.index.add(data)
 
     def warmup(self) -> None:
@@ -80,15 +80,15 @@
             self.search(random_data, 10)
 
     def search(self, query: np.ndarray, k: int) -> Tuple[List[float], List[int]]:
         return self.index.search(query, k)
 
     def update_search_args(self, **kwargs):
         if "nprobe" in kwargs:
-            self.index.nprobe = kwargs["nprobe"]
+            self.index.nprobe = int(kwargs["nprobe"])
 
     def cleanup(self) -> None:
         self.index.reset()
 
 
 class FaissIndexUnderTestFactory(IndexUnderTestFactory):
     def create(
```

### Comparing `annb-0.1.3/annb/cli.py` & `annb-0.1.4/annb/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from argparse import ArgumentParser
 from typing import Union
 from logging import getLogger, Formatter, StreamHandler, FileHandler
 from sys import stdout
+from tempfile import gettempdir
+from os import path
 
 from .dataset.hdf5_dataset import AnnbHdf5Dataset
 from .dataset.random_dataset import RandomDataset
 from .indexes import IndexUnderTestFactory
 from .plot import plot_result_recall_vs_qps
 from .result import BenchmarkResult
 from .runner import Runner
@@ -37,22 +39,21 @@
     >>> load_dict('a=1,b=2')
     {'a': 1, 'b': 2}
     """
     s = s.strip()
     data = {}
     for x in s.split(','):
         k, v = x.split('=')
-        try:
-            v = int(v)
-        except ValueError:
-            v = str(v)
-        try:
-            v = float(v)
-        except ValueError:
-            v = str(v)
+        possible_types = [int, float, str]
+        for t in possible_types:
+            try:
+                v = t(v)
+                break
+            except ValueError:
+                pass
         data[k] = v
     return data
 
 
 def load_index_factory(index_factory, index_factory_args) -> IndexUnderTestFactory:
     """
     >>> load_index_factory('annb.anns.faiss.indexes.index_under_test_factory')
@@ -63,28 +64,29 @@
         module = __import__(module_name, fromlist=[class_name])
         return getattr(module, class_name)(**index_factory_args)
     except Exception as e:
         logger.error('Load index factory failed', e)
         exit(1)
 
 
-def create_or_load_dataset(dataset_file: str, dimension: int, metric_type: str):
+def create_or_load_dataset(dataset_file: str, dimension: int, metric_type: str, count: int):
     """
     >>> create_or_load_dataset('sift-128-euclidean.hdf5', 128, 'euclidean')
     <annb.dataset.hdf5_dataset.AnnbHdf5Dataset object at 0x7f6b3d0b9e10>
     """
     if dataset_file:
         try:
             dataset = AnnbHdf5Dataset(dataset_file)
         except Exception as e:
             logger.error('Load dataset failed', e)
             exit(1)
     else:
-        temp_file = f'.random_d{dimension}_{metric_type}.hdf5'
-        dataset = RandomDataset(temp_file, dimension=dimension, metric=metric_type)
+
+        temp_file = path.join(gettempdir(), f'.annb_random_d{dimension}_{metric_type}_{count}.hdf5')
+        dataset = RandomDataset(temp_file, dimension=dimension, metric=metric_type, count=count)
     logger.info(
         'use dataset: %s, dim: %d, metric: %s',
         dataset,
         dataset.dimension,
         dataset.metric_type,
     )
     return dataset, dataset.dimension, dataset.metric_type
@@ -101,18 +103,19 @@
     query_args,
     dataset,
     result,
     topk,
     jobs,
     loop,
     step,
+    count,
 ):
     factory = load_index_factory(index_factory, index_factory_args)
     dataset, index_dim, index_metric_type = create_or_load_dataset(
-        dataset, index_dim, index_metric_type
+        dataset, index_dim, index_metric_type, count
     )
     index = factory.create(index_name, index_dim, index_metric_type, **index_args)
     logger.info(
         'use index: %s, dim: %d, metric: %s, %s',
         index,
         index.dimension,
         index.metric_type,
@@ -149,14 +152,15 @@
             run['query_args'],
             run['dataset'],
             run['result'],
             run['topk'],
             run['jobs'],
             run['loop'],
             run['step'],
+            run.get('count', 1000),
         )
 
 
 def report_plain(inputs, output):
     output_file = stdout
     if output:
         output_file = open(output, 'w')
@@ -300,14 +304,20 @@
         '--dataset',
         default='',
         help='Dataset file, if not set will generate random dataset',
     )
     parser.add_argument(
         '--result', default='', help='Result file, if not set will print to stdout'
     )
+    parser.add_argument(
+        '--count',
+        default=1000,
+        type=int,
+        help='Count, only used when generate random dataset',
+    )
 
     opts = parser.parse_args()
     init_logger(opts.log_level, opts.log_file)
     logger.debug('run with options: %s', opts)
     if opts.run_file:
         run_file(opts.run_file)
     else:
@@ -322,12 +332,13 @@
             opts.query_args,
             opts.dataset,
             opts.result,
             opts.topk,
             opts.jobs,
             opts.loop,
             opts.step,
+            opts.count,
         )
 
 
 if __name__ == '__main__':
     test_main()
```

### Comparing `annb-0.1.3/annb/config.py` & `annb-0.1.4/annb/config.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/dataset/base_dataset.py` & `annb-0.1.4/annb/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/dataset/hdf5_dataset.py` & `annb-0.1.4/annb/dataset/hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/dataset/random_dataset.py` & `annb-0.1.4/annb/dataset/random_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/dataset/utils.py` & `annb-0.1.4/annb/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/indexes.py` & `annb-0.1.4/annb/indexes.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/plot.py` & `annb-0.1.4/annb/plot.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/result.py` & `annb-0.1.4/annb/result.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/annb/runner.py` & `annb-0.1.4/annb/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from queue import Empty
 import sys
 from collections import namedtuple
 from logging import getLogger
 from time import monotonic_ns
-from multiprocessing import Process, Queue
+from multiprocessing.dummy import Process, Queue
 from typing import List, Dict
 from datetime import datetime
 
 import numpy as np
 
 from .indexes import IndexUnderTest
 from .dataset import BaseDataset
@@ -116,17 +116,15 @@
         correct_count = 0
         total_count = 0
         ground_truth_neighbors = self.dataset.ground_truth_neighbors[:, : self.topk]
 
         # calc recall between ground_truth_neighbors and labels
         for i, (gt, test_items) in enumerate(zip(ground_truth_neighbors, labels)):
             total_count += len(gt)
-            for test_item in test_items:
-                if test_item in gt:
-                    correct_count += 1
+            correct_count += len(set(gt) & set(test_items))
         recall = correct_count / total_count
         self.log.info('recall %.6f(%d/%d)', recall, correct_count, total_count)
         self.benchmark_result.add_query_result(
             recall=recall, durations=durations, query_arg=query_arg
         )
 
     def find_best_loop(self):
```

### Comparing `annb-0.1.3/annb.egg-info/PKG-INFO` & `annb-0.1.4/annb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annb
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple ANN benchmark tools
 Home-page: https://github.com/matrixji/annb
 Author: Ji Bin
 Author-email: matrixji@live.com
 License: Apache-2.0
 Keywords: ANN benchmark,Test tools
 Requires-Python: >=3.6
```

### Comparing `annb-0.1.3/annb.egg-info/SOURCES.txt` & `annb-0.1.4/annb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annb-0.1.3/setup.cfg` & `annb-0.1.4/setup.cfg`

 * *Files identical despite different names*

