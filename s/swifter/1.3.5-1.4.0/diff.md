# Comparing `tmp/swifter-1.3.5.tar.gz` & `tmp/swifter-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swifter-1.3.5.tar", last modified: Tue Jun 13 03:04:35 2023, max compression
+gzip compressed data, was "swifter-1.4.0.tar", last modified: Mon Jul 31 18:46:24 2023, max compression
```

## Comparing `swifter-1.3.5.tar` & `swifter-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,53 @@
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.815509 swifter-1.3.5/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     1072 2021-06-25 15:03:32.000000 swifter-1.3.5/LICENSE
--rw-r--r--   0 jmcarpenter   (501) staff       (20)       56 2021-06-25 15:03:32.000000 swifter-1.3.5/MANIFEST.in
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      499 2023-06-13 03:04:35.815761 swifter-1.3.5/PKG-INFO
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     4813 2023-06-13 03:00:36.000000 swifter-1.3.5/README.md
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.808362 swifter-1.3.5/assets/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    25427 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_log10.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    21371 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_real.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    22263 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_text_log10.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    19696 2023-06-13 03:00:36.000000 swifter-1.3.5/assets/groupby_parallel_v_single_text_real.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    19922 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/modin_swifter_performance_benchmark_log10.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    17220 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/modin_swifter_performance_benchmark_real.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    22488 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/multiprocessing_v_single_log10.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    17977 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/multiprocessing_v_single_real.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    20448 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/vectorizes_when_possible_log10.png
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    18628 2021-06-25 15:03:32.000000 swifter-1.3.5/assets/vectorizes_when_possible_real.png
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.809083 swifter-1.3.5/docs/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    10684 2023-06-13 03:03:47.000000 swifter-1.3.5/docs/changelog.md
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     9651 2023-06-13 03:00:36.000000 swifter-1.3.5/docs/documentation.md
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.810269 swifter-1.3.5/examples/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    52404 2021-06-25 15:03:32.000000 swifter-1.3.5/examples/modin_dataframe_swifter_performance_benchmark.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    48413 2023-06-13 03:00:36.000000 swifter-1.3.5/examples/swifter_apply_examples.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)   348083 2023-06-13 03:00:36.000000 swifter-1.3.5/examples/swifter_speed_comparison.ipynb
--rw-r--r--   0 jmcarpenter   (501) staff       (20)       79 2023-06-13 03:04:35.816673 swifter-1.3.5/setup.cfg
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      931 2023-06-13 03:03:47.000000 swifter-1.3.5/setup.py
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.813217 swifter-1.3.5/swifter/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      600 2023-06-13 03:03:47.000000 swifter-1.3.5/swifter/__init__.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     1907 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/base.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     5915 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/parallel_accessor.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    33450 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/swifter.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)    48584 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/swifter_tests.py
--rw-r--r--   0 jmcarpenter   (501) staff       (20)     1160 2023-06-13 03:00:36.000000 swifter-1.3.5/swifter/tqdm_dask_progressbar.py
-drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-06-13 03:04:35.815127 swifter-1.3.5/swifter.egg-info/
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      499 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/PKG-INFO
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      974 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/SOURCES.txt
--rw-r--r--   0 jmcarpenter   (501) staff       (20)        1 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/dependency_links.txt
--rw-r--r--   0 jmcarpenter   (501) staff       (20)      150 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/requires.txt
--rw-r--r--   0 jmcarpenter   (501) staff       (20)        8 2023-06-13 03:04:35.000000 swifter-1.3.5/swifter.egg-info/top_level.txt
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-07-31 18:46:24.659478 swifter-1.4.0/
+-rw-------   0 jmcarpenter   (501) staff       (20)     1072 2018-08-21 19:54:00.000000 swifter-1.4.0/LICENSE
+-rw-------   0 jmcarpenter   (501) staff       (20)       56 2020-07-26 20:36:18.000000 swifter-1.4.0/MANIFEST.in
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      535 2023-07-31 18:46:24.659625 swifter-1.4.0/PKG-INFO
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     5007 2023-07-24 16:33:09.000000 swifter-1.4.0/README.md
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-07-31 18:46:24.598213 swifter-1.4.0/assets/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     8196 2023-07-21 16:22:34.000000 swifter-1.4.0/assets/.DS_Store
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    25427 2022-08-16 20:06:27.000000 swifter-1.4.0/assets/groupby_parallel_v_single_log10.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    21371 2022-08-16 20:06:27.000000 swifter-1.4.0/assets/groupby_parallel_v_single_real.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    22263 2022-07-24 04:45:29.000000 swifter-1.4.0/assets/groupby_parallel_v_single_text_log10.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    19696 2022-07-24 04:45:29.000000 swifter-1.4.0/assets/groupby_parallel_v_single_text_real.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)   128764 2023-07-21 15:36:12.000000 swifter-1.4.0/assets/groupby_parallel_vs_single_compatible.png
+-rw-------   0 jmcarpenter   (501) staff       (20)    19922 2020-09-19 23:37:53.000000 swifter-1.4.0/assets/modin_swifter_performance_benchmark_log10.png
+-rw-------   0 jmcarpenter   (501) staff       (20)    17220 2020-09-19 23:37:53.000000 swifter-1.4.0/assets/modin_swifter_performance_benchmark_real.png
+-rw-------   0 jmcarpenter   (501) staff       (20)    22488 2020-07-26 20:36:18.000000 swifter-1.4.0/assets/multiprocessing_v_single_log10.png
+-rw-------   0 jmcarpenter   (501) staff       (20)    17977 2020-07-26 20:36:18.000000 swifter-1.4.0/assets/multiprocessing_v_single_real.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)   127263 2023-07-21 15:36:06.000000 swifter-1.4.0/assets/multiprocessing_vs_single_compatible.png
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)   113382 2023-07-21 15:40:48.000000 swifter-1.4.0/assets/vectorizes_when_possible_compatible.png
+-rw-------   0 jmcarpenter   (501) staff       (20)    20448 2020-07-26 20:36:18.000000 swifter-1.4.0/assets/vectorizes_when_possible_log10.png
+-rw-------   0 jmcarpenter   (501) staff       (20)    18628 2020-07-26 20:36:18.000000 swifter-1.4.0/assets/vectorizes_when_possible_real.png
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-07-31 18:46:24.600760 swifter-1.4.0/docs/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    11152 2023-07-21 22:45:43.000000 swifter-1.4.0/docs/changelog.md
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     9651 2022-07-24 04:45:29.000000 swifter-1.4.0/docs/documentation.md
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-07-31 18:46:24.606813 swifter-1.4.0/examples/
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-07-31 18:46:24.621448 swifter-1.4.0/examples/.ipynb_checkpoints/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    11549 2022-07-28 20:00:33.000000 swifter-1.4.0/examples/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)       72 2022-04-12 17:18:09.000000 swifter-1.4.0/examples/.ipynb_checkpoints/bug-checkpoint.ipynb
+-rw-------   0 jmcarpenter   (501) staff       (20)    52404 2020-08-03 18:49:01.000000 swifter-1.4.0/examples/.ipynb_checkpoints/modin_performance_benchmark-checkpoint.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    15945 2022-07-28 21:40:32.000000 swifter-1.4.0/examples/.ipynb_checkpoints/quick_demo-checkpoint.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    48413 2022-07-24 03:42:55.000000 swifter-1.4.0/examples/.ipynb_checkpoints/swifter_apply_examples-checkpoint.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    49408 2022-07-23 00:16:46.000000 swifter-1.4.0/examples/.ipynb_checkpoints/swifter_groupby_example-checkpoint.ipynb
+-rw-------   0 jmcarpenter   (501) staff       (20)   230137 2020-08-03 19:50:22.000000 swifter-1.4.0/examples/.ipynb_checkpoints/swifter_speed_comparison-Copy1-checkpoint.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)   212635 2022-02-05 00:30:50.000000 swifter-1.4.0/examples/.ipynb_checkpoints/swifter_speed_comparison-checkpoint.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    19386 2023-07-20 16:33:19.000000 swifter-1.4.0/examples/Untitled.ipynb
+-rw-------   0 jmcarpenter   (501) staff       (20)    52404 2020-09-19 23:37:53.000000 swifter-1.4.0/examples/modin_dataframe_swifter_performance_benchmark.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    34584 2023-07-24 20:33:01.000000 swifter-1.4.0/examples/quick_demo.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    48413 2022-07-24 04:45:29.000000 swifter-1.4.0/examples/swifter_apply_examples.ipynb
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)   348083 2022-07-26 00:02:58.000000 swifter-1.4.0/examples/swifter_speed_comparison.ipynb
+-rw-------   0 jmcarpenter   (501) staff       (20)       79 2023-07-31 18:46:24.662166 swifter-1.4.0/setup.cfg
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      867 2023-07-24 16:33:20.000000 swifter-1.4.0/setup.py
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-07-31 18:46:24.647325 swifter-1.4.0/swifter/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      600 2023-07-21 15:42:35.000000 swifter-1.4.0/swifter/__init__.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     1907 2023-07-24 16:59:02.000000 swifter-1.4.0/swifter/base.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     5915 2022-07-07 00:19:34.000000 swifter-1.4.0/swifter/parallel_accessor.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    33496 2023-07-24 20:26:19.000000 swifter-1.4.0/swifter/swifter.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)    48584 2023-06-13 16:43:48.000000 swifter-1.4.0/swifter/swifter_tests.py
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     1160 2022-04-13 00:28:39.000000 swifter-1.4.0/swifter/tqdm_dask_progressbar.py
+drwxr-xr-x   0 jmcarpenter   (501) staff       (20)        0 2023-07-31 18:46:24.658796 swifter-1.4.0/swifter.egg-info/
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      535 2023-07-31 18:46:24.000000 swifter-1.4.0/swifter.egg-info/PKG-INFO
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)     1700 2023-07-31 18:46:24.000000 swifter-1.4.0/swifter.egg-info/SOURCES.txt
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)        1 2023-07-31 18:46:24.000000 swifter-1.4.0/swifter.egg-info/dependency_links.txt
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)      117 2023-07-31 18:46:24.000000 swifter-1.4.0/swifter.egg-info/requires.txt
+-rw-r--r--   0 jmcarpenter   (501) staff       (20)        8 2023-07-31 18:46:24.000000 swifter-1.4.0/swifter.egg-info/top_level.txt
```

### Comparing `swifter-1.3.5/LICENSE` & `swifter-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/README.md` & `swifter-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 
 Check out the [examples notebook](examples/swifter_apply_examples.ipynb), along with the [speed benchmark notebook](examples/swifter_speed_comparison.ipynb). The benchmarks are created using the library [perfplot](https://github.com/unutbu/perfplot).
 
 ## Installation:
 ```
 $ pip install -U pandas # upgrade pandas
 $ pip install swifter # first time installation
+$ pip install swifter[notebook] # first time installation including dependency for rich progress bar in jupyter notebooks
 $ pip install swifter[groupby] # first time installation including dependency for groupby.apply functionality
 
 $ pip install -U swifter # upgrade to latest version if already installed
+$ pip install -U swifter[notebook] # upgrade to latest version to include dependency for rich progress bar in jupyter notebooks
 $ pip install -U swifter[groupby] # upgrade to latest version to include dependency for groupby.apply functionality
 ```
 
 alternatively, to install on [Anaconda](https://anaconda.org/conda-forge/swifter):
 ```
 conda install -c conda-forge swifter  # Install swifter
 conda install -c conda-forge swifter>=1.3.2 ray>=1.0.0  # Install swifter with dependency for groupby.apply
@@ -64,24 +66,23 @@
 # use swifter apply on specific columns
 df['outCol'] = df[['inCol1', 'inCol2']].swifter.apply(my_func)
 df['outCol'] = df[['inCol1', 'inCol2', 'inCol3']].swifter.apply(my_func,
              positional_arg, keyword_arg=keyword_argval)
 ```
 
 ## Vectorizes your function, when possible
-![Alt text](/assets/vectorizes_when_possible_real.png?raw=true)
-![Alt text](/assets/vectorizes_when_possible_log10.png?raw=true)
+![Alt text](/assets/vectorizes_when_possible_compatible.png?raw=true)
 
 ## When vectorization is not possible, automatically decides which is faster: to use dask parallel processing or a simple pandas apply
-![Alt text](/assets/multiprocessing_v_single_real.png?raw=true)
-![Alt text](/assets/multiprocessing_v_single_log10.png?raw=true)
+![Alt text](/assets/multiprocessing_vs_single_compatible.png?raw=true)
 
 ## Highly performant, even for groupby applies
-![Alt text](/assets/groupby_parallel_v_single_real.png?raw=true)
-![Alt text](/assets/groupby_parallel_v_single_log10.png?raw=true)
+![Alt text](/assets/groupby_parallel_vs_single_compatible.png?raw=true)
+
+See the [speed benchmark notebook](examples/swifter_speed_comparison.ipynb) for source of the above performance plots.
 
 ## Notes
 1. The function is documented in the .py file. In Jupyter Notebooks, you can see the docs by pressing Shift+Tab(x3). Also, check out the complete documentation [here](docs/documentation.md) along with the [changelog](docs/changelog.md).
 
 2. Please upgrade your version of pandas, as the pandas extension api used in this module is a recent addition to pandas.
 
 3. Import modin before importing swifter, if you wish to use modin with swifter. Otherwise, use `swifter.register_modin()` to access it.
```

### Comparing `swifter-1.3.5/assets/groupby_parallel_v_single_log10.png` & `swifter-1.4.0/assets/groupby_parallel_v_single_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/groupby_parallel_v_single_real.png` & `swifter-1.4.0/assets/groupby_parallel_v_single_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/groupby_parallel_v_single_text_log10.png` & `swifter-1.4.0/assets/groupby_parallel_v_single_text_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/groupby_parallel_v_single_text_real.png` & `swifter-1.4.0/assets/groupby_parallel_v_single_text_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/modin_swifter_performance_benchmark_log10.png` & `swifter-1.4.0/assets/modin_swifter_performance_benchmark_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/modin_swifter_performance_benchmark_real.png` & `swifter-1.4.0/assets/modin_swifter_performance_benchmark_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/multiprocessing_v_single_log10.png` & `swifter-1.4.0/assets/multiprocessing_v_single_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/multiprocessing_v_single_real.png` & `swifter-1.4.0/assets/multiprocessing_v_single_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/vectorizes_when_possible_log10.png` & `swifter-1.4.0/assets/vectorizes_when_possible_log10.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/assets/vectorizes_when_possible_real.png` & `swifter-1.4.0/assets/vectorizes_when_possible_real.png`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/docs/changelog.md` & `swifter-1.4.0/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## Version 1.4.0 -- 2023-07-21
+* Significantly reduced core dependencies of swifter library. See https://github.com/jmcarpenter2/swifter/issues/219 for discussion
+  - Big shout out to @PeterJCLaw for starting this discussion and contributions from @xquyvu as well
+* Removed deprecated `loffset` parameter
+  - Thanks to @bnavigator for identifying this bug
+* Updated README to be more readable for darkmode users
+  - Thank you to @MemphisMeng for identifying this gap
+
 ## Version 1.3.5 -- 2023-06-12
 * Add secondary fallback for series applies
 * Code refactoring for simplicity
 
 ## Version 1.3.4 -- 2022-08-16
 * Enable indexing after a groupby, e.g. `df.swifter.groupby(by)[key].apply(func)`
 * Improve groupby apply progress bar
```

### Comparing `swifter-1.3.5/docs/documentation.md` & `swifter-1.4.0/docs/documentation.md`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/examples/modin_dataframe_swifter_performance_benchmark.ipynb` & `swifter-1.4.0/examples/.ipynb_checkpoints/modin_performance_benchmark-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/examples/swifter_apply_examples.ipynb` & `swifter-1.4.0/examples/.ipynb_checkpoints/swifter_apply_examples-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/examples/swifter_speed_comparison.ipynb` & `swifter-1.4.0/examples/swifter_speed_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/setup.py` & `swifter-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from setuptools import setup
 
 setup(
     name="swifter",
     packages=["swifter"],  # this must be the same as the name above
-    version="1.3.5",
+    version="1.4.0",
     description="A package which efficiently applies any function to a pandas dataframe or series in the fastest available manner",
     author="Jason Carpenter",
     author_email="jcarpenter@manifold.ai",
     url="https://github.com/jmcarpenter2/swifter",  # use the URL to the github repo
-    download_url=f"https://github.com/jmcarpenter2/swifter/archive/1.3.5.tar.gz",
+    download_url="https://github.com/jmcarpenter2/swifter/archive/1.4.0.tar.gz",
     keywords=["pandas", "dask", "apply", "function", "parallelize", "vectorize"],
     install_requires=[
         "pandas>=1.0.0",
         "psutil>=5.6.6",
         "dask[dataframe]>=2.10.0",
         "tqdm>=4.33.0",
-        "ipywidgets>=7.0.0",
-        "cloudpickle>=0.2.2",
-        "parso>0.4.0",
-        "bleach>=3.1.1",
     ],
     extras_require={
-        "groupby": ["ray>=1.0.0"]
+        "groupby": ["ray>=1.0.0"],
+        "notebook": ["ipywidgets>=7.0.0"],
     },
     classifiers=[],
 )
```

### Comparing `swifter-1.3.5/swifter/__init__.py` & `swifter-1.4.0/swifter/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     "set_defaults",
     "SeriesAccessor",
     "DataFrameAccessor",
     "register_parallel_dataframe_accessor",
     "register_parallel_series_accessor",
     "register_modin",
 ]
-__version__ = "1.3.5"
+__version__ = "1.4.0"
```

### Comparing `swifter-1.3.5/swifter/base.py` & `swifter-1.4.0/swifter/base.py`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/swifter/parallel_accessor.py` & `swifter-1.4.0/swifter/parallel_accessor.py`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/swifter/swifter.py` & `swifter-1.4.0/swifter/swifter.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,23 +192,24 @@
         kwds = {
             "rule": rule,
             "axis": axis,
             "closed": closed,
             "label": label,
             "convention": convention,
             "kind": kind,
-            "loffset": loffset,
             "base": base,
             "on": on,
             "level": level,
             "origin": origin,
             "offset": offset,
         }
         if not base:
             kwds.pop("base")
+        if loffset is not None:
+            kwds.update({"loffset": loffset})
 
         return Resampler(
             self._obj,
             npartitions=self._npartitions,
             dask_threshold=self._dask_threshold,
             scheduler=self._scheduler,
             progress_bar=self._progress_bar,
```

### Comparing `swifter-1.3.5/swifter/swifter_tests.py` & `swifter-1.4.0/swifter/swifter_tests.py`

 * *Files identical despite different names*

### Comparing `swifter-1.3.5/swifter/tqdm_dask_progressbar.py` & `swifter-1.4.0/swifter/tqdm_dask_progressbar.py`

 * *Files identical despite different names*

