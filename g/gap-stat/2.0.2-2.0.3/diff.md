# Comparing `tmp/gap-stat-2.0.2.tar.gz` & `tmp/gap-stat-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gap-stat-2.0.2.tar", last modified: Sat Jan 21 10:44:07 2023, max compression
+gzip compressed data, was "gap-stat-2.0.3.tar", last modified: Mon Jul 31 04:19:36 2023, max compression
```

## Comparing `gap-stat-2.0.2.tar` & `gap-stat-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-01-21 10:44:07.000000 gap-stat-2.0.2/
--rw-r--r--   0 milesg    (1000) milesg    (1000)      415 2023-01-21 10:41:59.000000 gap-stat-2.0.2/Cargo.toml
--rw-r--r--   0 milesg    (1000) milesg    (1000)     1081 2023-01-21 10:41:59.000000 gap-stat-2.0.2/LICENSE-MIT
--rw-r--r--   0 milesg    (1000) milesg    (1000)       43 2023-01-21 10:41:59.000000 gap-stat-2.0.2/MANIFEST.in
--rw-r--r--   0 milesg    (1000) milesg    (1000)     1218 2023-01-21 10:44:07.000000 gap-stat-2.0.2/PKG-INFO
--rw-r--r--   0 milesg    (1000) milesg    (1000)     6349 2023-01-21 10:41:59.000000 gap-stat-2.0.2/README.md
-drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-01-21 10:44:07.000000 gap-stat-2.0.2/gap_stat.egg-info/
--rw-r--r--   0 milesg    (1000) milesg    (1000)     1218 2023-01-21 10:44:07.000000 gap-stat-2.0.2/gap_stat.egg-info/PKG-INFO
--rw-r--r--   0 milesg    (1000) milesg    (1000)      391 2023-01-21 10:44:07.000000 gap-stat-2.0.2/gap_stat.egg-info/SOURCES.txt
--rw-r--r--   0 milesg    (1000) milesg    (1000)        1 2023-01-21 10:44:07.000000 gap-stat-2.0.2/gap_stat.egg-info/dependency_links.txt
--rw-r--r--   0 milesg    (1000) milesg    (1000)        1 2023-01-21 10:42:30.000000 gap-stat-2.0.2/gap_stat.egg-info/not-zip-safe
--rw-r--r--   0 milesg    (1000) milesg    (1000)       38 2023-01-21 10:44:07.000000 gap-stat-2.0.2/gap_stat.egg-info/requires.txt
--rw-r--r--   0 milesg    (1000) milesg    (1000)       14 2023-01-21 10:44:07.000000 gap-stat-2.0.2/gap_stat.egg-info/top_level.txt
-drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-01-21 10:44:07.000000 gap-stat-2.0.2/gap_statistic/
--rw-r--r--   0 milesg    (1000) milesg    (1000)       70 2023-01-21 10:41:59.000000 gap-stat-2.0.2/gap_statistic/__init__.py
--rw-r--r--   0 milesg    (1000) milesg    (1000)    15547 2023-01-21 10:41:59.000000 gap-stat-2.0.2/gap_statistic/optimalK.py
--rw-r--r--   0 milesg    (1000) milesg    (1000)       77 2023-01-21 10:41:59.000000 gap-stat-2.0.2/pyproject.toml
--rw-r--r--   0 milesg    (1000) milesg    (1000)       93 2023-01-21 10:44:07.000000 gap-stat-2.0.2/setup.cfg
--rw-r--r--   0 milesg    (1000) milesg    (1000)     1793 2023-01-21 10:41:59.000000 gap-stat-2.0.2/setup.py
-drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-01-21 10:44:07.000000 gap-stat-2.0.2/src/
-drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-01-21 10:44:07.000000 gap-stat-2.0.2/src/gap_statistic/
--rw-r--r--   0 milesg    (1000) milesg    (1000)     4767 2023-01-21 10:41:59.000000 gap-stat-2.0.2/src/gap_statistic/mod.rs
-drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-01-21 10:44:07.000000 gap-stat-2.0.2/src/kmeans/
--rw-r--r--   0 milesg    (1000) milesg    (1000)    10659 2023-01-21 10:41:59.000000 gap-stat-2.0.2/src/kmeans/mod.rs
--rw-r--r--   0 milesg    (1000) milesg    (1000)     1923 2023-01-21 10:41:59.000000 gap-stat-2.0.2/src/lib.rs
-drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-01-21 10:44:07.000000 gap-stat-2.0.2/src/tests/
--rw-r--r--   0 milesg    (1000) milesg    (1000)     6383 2023-01-21 10:41:59.000000 gap-stat-2.0.2/src/tests/mod.rs
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.659351 gap-stat-2.0.3/
+-rw-r--r--   0 milesg    (1000) milesg    (1000)      415 2023-01-21 10:41:59.000000 gap-stat-2.0.3/Cargo.toml
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     1081 2023-01-21 10:41:59.000000 gap-stat-2.0.3/LICENSE-MIT
+-rw-r--r--   0 milesg    (1000) milesg    (1000)       43 2023-01-21 10:41:59.000000 gap-stat-2.0.3/MANIFEST.in
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     1218 2023-07-31 04:19:36.659351 gap-stat-2.0.3/PKG-INFO
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     6349 2023-01-21 10:41:59.000000 gap-stat-2.0.3/README.md
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.658351 gap-stat-2.0.3/gap_stat.egg-info/
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     1218 2023-07-31 04:19:36.000000 gap-stat-2.0.3/gap_stat.egg-info/PKG-INFO
+-rw-r--r--   0 milesg    (1000) milesg    (1000)      439 2023-07-31 04:19:36.000000 gap-stat-2.0.3/gap_stat.egg-info/SOURCES.txt
+-rw-r--r--   0 milesg    (1000) milesg    (1000)        1 2023-07-31 04:19:36.000000 gap-stat-2.0.3/gap_stat.egg-info/dependency_links.txt
+-rw-r--r--   0 milesg    (1000) milesg    (1000)        1 2023-01-21 10:42:30.000000 gap-stat-2.0.3/gap_stat.egg-info/not-zip-safe
+-rw-r--r--   0 milesg    (1000) milesg    (1000)       38 2023-07-31 04:19:36.000000 gap-stat-2.0.3/gap_stat.egg-info/requires.txt
+-rw-r--r--   0 milesg    (1000) milesg    (1000)       14 2023-07-31 04:19:36.000000 gap-stat-2.0.3/gap_stat.egg-info/top_level.txt
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.659351 gap-stat-2.0.3/gap_statistic/
+-rw-r--r--   0 milesg    (1000) milesg    (1000)       70 2023-07-31 04:18:27.000000 gap-stat-2.0.3/gap_statistic/__init__.py
+-rw-r--r--   0 milesg    (1000) milesg    (1000)    15723 2023-07-31 04:18:27.000000 gap-stat-2.0.3/gap_statistic/optimalK.py
+-rw-r--r--   0 milesg    (1000) milesg    (1000)       77 2023-01-21 10:41:59.000000 gap-stat-2.0.3/pyproject.toml
+-rw-r--r--   0 milesg    (1000) milesg    (1000)       93 2023-07-31 04:19:36.659351 gap-stat-2.0.3/setup.cfg
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     1793 2023-07-31 04:18:27.000000 gap-stat-2.0.3/setup.py
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.659351 gap-stat-2.0.3/src/
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.659351 gap-stat-2.0.3/src/gap_statistic/
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     4767 2023-01-21 10:41:59.000000 gap-stat-2.0.3/src/gap_statistic/mod.rs
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.659351 gap-stat-2.0.3/src/kmeans/
+-rw-r--r--   0 milesg    (1000) milesg    (1000)    10659 2023-01-21 10:41:59.000000 gap-stat-2.0.3/src/kmeans/mod.rs
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     1923 2023-01-21 10:41:59.000000 gap-stat-2.0.3/src/lib.rs
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.659351 gap-stat-2.0.3/src/tests/
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     6383 2023-01-21 10:41:59.000000 gap-stat-2.0.3/src/tests/mod.rs
+drwxr-xr-x   0 milesg    (1000) milesg    (1000)        0 2023-07-31 04:19:36.659351 gap-stat-2.0.3/tests/
+-rw-r--r--   0 milesg    (1000) milesg    (1000)      682 2023-01-21 10:41:59.000000 gap-stat-2.0.3/tests/test_formatting.py
+-rw-r--r--   0 milesg    (1000) milesg    (1000)     4799 2023-01-21 10:41:59.000000 gap-stat-2.0.3/tests/test_optimalK.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gap-stat-2.0.2/LICENSE-MIT` & `gap-stat-2.0.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `gap-stat-2.0.2/PKG-INFO` & `gap-stat-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gap-stat
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python implementation of the gap statistic with optional Rust optimizations.
 Home-page: https://github.com/milesgranger/gap_statistic
 Author: Miles Granger
 Author-email: miles59923@gmail.com
 Maintainer: Miles Granger
 Maintainer-email: miles59923@gmail.com
 License: MIT
```

### Comparing `gap-stat-2.0.2/README.md` & `gap-stat-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gap-stat-2.0.2/gap_stat.egg-info/PKG-INFO` & `gap-stat-2.0.3/gap_stat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gap-stat
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python implementation of the gap statistic with optional Rust optimizations.
 Home-page: https://github.com/milesgranger/gap_statistic
 Author: Miles Granger
 Author-email: miles59923@gmail.com
 Maintainer: Miles Granger
 Maintainer-email: miles59923@gmail.com
 License: MIT
```

### Comparing `gap-stat-2.0.2/gap_statistic/optimalK.py` & `gap-stat-2.0.3/gap_statistic/optimalK.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,24 +50,26 @@
     def __init__(
         self,
         n_jobs: int = -1,
         parallel_backend: str = "joblib",
         clusterer: Callable = None,
         clusterer_kwargs: dict = None,
         n_iter: int = 10,
+        random_state: int = None
     ) -> None:
         """
         Construct OptimalK to use n_jobs (multiprocessing using joblib, multiprocessing, or single core.
         if parallel_backend == 'rust' it will use all cores.
 
         :param n_jobs:
         :param parallel_backend:
         :param clusterer:
         :param clusterer_kwargs:
         :param n_iter int: only valid for 'rust' backend, iterations for Kmeans
+        :param random_state int: initialize RNG used to create random reference set
         """
         if clusterer is not None and parallel_backend == "rust":
             raise ValueError(
                 "Cannot use 'rust' backend with a user defined clustering function, only KMeans"
                 " is supported on the rust implementation"
             )
         self.parallel_backend = (
@@ -80,14 +82,15 @@
         self.n_jobs = 1 if parallel_backend is None else self.n_jobs
         self.clusterer = clusterer if clusterer is not None else kmeans2
         self.clusterer_kwargs = (
             clusterer_kwargs or dict()
             if clusterer is not None
             else dict(iter=10, minit="points")
         )
+        self._rs = np.random.RandomState(seed=random_state)
 
     def __call__(
         self,
         X: Union[pd.DataFrame, np.ndarray],
         n_refs: int = 3,
         cluster_array: Iterable[int] = (),
     ):
@@ -256,27 +259,27 @@
         return disp
 
     def _calculate_gap(
         self, X: Union[pd.DataFrame, np.ndarray], n_refs: int, n_clusters: int
     ) -> GapCalcResult:
         """
         Calculate the gap value of the given data, n_refs, and number of clusters.
-        Return the resutling gap value and n_clusters
+        Return the resulting gap value and n_clusters
         """
         # Holder for reference dispersion results
         ref_dispersions = np.zeros(n_refs)
 
         # Compute the range of each feature
         X = np.asarray(X)
         a, b = X.min(axis=0, keepdims=True), X.max(axis=0, keepdims=True)
 
         # For n_references, generate random sample and perform kmeans getting resulting dispersion of each loop
         for i in range(n_refs):
             # Create new random reference set uniformly over the range of each feature
-            random_data = np.random.random_sample(size=X.shape) * (b - a) + a
+            random_data = self._rs.random_sample(size=X.shape) * (b - a) + a
 
             # Fit to it, getting the centroids and labels, and add to accumulated reference dispersions array.
             centroids, labels = self.clusterer(
                 random_data, n_clusters, **self.clusterer_kwargs
             )  # type: Tuple[np.ndarray, np.ndarray]
             dispersion = self._calculate_dispersion(
                 X=random_data, labels=labels, centroids=centroids
```

### Comparing `gap-stat-2.0.2/setup.py` & `gap-stat-2.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "scipy",
     "pandas",
 ]
 tests_require = ["scikit-learn>=0.24.0", "pytest", "joblib", "black", "click"]
 
 setup(
     name="gap-stat",
-    version="2.0.2",
+    version="2.0.3",
     author="Miles Granger",
     maintainer="Miles Granger",
     author_email="miles59923@gmail.com",
     maintainer_email="miles59923@gmail.com",
     keywords="kmeans unsupervised learning machine-learning clustering",
     description="Python implementation of the gap statistic with optional Rust optimizations.",
     long_description="Uses the gap statistic method by Tibshirani, Walther, Hastie to suggest n_clusters.",
```

### Comparing `gap-stat-2.0.2/src/gap_statistic/mod.rs` & `gap-stat-2.0.3/src/gap_statistic/mod.rs`

 * *Files identical despite different names*

### Comparing `gap-stat-2.0.2/src/kmeans/mod.rs` & `gap-stat-2.0.3/src/kmeans/mod.rs`

 * *Files identical despite different names*

### Comparing `gap-stat-2.0.2/src/lib.rs` & `gap-stat-2.0.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `gap-stat-2.0.2/src/tests/mod.rs` & `gap-stat-2.0.3/src/tests/mod.rs`

 * *Files identical despite different names*

