# Comparing `tmp/KKMeans-0.0.3.tar.gz` & `tmp/KKMeans-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KKMeans-0.0.3.tar", last modified: Mon Jul 31 11:18:17 2023, max compression
+gzip compressed data, was "KKMeans-0.0.4.tar", last modified: Mon Jul 31 11:50:01 2023, max compression
```

## Comparing `KKMeans-0.0.3.tar` & `KKMeans-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.817079 KKMeans-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.787474 KKMeans-0.0.3/KKMeans.egg-info/
--rw-rw-rw-   0        0        0      607 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      607 2023-07-31 11:18:17.817079 KKMeans-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-30 20:10:21.000000 KKMeans-0.0.3/README.md
--rw-rw-rw-   0        0        0      565 2023-07-31 11:17:57.000000 KKMeans-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 11:18:17.818152 KKMeans-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1637 2023-07-31 11:16:17.000000 KKMeans-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.770835 KKMeans-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.816078 KKMeans-0.0.3/src/KKMeans/
--rw-rw-rw-   0        0        0   904324 2023-07-29 08:22:59.000000 KKMeans-0.0.3/src/KKMeans/KKMeans.c
--rw-rw-rw-   0        0        0    27766 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/KKMeans.py
--rw-rw-rw-   0        0        0       43 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/__init__.py
--rw-rw-rw-   0        0        0  1170842 2023-07-31 11:18:16.000000 KKMeans-0.0.3/src/KKMeans/elkan.c
--rw-rw-rw-   0        0        0     9984 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/elkan.pyx
--rw-rw-rw-   0        0        0  1182482 2023-07-31 11:18:16.000000 KKMeans-0.0.3/src/KKMeans/kernels.c
--rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/kernels.pyx
--rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.3/src/KKMeans/lloyd.c
--rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/lloyd.pyx
--rw-rw-rw-   0        0        0  1020999 2023-07-29 08:23:01.000000 KKMeans-0.0.3/src/KKMeans/quality.c
--rw-rw-rw-   0        0        0     2757 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/quality.pyx
--rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.3/src/KKMeans/utils.c
--rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.987842 KKMeans-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.963330 KKMeans-0.0.4/KKMeans.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      634 2023-07-31 11:50:01.987332 KKMeans-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-07-30 20:10:21.000000 KKMeans-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.4/license.txt
+-rw-rw-rw-   0        0        0      565 2023-07-31 11:49:38.000000 KKMeans-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:50:01.987842 KKMeans-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1684 2023-07-31 11:49:30.000000 KKMeans-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.946003 KKMeans-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.986307 KKMeans-0.0.4/src/KKMeans/
+-rw-rw-rw-   0        0        0   875796 2023-07-31 11:49:59.000000 KKMeans-0.0.4/src/KKMeans/KKMeans.c
+-rw-rw-rw-   0        0        0    27233 2023-07-31 11:36:19.000000 KKMeans-0.0.4/src/KKMeans/KKMeans.py
+-rw-rw-rw-   0        0        0       43 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/__init__.py
+-rw-rw-rw-   0        0        0  1170842 2023-07-31 11:50:00.000000 KKMeans-0.0.4/src/KKMeans/elkan.c
+-rw-rw-rw-   0        0        0     9984 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/elkan.pyx
+-rw-rw-rw-   0        0        0  1182482 2023-07-31 11:50:01.000000 KKMeans-0.0.4/src/KKMeans/kernels.c
+-rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/kernels.pyx
+-rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.4/src/KKMeans/lloyd.c
+-rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/lloyd.pyx
+-rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.4/src/KKMeans/quality.c
+-rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.4/src/KKMeans/quality.pyx
+-rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.4/src/KKMeans/utils.c
+-rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/utils.pyx
```

### Comparing `KKMeans-0.0.3/KKMeans.egg-info/PKG-INFO` & `KKMeans-0.0.4/KKMeans.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: KKMeans
-Version: 0.0.3
+Version: 0.0.4
 Summary: https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy
 Author-email: Paul Theis <keymailt7@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: license.txt
 
 This is the github repository for my bachelor thesis.<br>
 <br>
 pip install . <br>
 works for windows11 and ubuntu 22 <br>
 if package is installed as UNKOWN upgrade pip and setuptools <br>
```

### Comparing `KKMeans-0.0.3/KKMeans.egg-info/SOURCES.txt` & `KKMeans-0.0.4/KKMeans.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+license.txt
 pyproject.toml
 setup.py
 KKMeans.egg-info/PKG-INFO
 KKMeans.egg-info/SOURCES.txt
 KKMeans.egg-info/dependency_links.txt
 KKMeans.egg-info/requires.txt
 KKMeans.egg-info/top_level.txt
```

### Comparing `KKMeans-0.0.3/PKG-INFO` & `KKMeans-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: KKMeans
-Version: 0.0.3
+Version: 0.0.4
 Summary: https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy
 Author-email: Paul Theis <keymailt7@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: license.txt
 
 This is the github repository for my bachelor thesis.<br>
 <br>
 pip install . <br>
 works for windows11 and ubuntu 22 <br>
 if package is installed as UNKOWN upgrade pip and setuptools <br>
```

### Comparing `KKMeans-0.0.3/pyproject.toml` & `KKMeans-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=63", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "KKMeans"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Paul Theis", email="keymailt7@gmail.com" },
 ]
 dependencies = ["numpy>=1.25"]
 description = "https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `KKMeans-0.0.3/setup.py` & `KKMeans-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,8 +31,14 @@
 # https://stackoverflow.com/questions/73766918/creating-python-package-which-uses-cython-valueerror
 package_data = {
     "KKMeans" : ["utils.pyx", "lloyd.pyx", "elkan.pyx", "kernels.pyx", "quality.pyx", "KKMeans.py"]
 }
 
 # variables set here (except ext_modules) and not in Pyproject.toml as setuptool-specifics is still in beta
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
-setup(ext_modules=cythonize(extensions, compiler_directives=compiler_directives),package_dir={"KKMeans":"src/KKMeans"}, package_data=package_data, include_package_data=True)
+setup(
+    name="KKMeans",
+    ext_modules=cythonize(extensions, compiler_directives=compiler_directives),
+    package_dir={"KKMeans":"src/KKMeans"}, 
+    package_data=package_data, 
+    include_package_data=True
+)
```

### Comparing `KKMeans-0.0.3/src/KKMeans/KKMeans.c` & `KKMeans-0.0.4/src/KKMeans/KKMeans.c`

 * *Files 1% similar despite different names*

```diff
@@ -1803,31 +1803,14 @@
     ((likely(PyLong_CheckExact(x))) ?\
          (likely(__Pyx_PyLong_IsNonNeg(x)) ? (Py_INCREF(x), (x)) : __Pyx_PyLong_AbsNeg(x)) :\
          PyNumber_Absolute(x))
 #else
 #define __Pyx_PyNumber_Absolute(x)  PyNumber_Absolute(x)
 #endif
 
-/* ListCompAppend.proto */
-#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
-static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
-    PyListObject* L = (PyListObject*) list;
-    Py_ssize_t len = Py_SIZE(list);
-    if (likely(L->allocated > len)) {
-        Py_INCREF(x);
-        PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
-        return 0;
-    }
-    return PyList_Append(list, x);
-}
-#else
-#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
-#endif
-
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
 #if PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
@@ -2089,42 +2072,35 @@
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_all;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_T[] = "T";
 static const char __pyx_k_X[] = "X_";
 static const char __pyx_k_Y[] = "Y";
-static const char __pyx_k_c[] = "c";
 static const char __pyx_k_p[] = "p";
-static const char __pyx_k_x[] = "x";
-static const char __pyx_k_3d[] = "3d";
-static const char __pyx_k_ax[] = "ax";
 static const char __pyx_k_it[] = "it";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_X_2[] = "X";
 static const char __pyx_k__16[] = ":";
-static const char __pyx_k__27[] = "*";
-static const char __pyx_k__28[] = ".";
-static const char __pyx_k__77[] = "?";
+static const char __pyx_k__23[] = "*";
+static const char __pyx_k__24[] = ".";
+static const char __pyx_k__71[] = "?";
 static const char __pyx_k_all[] = "all";
 static const char __pyx_k_doc[] = "__doc__";
-static const char __pyx_k_fig[] = "fig";
 static const char __pyx_k_fit[] = "fit";
 static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_low[] = "low";
-static const char __pyx_k_plt[] = "plt";
 static const char __pyx_k_rbf[] = "rbf";
 static const char __pyx_k_rng[] = "rng";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_tol[] = "tol";
 static const char __pyx_k_Best[] = "Best ";
 static const char __pyx_k_NINF[] = "NINF";
 static const char __pyx_k_amin[] = "amin";
 static const char __pyx_k_axis[] = "axis";
-static const char __pyx_k_data[] = "data";
 static const char __pyx_k_diag[] = "diag";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_high[] = "high";
 static const char __pyx_k_init[] = "init";
 static const char __pyx_k_iter[] = "__iter__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -2149,39 +2125,36 @@
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_argmax[] = "argmax";
 static const char __pyx_k_argmin[] = "argmin";
 static const char __pyx_k_center[] = "center";
 static const char __pyx_k_choice[] = "choice";
 static const char __pyx_k_double[] = "double";
-static const char __pyx_k_figure[] = "figure";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_init_2[] = "__init__";
 static const char __pyx_k_iter_2[] = "iter";
 static const char __pyx_k_kernel[] = "kernel";
 static const char __pyx_k_kmeans[] = "kmeans++";
 static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_labels[] = "labels_";
 static const char __pyx_k_linear[] = "linear";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_n_init[] = "n_init";
-static const char __pyx_k_pyplot[] = "pyplot";
 static const char __pyx_k_random[] = "random";
 static const char __pyx_k_KKMeans[] = "KKMeans";
 static const char __pyx_k_asarray[] = "asarray";
 static const char __pyx_k_centers[] = "centers";
 static const char __pyx_k_cluster[] = "cluster";
 static const char __pyx_k_inertia[] = "inertia";
 static const char __pyx_k_isclose[] = "isclose";
 static const char __pyx_k_ndarray[] = "ndarray";
 static const char __pyx_k_predict[] = "predict";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_quality[] = "quality_";
 static const char __pyx_k_reshape[] = "reshape";
-static const char __pyx_k_scatter[] = "scatter";
 static const char __pyx_k_verbose[] = "verbose";
 static const char __pyx_k_gaussian[] = "gaussian";
 static const char __pyx_k_integers[] = "integers";
 static const char __pyx_k_kmeanspp[] = "kmeanspp";
 static const char __pyx_k_l_bounds[] = "l_bounds";
 static const char __pyx_k_labels_2[] = "labels";
 static const char __pyx_k_max_iter[] = "max_iter";
@@ -2199,23 +2172,20 @@
 static const char __pyx_k_outer_sum[] = "outer_sum";
 static const char __pyx_k_quality_2[] = "quality";
 static const char __pyx_k_sizes_old[] = "sizes_old";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_X_is_empty[] = "X is empty";
 static const char __pyx_k_inner_sums[] = "inner_sums_";
 static const char __pyx_k_labels_old[] = "labels_old";
-static const char __pyx_k_matplotlib[] = "matplotlib";
 static const char __pyx_k_n_clusters[] = "n_clusters";
 static const char __pyx_k_out_finish[] = "_out_finish";
 static const char __pyx_k_polynomial[] = "polynomial";
-static const char __pyx_k_projection[] = "projection";
 static const char __pyx_k_silhouette[] = "silhouette";
 static const char __pyx_k_truerandom[] = "truerandom";
 static const char __pyx_k_KKMeans_fit[] = "KKMeans.fit";
-static const char __pyx_k_add_subplot[] = "add_subplot";
 static const char __pyx_k_default_rng[] = "default_rng";
 static const char __pyx_k_init_labels[] = "_init_labels";
 static const char __pyx_k_out_verbose[] = "_out_verbose";
 static const char __pyx_k_quality_old[] = "quality_old";
 static const char __pyx_k_sizes_store[] = "sizes_store";
 static const char __pyx_k_start_dists[] = "start_dists";
 static const char __pyx_k_start_elkan[] = "start_elkan";
@@ -2240,15 +2210,14 @@
 static const char __pyx_k_get_best_init[] = "_get_best_init";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
 static const char __pyx_k_kernel_matrix[] = "kernel_matrix";
 static const char __pyx_k_min_dist_each[] = "min_dist_each";
 static const char __pyx_k_quality_store[] = "quality_store";
 static const char __pyx_k_validate_data[] = "_validate_data";
 static const char __pyx_k_validate_init[] = "__validate_init";
-static const char __pyx_k_visualize_kkm[] = "visualize_kkm";
 static const char __pyx_k_KKMeans___init[] = "KKMeans.__init__";
 static const char __pyx_k_avg_silhouette[] = "avg_silhouette";
 static const char __pyx_k_kernel_wrapper[] = "kernel_wrapper";
 static const char __pyx_k_KKMeans_kernels[] = "KKMeans.kernels";
 static const char __pyx_k_KKMeans_predict[] = "KKMeans.predict";
 static const char __pyx_k_KKMeans_quality[] = "KKMeans.quality";
 static const char __pyx_k_X_center_kernel[] = "X_center_kernel";
@@ -2323,15 +2292,14 @@
 static const char __pyx_k_Kernel_K_Means_Clustering_Read[] = "\n    Kernel K-Means Clustering.\n\n    Read more in the thesis. TODO\n    Designed to mimic sklearn.cluster.KMeans\n    limitations: kernel matrix\n\n    Parameters \n    ----------\n\n    n_clusters: int, default=8\n        The number of clusters to form.\n\n    init: {kmeans++, random, truerandom} or arraylike of shape(n_clusters, n_features), default = kmeans++\n        Initialization method. \n        kmeans++: heuristic to choose \"good\" starting centers\n            For more, see: thesis or\n            Arthur and Vassilvitskii, Kmeans++ the \n            advantage of carefull seeding, 2007\n        random: Randomly takes existing datapoints as centers\n        truerandom: assigns random labels to each datapoint\n    \n        If arraylike is passed, init is cast to ndarray of\n        doubles and its content is used as centers.\n\n    n_init: int, default=3 \n        The number of clusterings computed. As KKMeans is \n        a heuristic that converges to local optima, \n        mutliple runs are beneficial. \n    \n    max_iter: int, default=300\n        Maximal amount of iterations for each run.\n    \n    tol: float, default = 0.0001    \n        Max difference of quality-metric between iterations\n        to declare run for converged.\n        If 0., run converges only when labels do not change\n        or max_iter is reached.\n    \n    q_metrics: {inertia, silhouette}, default=inertia\n        Quality metric by which each clustering is measured.\n\n        inertia:  also called variance, sum of squared distances \n            from each point to its assigned center. Objective function in \n            (Kernel) K-means. \n\n        silhouette: Measures how \"ambiguous\" the assignment of a point\n            to its cluster is; if the loss function would not change\n            if it were assigned to the next best cluster, the silhouette \n            of said point would be 0.\n            -1 <= silhouette <= 1\n            For elkan, this does not work ""as elkan does not calculate\n            the distance to every cluster centers.\n            calculated via:\n            a(x) = d(x, centers[x])\n            b(x) = min_y(d(x, centers[y])) where y != x\n            silhouette(x) = (b(x) - a(x))/max{a(x), b(x)}\n            This is then averaged for every point.  \n    \n    verbose: bool, default=False\n    \n    rng: int, default=None\n        Seed which will be passed to np.random.defaul_rng\n        to create random generator.\n        When none, \"fresh, unpredictable entropy will be pulled from the OS\"\n            - np random generator docpage.\n    \n    algorithm: {\"lloyd\", \"elkan\"}, default=\"lloyd\"\n        The algorithm which will be used for commputation.\n        lloyd is the standard heuristic used to solve the k-means   \n        problem. This is a simplified version of Elkan's algorithm\n        that does not need to calculate pairwise cluster distances.\n        The original elkan (wiht pw cluster distances) is slower\n        than lloyd's when utilizing a kernel matrix.\n\n    kernel: {\"linear\", \"rbf\", \"polynomial\", \"sigmoid\", \"gaussian\", \"laplacian\"}, default=\"linear\"\n        Which kernel shall be used to compute the kernel matrix.\n        Gaussian is equal to rbf with gamma = variance**-2\n        Linear calculates a regular kmeans clustering.\n\n    **kwargs: \n        Arguments which are passed to the kernel function.\n        Dependant on kernel used\n\n    Attributes\n    ----------\n\n    labels_: ndarray of shape (n_samples)\n        labels of each point\n    \n    inner_sums_: ndarray of shape (n_clusters)\n        Mathematical term used for prediction, stored\n        to avoid recomputing/storing full kernel matrix.\n        =SUM(K(x, x')) -> for each x, x' in cluster C\n            -> for each cluster C\n    \n    cluster_sizes_: ndarray of shape(n_clusters)\n        amount of points in each clusters\n    \n    X_: ndarray of shape(n_samples, n_features)\n        T""he data which was passed to be clustered.\n\n    quality_: float\n        Quality measured by the passed q_metric.\n        If tol=0 only gets measured at the end of a \"run\".\n\n    ";
 static const char __pyx_k_Quality_metric_not_implemented[] = "Quality metric not implemented";
 static const char __pyx_k_algorithm_not_implemented_this[] = " algorithm not implemented;                                  this should have been caught in _check_params";
 static const char __pyx_k_quality_metric_not_implemented[] = " quality metric not implemented";
 static const char __pyx_k_Amount_of_given_centers_must_be[] = "Amount of given centers must be equal to n_clusters";
 static const char __pyx_k_Warning_tol_0_passed_tol_set_to[] = "Warning! tol < 0 passed, tol set to 0";
 static const char __pyx_k_metric_not_implemented_this_sho[] = " metric not implemented;                 this should have been caught in _validate_params";
-static const char __pyx_k_Dimensionality_is_too_high_for_v[] = "Dimensionality is too high for visualization";
 static const char __pyx_k_Given_centers_need_to_be_2_d_arr[] = "Given centers need to be 2-d array";
 static const char __pyx_k_Initialisation_method_not_implem[] = "Initialisation method not implemented";
 static const char __pyx_k_KKMeans__build_starting_distance[] = "KKMeans._build_starting_distance";
 static const char __pyx_k_WARNING_using_silhouette_with_el[] = "WARNING: using silhouette with elkan will most likely be inaccurate                  as elkan does not calculate exact distances to every center";
 static const char __pyx_k_sample_cluster_ratio_needs_to_be[] = "sample:cluster ratio needs to be at least one";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_7KKMeans_7KKMeans___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_n_clusters, PyObject *__pyx_v_init, PyObject *__pyx_v_n_init, PyObject *__pyx_v_max_iter, PyObject *__pyx_v_tol, PyObject *__pyx_v_q_metric, PyObject *__pyx_v_verbose, PyObject *__pyx_v_rng, PyObject *__pyx_v_algorithm, PyObject *__pyx_v_kernel, PyObject *__pyx_v_kwargs); /* proto */
@@ -2357,15 +2325,14 @@
 static PyObject *__pyx_pf_7KKMeans_7KKMeans_40_measure_iter(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_sq_distances, PyObject *__pyx_v_labels, PyObject *__pyx_v_labels_old, PyObject *__pyx_v_quality); /* proto */
 static PyObject *__pyx_pf_7KKMeans_7KKMeans_42calc_q_metric(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_sq_distances, PyObject *__pyx_v_labels); /* proto */
 static PyObject *__pyx_pf_7KKMeans_7KKMeans_44calc_silhouette(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_sq_distances, PyObject *__pyx_v_labels); /* proto */
 static PyObject *__pyx_pf_7KKMeans_7KKMeans_46_build_starting_distance(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kernel_matrix); /* proto */
 static PyObject *__pyx_pf_7KKMeans_7KKMeans_48elkan(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_kernel_matrix, PyObject *__pyx_v_labels); /* proto */
 static PyObject *__pyx_pf_7KKMeans_7KKMeans_50kmeanspp(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_X, PyObject *__pyx_v_kernel_matrix); /* proto */
 static PyObject *__pyx_pf_7KKMeans_7KKMeans_52predict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_X); /* proto */
-static PyObject *__pyx_pf_7KKMeans_visualize_kkm(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_labels); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
@@ -2387,19 +2354,17 @@
   PyTypeObject *__pyx_CoroutineAwaitType;
   #endif
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
-  PyObject *__pyx_kp_u_3d;
   PyObject *__pyx_kp_u_Amount_of_given_centers_must_be;
   PyObject *__pyx_kp_u_Best;
   PyObject *__pyx_kp_u_Converged_at_iteration;
-  PyObject *__pyx_kp_u_Dimensionality_is_too_high_for_v;
   PyObject *__pyx_kp_u_Found_at_init;
   PyObject *__pyx_kp_u_Given_centers_are_empty;
   PyObject *__pyx_kp_u_Given_centers_need_to_be_2_d_arr;
   PyObject *__pyx_kp_u_Initialisation_method_not_implem;
   PyObject *__pyx_kp_u_Invalid_kernel_provided;
   PyObject *__pyx_kp_u_Iteration;
   PyObject *__pyx_n_s_KKMeans;
@@ -2456,61 +2421,55 @@
   PyObject *__pyx_n_s_X;
   PyObject *__pyx_n_s_X_2;
   PyObject *__pyx_n_s_X_center_kernel;
   PyObject *__pyx_kp_u_X_is_empty;
   PyObject *__pyx_kp_u_X_needs_to_be_2_d_Array;
   PyObject *__pyx_n_s_Y;
   PyObject *__pyx_kp_u__16;
-  PyObject *__pyx_n_s__27;
-  PyObject *__pyx_kp_u__28;
-  PyObject *__pyx_n_s__77;
-  PyObject *__pyx_n_s_add_subplot;
+  PyObject *__pyx_n_s__23;
+  PyObject *__pyx_kp_u__24;
+  PyObject *__pyx_n_s__71;
   PyObject *__pyx_n_s_algorithm;
   PyObject *__pyx_kp_u_algorithm_not_implemented_this;
   PyObject *__pyx_n_s_all;
   PyObject *__pyx_n_s_amin;
   PyObject *__pyx_n_s_argmax;
   PyObject *__pyx_n_s_argmin;
   PyObject *__pyx_n_s_array;
   PyObject *__pyx_n_s_asarray;
   PyObject *__pyx_n_s_ascontiguousarray;
   PyObject *__pyx_n_s_assign_to_centers;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_avg_silhouette;
-  PyObject *__pyx_n_s_ax;
   PyObject *__pyx_n_s_axis;
   PyObject *__pyx_n_s_best_init;
   PyObject *__pyx_n_s_build_kernel_matrix;
   PyObject *__pyx_n_s_build_starting_distance;
-  PyObject *__pyx_n_s_c;
   PyObject *__pyx_n_s_calc_q_metric;
   PyObject *__pyx_n_s_calc_silhouette;
   PyObject *__pyx_n_s_calc_sq_distances;
   PyObject *__pyx_n_s_center;
   PyObject *__pyx_n_s_center_dists;
   PyObject *__pyx_n_s_centers;
   PyObject *__pyx_n_s_choice;
   PyObject *__pyx_n_s_class_getitem;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_cluster;
   PyObject *__pyx_n_s_cluster_sizes;
   PyObject *__pyx_n_s_cluster_sizes_2;
   PyObject *__pyx_n_s_converged;
-  PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_default_rng;
   PyObject *__pyx_n_s_diag;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dists_to_centers;
   PyObject *__pyx_n_s_doc;
   PyObject *__pyx_n_s_double;
   PyObject *__pyx_n_s_dtype;
   PyObject *__pyx_n_s_elkan;
   PyObject *__pyx_n_u_elkan;
-  PyObject *__pyx_n_s_fig;
-  PyObject *__pyx_n_s_figure;
   PyObject *__pyx_n_s_fill_empty_clusters;
   PyObject *__pyx_n_s_fit;
   PyObject *__pyx_n_u_gaussian;
   PyObject *__pyx_n_s_get_best_init;
   PyObject *__pyx_n_s_high;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_index;
@@ -2545,15 +2504,14 @@
   PyObject *__pyx_n_s_labels_store;
   PyObject *__pyx_n_u_laplacian;
   PyObject *__pyx_n_u_linear;
   PyObject *__pyx_n_s_lloyd;
   PyObject *__pyx_n_u_lloyd;
   PyObject *__pyx_n_s_low;
   PyObject *__pyx_n_s_main;
-  PyObject *__pyx_n_s_matplotlib;
   PyObject *__pyx_n_s_max_iter;
   PyObject *__pyx_kp_u_max_iter_must_be_1;
   PyObject *__pyx_kp_u_max_iter_must_be_int;
   PyObject *__pyx_n_s_measure_iter;
   PyObject *__pyx_n_s_metaclass;
   PyObject *__pyx_kp_u_metric_not_implemented_this_sho;
   PyObject *__pyx_n_s_min_dist_each;
@@ -2571,37 +2529,33 @@
   PyObject *__pyx_kp_u_not_implemented;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_numpy;
   PyObject *__pyx_n_s_out_finish;
   PyObject *__pyx_n_s_out_verbose;
   PyObject *__pyx_n_s_outer_sum;
   PyObject *__pyx_n_s_p;
-  PyObject *__pyx_n_s_plt;
   PyObject *__pyx_n_u_polynomial;
   PyObject *__pyx_n_s_predict;
   PyObject *__pyx_n_s_prepare;
   PyObject *__pyx_n_s_print;
   PyObject *__pyx_n_s_probs;
-  PyObject *__pyx_n_s_projection;
-  PyObject *__pyx_n_s_pyplot;
   PyObject *__pyx_n_s_q_metric;
   PyObject *__pyx_n_s_quality;
   PyObject *__pyx_n_s_quality_2;
   PyObject *__pyx_kp_u_quality_metric_not_implemented;
   PyObject *__pyx_n_s_quality_old;
   PyObject *__pyx_n_s_quality_store;
   PyObject *__pyx_n_s_qualname;
   PyObject *__pyx_n_s_random;
   PyObject *__pyx_n_u_random;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_u_rbf;
   PyObject *__pyx_n_s_reshape;
   PyObject *__pyx_n_s_rng;
   PyObject *__pyx_kp_u_sample_cluster_ratio_needs_to_be;
-  PyObject *__pyx_n_s_scatter;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_n_s_set_name;
   PyObject *__pyx_n_s_shape;
   PyObject *__pyx_n_u_silhouette;
   PyObject *__pyx_kp_u_silhouette_inertia;
   PyObject *__pyx_n_s_size;
   PyObject *__pyx_n_s_sizes;
@@ -2630,16 +2584,14 @@
   PyObject *__pyx_n_s_validate_max_iter;
   PyObject *__pyx_n_s_validate_n_clusters;
   PyObject *__pyx_n_s_validate_n_init;
   PyObject *__pyx_n_s_validate_params;
   PyObject *__pyx_n_s_validate_q_metric;
   PyObject *__pyx_n_s_validate_tol;
   PyObject *__pyx_n_s_verbose;
-  PyObject *__pyx_n_s_visualize_kkm;
-  PyObject *__pyx_n_s_x;
   PyObject *__pyx_n_s_zeros;
   PyObject *__pyx_float_1eneg_4;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_2;
   PyObject *__pyx_int_3;
   PyObject *__pyx_int_8;
@@ -2662,66 +2614,60 @@
   PyObject *__pyx_tuple__14;
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__18;
   PyObject *__pyx_tuple__19;
   PyObject *__pyx_tuple__20;
   PyObject *__pyx_tuple__22;
-  PyObject *__pyx_tuple__23;
-  PyObject *__pyx_tuple__24;
   PyObject *__pyx_tuple__25;
-  PyObject *__pyx_tuple__26;
-  PyObject *__pyx_tuple__29;
-  PyObject *__pyx_tuple__31;
-  PyObject *__pyx_tuple__32;
-  PyObject *__pyx_tuple__43;
-  PyObject *__pyx_tuple__45;
+  PyObject *__pyx_tuple__27;
+  PyObject *__pyx_tuple__28;
+  PyObject *__pyx_tuple__39;
+  PyObject *__pyx_tuple__41;
+  PyObject *__pyx_tuple__42;
+  PyObject *__pyx_tuple__44;
   PyObject *__pyx_tuple__46;
   PyObject *__pyx_tuple__48;
   PyObject *__pyx_tuple__50;
   PyObject *__pyx_tuple__52;
   PyObject *__pyx_tuple__54;
   PyObject *__pyx_tuple__56;
   PyObject *__pyx_tuple__58;
   PyObject *__pyx_tuple__60;
-  PyObject *__pyx_tuple__62;
-  PyObject *__pyx_tuple__64;
+  PyObject *__pyx_tuple__63;
+  PyObject *__pyx_tuple__65;
   PyObject *__pyx_tuple__67;
   PyObject *__pyx_tuple__69;
-  PyObject *__pyx_tuple__71;
-  PyObject *__pyx_tuple__73;
-  PyObject *__pyx_tuple__75;
+  PyObject *__pyx_codeobj__26;
+  PyObject *__pyx_codeobj__29;
   PyObject *__pyx_codeobj__30;
+  PyObject *__pyx_codeobj__31;
+  PyObject *__pyx_codeobj__32;
   PyObject *__pyx_codeobj__33;
   PyObject *__pyx_codeobj__34;
   PyObject *__pyx_codeobj__35;
   PyObject *__pyx_codeobj__36;
   PyObject *__pyx_codeobj__37;
   PyObject *__pyx_codeobj__38;
-  PyObject *__pyx_codeobj__39;
   PyObject *__pyx_codeobj__40;
-  PyObject *__pyx_codeobj__41;
-  PyObject *__pyx_codeobj__42;
-  PyObject *__pyx_codeobj__44;
+  PyObject *__pyx_codeobj__43;
+  PyObject *__pyx_codeobj__45;
   PyObject *__pyx_codeobj__47;
   PyObject *__pyx_codeobj__49;
   PyObject *__pyx_codeobj__51;
   PyObject *__pyx_codeobj__53;
   PyObject *__pyx_codeobj__55;
   PyObject *__pyx_codeobj__57;
   PyObject *__pyx_codeobj__59;
   PyObject *__pyx_codeobj__61;
-  PyObject *__pyx_codeobj__63;
-  PyObject *__pyx_codeobj__65;
+  PyObject *__pyx_codeobj__62;
+  PyObject *__pyx_codeobj__64;
   PyObject *__pyx_codeobj__66;
   PyObject *__pyx_codeobj__68;
   PyObject *__pyx_codeobj__70;
-  PyObject *__pyx_codeobj__72;
-  PyObject *__pyx_codeobj__74;
-  PyObject *__pyx_codeobj__76;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2756,19 +2702,17 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_CLEAR(clear_module_state->__pyx_kp_u_3d);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Amount_of_given_centers_must_be);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Best);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Converged_at_iteration);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Dimensionality_is_too_high_for_v);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Found_at_init);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Given_centers_are_empty);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Given_centers_need_to_be_2_d_arr);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Initialisation_method_not_implem);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_kernel_provided);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Iteration);
   Py_CLEAR(clear_module_state->__pyx_n_s_KKMeans);
@@ -2825,61 +2769,55 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_X);
   Py_CLEAR(clear_module_state->__pyx_n_s_X_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_X_center_kernel);
   Py_CLEAR(clear_module_state->__pyx_kp_u_X_is_empty);
   Py_CLEAR(clear_module_state->__pyx_kp_u_X_needs_to_be_2_d_Array);
   Py_CLEAR(clear_module_state->__pyx_n_s_Y);
   Py_CLEAR(clear_module_state->__pyx_kp_u__16);
-  Py_CLEAR(clear_module_state->__pyx_n_s__27);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__28);
-  Py_CLEAR(clear_module_state->__pyx_n_s__77);
-  Py_CLEAR(clear_module_state->__pyx_n_s_add_subplot);
+  Py_CLEAR(clear_module_state->__pyx_n_s__23);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__24);
+  Py_CLEAR(clear_module_state->__pyx_n_s__71);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithm);
   Py_CLEAR(clear_module_state->__pyx_kp_u_algorithm_not_implemented_this);
   Py_CLEAR(clear_module_state->__pyx_n_s_all);
   Py_CLEAR(clear_module_state->__pyx_n_s_amin);
   Py_CLEAR(clear_module_state->__pyx_n_s_argmax);
   Py_CLEAR(clear_module_state->__pyx_n_s_argmin);
   Py_CLEAR(clear_module_state->__pyx_n_s_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_asarray);
   Py_CLEAR(clear_module_state->__pyx_n_s_ascontiguousarray);
   Py_CLEAR(clear_module_state->__pyx_n_s_assign_to_centers);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_avg_silhouette);
-  Py_CLEAR(clear_module_state->__pyx_n_s_ax);
   Py_CLEAR(clear_module_state->__pyx_n_s_axis);
   Py_CLEAR(clear_module_state->__pyx_n_s_best_init);
   Py_CLEAR(clear_module_state->__pyx_n_s_build_kernel_matrix);
   Py_CLEAR(clear_module_state->__pyx_n_s_build_starting_distance);
-  Py_CLEAR(clear_module_state->__pyx_n_s_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_q_metric);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_silhouette);
   Py_CLEAR(clear_module_state->__pyx_n_s_calc_sq_distances);
   Py_CLEAR(clear_module_state->__pyx_n_s_center);
   Py_CLEAR(clear_module_state->__pyx_n_s_center_dists);
   Py_CLEAR(clear_module_state->__pyx_n_s_centers);
   Py_CLEAR(clear_module_state->__pyx_n_s_choice);
   Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_cluster);
   Py_CLEAR(clear_module_state->__pyx_n_s_cluster_sizes);
   Py_CLEAR(clear_module_state->__pyx_n_s_cluster_sizes_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_converged);
-  Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_default_rng);
   Py_CLEAR(clear_module_state->__pyx_n_s_diag);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dists_to_centers);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
   Py_CLEAR(clear_module_state->__pyx_n_s_double);
   Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
   Py_CLEAR(clear_module_state->__pyx_n_s_elkan);
   Py_CLEAR(clear_module_state->__pyx_n_u_elkan);
-  Py_CLEAR(clear_module_state->__pyx_n_s_fig);
-  Py_CLEAR(clear_module_state->__pyx_n_s_figure);
   Py_CLEAR(clear_module_state->__pyx_n_s_fill_empty_clusters);
   Py_CLEAR(clear_module_state->__pyx_n_s_fit);
   Py_CLEAR(clear_module_state->__pyx_n_u_gaussian);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_best_init);
   Py_CLEAR(clear_module_state->__pyx_n_s_high);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
@@ -2914,15 +2852,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_labels_store);
   Py_CLEAR(clear_module_state->__pyx_n_u_laplacian);
   Py_CLEAR(clear_module_state->__pyx_n_u_linear);
   Py_CLEAR(clear_module_state->__pyx_n_s_lloyd);
   Py_CLEAR(clear_module_state->__pyx_n_u_lloyd);
   Py_CLEAR(clear_module_state->__pyx_n_s_low);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
-  Py_CLEAR(clear_module_state->__pyx_n_s_matplotlib);
   Py_CLEAR(clear_module_state->__pyx_n_s_max_iter);
   Py_CLEAR(clear_module_state->__pyx_kp_u_max_iter_must_be_1);
   Py_CLEAR(clear_module_state->__pyx_kp_u_max_iter_must_be_int);
   Py_CLEAR(clear_module_state->__pyx_n_s_measure_iter);
   Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
   Py_CLEAR(clear_module_state->__pyx_kp_u_metric_not_implemented_this_sho);
   Py_CLEAR(clear_module_state->__pyx_n_s_min_dist_each);
@@ -2940,37 +2877,33 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_not_implemented);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
   Py_CLEAR(clear_module_state->__pyx_n_s_out_finish);
   Py_CLEAR(clear_module_state->__pyx_n_s_out_verbose);
   Py_CLEAR(clear_module_state->__pyx_n_s_outer_sum);
   Py_CLEAR(clear_module_state->__pyx_n_s_p);
-  Py_CLEAR(clear_module_state->__pyx_n_s_plt);
   Py_CLEAR(clear_module_state->__pyx_n_u_polynomial);
   Py_CLEAR(clear_module_state->__pyx_n_s_predict);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
   Py_CLEAR(clear_module_state->__pyx_n_s_print);
   Py_CLEAR(clear_module_state->__pyx_n_s_probs);
-  Py_CLEAR(clear_module_state->__pyx_n_s_projection);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyplot);
   Py_CLEAR(clear_module_state->__pyx_n_s_q_metric);
   Py_CLEAR(clear_module_state->__pyx_n_s_quality);
   Py_CLEAR(clear_module_state->__pyx_n_s_quality_2);
   Py_CLEAR(clear_module_state->__pyx_kp_u_quality_metric_not_implemented);
   Py_CLEAR(clear_module_state->__pyx_n_s_quality_old);
   Py_CLEAR(clear_module_state->__pyx_n_s_quality_store);
   Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
   Py_CLEAR(clear_module_state->__pyx_n_s_random);
   Py_CLEAR(clear_module_state->__pyx_n_u_random);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_u_rbf);
   Py_CLEAR(clear_module_state->__pyx_n_s_reshape);
   Py_CLEAR(clear_module_state->__pyx_n_s_rng);
   Py_CLEAR(clear_module_state->__pyx_kp_u_sample_cluster_ratio_needs_to_be);
-  Py_CLEAR(clear_module_state->__pyx_n_s_scatter);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_shape);
   Py_CLEAR(clear_module_state->__pyx_n_u_silhouette);
   Py_CLEAR(clear_module_state->__pyx_kp_u_silhouette_inertia);
   Py_CLEAR(clear_module_state->__pyx_n_s_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_sizes);
@@ -2999,16 +2932,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_validate_max_iter);
   Py_CLEAR(clear_module_state->__pyx_n_s_validate_n_clusters);
   Py_CLEAR(clear_module_state->__pyx_n_s_validate_n_init);
   Py_CLEAR(clear_module_state->__pyx_n_s_validate_params);
   Py_CLEAR(clear_module_state->__pyx_n_s_validate_q_metric);
   Py_CLEAR(clear_module_state->__pyx_n_s_validate_tol);
   Py_CLEAR(clear_module_state->__pyx_n_s_verbose);
-  Py_CLEAR(clear_module_state->__pyx_n_s_visualize_kkm);
-  Py_CLEAR(clear_module_state->__pyx_n_s_x);
   Py_CLEAR(clear_module_state->__pyx_n_s_zeros);
   Py_CLEAR(clear_module_state->__pyx_float_1eneg_4);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_2);
   Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_int_8);
@@ -3031,66 +2962,60 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__14);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
   Py_CLEAR(clear_module_state->__pyx_tuple__19);
   Py_CLEAR(clear_module_state->__pyx_tuple__20);
   Py_CLEAR(clear_module_state->__pyx_tuple__22);
-  Py_CLEAR(clear_module_state->__pyx_tuple__23);
-  Py_CLEAR(clear_module_state->__pyx_tuple__24);
   Py_CLEAR(clear_module_state->__pyx_tuple__25);
-  Py_CLEAR(clear_module_state->__pyx_tuple__26);
-  Py_CLEAR(clear_module_state->__pyx_tuple__29);
-  Py_CLEAR(clear_module_state->__pyx_tuple__31);
-  Py_CLEAR(clear_module_state->__pyx_tuple__32);
-  Py_CLEAR(clear_module_state->__pyx_tuple__43);
-  Py_CLEAR(clear_module_state->__pyx_tuple__45);
+  Py_CLEAR(clear_module_state->__pyx_tuple__27);
+  Py_CLEAR(clear_module_state->__pyx_tuple__28);
+  Py_CLEAR(clear_module_state->__pyx_tuple__39);
+  Py_CLEAR(clear_module_state->__pyx_tuple__41);
+  Py_CLEAR(clear_module_state->__pyx_tuple__42);
+  Py_CLEAR(clear_module_state->__pyx_tuple__44);
   Py_CLEAR(clear_module_state->__pyx_tuple__46);
   Py_CLEAR(clear_module_state->__pyx_tuple__48);
   Py_CLEAR(clear_module_state->__pyx_tuple__50);
   Py_CLEAR(clear_module_state->__pyx_tuple__52);
   Py_CLEAR(clear_module_state->__pyx_tuple__54);
   Py_CLEAR(clear_module_state->__pyx_tuple__56);
   Py_CLEAR(clear_module_state->__pyx_tuple__58);
   Py_CLEAR(clear_module_state->__pyx_tuple__60);
-  Py_CLEAR(clear_module_state->__pyx_tuple__62);
-  Py_CLEAR(clear_module_state->__pyx_tuple__64);
+  Py_CLEAR(clear_module_state->__pyx_tuple__63);
+  Py_CLEAR(clear_module_state->__pyx_tuple__65);
   Py_CLEAR(clear_module_state->__pyx_tuple__67);
   Py_CLEAR(clear_module_state->__pyx_tuple__69);
-  Py_CLEAR(clear_module_state->__pyx_tuple__71);
-  Py_CLEAR(clear_module_state->__pyx_tuple__73);
-  Py_CLEAR(clear_module_state->__pyx_tuple__75);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
   Py_CLEAR(clear_module_state->__pyx_codeobj__30);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__31);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__32);
   Py_CLEAR(clear_module_state->__pyx_codeobj__33);
   Py_CLEAR(clear_module_state->__pyx_codeobj__34);
   Py_CLEAR(clear_module_state->__pyx_codeobj__35);
   Py_CLEAR(clear_module_state->__pyx_codeobj__36);
   Py_CLEAR(clear_module_state->__pyx_codeobj__37);
   Py_CLEAR(clear_module_state->__pyx_codeobj__38);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__39);
   Py_CLEAR(clear_module_state->__pyx_codeobj__40);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__41);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__42);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__44);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__43);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__45);
   Py_CLEAR(clear_module_state->__pyx_codeobj__47);
   Py_CLEAR(clear_module_state->__pyx_codeobj__49);
   Py_CLEAR(clear_module_state->__pyx_codeobj__51);
   Py_CLEAR(clear_module_state->__pyx_codeobj__53);
   Py_CLEAR(clear_module_state->__pyx_codeobj__55);
   Py_CLEAR(clear_module_state->__pyx_codeobj__57);
   Py_CLEAR(clear_module_state->__pyx_codeobj__59);
   Py_CLEAR(clear_module_state->__pyx_codeobj__61);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__63);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__65);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__62);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__64);
   Py_CLEAR(clear_module_state->__pyx_codeobj__66);
   Py_CLEAR(clear_module_state->__pyx_codeobj__68);
   Py_CLEAR(clear_module_state->__pyx_codeobj__70);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__72);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__74);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__76);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3103,19 +3028,17 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
-  Py_VISIT(traverse_module_state->__pyx_kp_u_3d);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Amount_of_given_centers_must_be);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Best);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Converged_at_iteration);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Dimensionality_is_too_high_for_v);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Found_at_init);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Given_centers_are_empty);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Given_centers_need_to_be_2_d_arr);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Initialisation_method_not_implem);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_kernel_provided);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Iteration);
   Py_VISIT(traverse_module_state->__pyx_n_s_KKMeans);
@@ -3172,61 +3095,55 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_X);
   Py_VISIT(traverse_module_state->__pyx_n_s_X_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_X_center_kernel);
   Py_VISIT(traverse_module_state->__pyx_kp_u_X_is_empty);
   Py_VISIT(traverse_module_state->__pyx_kp_u_X_needs_to_be_2_d_Array);
   Py_VISIT(traverse_module_state->__pyx_n_s_Y);
   Py_VISIT(traverse_module_state->__pyx_kp_u__16);
-  Py_VISIT(traverse_module_state->__pyx_n_s__27);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__28);
-  Py_VISIT(traverse_module_state->__pyx_n_s__77);
-  Py_VISIT(traverse_module_state->__pyx_n_s_add_subplot);
+  Py_VISIT(traverse_module_state->__pyx_n_s__23);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__24);
+  Py_VISIT(traverse_module_state->__pyx_n_s__71);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithm);
   Py_VISIT(traverse_module_state->__pyx_kp_u_algorithm_not_implemented_this);
   Py_VISIT(traverse_module_state->__pyx_n_s_all);
   Py_VISIT(traverse_module_state->__pyx_n_s_amin);
   Py_VISIT(traverse_module_state->__pyx_n_s_argmax);
   Py_VISIT(traverse_module_state->__pyx_n_s_argmin);
   Py_VISIT(traverse_module_state->__pyx_n_s_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_asarray);
   Py_VISIT(traverse_module_state->__pyx_n_s_ascontiguousarray);
   Py_VISIT(traverse_module_state->__pyx_n_s_assign_to_centers);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_avg_silhouette);
-  Py_VISIT(traverse_module_state->__pyx_n_s_ax);
   Py_VISIT(traverse_module_state->__pyx_n_s_axis);
   Py_VISIT(traverse_module_state->__pyx_n_s_best_init);
   Py_VISIT(traverse_module_state->__pyx_n_s_build_kernel_matrix);
   Py_VISIT(traverse_module_state->__pyx_n_s_build_starting_distance);
-  Py_VISIT(traverse_module_state->__pyx_n_s_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_q_metric);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_silhouette);
   Py_VISIT(traverse_module_state->__pyx_n_s_calc_sq_distances);
   Py_VISIT(traverse_module_state->__pyx_n_s_center);
   Py_VISIT(traverse_module_state->__pyx_n_s_center_dists);
   Py_VISIT(traverse_module_state->__pyx_n_s_centers);
   Py_VISIT(traverse_module_state->__pyx_n_s_choice);
   Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_cluster);
   Py_VISIT(traverse_module_state->__pyx_n_s_cluster_sizes);
   Py_VISIT(traverse_module_state->__pyx_n_s_cluster_sizes_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_converged);
-  Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_default_rng);
   Py_VISIT(traverse_module_state->__pyx_n_s_diag);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dists_to_centers);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
   Py_VISIT(traverse_module_state->__pyx_n_s_double);
   Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
   Py_VISIT(traverse_module_state->__pyx_n_s_elkan);
   Py_VISIT(traverse_module_state->__pyx_n_u_elkan);
-  Py_VISIT(traverse_module_state->__pyx_n_s_fig);
-  Py_VISIT(traverse_module_state->__pyx_n_s_figure);
   Py_VISIT(traverse_module_state->__pyx_n_s_fill_empty_clusters);
   Py_VISIT(traverse_module_state->__pyx_n_s_fit);
   Py_VISIT(traverse_module_state->__pyx_n_u_gaussian);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_best_init);
   Py_VISIT(traverse_module_state->__pyx_n_s_high);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
@@ -3261,15 +3178,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_labels_store);
   Py_VISIT(traverse_module_state->__pyx_n_u_laplacian);
   Py_VISIT(traverse_module_state->__pyx_n_u_linear);
   Py_VISIT(traverse_module_state->__pyx_n_s_lloyd);
   Py_VISIT(traverse_module_state->__pyx_n_u_lloyd);
   Py_VISIT(traverse_module_state->__pyx_n_s_low);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
-  Py_VISIT(traverse_module_state->__pyx_n_s_matplotlib);
   Py_VISIT(traverse_module_state->__pyx_n_s_max_iter);
   Py_VISIT(traverse_module_state->__pyx_kp_u_max_iter_must_be_1);
   Py_VISIT(traverse_module_state->__pyx_kp_u_max_iter_must_be_int);
   Py_VISIT(traverse_module_state->__pyx_n_s_measure_iter);
   Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
   Py_VISIT(traverse_module_state->__pyx_kp_u_metric_not_implemented_this_sho);
   Py_VISIT(traverse_module_state->__pyx_n_s_min_dist_each);
@@ -3287,37 +3203,33 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_not_implemented);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
   Py_VISIT(traverse_module_state->__pyx_n_s_out_finish);
   Py_VISIT(traverse_module_state->__pyx_n_s_out_verbose);
   Py_VISIT(traverse_module_state->__pyx_n_s_outer_sum);
   Py_VISIT(traverse_module_state->__pyx_n_s_p);
-  Py_VISIT(traverse_module_state->__pyx_n_s_plt);
   Py_VISIT(traverse_module_state->__pyx_n_u_polynomial);
   Py_VISIT(traverse_module_state->__pyx_n_s_predict);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
   Py_VISIT(traverse_module_state->__pyx_n_s_print);
   Py_VISIT(traverse_module_state->__pyx_n_s_probs);
-  Py_VISIT(traverse_module_state->__pyx_n_s_projection);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyplot);
   Py_VISIT(traverse_module_state->__pyx_n_s_q_metric);
   Py_VISIT(traverse_module_state->__pyx_n_s_quality);
   Py_VISIT(traverse_module_state->__pyx_n_s_quality_2);
   Py_VISIT(traverse_module_state->__pyx_kp_u_quality_metric_not_implemented);
   Py_VISIT(traverse_module_state->__pyx_n_s_quality_old);
   Py_VISIT(traverse_module_state->__pyx_n_s_quality_store);
   Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
   Py_VISIT(traverse_module_state->__pyx_n_s_random);
   Py_VISIT(traverse_module_state->__pyx_n_u_random);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_u_rbf);
   Py_VISIT(traverse_module_state->__pyx_n_s_reshape);
   Py_VISIT(traverse_module_state->__pyx_n_s_rng);
   Py_VISIT(traverse_module_state->__pyx_kp_u_sample_cluster_ratio_needs_to_be);
-  Py_VISIT(traverse_module_state->__pyx_n_s_scatter);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_shape);
   Py_VISIT(traverse_module_state->__pyx_n_u_silhouette);
   Py_VISIT(traverse_module_state->__pyx_kp_u_silhouette_inertia);
   Py_VISIT(traverse_module_state->__pyx_n_s_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_sizes);
@@ -3346,16 +3258,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_validate_max_iter);
   Py_VISIT(traverse_module_state->__pyx_n_s_validate_n_clusters);
   Py_VISIT(traverse_module_state->__pyx_n_s_validate_n_init);
   Py_VISIT(traverse_module_state->__pyx_n_s_validate_params);
   Py_VISIT(traverse_module_state->__pyx_n_s_validate_q_metric);
   Py_VISIT(traverse_module_state->__pyx_n_s_validate_tol);
   Py_VISIT(traverse_module_state->__pyx_n_s_verbose);
-  Py_VISIT(traverse_module_state->__pyx_n_s_visualize_kkm);
-  Py_VISIT(traverse_module_state->__pyx_n_s_x);
   Py_VISIT(traverse_module_state->__pyx_n_s_zeros);
   Py_VISIT(traverse_module_state->__pyx_float_1eneg_4);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_2);
   Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_int_8);
@@ -3378,66 +3288,60 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__14);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
   Py_VISIT(traverse_module_state->__pyx_tuple__19);
   Py_VISIT(traverse_module_state->__pyx_tuple__20);
   Py_VISIT(traverse_module_state->__pyx_tuple__22);
-  Py_VISIT(traverse_module_state->__pyx_tuple__23);
-  Py_VISIT(traverse_module_state->__pyx_tuple__24);
   Py_VISIT(traverse_module_state->__pyx_tuple__25);
-  Py_VISIT(traverse_module_state->__pyx_tuple__26);
-  Py_VISIT(traverse_module_state->__pyx_tuple__29);
-  Py_VISIT(traverse_module_state->__pyx_tuple__31);
-  Py_VISIT(traverse_module_state->__pyx_tuple__32);
-  Py_VISIT(traverse_module_state->__pyx_tuple__43);
-  Py_VISIT(traverse_module_state->__pyx_tuple__45);
+  Py_VISIT(traverse_module_state->__pyx_tuple__27);
+  Py_VISIT(traverse_module_state->__pyx_tuple__28);
+  Py_VISIT(traverse_module_state->__pyx_tuple__39);
+  Py_VISIT(traverse_module_state->__pyx_tuple__41);
+  Py_VISIT(traverse_module_state->__pyx_tuple__42);
+  Py_VISIT(traverse_module_state->__pyx_tuple__44);
   Py_VISIT(traverse_module_state->__pyx_tuple__46);
   Py_VISIT(traverse_module_state->__pyx_tuple__48);
   Py_VISIT(traverse_module_state->__pyx_tuple__50);
   Py_VISIT(traverse_module_state->__pyx_tuple__52);
   Py_VISIT(traverse_module_state->__pyx_tuple__54);
   Py_VISIT(traverse_module_state->__pyx_tuple__56);
   Py_VISIT(traverse_module_state->__pyx_tuple__58);
   Py_VISIT(traverse_module_state->__pyx_tuple__60);
-  Py_VISIT(traverse_module_state->__pyx_tuple__62);
-  Py_VISIT(traverse_module_state->__pyx_tuple__64);
+  Py_VISIT(traverse_module_state->__pyx_tuple__63);
+  Py_VISIT(traverse_module_state->__pyx_tuple__65);
   Py_VISIT(traverse_module_state->__pyx_tuple__67);
   Py_VISIT(traverse_module_state->__pyx_tuple__69);
-  Py_VISIT(traverse_module_state->__pyx_tuple__71);
-  Py_VISIT(traverse_module_state->__pyx_tuple__73);
-  Py_VISIT(traverse_module_state->__pyx_tuple__75);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
   Py_VISIT(traverse_module_state->__pyx_codeobj__30);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__31);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__32);
   Py_VISIT(traverse_module_state->__pyx_codeobj__33);
   Py_VISIT(traverse_module_state->__pyx_codeobj__34);
   Py_VISIT(traverse_module_state->__pyx_codeobj__35);
   Py_VISIT(traverse_module_state->__pyx_codeobj__36);
   Py_VISIT(traverse_module_state->__pyx_codeobj__37);
   Py_VISIT(traverse_module_state->__pyx_codeobj__38);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__39);
   Py_VISIT(traverse_module_state->__pyx_codeobj__40);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__41);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__42);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__44);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__43);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__45);
   Py_VISIT(traverse_module_state->__pyx_codeobj__47);
   Py_VISIT(traverse_module_state->__pyx_codeobj__49);
   Py_VISIT(traverse_module_state->__pyx_codeobj__51);
   Py_VISIT(traverse_module_state->__pyx_codeobj__53);
   Py_VISIT(traverse_module_state->__pyx_codeobj__55);
   Py_VISIT(traverse_module_state->__pyx_codeobj__57);
   Py_VISIT(traverse_module_state->__pyx_codeobj__59);
   Py_VISIT(traverse_module_state->__pyx_codeobj__61);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__63);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__65);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__62);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__64);
   Py_VISIT(traverse_module_state->__pyx_codeobj__66);
   Py_VISIT(traverse_module_state->__pyx_codeobj__68);
   Py_VISIT(traverse_module_state->__pyx_codeobj__70);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__72);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__74);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__76);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3460,19 +3364,17 @@
 #define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
 #endif
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
-#define __pyx_kp_u_3d __pyx_mstate_global->__pyx_kp_u_3d
 #define __pyx_kp_u_Amount_of_given_centers_must_be __pyx_mstate_global->__pyx_kp_u_Amount_of_given_centers_must_be
 #define __pyx_kp_u_Best __pyx_mstate_global->__pyx_kp_u_Best
 #define __pyx_kp_u_Converged_at_iteration __pyx_mstate_global->__pyx_kp_u_Converged_at_iteration
-#define __pyx_kp_u_Dimensionality_is_too_high_for_v __pyx_mstate_global->__pyx_kp_u_Dimensionality_is_too_high_for_v
 #define __pyx_kp_u_Found_at_init __pyx_mstate_global->__pyx_kp_u_Found_at_init
 #define __pyx_kp_u_Given_centers_are_empty __pyx_mstate_global->__pyx_kp_u_Given_centers_are_empty
 #define __pyx_kp_u_Given_centers_need_to_be_2_d_arr __pyx_mstate_global->__pyx_kp_u_Given_centers_need_to_be_2_d_arr
 #define __pyx_kp_u_Initialisation_method_not_implem __pyx_mstate_global->__pyx_kp_u_Initialisation_method_not_implem
 #define __pyx_kp_u_Invalid_kernel_provided __pyx_mstate_global->__pyx_kp_u_Invalid_kernel_provided
 #define __pyx_kp_u_Iteration __pyx_mstate_global->__pyx_kp_u_Iteration
 #define __pyx_n_s_KKMeans __pyx_mstate_global->__pyx_n_s_KKMeans
@@ -3529,61 +3431,55 @@
 #define __pyx_n_s_X __pyx_mstate_global->__pyx_n_s_X
 #define __pyx_n_s_X_2 __pyx_mstate_global->__pyx_n_s_X_2
 #define __pyx_n_s_X_center_kernel __pyx_mstate_global->__pyx_n_s_X_center_kernel
 #define __pyx_kp_u_X_is_empty __pyx_mstate_global->__pyx_kp_u_X_is_empty
 #define __pyx_kp_u_X_needs_to_be_2_d_Array __pyx_mstate_global->__pyx_kp_u_X_needs_to_be_2_d_Array
 #define __pyx_n_s_Y __pyx_mstate_global->__pyx_n_s_Y
 #define __pyx_kp_u__16 __pyx_mstate_global->__pyx_kp_u__16
-#define __pyx_n_s__27 __pyx_mstate_global->__pyx_n_s__27
-#define __pyx_kp_u__28 __pyx_mstate_global->__pyx_kp_u__28
-#define __pyx_n_s__77 __pyx_mstate_global->__pyx_n_s__77
-#define __pyx_n_s_add_subplot __pyx_mstate_global->__pyx_n_s_add_subplot
+#define __pyx_n_s__23 __pyx_mstate_global->__pyx_n_s__23
+#define __pyx_kp_u__24 __pyx_mstate_global->__pyx_kp_u__24
+#define __pyx_n_s__71 __pyx_mstate_global->__pyx_n_s__71
 #define __pyx_n_s_algorithm __pyx_mstate_global->__pyx_n_s_algorithm
 #define __pyx_kp_u_algorithm_not_implemented_this __pyx_mstate_global->__pyx_kp_u_algorithm_not_implemented_this
 #define __pyx_n_s_all __pyx_mstate_global->__pyx_n_s_all
 #define __pyx_n_s_amin __pyx_mstate_global->__pyx_n_s_amin
 #define __pyx_n_s_argmax __pyx_mstate_global->__pyx_n_s_argmax
 #define __pyx_n_s_argmin __pyx_mstate_global->__pyx_n_s_argmin
 #define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
 #define __pyx_n_s_asarray __pyx_mstate_global->__pyx_n_s_asarray
 #define __pyx_n_s_ascontiguousarray __pyx_mstate_global->__pyx_n_s_ascontiguousarray
 #define __pyx_n_s_assign_to_centers __pyx_mstate_global->__pyx_n_s_assign_to_centers
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_avg_silhouette __pyx_mstate_global->__pyx_n_s_avg_silhouette
-#define __pyx_n_s_ax __pyx_mstate_global->__pyx_n_s_ax
 #define __pyx_n_s_axis __pyx_mstate_global->__pyx_n_s_axis
 #define __pyx_n_s_best_init __pyx_mstate_global->__pyx_n_s_best_init
 #define __pyx_n_s_build_kernel_matrix __pyx_mstate_global->__pyx_n_s_build_kernel_matrix
 #define __pyx_n_s_build_starting_distance __pyx_mstate_global->__pyx_n_s_build_starting_distance
-#define __pyx_n_s_c __pyx_mstate_global->__pyx_n_s_c
 #define __pyx_n_s_calc_q_metric __pyx_mstate_global->__pyx_n_s_calc_q_metric
 #define __pyx_n_s_calc_silhouette __pyx_mstate_global->__pyx_n_s_calc_silhouette
 #define __pyx_n_s_calc_sq_distances __pyx_mstate_global->__pyx_n_s_calc_sq_distances
 #define __pyx_n_s_center __pyx_mstate_global->__pyx_n_s_center
 #define __pyx_n_s_center_dists __pyx_mstate_global->__pyx_n_s_center_dists
 #define __pyx_n_s_centers __pyx_mstate_global->__pyx_n_s_centers
 #define __pyx_n_s_choice __pyx_mstate_global->__pyx_n_s_choice
 #define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_cluster __pyx_mstate_global->__pyx_n_s_cluster
 #define __pyx_n_s_cluster_sizes __pyx_mstate_global->__pyx_n_s_cluster_sizes
 #define __pyx_n_s_cluster_sizes_2 __pyx_mstate_global->__pyx_n_s_cluster_sizes_2
 #define __pyx_n_s_converged __pyx_mstate_global->__pyx_n_s_converged
-#define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_default_rng __pyx_mstate_global->__pyx_n_s_default_rng
 #define __pyx_n_s_diag __pyx_mstate_global->__pyx_n_s_diag
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dists_to_centers __pyx_mstate_global->__pyx_n_s_dists_to_centers
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
 #define __pyx_n_s_double __pyx_mstate_global->__pyx_n_s_double
 #define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
 #define __pyx_n_s_elkan __pyx_mstate_global->__pyx_n_s_elkan
 #define __pyx_n_u_elkan __pyx_mstate_global->__pyx_n_u_elkan
-#define __pyx_n_s_fig __pyx_mstate_global->__pyx_n_s_fig
-#define __pyx_n_s_figure __pyx_mstate_global->__pyx_n_s_figure
 #define __pyx_n_s_fill_empty_clusters __pyx_mstate_global->__pyx_n_s_fill_empty_clusters
 #define __pyx_n_s_fit __pyx_mstate_global->__pyx_n_s_fit
 #define __pyx_n_u_gaussian __pyx_mstate_global->__pyx_n_u_gaussian
 #define __pyx_n_s_get_best_init __pyx_mstate_global->__pyx_n_s_get_best_init
 #define __pyx_n_s_high __pyx_mstate_global->__pyx_n_s_high
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
@@ -3618,15 +3514,14 @@
 #define __pyx_n_s_labels_store __pyx_mstate_global->__pyx_n_s_labels_store
 #define __pyx_n_u_laplacian __pyx_mstate_global->__pyx_n_u_laplacian
 #define __pyx_n_u_linear __pyx_mstate_global->__pyx_n_u_linear
 #define __pyx_n_s_lloyd __pyx_mstate_global->__pyx_n_s_lloyd
 #define __pyx_n_u_lloyd __pyx_mstate_global->__pyx_n_u_lloyd
 #define __pyx_n_s_low __pyx_mstate_global->__pyx_n_s_low
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
-#define __pyx_n_s_matplotlib __pyx_mstate_global->__pyx_n_s_matplotlib
 #define __pyx_n_s_max_iter __pyx_mstate_global->__pyx_n_s_max_iter
 #define __pyx_kp_u_max_iter_must_be_1 __pyx_mstate_global->__pyx_kp_u_max_iter_must_be_1
 #define __pyx_kp_u_max_iter_must_be_int __pyx_mstate_global->__pyx_kp_u_max_iter_must_be_int
 #define __pyx_n_s_measure_iter __pyx_mstate_global->__pyx_n_s_measure_iter
 #define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
 #define __pyx_kp_u_metric_not_implemented_this_sho __pyx_mstate_global->__pyx_kp_u_metric_not_implemented_this_sho
 #define __pyx_n_s_min_dist_each __pyx_mstate_global->__pyx_n_s_min_dist_each
@@ -3644,37 +3539,33 @@
 #define __pyx_kp_u_not_implemented __pyx_mstate_global->__pyx_kp_u_not_implemented
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
 #define __pyx_n_s_out_finish __pyx_mstate_global->__pyx_n_s_out_finish
 #define __pyx_n_s_out_verbose __pyx_mstate_global->__pyx_n_s_out_verbose
 #define __pyx_n_s_outer_sum __pyx_mstate_global->__pyx_n_s_outer_sum
 #define __pyx_n_s_p __pyx_mstate_global->__pyx_n_s_p
-#define __pyx_n_s_plt __pyx_mstate_global->__pyx_n_s_plt
 #define __pyx_n_u_polynomial __pyx_mstate_global->__pyx_n_u_polynomial
 #define __pyx_n_s_predict __pyx_mstate_global->__pyx_n_s_predict
 #define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
 #define __pyx_n_s_print __pyx_mstate_global->__pyx_n_s_print
 #define __pyx_n_s_probs __pyx_mstate_global->__pyx_n_s_probs
-#define __pyx_n_s_projection __pyx_mstate_global->__pyx_n_s_projection
-#define __pyx_n_s_pyplot __pyx_mstate_global->__pyx_n_s_pyplot
 #define __pyx_n_s_q_metric __pyx_mstate_global->__pyx_n_s_q_metric
 #define __pyx_n_s_quality __pyx_mstate_global->__pyx_n_s_quality
 #define __pyx_n_s_quality_2 __pyx_mstate_global->__pyx_n_s_quality_2
 #define __pyx_kp_u_quality_metric_not_implemented __pyx_mstate_global->__pyx_kp_u_quality_metric_not_implemented
 #define __pyx_n_s_quality_old __pyx_mstate_global->__pyx_n_s_quality_old
 #define __pyx_n_s_quality_store __pyx_mstate_global->__pyx_n_s_quality_store
 #define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
 #define __pyx_n_s_random __pyx_mstate_global->__pyx_n_s_random
 #define __pyx_n_u_random __pyx_mstate_global->__pyx_n_u_random
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_u_rbf __pyx_mstate_global->__pyx_n_u_rbf
 #define __pyx_n_s_reshape __pyx_mstate_global->__pyx_n_s_reshape
 #define __pyx_n_s_rng __pyx_mstate_global->__pyx_n_s_rng
 #define __pyx_kp_u_sample_cluster_ratio_needs_to_be __pyx_mstate_global->__pyx_kp_u_sample_cluster_ratio_needs_to_be
-#define __pyx_n_s_scatter __pyx_mstate_global->__pyx_n_s_scatter
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
 #define __pyx_n_s_shape __pyx_mstate_global->__pyx_n_s_shape
 #define __pyx_n_u_silhouette __pyx_mstate_global->__pyx_n_u_silhouette
 #define __pyx_kp_u_silhouette_inertia __pyx_mstate_global->__pyx_kp_u_silhouette_inertia
 #define __pyx_n_s_size __pyx_mstate_global->__pyx_n_s_size
 #define __pyx_n_s_sizes __pyx_mstate_global->__pyx_n_s_sizes
@@ -3703,16 +3594,14 @@
 #define __pyx_n_s_validate_max_iter __pyx_mstate_global->__pyx_n_s_validate_max_iter
 #define __pyx_n_s_validate_n_clusters __pyx_mstate_global->__pyx_n_s_validate_n_clusters
 #define __pyx_n_s_validate_n_init __pyx_mstate_global->__pyx_n_s_validate_n_init
 #define __pyx_n_s_validate_params __pyx_mstate_global->__pyx_n_s_validate_params
 #define __pyx_n_s_validate_q_metric __pyx_mstate_global->__pyx_n_s_validate_q_metric
 #define __pyx_n_s_validate_tol __pyx_mstate_global->__pyx_n_s_validate_tol
 #define __pyx_n_s_verbose __pyx_mstate_global->__pyx_n_s_verbose
-#define __pyx_n_s_visualize_kkm __pyx_mstate_global->__pyx_n_s_visualize_kkm
-#define __pyx_n_s_x __pyx_mstate_global->__pyx_n_s_x
 #define __pyx_n_s_zeros __pyx_mstate_global->__pyx_n_s_zeros
 #define __pyx_float_1eneg_4 __pyx_mstate_global->__pyx_float_1eneg_4
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_2 __pyx_mstate_global->__pyx_int_2
 #define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_int_8 __pyx_mstate_global->__pyx_int_8
@@ -3735,69 +3624,63 @@
 #define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
 #define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
 #define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
-#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
-#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
 #define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
-#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
-#define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
-#define __pyx_tuple__31 __pyx_mstate_global->__pyx_tuple__31
-#define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
-#define __pyx_tuple__43 __pyx_mstate_global->__pyx_tuple__43
-#define __pyx_tuple__45 __pyx_mstate_global->__pyx_tuple__45
+#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
+#define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
+#define __pyx_tuple__39 __pyx_mstate_global->__pyx_tuple__39
+#define __pyx_tuple__41 __pyx_mstate_global->__pyx_tuple__41
+#define __pyx_tuple__42 __pyx_mstate_global->__pyx_tuple__42
+#define __pyx_tuple__44 __pyx_mstate_global->__pyx_tuple__44
 #define __pyx_tuple__46 __pyx_mstate_global->__pyx_tuple__46
 #define __pyx_tuple__48 __pyx_mstate_global->__pyx_tuple__48
 #define __pyx_tuple__50 __pyx_mstate_global->__pyx_tuple__50
 #define __pyx_tuple__52 __pyx_mstate_global->__pyx_tuple__52
 #define __pyx_tuple__54 __pyx_mstate_global->__pyx_tuple__54
 #define __pyx_tuple__56 __pyx_mstate_global->__pyx_tuple__56
 #define __pyx_tuple__58 __pyx_mstate_global->__pyx_tuple__58
 #define __pyx_tuple__60 __pyx_mstate_global->__pyx_tuple__60
-#define __pyx_tuple__62 __pyx_mstate_global->__pyx_tuple__62
-#define __pyx_tuple__64 __pyx_mstate_global->__pyx_tuple__64
+#define __pyx_tuple__63 __pyx_mstate_global->__pyx_tuple__63
+#define __pyx_tuple__65 __pyx_mstate_global->__pyx_tuple__65
 #define __pyx_tuple__67 __pyx_mstate_global->__pyx_tuple__67
 #define __pyx_tuple__69 __pyx_mstate_global->__pyx_tuple__69
-#define __pyx_tuple__71 __pyx_mstate_global->__pyx_tuple__71
-#define __pyx_tuple__73 __pyx_mstate_global->__pyx_tuple__73
-#define __pyx_tuple__75 __pyx_mstate_global->__pyx_tuple__75
+#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
+#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 #define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
+#define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
+#define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
 #define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
 #define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 #define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
 #define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
 #define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
 #define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
-#define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
 #define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
-#define __pyx_codeobj__41 __pyx_mstate_global->__pyx_codeobj__41
-#define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
-#define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
+#define __pyx_codeobj__43 __pyx_mstate_global->__pyx_codeobj__43
+#define __pyx_codeobj__45 __pyx_mstate_global->__pyx_codeobj__45
 #define __pyx_codeobj__47 __pyx_mstate_global->__pyx_codeobj__47
 #define __pyx_codeobj__49 __pyx_mstate_global->__pyx_codeobj__49
 #define __pyx_codeobj__51 __pyx_mstate_global->__pyx_codeobj__51
 #define __pyx_codeobj__53 __pyx_mstate_global->__pyx_codeobj__53
 #define __pyx_codeobj__55 __pyx_mstate_global->__pyx_codeobj__55
 #define __pyx_codeobj__57 __pyx_mstate_global->__pyx_codeobj__57
 #define __pyx_codeobj__59 __pyx_mstate_global->__pyx_codeobj__59
 #define __pyx_codeobj__61 __pyx_mstate_global->__pyx_codeobj__61
-#define __pyx_codeobj__63 __pyx_mstate_global->__pyx_codeobj__63
-#define __pyx_codeobj__65 __pyx_mstate_global->__pyx_codeobj__65
+#define __pyx_codeobj__62 __pyx_mstate_global->__pyx_codeobj__62
+#define __pyx_codeobj__64 __pyx_mstate_global->__pyx_codeobj__64
 #define __pyx_codeobj__66 __pyx_mstate_global->__pyx_codeobj__66
 #define __pyx_codeobj__68 __pyx_mstate_global->__pyx_codeobj__68
 #define __pyx_codeobj__70 __pyx_mstate_global->__pyx_codeobj__70
-#define __pyx_codeobj__72 __pyx_mstate_global->__pyx_codeobj__72
-#define __pyx_codeobj__74 __pyx_mstate_global->__pyx_codeobj__74
-#define __pyx_codeobj__76 __pyx_mstate_global->__pyx_codeobj__76
 /* #### Code section: module_code ### */
 
-/* "KKMeans.py":117
+/* "KKMeans.py":116
  * 
  *     '''
  *     def __init__(self, n_clusters=8, init="kmeans++", n_init=3,             # <<<<<<<<<<<<<<
  *                  max_iter=300, tol=1e-4, q_metric="inertia", verbose=False,
  *                  rng=None, algorithm="lloyd", kernel="linear", **kwargs):
  */
 
@@ -3848,24 +3731,24 @@
     values[1] = ((PyObject *)((PyObject *)__pyx_int_8));
     values[2] = ((PyObject *)((PyObject*)__pyx_kp_u_kmeans));
     values[3] = ((PyObject *)((PyObject *)__pyx_int_3));
     values[4] = ((PyObject *)((PyObject *)__pyx_int_300));
     values[5] = ((PyObject *)((PyObject*)__pyx_float_1eneg_4));
     values[6] = ((PyObject *)((PyObject*)__pyx_n_u_inertia));
 
-    /* "KKMeans.py":118
+    /* "KKMeans.py":117
  *     '''
  *     def __init__(self, n_clusters=8, init="kmeans++", n_init=3,
  *                  max_iter=300, tol=1e-4, q_metric="inertia", verbose=False,             # <<<<<<<<<<<<<<
  *                  rng=None, algorithm="lloyd", kernel="linear", **kwargs):
  *         '''
  */
     values[7] = ((PyObject *)((PyObject *)Py_False));
 
-    /* "KKMeans.py":119
+    /* "KKMeans.py":118
  *     def __init__(self, n_clusters=8, init="kmeans++", n_init=3,
  *                  max_iter=300, tol=1e-4, q_metric="inertia", verbose=False,
  *                  rng=None, algorithm="lloyd", kernel="linear", **kwargs):             # <<<<<<<<<<<<<<
  *         '''
  *         Ctor for KKMeans, more details in class docstring.
  */
     values[8] = ((PyObject *)((PyObject *)Py_None));
@@ -3899,90 +3782,90 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_clusters);
           if (value) { values[1] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_init);
           if (value) { values[2] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_init);
           if (value) { values[3] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_iter);
           if (value) { values[4] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_tol);
           if (value) { values[5] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_q_metric);
           if (value) { values[6] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_verbose);
           if (value) { values[7] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_rng);
           if (value) { values[8] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_algorithm);
           if (value) { values[9] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel);
           if (value) { values[10] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 117, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
         CYTHON_FALLTHROUGH;
         case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
@@ -4017,24 +3900,24 @@
     __pyx_v_verbose = values[7];
     __pyx_v_rng = values[8];
     __pyx_v_algorithm = values[9];
     __pyx_v_kernel = values[10];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 11, __pyx_nargs); __PYX_ERR(0, 117, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 11, __pyx_nargs); __PYX_ERR(0, 116, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("KKMeans.KKMeans.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans___init__(__pyx_self, __pyx_v_self, __pyx_v_n_clusters, __pyx_v_init, __pyx_v_n_init, __pyx_v_max_iter, __pyx_v_tol, __pyx_v_q_metric, __pyx_v_verbose, __pyx_v_rng, __pyx_v_algorithm, __pyx_v_kernel, __pyx_v_kwargs);
 
-  /* "KKMeans.py":117
+  /* "KKMeans.py":116
  * 
  *     '''
  *     def __init__(self, n_clusters=8, init="kmeans++", n_init=3,             # <<<<<<<<<<<<<<
  *                  max_iter=300, tol=1e-4, q_metric="inertia", verbose=False,
  *                  rng=None, algorithm="lloyd", kernel="linear", **kwargs):
  */
 
@@ -4053,94 +3936,94 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "KKMeans.py":139
+  /* "KKMeans.py":138
  * 
  *         '''
  *         self.n_clusters = n_clusters             # <<<<<<<<<<<<<<
  *         self.init = init
  *         self.n_init = n_init
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters, __pyx_v_n_clusters) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters, __pyx_v_n_clusters) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "KKMeans.py":140
+  /* "KKMeans.py":139
  *         '''
  *         self.n_clusters = n_clusters
  *         self.init = init             # <<<<<<<<<<<<<<
  *         self.n_init = n_init
  *         self.max_iter = max_iter
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_init, __pyx_v_init) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_init, __pyx_v_init) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
 
-  /* "KKMeans.py":141
+  /* "KKMeans.py":140
  *         self.n_clusters = n_clusters
  *         self.init = init
  *         self.n_init = n_init             # <<<<<<<<<<<<<<
  *         self.max_iter = max_iter
  *         self.tol = tol
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_n_init, __pyx_v_n_init) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_n_init, __pyx_v_n_init) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
 
-  /* "KKMeans.py":142
+  /* "KKMeans.py":141
  *         self.init = init
  *         self.n_init = n_init
  *         self.max_iter = max_iter             # <<<<<<<<<<<<<<
  *         self.tol = tol
  *         self.q_metric = q_metric
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_iter, __pyx_v_max_iter) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_iter, __pyx_v_max_iter) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
 
-  /* "KKMeans.py":143
+  /* "KKMeans.py":142
  *         self.n_init = n_init
  *         self.max_iter = max_iter
  *         self.tol = tol             # <<<<<<<<<<<<<<
  *         self.q_metric = q_metric
  *         self.verbose = bool(verbose)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_tol, __pyx_v_tol) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_tol, __pyx_v_tol) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
 
-  /* "KKMeans.py":144
+  /* "KKMeans.py":143
  *         self.max_iter = max_iter
  *         self.tol = tol
  *         self.q_metric = q_metric             # <<<<<<<<<<<<<<
  *         self.verbose = bool(verbose)
  *         self.rng = np.random.default_rng(rng)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_q_metric, __pyx_v_q_metric) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_q_metric, __pyx_v_q_metric) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
 
-  /* "KKMeans.py":145
+  /* "KKMeans.py":144
  *         self.tol = tol
  *         self.q_metric = q_metric
  *         self.verbose = bool(verbose)             # <<<<<<<<<<<<<<
  *         self.rng = np.random.default_rng(rng)
  *         self.algorithm = algorithm
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_verbose); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 145, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyBool_FromLong((!(!__pyx_t_1))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_verbose); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong((!(!__pyx_t_1))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_verbose, __pyx_t_2) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_verbose, __pyx_t_2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":146
+  /* "KKMeans.py":145
  *         self.q_metric = q_metric
  *         self.verbose = bool(verbose)
  *         self.rng = np.random.default_rng(rng)             # <<<<<<<<<<<<<<
  *         self.algorithm = algorithm
  *         self.kernel = kernel
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_default_rng); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_default_rng); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -4151,56 +4034,56 @@
       __pyx_t_5 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_rng};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_rng, __pyx_t_2) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_rng, __pyx_t_2) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":147
+  /* "KKMeans.py":146
  *         self.verbose = bool(verbose)
  *         self.rng = np.random.default_rng(rng)
  *         self.algorithm = algorithm             # <<<<<<<<<<<<<<
  *         self.kernel = kernel
  *         self.kwargs = kwargs
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_algorithm, __pyx_v_algorithm) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_algorithm, __pyx_v_algorithm) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
 
-  /* "KKMeans.py":148
+  /* "KKMeans.py":147
  *         self.rng = np.random.default_rng(rng)
  *         self.algorithm = algorithm
  *         self.kernel = kernel             # <<<<<<<<<<<<<<
  *         self.kwargs = kwargs
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_kernel, __pyx_v_kernel) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_kernel, __pyx_v_kernel) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
 
-  /* "KKMeans.py":149
+  /* "KKMeans.py":148
  *         self.algorithm = algorithm
  *         self.kernel = kernel
  *         self.kwargs = kwargs             # <<<<<<<<<<<<<<
  * 
  *         self._validate_params()
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_kwargs, __pyx_v_kwargs) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_kwargs, __pyx_v_kwargs) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
 
-  /* "KKMeans.py":151
+  /* "KKMeans.py":150
  *         self.kwargs = kwargs
  * 
  *         self._validate_params()             # <<<<<<<<<<<<<<
  * 
  *         # Class attributes that are used for information storage
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_validate_params); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_validate_params); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4210,66 +4093,66 @@
       __pyx_t_5 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_4, };
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":155
+  /* "KKMeans.py":154
  *         # Class attributes that are used for information storage
  * 
  *         self.labels_ = None             # <<<<<<<<<<<<<<
  *         self.inner_sums_ = None
  *         self.cluster_sizes_ = None
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, Py_None) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, Py_None) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
 
-  /* "KKMeans.py":156
+  /* "KKMeans.py":155
  * 
  *         self.labels_ = None
  *         self.inner_sums_ = None             # <<<<<<<<<<<<<<
  *         self.cluster_sizes_ = None
  *         self.X_ = None
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_inner_sums, Py_None) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_inner_sums, Py_None) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
 
-  /* "KKMeans.py":157
+  /* "KKMeans.py":156
  *         self.labels_ = None
  *         self.inner_sums_ = None
  *         self.cluster_sizes_ = None             # <<<<<<<<<<<<<<
  *         self.X_ = None
  *         self.quality_ = None
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cluster_sizes, Py_None) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cluster_sizes, Py_None) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
 
-  /* "KKMeans.py":158
+  /* "KKMeans.py":157
  *         self.inner_sums_ = None
  *         self.cluster_sizes_ = None
  *         self.X_ = None             # <<<<<<<<<<<<<<
  *         self.quality_ = None
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_X, Py_None) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_X, Py_None) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
 
-  /* "KKMeans.py":159
+  /* "KKMeans.py":158
  *         self.cluster_sizes_ = None
  *         self.X_ = None
  *         self.quality_ = None             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_quality, Py_None) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_quality, Py_None) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
 
-  /* "KKMeans.py":117
+  /* "KKMeans.py":116
  * 
  *     '''
  *     def __init__(self, n_clusters=8, init="kmeans++", n_init=3,             # <<<<<<<<<<<<<<
  *                  max_iter=300, tol=1e-4, q_metric="inertia", verbose=False,
  *                  rng=None, algorithm="lloyd", kernel="linear", **kwargs):
  */
 
@@ -4284,15 +4167,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":162
+/* "KKMeans.py":161
  * 
  * 
  *     def _validate_params(self):             # <<<<<<<<<<<<<<
  *         '''Checks for possible errors in the parameters, can raise exceptions'''
  *         self.__validate_n_clusters()
  */
 
@@ -4335,31 +4218,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 162, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_validate_params") < 0)) __PYX_ERR(0, 162, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_validate_params") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_validate_params", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 162, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_validate_params", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 161, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._validate_params", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_2_validate_params(__pyx_self, __pyx_v_self);
 
@@ -4378,22 +4261,22 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_validate_params", 0);
 
-  /* "KKMeans.py":164
+  /* "KKMeans.py":163
  *     def _validate_params(self):
  *         '''Checks for possible errors in the parameters, can raise exceptions'''
  *         self.__validate_n_clusters()             # <<<<<<<<<<<<<<
  *         self.__validate_init()
  *         self.__validate_n_init()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4403,28 +4286,28 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":165
+  /* "KKMeans.py":164
  *         '''Checks for possible errors in the parameters, can raise exceptions'''
  *         self.__validate_n_clusters()
  *         self.__validate_init()             # <<<<<<<<<<<<<<
  *         self.__validate_n_init()
  *         self.__validate_max_iter()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4434,28 +4317,28 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":166
+  /* "KKMeans.py":165
  *         self.__validate_n_clusters()
  *         self.__validate_init()
  *         self.__validate_n_init()             # <<<<<<<<<<<<<<
  *         self.__validate_max_iter()
  *         self.__validate_tol()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_n_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_n_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4465,28 +4348,28 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":167
+  /* "KKMeans.py":166
  *         self.__validate_init()
  *         self.__validate_n_init()
  *         self.__validate_max_iter()             # <<<<<<<<<<<<<<
  *         self.__validate_tol()
  *         self.__validate_q_metric()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_max_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_max_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4496,28 +4379,28 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":168
+  /* "KKMeans.py":167
  *         self.__validate_n_init()
  *         self.__validate_max_iter()
  *         self.__validate_tol()             # <<<<<<<<<<<<<<
  *         self.__validate_q_metric()
  *         self.__validate_algorithm()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_tol); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_tol); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4527,28 +4410,28 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":169
+  /* "KKMeans.py":168
  *         self.__validate_max_iter()
  *         self.__validate_tol()
  *         self.__validate_q_metric()             # <<<<<<<<<<<<<<
  *         self.__validate_algorithm()
  *         self.__validate_kernel()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_q_metric); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_q_metric); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4558,28 +4441,28 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":170
+  /* "KKMeans.py":169
  *         self.__validate_tol()
  *         self.__validate_q_metric()
  *         self.__validate_algorithm()             # <<<<<<<<<<<<<<
  *         self.__validate_kernel()
  *         if self.algorithm == "elkan" and self.q_metric == "silhouette":
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_algorithm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_algorithm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4589,28 +4472,28 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":171
+  /* "KKMeans.py":170
  *         self.__validate_q_metric()
  *         self.__validate_algorithm()
  *         self.__validate_kernel()             # <<<<<<<<<<<<<<
  *         if self.algorithm == "elkan" and self.q_metric == "silhouette":
  *             print("WARNING: using silhouette with elkan will most likely be inaccurate\
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_kernel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_kernel); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4620,65 +4503,65 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":172
+  /* "KKMeans.py":171
  *         self.__validate_algorithm()
  *         self.__validate_kernel()
  *         if self.algorithm == "elkan" and self.q_metric == "silhouette":             # <<<<<<<<<<<<<<
  *             print("WARNING: using silhouette with elkan will most likely be inaccurate\
  *                   as elkan does not calculate exact distances to every center")
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_elkan, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_elkan, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
   } else {
     __pyx_t_5 = __pyx_t_6;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_silhouette, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_silhouette, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = __pyx_t_6;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "KKMeans.py":173
+    /* "KKMeans.py":172
  *         self.__validate_kernel()
  *         if self.algorithm == "elkan" and self.q_metric == "silhouette":
  *             print("WARNING: using silhouette with elkan will most likely be inaccurate\             # <<<<<<<<<<<<<<
  *                   as elkan does not calculate exact distances to every center")
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "KKMeans.py":172
+    /* "KKMeans.py":171
  *         self.__validate_algorithm()
  *         self.__validate_kernel()
  *         if self.algorithm == "elkan" and self.q_metric == "silhouette":             # <<<<<<<<<<<<<<
  *             print("WARNING: using silhouette with elkan will most likely be inaccurate\
  *                   as elkan does not calculate exact distances to every center")
  */
   }
 
-  /* "KKMeans.py":162
+  /* "KKMeans.py":161
  * 
  * 
  *     def _validate_params(self):             # <<<<<<<<<<<<<<
  *         '''Checks for possible errors in the parameters, can raise exceptions'''
  *         self.__validate_n_clusters()
  */
 
@@ -4693,15 +4576,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":176
+/* "KKMeans.py":175
  *                   as elkan does not calculate exact distances to every center")
  * 
  *     def __validate_n_clusters(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")
  */
 
@@ -4743,31 +4626,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 175, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_n_clusters") < 0)) __PYX_ERR(0, 176, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_n_clusters") < 0)) __PYX_ERR(0, 175, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_n_clusters", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 176, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_n_clusters", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 175, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_n_clusters", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_4__validate_n_clusters(__pyx_self, __pyx_v_self);
 
@@ -4784,88 +4667,88 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_n_clusters", 0);
 
-  /* "KKMeans.py":177
+  /* "KKMeans.py":176
  * 
  *     def __validate_n_clusters(self):
  *         if not isinstance(self.n_clusters, int):             # <<<<<<<<<<<<<<
  *             raise ValueError("n_clusters must be int")
  *         if self.n_clusters < 1:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyInt_Check(__pyx_t_1); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (!__pyx_t_2);
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":178
+    /* "KKMeans.py":177
  *     def __validate_n_clusters(self):
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")             # <<<<<<<<<<<<<<
  *         if self.n_clusters < 1:
  *             raise ValueError("n_cluster must be >= 1")
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 178, __pyx_L1_error)
+    __PYX_ERR(0, 177, __pyx_L1_error)
 
-    /* "KKMeans.py":177
+    /* "KKMeans.py":176
  * 
  *     def __validate_n_clusters(self):
  *         if not isinstance(self.n_clusters, int):             # <<<<<<<<<<<<<<
  *             raise ValueError("n_clusters must be int")
  *         if self.n_clusters < 1:
  */
   }
 
-  /* "KKMeans.py":179
+  /* "KKMeans.py":178
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")
  *         if self.n_clusters < 1:             # <<<<<<<<<<<<<<
  *             raise ValueError("n_cluster must be >= 1")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_1, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_1, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":180
+    /* "KKMeans.py":179
  *             raise ValueError("n_clusters must be int")
  *         if self.n_clusters < 1:
  *             raise ValueError("n_cluster must be >= 1")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_init(self):
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 180, __pyx_L1_error)
+    __PYX_ERR(0, 179, __pyx_L1_error)
 
-    /* "KKMeans.py":179
+    /* "KKMeans.py":178
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")
  *         if self.n_clusters < 1:             # <<<<<<<<<<<<<<
  *             raise ValueError("n_cluster must be >= 1")
  * 
  */
   }
 
-  /* "KKMeans.py":176
+  /* "KKMeans.py":175
  *                   as elkan does not calculate exact distances to every center")
  * 
  *     def __validate_n_clusters(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")
  */
 
@@ -4879,15 +4762,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":182
+/* "KKMeans.py":181
  *             raise ValueError("n_cluster must be >= 1")
  * 
  *     def __validate_init(self):             # <<<<<<<<<<<<<<
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *             self.__validate_centers()
  */
 
@@ -4929,31 +4812,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_init") < 0)) __PYX_ERR(0, 182, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_init") < 0)) __PYX_ERR(0, 181, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_init", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 182, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_init", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 181, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_6__validate_init(__pyx_self, __pyx_v_self);
 
@@ -4973,47 +4856,47 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_init", 0);
 
-  /* "KKMeans.py":183
+  /* "KKMeans.py":182
  * 
  *     def __validate_init(self):
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):             # <<<<<<<<<<<<<<
  *             self.__validate_centers()
  *         elif self.init not in ("kmeans++", "random", "truerandom") :
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_HasAttr(__pyx_t_2, __pyx_n_u_iter); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_HasAttr(__pyx_t_2, __pyx_n_u_iter); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyUnicode_Check(__pyx_t_2); 
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (!__pyx_t_3);
   __pyx_t_1 = __pyx_t_4;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "KKMeans.py":184
+    /* "KKMeans.py":183
  *     def __validate_init(self):
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *             self.__validate_centers()             # <<<<<<<<<<<<<<
  *         elif self.init not in ("kmeans++", "random", "truerandom") :
  *             raise NotImplementedError("Initialisation method not implemented")
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_centers); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_KKMeans__validate_centers); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -5023,82 +4906,82 @@
         __pyx_t_7 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[1] = {__pyx_t_6, };
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "KKMeans.py":183
+    /* "KKMeans.py":182
  * 
  *     def __validate_init(self):
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):             # <<<<<<<<<<<<<<
  *             self.__validate_centers()
  *         elif self.init not in ("kmeans++", "random", "truerandom") :
  */
     goto __pyx_L3;
   }
 
-  /* "KKMeans.py":185
+  /* "KKMeans.py":184
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *             self.__validate_centers()
  *         elif self.init not in ("kmeans++", "random", "truerandom") :             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Initialisation method not implemented")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_kp_u_kmeans, Py_NE)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_kp_u_kmeans, Py_NE)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 184, __pyx_L1_error)
   if (__pyx_t_4) {
   } else {
     __pyx_t_1 = __pyx_t_4;
     goto __pyx_L6_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_random, Py_NE)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_random, Py_NE)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 184, __pyx_L1_error)
   if (__pyx_t_4) {
   } else {
     __pyx_t_1 = __pyx_t_4;
     goto __pyx_L6_bool_binop_done;
   }
-  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_truerandom, Py_NE)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_truerandom, Py_NE)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 184, __pyx_L1_error)
   __pyx_t_1 = __pyx_t_4;
   __pyx_L6_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __pyx_t_1;
   if (unlikely(__pyx_t_4)) {
 
-    /* "KKMeans.py":186
+    /* "KKMeans.py":185
  *             self.__validate_centers()
  *         elif self.init not in ("kmeans++", "random", "truerandom") :
  *             raise NotImplementedError("Initialisation method not implemented")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_centers(self):
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 186, __pyx_L1_error)
+    __PYX_ERR(0, 185, __pyx_L1_error)
 
-    /* "KKMeans.py":185
+    /* "KKMeans.py":184
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *             self.__validate_centers()
  *         elif self.init not in ("kmeans++", "random", "truerandom") :             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Initialisation method not implemented")
  * 
  */
   }
   __pyx_L3:;
 
-  /* "KKMeans.py":182
+  /* "KKMeans.py":181
  *             raise ValueError("n_cluster must be >= 1")
  * 
  *     def __validate_init(self):             # <<<<<<<<<<<<<<
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *             self.__validate_centers()
  */
 
@@ -5113,15 +4996,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":188
+/* "KKMeans.py":187
  *             raise NotImplementedError("Initialisation method not implemented")
  * 
  *     def __validate_centers(self):             # <<<<<<<<<<<<<<
  *         '''checks for invalid centers, can raise exceptions.'''
  *         self.init = np.asarray(self.init, dtype=np.double)
  */
 
@@ -5164,31 +5047,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_centers") < 0)) __PYX_ERR(0, 188, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_centers") < 0)) __PYX_ERR(0, 187, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_centers", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 188, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_centers", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 187, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_centers", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_8__validate_centers(__pyx_self, __pyx_v_self);
 
@@ -5207,187 +5090,187 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_centers", 0);
 
-  /* "KKMeans.py":190
+  /* "KKMeans.py":189
  *     def __validate_centers(self):
  *         '''checks for invalid centers, can raise exceptions.'''
  *         self.init = np.asarray(self.init, dtype=np.double)             # <<<<<<<<<<<<<<
  *         if self.init.ndim != 2:
  *             raise ValueError("Given centers need to be 2-d array")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "KKMeans.py":191
+  /* "KKMeans.py":190
  *         '''checks for invalid centers, can raise exceptions.'''
  *         self.init = np.asarray(self.init, dtype=np.double)
  *         if self.init.ndim != 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("Given centers need to be 2-d array")
  *         if 0 in self.init.shape:
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_6 = (__Pyx_PyInt_BoolNeObjC(__pyx_t_1, __pyx_int_2, 2, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PyInt_BoolNeObjC(__pyx_t_1, __pyx_int_2, 2, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_6)) {
 
-    /* "KKMeans.py":192
+    /* "KKMeans.py":191
  *         self.init = np.asarray(self.init, dtype=np.double)
  *         if self.init.ndim != 2:
  *             raise ValueError("Given centers need to be 2-d array")             # <<<<<<<<<<<<<<
  *         if 0 in self.init.shape:
  *             raise ValueError("Given centers are empty")
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 192, __pyx_L1_error)
+    __PYX_ERR(0, 191, __pyx_L1_error)
 
-    /* "KKMeans.py":191
+    /* "KKMeans.py":190
  *         '''checks for invalid centers, can raise exceptions.'''
  *         self.init = np.asarray(self.init, dtype=np.double)
  *         if self.init.ndim != 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("Given centers need to be 2-d array")
  *         if 0 in self.init.shape:
  */
   }
 
-  /* "KKMeans.py":193
+  /* "KKMeans.py":192
  *         if self.init.ndim != 2:
  *             raise ValueError("Given centers need to be 2-d array")
  *         if 0 in self.init.shape:             # <<<<<<<<<<<<<<
  *             raise ValueError("Given centers are empty")
  *         if self.init.shape[0] != self.n_clusters:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_int_0, __pyx_t_5, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PySequence_ContainsTF(__pyx_int_0, __pyx_t_5, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(__pyx_t_6)) {
 
-    /* "KKMeans.py":194
+    /* "KKMeans.py":193
  *             raise ValueError("Given centers need to be 2-d array")
  *         if 0 in self.init.shape:
  *             raise ValueError("Given centers are empty")             # <<<<<<<<<<<<<<
  *         if self.init.shape[0] != self.n_clusters:
  *             raise ValueError("Amount of given centers must be equal to n_clusters")
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 194, __pyx_L1_error)
+    __PYX_ERR(0, 193, __pyx_L1_error)
 
-    /* "KKMeans.py":193
+    /* "KKMeans.py":192
  *         if self.init.ndim != 2:
  *             raise ValueError("Given centers need to be 2-d array")
  *         if 0 in self.init.shape:             # <<<<<<<<<<<<<<
  *             raise ValueError("Given centers are empty")
  *         if self.init.shape[0] != self.n_clusters:
  */
   }
 
-  /* "KKMeans.py":195
+  /* "KKMeans.py":194
  *         if 0 in self.init.shape:
  *             raise ValueError("Given centers are empty")
  *         if self.init.shape[0] != self.n_clusters:             # <<<<<<<<<<<<<<
  *             raise ValueError("Amount of given centers must be equal to n_clusters")
  *         return self.init
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_5, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_5, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_t_6)) {
 
-    /* "KKMeans.py":196
+    /* "KKMeans.py":195
  *             raise ValueError("Given centers are empty")
  *         if self.init.shape[0] != self.n_clusters:
  *             raise ValueError("Amount of given centers must be equal to n_clusters")             # <<<<<<<<<<<<<<
  *         return self.init
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 196, __pyx_L1_error)
+    __PYX_ERR(0, 195, __pyx_L1_error)
 
-    /* "KKMeans.py":195
+    /* "KKMeans.py":194
  *         if 0 in self.init.shape:
  *             raise ValueError("Given centers are empty")
  *         if self.init.shape[0] != self.n_clusters:             # <<<<<<<<<<<<<<
  *             raise ValueError("Amount of given centers must be equal to n_clusters")
  *         return self.init
  */
   }
 
-  /* "KKMeans.py":197
+  /* "KKMeans.py":196
  *         if self.init.shape[0] != self.n_clusters:
  *             raise ValueError("Amount of given centers must be equal to n_clusters")
  *         return self.init             # <<<<<<<<<<<<<<
  * 
  *     def __validate_n_init(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":188
+  /* "KKMeans.py":187
  *             raise NotImplementedError("Initialisation method not implemented")
  * 
  *     def __validate_centers(self):             # <<<<<<<<<<<<<<
  *         '''checks for invalid centers, can raise exceptions.'''
  *         self.init = np.asarray(self.init, dtype=np.double)
  */
 
@@ -5402,15 +5285,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":199
+/* "KKMeans.py":198
  *         return self.init
  * 
  *     def __validate_n_init(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")
  */
 
@@ -5452,31 +5335,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_n_init") < 0)) __PYX_ERR(0, 199, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_n_init") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_n_init", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 199, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_n_init", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 198, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_n_init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_10__validate_n_init(__pyx_self, __pyx_v_self);
 
@@ -5493,88 +5376,88 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_n_init", 0);
 
-  /* "KKMeans.py":200
+  /* "KKMeans.py":199
  * 
  *     def __validate_n_init(self):
  *         if not isinstance(self.n_init, int):             # <<<<<<<<<<<<<<
  *             raise ValueError("n_init must be int")
  *         if self.n_init <= 0:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyInt_Check(__pyx_t_1); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (!__pyx_t_2);
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":201
+    /* "KKMeans.py":200
  *     def __validate_n_init(self):
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")             # <<<<<<<<<<<<<<
  *         if self.n_init <= 0:
  *             raise ValueError("n_inits must be => 1")
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 201, __pyx_L1_error)
+    __PYX_ERR(0, 200, __pyx_L1_error)
 
-    /* "KKMeans.py":200
+    /* "KKMeans.py":199
  * 
  *     def __validate_n_init(self):
  *         if not isinstance(self.n_init, int):             # <<<<<<<<<<<<<<
  *             raise ValueError("n_init must be int")
  *         if self.n_init <= 0:
  */
   }
 
-  /* "KKMeans.py":202
+  /* "KKMeans.py":201
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")
  *         if self.n_init <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("n_inits must be => 1")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":203
+    /* "KKMeans.py":202
  *             raise ValueError("n_init must be int")
  *         if self.n_init <= 0:
  *             raise ValueError("n_inits must be => 1")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_max_iter(self):
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 203, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 203, __pyx_L1_error)
+    __PYX_ERR(0, 202, __pyx_L1_error)
 
-    /* "KKMeans.py":202
+    /* "KKMeans.py":201
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")
  *         if self.n_init <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("n_inits must be => 1")
  * 
  */
   }
 
-  /* "KKMeans.py":199
+  /* "KKMeans.py":198
  *         return self.init
  * 
  *     def __validate_n_init(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")
  */
 
@@ -5588,15 +5471,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":205
+/* "KKMeans.py":204
  *             raise ValueError("n_inits must be => 1")
  * 
  *     def __validate_max_iter(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")
  */
 
@@ -5638,31 +5521,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 205, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 204, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_max_iter") < 0)) __PYX_ERR(0, 205, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_max_iter") < 0)) __PYX_ERR(0, 204, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_max_iter", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 205, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_max_iter", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 204, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_max_iter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_12__validate_max_iter(__pyx_self, __pyx_v_self);
 
@@ -5679,88 +5562,88 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_max_iter", 0);
 
-  /* "KKMeans.py":206
+  /* "KKMeans.py":205
  * 
  *     def __validate_max_iter(self):
  *         if not isinstance(self.max_iter, int):             # <<<<<<<<<<<<<<
  *             raise ValueError("max_iter must be int")
  *         if self.max_iter <= 0:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyInt_Check(__pyx_t_1); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (!__pyx_t_2);
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":207
+    /* "KKMeans.py":206
  *     def __validate_max_iter(self):
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")             # <<<<<<<<<<<<<<
  *         if self.max_iter <= 0:
  *             raise ValueError("max_iter must be => 1")
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 207, __pyx_L1_error)
+    __PYX_ERR(0, 206, __pyx_L1_error)
 
-    /* "KKMeans.py":206
+    /* "KKMeans.py":205
  * 
  *     def __validate_max_iter(self):
  *         if not isinstance(self.max_iter, int):             # <<<<<<<<<<<<<<
  *             raise ValueError("max_iter must be int")
  *         if self.max_iter <= 0:
  */
   }
 
-  /* "KKMeans.py":208
+  /* "KKMeans.py":207
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")
  *         if self.max_iter <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("max_iter must be => 1")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":209
+    /* "KKMeans.py":208
  *             raise ValueError("max_iter must be int")
  *         if self.max_iter <= 0:
  *             raise ValueError("max_iter must be => 1")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_algorithm(self):
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 209, __pyx_L1_error)
+    __PYX_ERR(0, 208, __pyx_L1_error)
 
-    /* "KKMeans.py":208
+    /* "KKMeans.py":207
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")
  *         if self.max_iter <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("max_iter must be => 1")
  * 
  */
   }
 
-  /* "KKMeans.py":205
+  /* "KKMeans.py":204
  *             raise ValueError("n_inits must be => 1")
  * 
  *     def __validate_max_iter(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")
  */
 
@@ -5774,15 +5657,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":211
+/* "KKMeans.py":210
  *             raise ValueError("max_iter must be => 1")
  * 
  *     def __validate_algorithm(self):             # <<<<<<<<<<<<<<
  *         if self.algorithm not in ("lloyd", "elkan"):
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  */
 
@@ -5824,31 +5707,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 210, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_algorithm") < 0)) __PYX_ERR(0, 211, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_algorithm") < 0)) __PYX_ERR(0, 210, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_algorithm", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 211, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_algorithm", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 210, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_algorithm", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_14__validate_algorithm(__pyx_self, __pyx_v_self);
 
@@ -5865,68 +5748,68 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_algorithm", 0);
 
-  /* "KKMeans.py":212
+  /* "KKMeans.py":211
  * 
  *     def __validate_algorithm(self):
  *         if self.algorithm not in ("lloyd", "elkan"):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_lloyd, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_lloyd, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 211, __pyx_L1_error)
   if (__pyx_t_3) {
   } else {
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_elkan, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_elkan, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 211, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __pyx_t_2;
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":213
+    /* "KKMeans.py":212
  *     def __validate_algorithm(self):
  *         if self.algorithm not in ("lloyd", "elkan"):
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_q_metric(self):
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_not_implemented); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_not_implemented); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 213, __pyx_L1_error)
+    __PYX_ERR(0, 212, __pyx_L1_error)
 
-    /* "KKMeans.py":212
+    /* "KKMeans.py":211
  * 
  *     def __validate_algorithm(self):
  *         if self.algorithm not in ("lloyd", "elkan"):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  * 
  */
   }
 
-  /* "KKMeans.py":211
+  /* "KKMeans.py":210
  *             raise ValueError("max_iter must be => 1")
  * 
  *     def __validate_algorithm(self):             # <<<<<<<<<<<<<<
  *         if self.algorithm not in ("lloyd", "elkan"):
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  */
 
@@ -5940,15 +5823,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":215
+/* "KKMeans.py":214
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  * 
  *     def __validate_q_metric(self):             # <<<<<<<<<<<<<<
  *         if self.q_metric not in ("silhouette, inertia"):
  *             raise NotImplementedError("Quality metric not implemented")
  */
 
@@ -5990,31 +5873,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 214, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_q_metric") < 0)) __PYX_ERR(0, 215, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_q_metric") < 0)) __PYX_ERR(0, 214, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_q_metric", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 215, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_q_metric", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 214, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_q_metric", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_16__validate_q_metric(__pyx_self, __pyx_v_self);
 
@@ -6029,50 +5912,50 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_q_metric", 0);
 
-  /* "KKMeans.py":216
+  /* "KKMeans.py":215
  * 
  *     def __validate_q_metric(self):
  *         if self.q_metric not in ("silhouette, inertia"):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Quality metric not implemented")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyUnicode_ContainsTF(__pyx_t_1, __pyx_kp_u_silhouette_inertia, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 216, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_ContainsTF(__pyx_t_1, __pyx_kp_u_silhouette_inertia, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "KKMeans.py":217
+    /* "KKMeans.py":216
  *     def __validate_q_metric(self):
  *         if self.q_metric not in ("silhouette, inertia"):
  *             raise NotImplementedError("Quality metric not implemented")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_tol(self):
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 217, __pyx_L1_error)
+    __PYX_ERR(0, 216, __pyx_L1_error)
 
-    /* "KKMeans.py":216
+    /* "KKMeans.py":215
  * 
  *     def __validate_q_metric(self):
  *         if self.q_metric not in ("silhouette, inertia"):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Quality metric not implemented")
  * 
  */
   }
 
-  /* "KKMeans.py":215
+  /* "KKMeans.py":214
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  * 
  *     def __validate_q_metric(self):             # <<<<<<<<<<<<<<
  *         if self.q_metric not in ("silhouette, inertia"):
  *             raise NotImplementedError("Quality metric not implemented")
  */
 
@@ -6085,15 +5968,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":219
+/* "KKMeans.py":218
  *             raise NotImplementedError("Quality metric not implemented")
  * 
  *     def __validate_tol(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")
  */
 
@@ -6135,31 +6018,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_tol") < 0)) __PYX_ERR(0, 219, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_tol") < 0)) __PYX_ERR(0, 218, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_tol", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 219, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_tol", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 218, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_tol", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_18__validate_tol(__pyx_self, __pyx_v_self);
 
@@ -6176,103 +6059,103 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_tol", 0);
 
-  /* "KKMeans.py":220
+  /* "KKMeans.py":219
  * 
  *     def __validate_tol(self):
  *         if not isinstance(self.tol, (int, float)):             # <<<<<<<<<<<<<<
  *             raise ValueError("tol must be numeric")
  *         if self.tol < 0:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = PyInt_Check(__pyx_t_1); 
   if (!__pyx_t_3) {
   } else {
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = PyFloat_Check(__pyx_t_1); 
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (!__pyx_t_2);
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":221
+    /* "KKMeans.py":220
  *     def __validate_tol(self):
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")             # <<<<<<<<<<<<<<
  *         if self.tol < 0:
  *             self.tol = 0
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 221, __pyx_L1_error)
+    __PYX_ERR(0, 220, __pyx_L1_error)
 
-    /* "KKMeans.py":220
+    /* "KKMeans.py":219
  * 
  *     def __validate_tol(self):
  *         if not isinstance(self.tol, (int, float)):             # <<<<<<<<<<<<<<
  *             raise ValueError("tol must be numeric")
  *         if self.tol < 0:
  */
   }
 
-  /* "KKMeans.py":222
+  /* "KKMeans.py":221
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")
  *         if self.tol < 0:             # <<<<<<<<<<<<<<
  *             self.tol = 0
  *             print("Warning! tol < 0 passed, tol set to 0")
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 221, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_3) {
 
-    /* "KKMeans.py":223
+    /* "KKMeans.py":222
  *             raise ValueError("tol must be numeric")
  *         if self.tol < 0:
  *             self.tol = 0             # <<<<<<<<<<<<<<
  *             print("Warning! tol < 0 passed, tol set to 0")
  * 
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_tol, __pyx_int_0) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_tol, __pyx_int_0) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
 
-    /* "KKMeans.py":224
+    /* "KKMeans.py":223
  *         if self.tol < 0:
  *             self.tol = 0
  *             print("Warning! tol < 0 passed, tol set to 0")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_kernel(self):
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "KKMeans.py":222
+    /* "KKMeans.py":221
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")
  *         if self.tol < 0:             # <<<<<<<<<<<<<<
  *             self.tol = 0
  *             print("Warning! tol < 0 passed, tol set to 0")
  */
   }
 
-  /* "KKMeans.py":219
+  /* "KKMeans.py":218
  *             raise NotImplementedError("Quality metric not implemented")
  * 
  *     def __validate_tol(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")
  */
 
@@ -6286,15 +6169,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":226
+/* "KKMeans.py":225
  *             print("Warning! tol < 0 passed, tol set to 0")
  * 
  *     def __validate_kernel(self):             # <<<<<<<<<<<<<<
  *         if self.kernel not in [
  *                 "linear", "rbf", "polynomial",
  */
 
@@ -6336,31 +6219,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 226, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_kernel") < 0)) __PYX_ERR(0, 226, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__validate_kernel") < 0)) __PYX_ERR(0, 225, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__validate_kernel", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 226, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__validate_kernel", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 225, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.__validate_kernel", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_20__validate_kernel(__pyx_self, __pyx_v_self);
 
@@ -6376,77 +6259,77 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__validate_kernel", 0);
 
-  /* "KKMeans.py":227
+  /* "KKMeans.py":226
  * 
  *     def __validate_kernel(self):
  *         if self.kernel not in [             # <<<<<<<<<<<<<<
  *                 "linear", "rbf", "polynomial",
  *                 "gaussian", "laplacian"]:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_linear, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_linear, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 226, __pyx_L1_error)
   if (__pyx_t_3) {
   } else {
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_rbf, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_rbf, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 226, __pyx_L1_error)
   if (__pyx_t_3) {
   } else {
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_polynomial, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_polynomial, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 226, __pyx_L1_error)
   if (__pyx_t_3) {
   } else {
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_gaussian, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_gaussian, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 226, __pyx_L1_error)
   if (__pyx_t_3) {
   } else {
     __pyx_t_2 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_laplacian, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_laplacian, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 226, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __pyx_t_2;
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":230
+    /* "KKMeans.py":229
  *                 "linear", "rbf", "polynomial",
  *                 "gaussian", "laplacian"]:
  *             raise ValueError("Invalid kernel provided.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 230, __pyx_L1_error)
+    __PYX_ERR(0, 229, __pyx_L1_error)
 
-    /* "KKMeans.py":227
+    /* "KKMeans.py":226
  * 
  *     def __validate_kernel(self):
  *         if self.kernel not in [             # <<<<<<<<<<<<<<
  *                 "linear", "rbf", "polynomial",
  *                 "gaussian", "laplacian"]:
  */
   }
 
-  /* "KKMeans.py":226
+  /* "KKMeans.py":225
  *             print("Warning! tol < 0 passed, tol set to 0")
  * 
  *     def __validate_kernel(self):             # <<<<<<<<<<<<<<
  *         if self.kernel not in [
  *                 "linear", "rbf", "polynomial",
  */
 
@@ -6459,15 +6342,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":234
+/* "KKMeans.py":233
  * 
  * 
  *     def kernel_wrapper(self, X, Y=None):             # <<<<<<<<<<<<<<
  *         '''
  *         Wrapper function to compute kernel matrix
  */
 
@@ -6517,34 +6400,34 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 233, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_X_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 233, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("kernel_wrapper", 0, 2, 3, 1); __PYX_ERR(0, 234, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("kernel_wrapper", 0, 2, 3, 1); __PYX_ERR(0, 233, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_Y);
           if (value) { values[2] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 234, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 233, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "kernel_wrapper") < 0)) __PYX_ERR(0, 234, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "kernel_wrapper") < 0)) __PYX_ERR(0, 233, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -6554,15 +6437,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_X = values[1];
     __pyx_v_Y = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("kernel_wrapper", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 234, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("kernel_wrapper", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 233, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.kernel_wrapper", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_22kernel_wrapper(__pyx_self, __pyx_v_self, __pyx_v_X, __pyx_v_Y);
 
@@ -6580,58 +6463,58 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("kernel_wrapper", 0);
 
-  /* "KKMeans.py":251
+  /* "KKMeans.py":250
  *             or (len(X), len(Y))
  *         '''
  *         return build_kernel_matrix(X, Y, kernel=self.kernel, **self.kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def fit(self, X):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_build_kernel_matrix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_build_kernel_matrix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_X);
   __Pyx_GIVEREF(__pyx_v_X);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_X);
   __Pyx_INCREF(__pyx_v_Y);
   __Pyx_GIVEREF(__pyx_v_Y);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_Y);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_kernel, __pyx_t_5) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_kernel, __pyx_t_5) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (unlikely(__pyx_t_4 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-    __PYX_ERR(0, 251, __pyx_L1_error)
+    __PYX_ERR(0, 250, __pyx_L1_error)
   }
-  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_t_4) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_t_4) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":234
+  /* "KKMeans.py":233
  * 
  * 
  *     def kernel_wrapper(self, X, Y=None):             # <<<<<<<<<<<<<<
  *         '''
  *         Wrapper function to compute kernel matrix
  */
 
@@ -6646,15 +6529,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":253
+/* "KKMeans.py":252
  *         return build_kernel_matrix(X, Y, kernel=self.kernel, **self.kwargs)
  * 
  *     def fit(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Fits the data X with the given parameters.
  */
 
@@ -6700,40 +6583,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_X_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 252, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("fit", 1, 2, 2, 1); __PYX_ERR(0, 253, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fit", 1, 2, 2, 1); __PYX_ERR(0, 252, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fit") < 0)) __PYX_ERR(0, 253, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fit") < 0)) __PYX_ERR(0, 252, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_X = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fit", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 253, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fit", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 252, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.fit", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_24fit(__pyx_self, __pyx_v_self, __pyx_v_X);
 
@@ -6771,56 +6654,56 @@
   PyObject *(*__pyx_t_12)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fit", 0);
   __Pyx_INCREF(__pyx_v_X);
 
-  /* "KKMeans.py":266
+  /* "KKMeans.py":265
  *             The data which should be fit.
  *         '''
  *         X = np.ascontiguousarray(X, dtype=np.double)             # <<<<<<<<<<<<<<
  *         X = self._validate_data(X)
  *         kernel_matrix = self.kernel_wrapper(X)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_X);
   __Pyx_GIVEREF(__pyx_v_X);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_X);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_X, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":267
+  /* "KKMeans.py":266
  *         '''
  *         X = np.ascontiguousarray(X, dtype=np.double)
  *         X = self._validate_data(X)             # <<<<<<<<<<<<<<
  *         kernel_matrix = self.kernel_wrapper(X)
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_validate_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_validate_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -6830,29 +6713,29 @@
       __pyx_t_6 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_X};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF_SET(__pyx_v_X, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":268
+  /* "KKMeans.py":267
  *         X = np.ascontiguousarray(X, dtype=np.double)
  *         X = self._validate_data(X)
  *         kernel_matrix = self.kernel_wrapper(X)             # <<<<<<<<<<<<<<
  * 
  *         #Storage for each attribute to be safed per iteration
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -6862,261 +6745,261 @@
       __pyx_t_6 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_X};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 268, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_kernel_matrix = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":271
+  /* "KKMeans.py":270
  * 
  *         #Storage for each attribute to be safed per iteration
  *         labels_store = np.zeros((self.n_init, X.shape[0]), dtype=np.int_)             # <<<<<<<<<<<<<<
  *         quality_store = np.zeros(self.n_init, dtype=np.double)
  *         inner_sums_store = np.zeros((self.n_init, self.n_clusters), dtype=np.double)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_5 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_labels_store = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "KKMeans.py":272
+  /* "KKMeans.py":271
  *         #Storage for each attribute to be safed per iteration
  *         labels_store = np.zeros((self.n_init, X.shape[0]), dtype=np.int_)
  *         quality_store = np.zeros(self.n_init, dtype=np.double)             # <<<<<<<<<<<<<<
  *         inner_sums_store = np.zeros((self.n_init, self.n_clusters), dtype=np.double)
  *         sizes_store = np.zeros((self.n_init, self.n_clusters), dtype=np.int_)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_double); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 272, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_quality_store = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":273
+  /* "KKMeans.py":272
  *         labels_store = np.zeros((self.n_init, X.shape[0]), dtype=np.int_)
  *         quality_store = np.zeros(self.n_init, dtype=np.double)
  *         inner_sums_store = np.zeros((self.n_init, self.n_clusters), dtype=np.double)             # <<<<<<<<<<<<<<
  *         sizes_store = np.zeros((self.n_init, self.n_clusters), dtype=np.int_)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
   __pyx_t_5 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_inner_sums_store = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "KKMeans.py":274
+  /* "KKMeans.py":273
  *         quality_store = np.zeros(self.n_init, dtype=np.double)
  *         inner_sums_store = np.zeros((self.n_init, self.n_clusters), dtype=np.double)
  *         sizes_store = np.zeros((self.n_init, self.n_clusters), dtype=np.int_)             # <<<<<<<<<<<<<<
  * 
  *         for init in range(self.n_init):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __pyx_t_3 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_sizes_store = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":276
+  /* "KKMeans.py":275
  *         sizes_store = np.zeros((self.n_init, self.n_clusters), dtype=np.int_)
  * 
  *         for init in range(self.n_init):             # <<<<<<<<<<<<<<
  *             start_labels = self._init_labels(X, kernel_matrix)
  *             if self.algorithm == "lloyd":
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
     __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 276, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 275, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 276, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 275, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 276, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 275, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_8(__pyx_t_5);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 276, __pyx_L1_error)
+          else __PYX_ERR(0, 275, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_init, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "KKMeans.py":277
+    /* "KKMeans.py":276
  * 
  *         for init in range(self.n_init):
  *             start_labels = self._init_labels(X, kernel_matrix)             # <<<<<<<<<<<<<<
  *             if self.algorithm == "lloyd":
  *                 labels, quality, inner_sums, sizes = self.lloyd(kernel_matrix, start_labels)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_labels); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init_labels); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7126,42 +7009,42 @@
         __pyx_t_6 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_1, __pyx_v_X, __pyx_v_kernel_matrix};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 277, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_start_labels, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "KKMeans.py":278
+    /* "KKMeans.py":277
  *         for init in range(self.n_init):
  *             start_labels = self._init_labels(X, kernel_matrix)
  *             if self.algorithm == "lloyd":             # <<<<<<<<<<<<<<
  *                 labels, quality, inner_sums, sizes = self.lloyd(kernel_matrix, start_labels)
  *             elif self.algorithm == "elkan":
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 278, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_lloyd, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 278, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_lloyd, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_9) {
 
-      /* "KKMeans.py":279
+      /* "KKMeans.py":278
  *             start_labels = self._init_labels(X, kernel_matrix)
  *             if self.algorithm == "lloyd":
  *                 labels, quality, inner_sums, sizes = self.lloyd(kernel_matrix, start_labels)             # <<<<<<<<<<<<<<
  *             elif self.algorithm == "elkan":
  *                 labels, quality, inner_sums, sizes = self.elkan(kernel_matrix, start_labels)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_lloyd); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_lloyd); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_1 = NULL;
       __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7171,25 +7054,25 @@
           __pyx_t_6 = 1;
         }
       }
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_1, __pyx_v_kernel_matrix, __pyx_v_start_labels};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 279, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 278, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
         PyObject* sequence = __pyx_t_4;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 4)) {
           if (size > 4) __Pyx_RaiseTooManyValuesError(4);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 279, __pyx_L1_error)
+          __PYX_ERR(0, 278, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
           __pyx_t_10 = PyTuple_GET_ITEM(sequence, 3); 
@@ -7204,84 +7087,84 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_10);
         #else
         {
           Py_ssize_t i;
           PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_1,&__pyx_t_3,&__pyx_t_10};
           for (i=0; i < 4; i++) {
-            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 279, __pyx_L1_error)
+            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 278, __pyx_L1_error)
             __Pyx_GOTREF(item);
             *(temps[i]) = item;
           }
         }
         #endif
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
         Py_ssize_t index = -1;
         PyObject** temps[4] = {&__pyx_t_2,&__pyx_t_1,&__pyx_t_3,&__pyx_t_10};
-        __pyx_t_11 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 279, __pyx_L1_error)
+        __pyx_t_11 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 278, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_11);
         for (index=0; index < 4; index++) {
           PyObject* item = __pyx_t_12(__pyx_t_11); if (unlikely(!item)) goto __pyx_L6_unpacking_failed;
           __Pyx_GOTREF(item);
           *(temps[index]) = item;
         }
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 4) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 4) < 0) __PYX_ERR(0, 278, __pyx_L1_error)
         __pyx_t_12 = NULL;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         goto __pyx_L7_unpacking_done;
         __pyx_L6_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __pyx_t_12 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 279, __pyx_L1_error)
+        __PYX_ERR(0, 278, __pyx_L1_error)
         __pyx_L7_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_labels, __pyx_t_2);
       __pyx_t_2 = 0;
       __Pyx_XDECREF_SET(__pyx_v_quality, __pyx_t_1);
       __pyx_t_1 = 0;
       __Pyx_XDECREF_SET(__pyx_v_inner_sums, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_sizes, __pyx_t_10);
       __pyx_t_10 = 0;
 
-      /* "KKMeans.py":278
+      /* "KKMeans.py":277
  *         for init in range(self.n_init):
  *             start_labels = self._init_labels(X, kernel_matrix)
  *             if self.algorithm == "lloyd":             # <<<<<<<<<<<<<<
  *                 labels, quality, inner_sums, sizes = self.lloyd(kernel_matrix, start_labels)
  *             elif self.algorithm == "elkan":
  */
       goto __pyx_L5;
     }
 
-    /* "KKMeans.py":280
+    /* "KKMeans.py":279
  *             if self.algorithm == "lloyd":
  *                 labels, quality, inner_sums, sizes = self.lloyd(kernel_matrix, start_labels)
  *             elif self.algorithm == "elkan":             # <<<<<<<<<<<<<<
  *                 labels, quality, inner_sums, sizes = self.elkan(kernel_matrix, start_labels)
  *             else:
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 279, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_elkan, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 280, __pyx_L1_error)
+    __pyx_t_9 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_elkan, Py_EQ)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 279, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (likely(__pyx_t_9)) {
 
-      /* "KKMeans.py":281
+      /* "KKMeans.py":280
  *                 labels, quality, inner_sums, sizes = self.lloyd(kernel_matrix, start_labels)
  *             elif self.algorithm == "elkan":
  *                 labels, quality, inner_sums, sizes = self.elkan(kernel_matrix, start_labels)             # <<<<<<<<<<<<<<
  *             else:
  *                 raise ValueError(str(self.algorithm) + " algorithm not implemented; \
  */
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elkan); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_elkan); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 280, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_3 = NULL;
       __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -7291,25 +7174,25 @@
           __pyx_t_6 = 1;
         }
       }
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_kernel_matrix, __pyx_v_start_labels};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 280, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
         PyObject* sequence = __pyx_t_4;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 4)) {
           if (size > 4) __Pyx_RaiseTooManyValuesError(4);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 281, __pyx_L1_error)
+          __PYX_ERR(0, 280, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_10 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_1 = PyTuple_GET_ITEM(sequence, 2); 
           __pyx_t_2 = PyTuple_GET_ITEM(sequence, 3); 
@@ -7324,142 +7207,142 @@
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_2);
         #else
         {
           Py_ssize_t i;
           PyObject** temps[4] = {&__pyx_t_10,&__pyx_t_3,&__pyx_t_1,&__pyx_t_2};
           for (i=0; i < 4; i++) {
-            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 281, __pyx_L1_error)
+            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 280, __pyx_L1_error)
             __Pyx_GOTREF(item);
             *(temps[i]) = item;
           }
         }
         #endif
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
         Py_ssize_t index = -1;
         PyObject** temps[4] = {&__pyx_t_10,&__pyx_t_3,&__pyx_t_1,&__pyx_t_2};
-        __pyx_t_11 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 281, __pyx_L1_error)
+        __pyx_t_11 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 280, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_11);
         for (index=0; index < 4; index++) {
           PyObject* item = __pyx_t_12(__pyx_t_11); if (unlikely(!item)) goto __pyx_L8_unpacking_failed;
           __Pyx_GOTREF(item);
           *(temps[index]) = item;
         }
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 4) < 0) __PYX_ERR(0, 281, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_11), 4) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
         __pyx_t_12 = NULL;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         goto __pyx_L9_unpacking_done;
         __pyx_L8_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __pyx_t_12 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 281, __pyx_L1_error)
+        __PYX_ERR(0, 280, __pyx_L1_error)
         __pyx_L9_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_v_labels, __pyx_t_10);
       __pyx_t_10 = 0;
       __Pyx_XDECREF_SET(__pyx_v_quality, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_inner_sums, __pyx_t_1);
       __pyx_t_1 = 0;
       __Pyx_XDECREF_SET(__pyx_v_sizes, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "KKMeans.py":280
+      /* "KKMeans.py":279
  *             if self.algorithm == "lloyd":
  *                 labels, quality, inner_sums, sizes = self.lloyd(kernel_matrix, start_labels)
  *             elif self.algorithm == "elkan":             # <<<<<<<<<<<<<<
  *                 labels, quality, inner_sums, sizes = self.elkan(kernel_matrix, start_labels)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "KKMeans.py":283
+    /* "KKMeans.py":282
  *                 labels, quality, inner_sums, sizes = self.elkan(kernel_matrix, start_labels)
  *             else:
  *                 raise ValueError(str(self.algorithm) + " algorithm not implemented; \             # <<<<<<<<<<<<<<
  *                                  this should have been caught in _check_params")
  *             labels_store[init] = labels
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_algorithm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = __Pyx_PyObject_Str(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Str(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyNumber_Add(__pyx_t_2, __pyx_kp_u_algorithm_not_implemented_this); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_4 = PyNumber_Add(__pyx_t_2, __pyx_kp_u_algorithm_not_implemented_this); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 283, __pyx_L1_error)
+      __PYX_ERR(0, 282, __pyx_L1_error)
     }
     __pyx_L5:;
 
-    /* "KKMeans.py":285
+    /* "KKMeans.py":284
  *                 raise ValueError(str(self.algorithm) + " algorithm not implemented; \
  *                                  this should have been caught in _check_params")
  *             labels_store[init] = labels             # <<<<<<<<<<<<<<
  *             quality_store[init] = quality
  *             inner_sums_store[init] = inner_sums
  */
-    if (unlikely((PyObject_SetItem(__pyx_v_labels_store, __pyx_v_init, __pyx_v_labels) < 0))) __PYX_ERR(0, 285, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_labels_store, __pyx_v_init, __pyx_v_labels) < 0))) __PYX_ERR(0, 284, __pyx_L1_error)
 
-    /* "KKMeans.py":286
+    /* "KKMeans.py":285
  *                                  this should have been caught in _check_params")
  *             labels_store[init] = labels
  *             quality_store[init] = quality             # <<<<<<<<<<<<<<
  *             inner_sums_store[init] = inner_sums
  *             sizes_store[init] = sizes
  */
-    if (unlikely((PyObject_SetItem(__pyx_v_quality_store, __pyx_v_init, __pyx_v_quality) < 0))) __PYX_ERR(0, 286, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_quality_store, __pyx_v_init, __pyx_v_quality) < 0))) __PYX_ERR(0, 285, __pyx_L1_error)
 
-    /* "KKMeans.py":287
+    /* "KKMeans.py":286
  *             labels_store[init] = labels
  *             quality_store[init] = quality
  *             inner_sums_store[init] = inner_sums             # <<<<<<<<<<<<<<
  *             sizes_store[init] = sizes
  * 
  */
-    if (unlikely((PyObject_SetItem(__pyx_v_inner_sums_store, __pyx_v_init, __pyx_v_inner_sums) < 0))) __PYX_ERR(0, 287, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_inner_sums_store, __pyx_v_init, __pyx_v_inner_sums) < 0))) __PYX_ERR(0, 286, __pyx_L1_error)
 
-    /* "KKMeans.py":288
+    /* "KKMeans.py":287
  *             quality_store[init] = quality
  *             inner_sums_store[init] = inner_sums
  *             sizes_store[init] = sizes             # <<<<<<<<<<<<<<
  * 
  *         best_init = self._get_best_init(quality_store)
  */
-    if (unlikely((PyObject_SetItem(__pyx_v_sizes_store, __pyx_v_init, __pyx_v_sizes) < 0))) __PYX_ERR(0, 288, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_sizes_store, __pyx_v_init, __pyx_v_sizes) < 0))) __PYX_ERR(0, 287, __pyx_L1_error)
 
-    /* "KKMeans.py":276
+    /* "KKMeans.py":275
  *         sizes_store = np.zeros((self.n_init, self.n_clusters), dtype=np.int_)
  * 
  *         for init in range(self.n_init):             # <<<<<<<<<<<<<<
  *             start_labels = self._init_labels(X, kernel_matrix)
  *             if self.algorithm == "lloyd":
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "KKMeans.py":290
+  /* "KKMeans.py":289
  *             sizes_store[init] = sizes
  * 
  *         best_init = self._get_best_init(quality_store)             # <<<<<<<<<<<<<<
  *         self.labels_ = labels_store[best_init]
  *         self.inner_sums_ = inner_sums_store[best_init]
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_best_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7469,86 +7352,86 @@
       __pyx_t_6 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_quality_store};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 289, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_best_init = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":291
+  /* "KKMeans.py":290
  * 
  *         best_init = self._get_best_init(quality_store)
  *         self.labels_ = labels_store[best_init]             # <<<<<<<<<<<<<<
  *         self.inner_sums_ = inner_sums_store[best_init]
  *         self.cluster_sizes_ = sizes_store[best_init]
  */
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_labels_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_labels_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_5) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_labels, __pyx_t_5) < 0) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "KKMeans.py":292
+  /* "KKMeans.py":291
  *         best_init = self._get_best_init(quality_store)
  *         self.labels_ = labels_store[best_init]
  *         self.inner_sums_ = inner_sums_store[best_init]             # <<<<<<<<<<<<<<
  *         self.cluster_sizes_ = sizes_store[best_init]
  *         self.quality_ = quality_store[best_init]
  */
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_inner_sums_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_inner_sums_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_inner_sums, __pyx_t_5) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_inner_sums, __pyx_t_5) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "KKMeans.py":293
+  /* "KKMeans.py":292
  *         self.labels_ = labels_store[best_init]
  *         self.inner_sums_ = inner_sums_store[best_init]
  *         self.cluster_sizes_ = sizes_store[best_init]             # <<<<<<<<<<<<<<
  *         self.quality_ = quality_store[best_init]
  *         self.X_ = X
  */
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_sizes_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_sizes_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cluster_sizes, __pyx_t_5) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cluster_sizes, __pyx_t_5) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "KKMeans.py":294
+  /* "KKMeans.py":293
  *         self.inner_sums_ = inner_sums_store[best_init]
  *         self.cluster_sizes_ = sizes_store[best_init]
  *         self.quality_ = quality_store[best_init]             # <<<<<<<<<<<<<<
  *         self.X_ = X
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_quality_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_quality_store, __pyx_v_best_init); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_quality, __pyx_t_5) < 0) __PYX_ERR(0, 294, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_quality, __pyx_t_5) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "KKMeans.py":295
+  /* "KKMeans.py":294
  *         self.cluster_sizes_ = sizes_store[best_init]
  *         self.quality_ = quality_store[best_init]
  *         self.X_ = X             # <<<<<<<<<<<<<<
  * 
  *         self._out_finish(best_init)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_X, __pyx_v_X) < 0) __PYX_ERR(0, 295, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_X, __pyx_v_X) < 0) __PYX_ERR(0, 294, __pyx_L1_error)
 
-  /* "KKMeans.py":297
+  /* "KKMeans.py":296
  *         self.X_ = X
  * 
  *         self._out_finish(best_init)             # <<<<<<<<<<<<<<
  * 
  *     def _get_best_init(self, quality_store):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_out_finish); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_out_finish); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7558,21 +7441,21 @@
       __pyx_t_6 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_best_init};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 296, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "KKMeans.py":253
+  /* "KKMeans.py":252
  *         return build_kernel_matrix(X, Y, kernel=self.kernel, **self.kwargs)
  * 
  *     def fit(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Fits the data X with the given parameters.
  */
 
@@ -7604,15 +7487,15 @@
   __Pyx_XDECREF(__pyx_v_best_init);
   __Pyx_XDECREF(__pyx_v_X);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":299
+/* "KKMeans.py":298
  *         self._out_finish(best_init)
  * 
  *     def _get_best_init(self, quality_store):             # <<<<<<<<<<<<<<
  *         """Returns best quality score given self.q_metric"""
  *         if self.q_metric == "inertia": # smalles is better
  */
 
@@ -7658,40 +7541,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 299, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 298, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_quality_store)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 299, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 298, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_get_best_init", 1, 2, 2, 1); __PYX_ERR(0, 299, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_get_best_init", 1, 2, 2, 1); __PYX_ERR(0, 298, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_get_best_init") < 0)) __PYX_ERR(0, 299, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_get_best_init") < 0)) __PYX_ERR(0, 298, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_quality_store = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_get_best_init", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 299, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_get_best_init", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 298, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._get_best_init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_26_get_best_init(__pyx_self, __pyx_v_self, __pyx_v_quality_store);
 
@@ -7709,38 +7592,38 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_best_init", 0);
 
-  /* "KKMeans.py":301
+  /* "KKMeans.py":300
  *     def _get_best_init(self, quality_store):
  *         """Returns best quality score given self.q_metric"""
  *         if self.q_metric == "inertia": # smalles is better             # <<<<<<<<<<<<<<
  *             return np.argmin(quality_store)
  *         elif self.q_metric == "silhouette": # bigger is better
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_inertia, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_inertia, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "KKMeans.py":302
+    /* "KKMeans.py":301
  *         """Returns best quality score given self.q_metric"""
  *         if self.q_metric == "inertia": # smalles is better
  *             return np.argmin(quality_store)             # <<<<<<<<<<<<<<
  *         elif self.q_metric == "silhouette": # bigger is better
  *             return np.argmax(quality_store)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 302, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 301, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_argmin); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 302, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_argmin); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 301, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -7751,55 +7634,55 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_quality_store};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":301
+    /* "KKMeans.py":300
  *     def _get_best_init(self, quality_store):
  *         """Returns best quality score given self.q_metric"""
  *         if self.q_metric == "inertia": # smalles is better             # <<<<<<<<<<<<<<
  *             return np.argmin(quality_store)
  *         elif self.q_metric == "silhouette": # bigger is better
  */
   }
 
-  /* "KKMeans.py":303
+  /* "KKMeans.py":302
  *         if self.q_metric == "inertia": # smalles is better
  *             return np.argmin(quality_store)
  *         elif self.q_metric == "silhouette": # bigger is better             # <<<<<<<<<<<<<<
  *             return np.argmax(quality_store)
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_silhouette, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_silhouette, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 302, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (likely(__pyx_t_2)) {
 
-    /* "KKMeans.py":304
+    /* "KKMeans.py":303
  *             return np.argmin(quality_store)
  *         elif self.q_metric == "silhouette": # bigger is better
  *             return np.argmax(quality_store)             # <<<<<<<<<<<<<<
  *         else:
  *             raise NotImplementedError(
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_argmax); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 304, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_argmax); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
@@ -7810,80 +7693,80 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_quality_store};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":303
+    /* "KKMeans.py":302
  *         if self.q_metric == "inertia": # smalles is better
  *             return np.argmin(quality_store)
  *         elif self.q_metric == "silhouette": # bigger is better             # <<<<<<<<<<<<<<
  *             return np.argmax(quality_store)
  *         else:
  */
   }
 
-  /* "KKMeans.py":306
+  /* "KKMeans.py":305
  *             return np.argmax(quality_store)
  *         else:
  *             raise NotImplementedError(             # <<<<<<<<<<<<<<
  *                 str(self.q_metric)
  *                 + " metric not implemented; \
  */
   /*else*/ {
 
-    /* "KKMeans.py":307
+    /* "KKMeans.py":306
  *         else:
  *             raise NotImplementedError(
  *                 str(self.q_metric)             # <<<<<<<<<<<<<<
  *                 + " metric not implemented; \
  *                 this should have been caught in _validate_params")
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "KKMeans.py":308
+    /* "KKMeans.py":307
  *             raise NotImplementedError(
  *                 str(self.q_metric)
  *                 + " metric not implemented; \             # <<<<<<<<<<<<<<
  *                 this should have been caught in _validate_params")
  * 
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_kp_u_metric_not_implemented_this_sho); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_3, __pyx_kp_u_metric_not_implemented_this_sho); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "KKMeans.py":306
+    /* "KKMeans.py":305
  *             return np.argmax(quality_store)
  *         else:
  *             raise NotImplementedError(             # <<<<<<<<<<<<<<
  *                 str(self.q_metric)
  *                 + " metric not implemented; \
  */
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 305, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 306, __pyx_L1_error)
+    __PYX_ERR(0, 305, __pyx_L1_error)
   }
 
-  /* "KKMeans.py":299
+  /* "KKMeans.py":298
  *         self._out_finish(best_init)
  * 
  *     def _get_best_init(self, quality_store):             # <<<<<<<<<<<<<<
  *         """Returns best quality score given self.q_metric"""
  *         if self.q_metric == "inertia": # smalles is better
  */
 
@@ -7896,15 +7779,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":311
+/* "KKMeans.py":310
  *                 this should have been caught in _validate_params")
  * 
  *     def _out_finish(self, best_init):             # <<<<<<<<<<<<<<
  *         '''output at the end of self.fit'''
  *         print("Best " + self.q_metric +":", self.quality_,
  */
 
@@ -7950,40 +7833,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_best_init)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_out_finish", 1, 2, 2, 1); __PYX_ERR(0, 311, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_out_finish", 1, 2, 2, 1); __PYX_ERR(0, 310, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_out_finish") < 0)) __PYX_ERR(0, 311, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_out_finish") < 0)) __PYX_ERR(0, 310, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_best_init = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_out_finish", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 311, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_out_finish", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 310, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._out_finish", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_28_out_finish(__pyx_self, __pyx_v_self, __pyx_v_best_init);
 
@@ -8000,69 +7883,69 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_out_finish", 0);
 
-  /* "KKMeans.py":313
+  /* "KKMeans.py":312
  *     def _out_finish(self, best_init):
  *         '''output at the end of self.fit'''
  *         print("Best " + self.q_metric +":", self.quality_,             # <<<<<<<<<<<<<<
  *               "Found at init:", best_init + 1)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_kp_u_Best, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_kp_u_Best, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quality); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quality); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "KKMeans.py":314
+  /* "KKMeans.py":313
  *         '''output at the end of self.fit'''
  *         print("Best " + self.q_metric +":", self.quality_,
  *               "Found at init:", best_init + 1)             # <<<<<<<<<<<<<<
  * 
  *     def _validate_data(self, X):
  */
-  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_best_init, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_best_init, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "KKMeans.py":313
+  /* "KKMeans.py":312
  *     def _out_finish(self, best_init):
  *         '''output at the end of self.fit'''
  *         print("Best " + self.q_metric +":", self.quality_,             # <<<<<<<<<<<<<<
  *               "Found at init:", best_init + 1)
  * 
  */
-  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_INCREF(__pyx_kp_u_Found_at_init);
   __Pyx_GIVEREF(__pyx_kp_u_Found_at_init);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u_Found_at_init);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "KKMeans.py":311
+  /* "KKMeans.py":310
  *                 this should have been caught in _validate_params")
  * 
  *     def _out_finish(self, best_init):             # <<<<<<<<<<<<<<
  *         '''output at the end of self.fit'''
  *         print("Best " + self.q_metric +":", self.quality_,
  */
 
@@ -8078,15 +7961,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":316
+/* "KKMeans.py":315
  *               "Found at init:", best_init + 1)
  * 
  *     def _validate_data(self, X):             # <<<<<<<<<<<<<<
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:
  */
 
@@ -8132,40 +8015,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_X_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_validate_data", 1, 2, 2, 1); __PYX_ERR(0, 316, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_validate_data", 1, 2, 2, 1); __PYX_ERR(0, 315, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_validate_data") < 0)) __PYX_ERR(0, 316, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_validate_data") < 0)) __PYX_ERR(0, 315, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_X = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_validate_data", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 316, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_validate_data", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 315, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._validate_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_30_validate_data(__pyx_self, __pyx_v_self, __pyx_v_X);
 
@@ -8183,141 +8066,141 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_validate_data", 0);
 
-  /* "KKMeans.py":318
+  /* "KKMeans.py":317
  *     def _validate_data(self, X):
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("X needs to be 2-d Array")
  *         if 0 in X.shape:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 2);
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":319
+    /* "KKMeans.py":318
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:
  *             raise ValueError("X needs to be 2-d Array")             # <<<<<<<<<<<<<<
  *         if 0 in X.shape:
  *             raise ValueError("X is empty")
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 319, __pyx_L1_error)
+    __PYX_ERR(0, 318, __pyx_L1_error)
 
-    /* "KKMeans.py":318
+    /* "KKMeans.py":317
  *     def _validate_data(self, X):
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:             # <<<<<<<<<<<<<<
  *             raise ValueError("X needs to be 2-d Array")
  *         if 0 in X.shape:
  */
   }
 
-  /* "KKMeans.py":320
+  /* "KKMeans.py":319
  *         if len(X.shape) != 2:
  *             raise ValueError("X needs to be 2-d Array")
  *         if 0 in X.shape:             # <<<<<<<<<<<<<<
  *             raise ValueError("X is empty")
  *         if X.shape[0] <  self.n_clusters:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_int_0, __pyx_t_1, Py_EQ)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_int_0, __pyx_t_1, Py_EQ)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":321
+    /* "KKMeans.py":320
  *             raise ValueError("X needs to be 2-d Array")
  *         if 0 in X.shape:
  *             raise ValueError("X is empty")             # <<<<<<<<<<<<<<
  *         if X.shape[0] <  self.n_clusters:
  *             raise ValueError("sample:cluster ratio needs to be at least one")
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 321, __pyx_L1_error)
+    __PYX_ERR(0, 320, __pyx_L1_error)
 
-    /* "KKMeans.py":320
+    /* "KKMeans.py":319
  *         if len(X.shape) != 2:
  *             raise ValueError("X needs to be 2-d Array")
  *         if 0 in X.shape:             # <<<<<<<<<<<<<<
  *             raise ValueError("X is empty")
  *         if X.shape[0] <  self.n_clusters:
  */
   }
 
-  /* "KKMeans.py":322
+  /* "KKMeans.py":321
  *         if 0 in X.shape:
  *             raise ValueError("X is empty")
  *         if X.shape[0] <  self.n_clusters:             # <<<<<<<<<<<<<<
  *             raise ValueError("sample:cluster ratio needs to be at least one")
  *         return X
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 322, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "KKMeans.py":323
+    /* "KKMeans.py":322
  *             raise ValueError("X is empty")
  *         if X.shape[0] <  self.n_clusters:
  *             raise ValueError("sample:cluster ratio needs to be at least one")             # <<<<<<<<<<<<<<
  *         return X
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 323, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 322, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 323, __pyx_L1_error)
+    __PYX_ERR(0, 322, __pyx_L1_error)
 
-    /* "KKMeans.py":322
+    /* "KKMeans.py":321
  *         if 0 in X.shape:
  *             raise ValueError("X is empty")
  *         if X.shape[0] <  self.n_clusters:             # <<<<<<<<<<<<<<
  *             raise ValueError("sample:cluster ratio needs to be at least one")
  *         return X
  */
   }
 
-  /* "KKMeans.py":324
+  /* "KKMeans.py":323
  *         if X.shape[0] <  self.n_clusters:
  *             raise ValueError("sample:cluster ratio needs to be at least one")
  *         return X             # <<<<<<<<<<<<<<
  * 
  *     def _init_labels(self, X, kernel_matrix):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_X);
   __pyx_r = __pyx_v_X;
   goto __pyx_L0;
 
-  /* "KKMeans.py":316
+  /* "KKMeans.py":315
  *               "Found at init:", best_init + 1)
  * 
  *     def _validate_data(self, X):             # <<<<<<<<<<<<<<
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:
  */
 
@@ -8330,15 +8213,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":326
+/* "KKMeans.py":325
  *         return X
  * 
  *     def _init_labels(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''Assign labels to each datapoint by given method'''
  * 
  */
 
@@ -8387,49 +8270,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 325, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_X_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 325, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_init_labels", 1, 3, 3, 1); __PYX_ERR(0, 326, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_init_labels", 1, 3, 3, 1); __PYX_ERR(0, 325, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 325, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_init_labels", 1, 3, 3, 2); __PYX_ERR(0, 326, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_init_labels", 1, 3, 3, 2); __PYX_ERR(0, 325, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_init_labels") < 0)) __PYX_ERR(0, 326, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_init_labels") < 0)) __PYX_ERR(0, 325, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_X = values[1];
     __pyx_v_kernel_matrix = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_init_labels", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 326, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_init_labels", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 325, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._init_labels", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_32_init_labels(__pyx_self, __pyx_v_self, __pyx_v_X, __pyx_v_kernel_matrix);
 
@@ -8452,66 +8335,66 @@
   Py_ssize_t __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_init_labels", 0);
 
-  /* "KKMeans.py":331
+  /* "KKMeans.py":330
  *         # hasattr(x, __iter__) to check if object may be arraylike
  *         # if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *         if isinstance(self.init, np.ndarray) and self.init.dtype == np.double:             # <<<<<<<<<<<<<<
  *             return self._assign_to_centers(X, self.init)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_ndarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = PyObject_IsInstance(__pyx_t_2, __pyx_t_4); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_5 = PyObject_IsInstance(__pyx_t_2, __pyx_t_4); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
   } else {
     __pyx_t_1 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_dtype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_double); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "KKMeans.py":332
+    /* "KKMeans.py":331
  *         # if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *         if isinstance(self.init, np.ndarray) and self.init.dtype == np.double:
  *             return self._assign_to_centers(X, self.init)             # <<<<<<<<<<<<<<
  * 
  *         elif self.init == "random":
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_assign_to_centers); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 332, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_assign_to_centers); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -8522,57 +8405,57 @@
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_v_X, __pyx_t_2};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 332, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":331
+    /* "KKMeans.py":330
  *         # hasattr(x, __iter__) to check if object may be arraylike
  *         # if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *         if isinstance(self.init, np.ndarray) and self.init.dtype == np.double:             # <<<<<<<<<<<<<<
  *             return self._assign_to_centers(X, self.init)
  * 
  */
   }
 
-  /* "KKMeans.py":334
+  /* "KKMeans.py":333
  *             return self._assign_to_centers(X, self.init)
  * 
  *         elif self.init == "random":             # <<<<<<<<<<<<<<
  *             centers = self.rng.choice(X, self.n_clusters)
  *             return self._assign_to_centers(X, centers)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_random, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_random, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_1) {
 
-    /* "KKMeans.py":335
+    /* "KKMeans.py":334
  * 
  *         elif self.init == "random":
  *             centers = self.rng.choice(X, self.n_clusters)             # <<<<<<<<<<<<<<
  *             return self._assign_to_centers(X, centers)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8583,30 +8466,30 @@
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_v_X, __pyx_t_3};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 334, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_v_centers = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "KKMeans.py":336
+    /* "KKMeans.py":335
  *         elif self.init == "random":
  *             centers = self.rng.choice(X, self.n_clusters)
  *             return self._assign_to_centers(X, centers)             # <<<<<<<<<<<<<<
  * 
  *         elif self.init == "truerandom":
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_assign_to_centers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_assign_to_centers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8616,122 +8499,122 @@
         __pyx_t_7 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_X, __pyx_v_centers};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 336, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 335, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":334
+    /* "KKMeans.py":333
  *             return self._assign_to_centers(X, self.init)
  * 
  *         elif self.init == "random":             # <<<<<<<<<<<<<<
  *             centers = self.rng.choice(X, self.n_clusters)
  *             return self._assign_to_centers(X, centers)
  */
   }
 
-  /* "KKMeans.py":338
+  /* "KKMeans.py":337
  *             return self._assign_to_centers(X, centers)
  * 
  *         elif self.init == "truerandom":             # <<<<<<<<<<<<<<
  *             return self.rng.integers(0, self.n_clusters, len(X), dtype=np.int_)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_truerandom, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_n_u_truerandom, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_1) {
 
-    /* "KKMeans.py":339
+    /* "KKMeans.py":338
  * 
  *         elif self.init == "truerandom":
  *             return self.rng.integers(0, self.n_clusters, len(X), dtype=np.int_)             # <<<<<<<<<<<<<<
  * 
  *         elif self.init == "kmeans++":
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_integers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_integers); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyObject_Length(__pyx_v_X); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 339, __pyx_L1_error)
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_8 = PyObject_Length(__pyx_v_X); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 338, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_int_0);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 339, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 338, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_9;
     __pyx_t_9 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":338
+    /* "KKMeans.py":337
  *             return self._assign_to_centers(X, centers)
  * 
  *         elif self.init == "truerandom":             # <<<<<<<<<<<<<<
  *             return self.rng.integers(0, self.n_clusters, len(X), dtype=np.int_)
  * 
  */
   }
 
-  /* "KKMeans.py":341
+  /* "KKMeans.py":340
  *             return self.rng.integers(0, self.n_clusters, len(X), dtype=np.int_)
  * 
  *         elif self.init == "kmeans++":             # <<<<<<<<<<<<<<
  *             return self.kmeanspp(X, kernel_matrix)
  * 
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_init); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_9, __pyx_kp_u_kmeans, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_t_9, __pyx_kp_u_kmeans, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   if (__pyx_t_1) {
 
-    /* "KKMeans.py":342
+    /* "KKMeans.py":341
  * 
  *         elif self.init == "kmeans++":
  *             return self.kmeanspp(X, kernel_matrix)             # <<<<<<<<<<<<<<
  * 
  *         raise NotImplementedError("Unknown initialisation method")
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kmeanspp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 342, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kmeanspp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -8741,45 +8624,45 @@
         __pyx_t_7 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_v_X, __pyx_v_kernel_matrix};
       __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 342, __pyx_L1_error)
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 341, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_r = __pyx_t_9;
     __pyx_t_9 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":341
+    /* "KKMeans.py":340
  *             return self.rng.integers(0, self.n_clusters, len(X), dtype=np.int_)
  * 
  *         elif self.init == "kmeans++":             # <<<<<<<<<<<<<<
  *             return self.kmeanspp(X, kernel_matrix)
  * 
  */
   }
 
-  /* "KKMeans.py":344
+  /* "KKMeans.py":343
  *             return self.kmeanspp(X, kernel_matrix)
  * 
  *         raise NotImplementedError("Unknown initialisation method")             # <<<<<<<<<<<<<<
  * 
  *     def _assign_to_centers(self, X, centers):
  */
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_Raise(__pyx_t_9, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __PYX_ERR(0, 344, __pyx_L1_error)
+  __PYX_ERR(0, 343, __pyx_L1_error)
 
-  /* "KKMeans.py":326
+  /* "KKMeans.py":325
  *         return X
  * 
  *     def _init_labels(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''Assign labels to each datapoint by given method'''
  * 
  */
 
@@ -8795,15 +8678,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_centers);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":346
+/* "KKMeans.py":345
  *         raise NotImplementedError("Unknown initialisation method")
  * 
  *     def _assign_to_centers(self, X, centers):             # <<<<<<<<<<<<<<
  *         '''
  *         Assigns each datapoint to the closest given center.
  */
 
@@ -8852,49 +8735,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_X_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_assign_to_centers", 1, 3, 3, 1); __PYX_ERR(0, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_assign_to_centers", 1, 3, 3, 1); __PYX_ERR(0, 345, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_centers)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_assign_to_centers", 1, 3, 3, 2); __PYX_ERR(0, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_assign_to_centers", 1, 3, 3, 2); __PYX_ERR(0, 345, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_assign_to_centers") < 0)) __PYX_ERR(0, 346, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_assign_to_centers") < 0)) __PYX_ERR(0, 345, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_X = values[1];
     __pyx_v_centers = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_assign_to_centers", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 346, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_assign_to_centers", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 345, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._assign_to_centers", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_34_assign_to_centers(__pyx_self, __pyx_v_self, __pyx_v_X, __pyx_v_centers);
 
@@ -8919,22 +8802,22 @@
   PyObject *(*__pyx_t_8)(PyObject *);
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_assign_to_centers", 0);
 
-  /* "KKMeans.py":370
+  /* "KKMeans.py":369
  *             labels[i] == cluster X[i] is assigned to
  *         '''
  *         X_center_kernel = self.kernel_wrapper(X, centers)             # <<<<<<<<<<<<<<
  *         dists_to_centers = np.zeros((len(X), self.n_clusters))
  *         for cluster in range(self.n_clusters):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8944,39 +8827,39 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_X, __pyx_v_centers};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 370, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_X_center_kernel = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "KKMeans.py":371
+  /* "KKMeans.py":370
  *         '''
  *         X_center_kernel = self.kernel_wrapper(X, centers)
  *         dists_to_centers = np.zeros((len(X), self.n_clusters))             # <<<<<<<<<<<<<<
  *         for cluster in range(self.n_clusters):
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = PyObject_Length(__pyx_v_X); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 371, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_X); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 370, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6);
   __pyx_t_2 = 0;
   __pyx_t_6 = 0;
@@ -8993,108 +8876,108 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_7};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 370, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_dists_to_centers = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "KKMeans.py":372
+  /* "KKMeans.py":371
  *         X_center_kernel = self.kernel_wrapper(X, centers)
  *         dists_to_centers = np.zeros((len(X), self.n_clusters))
  *         for cluster in range(self.n_clusters):             # <<<<<<<<<<<<<<
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]
  *                                          + self.kernel_wrapper(centers[cluster]))
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
     __pyx_t_1 = __pyx_t_3; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 372, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 371, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 372, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 371, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 372, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 371, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_8(__pyx_t_1);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 372, __pyx_L1_error)
+          else __PYX_ERR(0, 371, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_cluster, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "KKMeans.py":373
+    /* "KKMeans.py":372
  *         dists_to_centers = np.zeros((len(X), self.n_clusters))
  *         for cluster in range(self.n_clusters):
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]             # <<<<<<<<<<<<<<
  *                                          + self.kernel_wrapper(centers[cluster]))
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  */
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_slice__21);
     __Pyx_GIVEREF(__pyx_slice__21);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_slice__21);
     __Pyx_INCREF(__pyx_v_cluster);
     __Pyx_GIVEREF(__pyx_v_cluster);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_cluster);
-    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_X_center_kernel, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 373, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_X_center_kernel, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_2, __pyx_t_7, -2L, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_2, __pyx_t_7, -2L, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "KKMeans.py":374
+    /* "KKMeans.py":373
  *         for cluster in range(self.n_clusters):
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]
  *                                          + self.kernel_wrapper(centers[cluster]))             # <<<<<<<<<<<<<<
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  * 
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_centers, __pyx_v_cluster); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_centers, __pyx_v_cluster); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_9 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -9105,107 +8988,107 @@
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_2};
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 374, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 373, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __pyx_t_6 = PyNumber_Add(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "KKMeans.py":373
+    /* "KKMeans.py":372
  *         dists_to_centers = np.zeros((len(X), self.n_clusters))
  *         for cluster in range(self.n_clusters):
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]             # <<<<<<<<<<<<<<
  *                                          + self.kernel_wrapper(centers[cluster]))
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  */
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 373, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(__pyx_slice__21);
     __Pyx_GIVEREF(__pyx_slice__21);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_slice__21);
     __Pyx_INCREF(__pyx_v_cluster);
     __Pyx_GIVEREF(__pyx_v_cluster);
     PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_cluster);
-    if (unlikely((PyObject_SetItem(__pyx_v_dists_to_centers, __pyx_t_7, __pyx_t_6) < 0))) __PYX_ERR(0, 373, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_dists_to_centers, __pyx_t_7, __pyx_t_6) < 0))) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "KKMeans.py":372
+    /* "KKMeans.py":371
  *         X_center_kernel = self.kernel_wrapper(X, centers)
  *         dists_to_centers = np.zeros((len(X), self.n_clusters))
  *         for cluster in range(self.n_clusters):             # <<<<<<<<<<<<<<
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]
  *                                          + self.kernel_wrapper(centers[cluster]))
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "KKMeans.py":375
+  /* "KKMeans.py":374
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]
  *                                          + self.kernel_wrapper(centers[cluster]))
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)             # <<<<<<<<<<<<<<
  * 
  *     def lloyd(self, kernel_matrix, labels):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_asarray); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_argmin); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_argmin); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_dists_to_centers);
   __Pyx_GIVEREF(__pyx_v_dists_to_centers);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dists_to_centers);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 375, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 375, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 375, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":346
+  /* "KKMeans.py":345
  *         raise NotImplementedError("Unknown initialisation method")
  * 
  *     def _assign_to_centers(self, X, centers):             # <<<<<<<<<<<<<<
  *         '''
  *         Assigns each datapoint to the closest given center.
  */
 
@@ -9224,15 +9107,15 @@
   __Pyx_XDECREF(__pyx_v_dists_to_centers);
   __Pyx_XDECREF(__pyx_v_cluster);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":377
+/* "KKMeans.py":376
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  * 
  *     def lloyd(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a run of lloyd's algorithm
  */
 
@@ -9281,49 +9164,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 377, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 377, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("lloyd", 1, 3, 3, 1); __PYX_ERR(0, 377, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("lloyd", 1, 3, 3, 1); __PYX_ERR(0, 376, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 377, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("lloyd", 1, 3, 3, 2); __PYX_ERR(0, 377, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("lloyd", 1, 3, 3, 2); __PYX_ERR(0, 376, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lloyd") < 0)) __PYX_ERR(0, 377, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lloyd") < 0)) __PYX_ERR(0, 376, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_kernel_matrix = values[1];
     __pyx_v_labels = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lloyd", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 377, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lloyd", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 376, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.lloyd", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_36lloyd(__pyx_self, __pyx_v_self, __pyx_v_kernel_matrix, __pyx_v_labels);
 
@@ -9355,173 +9238,173 @@
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lloyd", 0);
   __Pyx_INCREF(__pyx_v_labels);
 
-  /* "KKMeans.py":411
+  /* "KKMeans.py":410
  *         # Init with -INF so that first iteration cannot converge because
  *         # quality does not change.
  *         quality = np.NINF             # <<<<<<<<<<<<<<
  *         for it in range(self.max_iter):
  *             labels, cluster_sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NINF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_NINF); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_quality = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "KKMeans.py":412
+  /* "KKMeans.py":411
  *         # quality does not change.
  *         quality = np.NINF
  *         for it in range(self.max_iter):             # <<<<<<<<<<<<<<
  *             labels, cluster_sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             sq_distances = self._build_starting_distance(kernel_matrix)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 411, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 412, __pyx_L1_error)
+          else __PYX_ERR(0, 411, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":413
+    /* "KKMeans.py":412
  *         quality = np.NINF
  *         for it in range(self.max_iter):
  *             labels, cluster_sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)             # <<<<<<<<<<<<<<
  *             sq_distances = self._build_starting_distance(kernel_matrix)
  *             sq_distances, inner_sums, cluster_sizes = update_lloyd(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_fill_empty_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_fill_empty_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_labels);
     __Pyx_GIVEREF(__pyx_v_labels);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_labels);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_rng, __pyx_t_7) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_rng, __pyx_t_7) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if ((likely(PyTuple_CheckExact(__pyx_t_7))) || (PyList_CheckExact(__pyx_t_7))) {
       PyObject* sequence = __pyx_t_7;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 413, __pyx_L1_error)
+        __PYX_ERR(0, 412, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_5 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       #else
-      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       #endif
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_1 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __pyx_t_1 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1);
       index = 0; __pyx_t_5 = __pyx_t_8(__pyx_t_1); if (unlikely(!__pyx_t_5)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
       index = 1; __pyx_t_6 = __pyx_t_8(__pyx_t_1); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_1), 2) < 0) __PYX_ERR(0, 413, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_1), 2) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
       __pyx_t_8 = NULL;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_8 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 413, __pyx_L1_error)
+      __PYX_ERR(0, 412, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
     __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_cluster_sizes, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "KKMeans.py":414
+    /* "KKMeans.py":413
  *         for it in range(self.max_iter):
  *             labels, cluster_sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             sq_distances = self._build_starting_distance(kernel_matrix)             # <<<<<<<<<<<<<<
  *             sq_distances, inner_sums, cluster_sizes = update_lloyd(
  *                 sq_distances, kernel_matrix, labels,
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_build_starting_distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_build_starting_distance); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_5 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -9531,39 +9414,39 @@
         __pyx_t_9 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_kernel_matrix};
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 414, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 413, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_sq_distances, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "KKMeans.py":415
+    /* "KKMeans.py":414
  *             labels, cluster_sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             sq_distances = self._build_starting_distance(kernel_matrix)
  *             sq_distances, inner_sums, cluster_sizes = update_lloyd(             # <<<<<<<<<<<<<<
  *                 sq_distances, kernel_matrix, labels,
  *                 self.n_clusters, cluster_sizes)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_update_lloyd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_update_lloyd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "KKMeans.py":417
+    /* "KKMeans.py":416
  *             sq_distances, inner_sums, cluster_sizes = update_lloyd(
  *                 sq_distances, kernel_matrix, labels,
  *                 self.n_clusters, cluster_sizes)             # <<<<<<<<<<<<<<
  *             labels_old = labels
  *             labels = np.asarray(np.argmin(sq_distances, axis=1), dtype=np.int_)
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -9574,25 +9457,25 @@
       }
     }
     {
       PyObject *__pyx_callargs[6] = {__pyx_t_1, __pyx_v_sq_distances, __pyx_v_kernel_matrix, __pyx_v_labels, __pyx_t_5, __pyx_v_cluster_sizes};
       __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_9, 5+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 415, __pyx_L1_error)
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_7))) || (PyList_CheckExact(__pyx_t_7))) {
       PyObject* sequence = __pyx_t_7;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 3)) {
         if (size > 3) __Pyx_RaiseTooManyValuesError(3);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 415, __pyx_L1_error)
+        __PYX_ERR(0, 414, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
         __pyx_t_1 = PyTuple_GET_ITEM(sequence, 2); 
       } else {
@@ -9600,130 +9483,130 @@
         __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
         __pyx_t_1 = PyList_GET_ITEM(sequence, 2); 
       }
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_1);
       #else
-      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 415, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 415, __pyx_L1_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #endif
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_10 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 415, __pyx_L1_error)
+      __pyx_t_10 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_10);
       index = 0; __pyx_t_6 = __pyx_t_8(__pyx_t_10); if (unlikely(!__pyx_t_6)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
       index = 1; __pyx_t_5 = __pyx_t_8(__pyx_t_10); if (unlikely(!__pyx_t_5)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
       index = 2; __pyx_t_1 = __pyx_t_8(__pyx_t_10); if (unlikely(!__pyx_t_1)) goto __pyx_L7_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_1);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_10), 3) < 0) __PYX_ERR(0, 415, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_10), 3) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
       __pyx_t_8 = NULL;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       goto __pyx_L8_unpacking_done;
       __pyx_L7_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_8 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 415, __pyx_L1_error)
+      __PYX_ERR(0, 414, __pyx_L1_error)
       __pyx_L8_unpacking_done:;
     }
 
-    /* "KKMeans.py":415
+    /* "KKMeans.py":414
  *             labels, cluster_sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             sq_distances = self._build_starting_distance(kernel_matrix)
  *             sq_distances, inner_sums, cluster_sizes = update_lloyd(             # <<<<<<<<<<<<<<
  *                 sq_distances, kernel_matrix, labels,
  *                 self.n_clusters, cluster_sizes)
  */
     __Pyx_DECREF_SET(__pyx_v_sq_distances, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_inner_sums, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_cluster_sizes, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":418
+    /* "KKMeans.py":417
  *                 sq_distances, kernel_matrix, labels,
  *                 self.n_clusters, cluster_sizes)
  *             labels_old = labels             # <<<<<<<<<<<<<<
  *             labels = np.asarray(np.argmin(sq_distances, axis=1), dtype=np.int_)
  *             quality, converged = self._measure_iter(sq_distances, labels, labels_old, quality)
  */
     __Pyx_INCREF(__pyx_v_labels);
     __Pyx_XDECREF_SET(__pyx_v_labels_old, __pyx_v_labels);
 
-    /* "KKMeans.py":419
+    /* "KKMeans.py":418
  *                 self.n_clusters, cluster_sizes)
  *             labels_old = labels
  *             labels = np.asarray(np.argmin(sq_distances, axis=1), dtype=np.int_)             # <<<<<<<<<<<<<<
  *             quality, converged = self._measure_iter(sq_distances, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_argmin); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_argmin); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(__pyx_v_sq_distances);
     __Pyx_GIVEREF(__pyx_v_sq_distances);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_sq_distances);
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_10);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_10);
     __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_10); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "KKMeans.py":420
+    /* "KKMeans.py":419
  *             labels_old = labels
  *             labels = np.asarray(np.argmin(sq_distances, axis=1), dtype=np.int_)
  *             quality, converged = self._measure_iter(sq_distances, labels, labels_old, quality)             # <<<<<<<<<<<<<<
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:
  */
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_measure_iter); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_measure_iter); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_6 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -9733,150 +9616,150 @@
         __pyx_t_9 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[5] = {__pyx_t_6, __pyx_v_sq_distances, __pyx_v_labels, __pyx_v_labels_old, __pyx_v_quality};
       __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_9, 4+__pyx_t_9);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
       PyObject* sequence = __pyx_t_5;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 420, __pyx_L1_error)
+        __PYX_ERR(0, 419, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_10 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_10 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_6);
       #else
-      __pyx_t_10 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_10 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       #endif
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_1 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_1 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1);
       index = 0; __pyx_t_10 = __pyx_t_8(__pyx_t_1); if (unlikely(!__pyx_t_10)) goto __pyx_L9_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_10);
       index = 1; __pyx_t_6 = __pyx_t_8(__pyx_t_1); if (unlikely(!__pyx_t_6)) goto __pyx_L9_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_1), 2) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_1), 2) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
       __pyx_t_8 = NULL;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L10_unpacking_done;
       __pyx_L9_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_8 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 420, __pyx_L1_error)
+      __PYX_ERR(0, 419, __pyx_L1_error)
       __pyx_L10_unpacking_done:;
     }
     __Pyx_DECREF_SET(__pyx_v_quality, __pyx_t_10);
     __pyx_t_10 = 0;
     __Pyx_XDECREF_SET(__pyx_v_converged, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "KKMeans.py":421
+    /* "KKMeans.py":420
  *             labels = np.asarray(np.argmin(sq_distances, axis=1), dtype=np.int_)
  *             quality, converged = self._measure_iter(sq_distances, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)             # <<<<<<<<<<<<<<
  *             if converged:
  *                 break
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_out_verbose); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_out_verbose); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_v_it);
     __Pyx_GIVEREF(__pyx_v_it);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_it);
     __Pyx_INCREF(__pyx_v_quality);
     __Pyx_GIVEREF(__pyx_v_quality);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_quality);
-    __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_converged, __pyx_v_converged) < 0) __PYX_ERR(0, 421, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_converged, __pyx_v_converged) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "KKMeans.py":422
+    /* "KKMeans.py":421
  *             quality, converged = self._measure_iter(sq_distances, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
-    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_converged); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_v_converged); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 421, __pyx_L1_error)
     if (__pyx_t_11) {
 
-      /* "KKMeans.py":423
+      /* "KKMeans.py":422
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *         return labels, quality, inner_sums, cluster_sizes
  */
       goto __pyx_L4_break;
 
-      /* "KKMeans.py":422
+      /* "KKMeans.py":421
  *             quality, converged = self._measure_iter(sq_distances, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
     }
 
-    /* "KKMeans.py":412
+    /* "KKMeans.py":411
  *         # quality does not change.
  *         quality = np.NINF
  *         for it in range(self.max_iter):             # <<<<<<<<<<<<<<
  *             labels, cluster_sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             sq_distances = self._build_starting_distance(kernel_matrix)
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L12_for_end;
   __pyx_L4_break:;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L12_for_end;
   __pyx_L12_for_end:;
 
-  /* "KKMeans.py":425
+  /* "KKMeans.py":424
  *                 break
  * 
  *         return labels, quality, inner_sums, cluster_sizes             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_inner_sums)) { __Pyx_RaiseUnboundLocalError("inner_sums"); __PYX_ERR(0, 425, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_cluster_sizes)) { __Pyx_RaiseUnboundLocalError("cluster_sizes"); __PYX_ERR(0, 425, __pyx_L1_error) }
-  __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 425, __pyx_L1_error)
+  if (unlikely(!__pyx_v_inner_sums)) { __Pyx_RaiseUnboundLocalError("inner_sums"); __PYX_ERR(0, 424, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_cluster_sizes)) { __Pyx_RaiseUnboundLocalError("cluster_sizes"); __PYX_ERR(0, 424, __pyx_L1_error) }
+  __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_labels);
   __Pyx_GIVEREF(__pyx_v_labels);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_labels);
   __Pyx_INCREF(__pyx_v_quality);
   __Pyx_GIVEREF(__pyx_v_quality);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_quality);
@@ -9886,15 +9769,15 @@
   __Pyx_INCREF(__pyx_v_cluster_sizes);
   __Pyx_GIVEREF(__pyx_v_cluster_sizes);
   PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_v_cluster_sizes);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":377
+  /* "KKMeans.py":376
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  * 
  *     def lloyd(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a run of lloyd's algorithm
  */
 
@@ -9918,15 +9801,15 @@
   __Pyx_XDECREF(__pyx_v_converged);
   __Pyx_XDECREF(__pyx_v_labels);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":429
+/* "KKMeans.py":428
  * 
  * 
  *     def _out_verbose(self, iter, quality, converged):             # <<<<<<<<<<<<<<
  *         '''Checks if self.verbose and prints accordingly'''
  *         if not self.verbose:
  */
 
@@ -9978,41 +9861,41 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 429, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_iter_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 429, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, 1); __PYX_ERR(0, 429, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, 1); __PYX_ERR(0, 428, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_quality_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 429, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, 2); __PYX_ERR(0, 429, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, 2); __PYX_ERR(0, 428, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_converged)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 429, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, 3); __PYX_ERR(0, 429, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, 3); __PYX_ERR(0, 428, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_out_verbose") < 0)) __PYX_ERR(0, 429, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_out_verbose") < 0)) __PYX_ERR(0, 428, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -10021,15 +9904,15 @@
     __pyx_v_self = values[0];
     __pyx_v_iter = values[1];
     __pyx_v_quality = values[2];
     __pyx_v_converged = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 429, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_out_verbose", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 428, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._out_verbose", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_38_out_verbose(__pyx_self, __pyx_v_self, __pyx_v_iter, __pyx_v_quality, __pyx_v_converged);
 
@@ -10047,194 +9930,194 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_out_verbose", 0);
 
-  /* "KKMeans.py":431
+  /* "KKMeans.py":430
  *     def _out_verbose(self, iter, quality, converged):
  *         '''Checks if self.verbose and prints accordingly'''
  *         if not self.verbose:             # <<<<<<<<<<<<<<
  *             return
  *         if converged:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_verbose); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_verbose); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (!__pyx_t_2);
   if (__pyx_t_3) {
 
-    /* "KKMeans.py":432
+    /* "KKMeans.py":431
  *         '''Checks if self.verbose and prints accordingly'''
  *         if not self.verbose:
  *             return             # <<<<<<<<<<<<<<
  *         if converged:
  *             print("Converged at iteration:", iter + 1, self.q_metric + ":", quality)
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "KKMeans.py":431
+    /* "KKMeans.py":430
  *     def _out_verbose(self, iter, quality, converged):
  *         '''Checks if self.verbose and prints accordingly'''
  *         if not self.verbose:             # <<<<<<<<<<<<<<
  *             return
  *         if converged:
  */
   }
 
-  /* "KKMeans.py":433
+  /* "KKMeans.py":432
  *         if not self.verbose:
  *             return
  *         if converged:             # <<<<<<<<<<<<<<
  *             print("Converged at iteration:", iter + 1, self.q_metric + ":", quality)
  *         elif self.tol == 0:
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_converged); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_converged); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 432, __pyx_L1_error)
   if (__pyx_t_3) {
 
-    /* "KKMeans.py":434
+    /* "KKMeans.py":433
  *             return
  *         if converged:
  *             print("Converged at iteration:", iter + 1, self.q_metric + ":", quality)             # <<<<<<<<<<<<<<
  *         elif self.tol == 0:
  *             print("Iteration:", iter + 1, self.q_metric + ":", "Not calculated (Tol==0)")
  */
-    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_iter, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 434, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_iter, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 434, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_u__16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 434, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_u__16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 434, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_kp_u_Converged_at_iteration);
     __Pyx_GIVEREF(__pyx_kp_u_Converged_at_iteration);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_Converged_at_iteration);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_5);
     __Pyx_INCREF(__pyx_v_quality);
     __Pyx_GIVEREF(__pyx_v_quality);
     PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_v_quality);
     __pyx_t_1 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 434, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "KKMeans.py":433
+    /* "KKMeans.py":432
  *         if not self.verbose:
  *             return
  *         if converged:             # <<<<<<<<<<<<<<
  *             print("Converged at iteration:", iter + 1, self.q_metric + ":", quality)
  *         elif self.tol == 0:
  */
     goto __pyx_L4;
   }
 
-  /* "KKMeans.py":435
+  /* "KKMeans.py":434
  *         if converged:
  *             print("Converged at iteration:", iter + 1, self.q_metric + ":", quality)
  *         elif self.tol == 0:             # <<<<<<<<<<<<<<
  *             print("Iteration:", iter + 1, self.q_metric + ":", "Not calculated (Tol==0)")
  *         else:
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_5, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_5, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_3) {
 
-    /* "KKMeans.py":436
+    /* "KKMeans.py":435
  *             print("Converged at iteration:", iter + 1, self.q_metric + ":", quality)
  *         elif self.tol == 0:
  *             print("Iteration:", iter + 1, self.q_metric + ":", "Not calculated (Tol==0)")             # <<<<<<<<<<<<<<
  *         else:
  *             print("Iteration:", iter + 1, self.q_metric + ":", quality)
  */
-    __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_v_iter, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 436, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_v_iter, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 435, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u__16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 436, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u__16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_kp_u_Iteration);
     __Pyx_GIVEREF(__pyx_kp_u_Iteration);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_Iteration);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_1);
     __Pyx_INCREF(__pyx_kp_u_Not_calculated_Tol_0);
     __Pyx_GIVEREF(__pyx_kp_u_Not_calculated_Tol_0);
     PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_kp_u_Not_calculated_Tol_0);
     __pyx_t_5 = 0;
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 436, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "KKMeans.py":435
+    /* "KKMeans.py":434
  *         if converged:
  *             print("Converged at iteration:", iter + 1, self.q_metric + ":", quality)
  *         elif self.tol == 0:             # <<<<<<<<<<<<<<
  *             print("Iteration:", iter + 1, self.q_metric + ":", "Not calculated (Tol==0)")
  *         else:
  */
     goto __pyx_L4;
   }
 
-  /* "KKMeans.py":438
+  /* "KKMeans.py":437
  *             print("Iteration:", iter + 1, self.q_metric + ":", "Not calculated (Tol==0)")
  *         else:
  *             print("Iteration:", iter + 1, self.q_metric + ":", quality)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_iter, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_iter, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_u__16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_u__16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_kp_u_Iteration);
     __Pyx_GIVEREF(__pyx_kp_u_Iteration);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_Iteration);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_5);
     __Pyx_INCREF(__pyx_v_quality);
     __Pyx_GIVEREF(__pyx_v_quality);
     PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_v_quality);
     __pyx_t_1 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_L4:;
 
-  /* "KKMeans.py":429
+  /* "KKMeans.py":428
  * 
  * 
  *     def _out_verbose(self, iter, quality, converged):             # <<<<<<<<<<<<<<
  *         '''Checks if self.verbose and prints accordingly'''
  *         if not self.verbose:
  */
 
@@ -10249,15 +10132,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":441
+/* "KKMeans.py":440
  * 
  * 
  *     def _measure_iter(self, sq_distances, labels, labels_old, quality):             # <<<<<<<<<<<<<<
  *         '''
  *         Measures quality of iteration and checks for convergence
  */
 
@@ -10312,48 +10195,48 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sq_distances)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 1); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 1); __PYX_ERR(0, 440, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 2); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 2); __PYX_ERR(0, 440, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_old)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 3); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 3); __PYX_ERR(0, 440, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_quality_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 4); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, 4); __PYX_ERR(0, 440, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_measure_iter") < 0)) __PYX_ERR(0, 441, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_measure_iter") < 0)) __PYX_ERR(0, 440, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -10364,15 +10247,15 @@
     __pyx_v_sq_distances = values[1];
     __pyx_v_labels = values[2];
     __pyx_v_labels_old = values[3];
     __pyx_v_quality = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 441, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_measure_iter", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 440, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._measure_iter", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_40_measure_iter(__pyx_self, __pyx_v_self, __pyx_v_sq_distances, __pyx_v_labels, __pyx_v_labels_old, __pyx_v_quality);
 
@@ -10393,54 +10276,54 @@
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_measure_iter", 0);
   __Pyx_INCREF(__pyx_v_quality);
 
-  /* "KKMeans.py":469
+  /* "KKMeans.py":468
  *             is the algorithm converged?
  *         '''
  *         converged = False             # <<<<<<<<<<<<<<
  *         if self.tol != 0:
  *             quality_old = quality
  */
   __pyx_v_converged = 0;
 
-  /* "KKMeans.py":470
+  /* "KKMeans.py":469
  *         '''
  *         converged = False
  *         if self.tol != 0:             # <<<<<<<<<<<<<<
  *             quality_old = quality
  *             quality = self.calc_q_metric(sq_distances, labels)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyInt_BoolNeObjC(__pyx_t_1, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 470, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyInt_BoolNeObjC(__pyx_t_1, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 469, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "KKMeans.py":471
+    /* "KKMeans.py":470
  *         converged = False
  *         if self.tol != 0:
  *             quality_old = quality             # <<<<<<<<<<<<<<
  *             quality = self.calc_q_metric(sq_distances, labels)
  *             if abs(quality - quality_old) <= self.tol:
  */
     __Pyx_INCREF(__pyx_v_quality);
     __pyx_v_quality_old = __pyx_v_quality;
 
-    /* "KKMeans.py":472
+    /* "KKMeans.py":471
  *         if self.tol != 0:
  *             quality_old = quality
  *             quality = self.calc_q_metric(sq_distances, labels)             # <<<<<<<<<<<<<<
  *             if abs(quality - quality_old) <= self.tol:
  *                 converged = True
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calc_q_metric); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calc_q_metric); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 471, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -10450,105 +10333,105 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_sq_distances, __pyx_v_labels};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF_SET(__pyx_v_quality, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":473
+    /* "KKMeans.py":472
  *             quality_old = quality
  *             quality = self.calc_q_metric(sq_distances, labels)
  *             if abs(quality - quality_old) <= self.tol:             # <<<<<<<<<<<<<<
  *                 converged = True
  * 
  */
-    __pyx_t_1 = PyNumber_Subtract(__pyx_v_quality, __pyx_v_quality_old); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Subtract(__pyx_v_quality, __pyx_v_quality_old); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyNumber_Absolute(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyNumber_Absolute(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_1, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_1, Py_LE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_2) {
 
-      /* "KKMeans.py":474
+      /* "KKMeans.py":473
  *             quality = self.calc_q_metric(sq_distances, labels)
  *             if abs(quality - quality_old) <= self.tol:
  *                 converged = True             # <<<<<<<<<<<<<<
  * 
  *         if all(labels_old == labels):
  */
       __pyx_v_converged = 1;
 
-      /* "KKMeans.py":473
+      /* "KKMeans.py":472
  *             quality_old = quality
  *             quality = self.calc_q_metric(sq_distances, labels)
  *             if abs(quality - quality_old) <= self.tol:             # <<<<<<<<<<<<<<
  *                 converged = True
  * 
  */
     }
 
-    /* "KKMeans.py":470
+    /* "KKMeans.py":469
  *         '''
  *         converged = False
  *         if self.tol != 0:             # <<<<<<<<<<<<<<
  *             quality_old = quality
  *             quality = self.calc_q_metric(sq_distances, labels)
  */
   }
 
-  /* "KKMeans.py":476
+  /* "KKMeans.py":475
  *                 converged = True
  * 
  *         if all(labels_old == labels):             # <<<<<<<<<<<<<<
  *             if self.tol == 0:
  *                 quality = self.calc_q_metric(sq_distances, labels)
  */
-  __pyx_t_4 = PyObject_RichCompare(__pyx_v_labels_old, __pyx_v_labels, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 476, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_all, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_v_labels_old, __pyx_v_labels, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_all, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 475, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "KKMeans.py":477
+    /* "KKMeans.py":476
  * 
  *         if all(labels_old == labels):
  *             if self.tol == 0:             # <<<<<<<<<<<<<<
  *                 quality = self.calc_q_metric(sq_distances, labels)
  *             converged = True
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 477, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_tol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 477, __pyx_L1_error)
+    __pyx_t_2 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 476, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_2) {
 
-      /* "KKMeans.py":478
+      /* "KKMeans.py":477
  *         if all(labels_old == labels):
  *             if self.tol == 0:
  *                 quality = self.calc_q_metric(sq_distances, labels)             # <<<<<<<<<<<<<<
  *             converged = True
  * 
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calc_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calc_q_metric); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 477, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_3 = NULL;
       __pyx_t_5 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -10558,71 +10441,71 @@
           __pyx_t_5 = 1;
         }
       }
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_sq_distances, __pyx_v_labels};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 477, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __Pyx_DECREF_SET(__pyx_v_quality, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "KKMeans.py":477
+      /* "KKMeans.py":476
  * 
  *         if all(labels_old == labels):
  *             if self.tol == 0:             # <<<<<<<<<<<<<<
  *                 quality = self.calc_q_metric(sq_distances, labels)
  *             converged = True
  */
     }
 
-    /* "KKMeans.py":479
+    /* "KKMeans.py":478
  *             if self.tol == 0:
  *                 quality = self.calc_q_metric(sq_distances, labels)
  *             converged = True             # <<<<<<<<<<<<<<
  * 
  *         return quality, converged
  */
     __pyx_v_converged = 1;
 
-    /* "KKMeans.py":476
+    /* "KKMeans.py":475
  *                 converged = True
  * 
  *         if all(labels_old == labels):             # <<<<<<<<<<<<<<
  *             if self.tol == 0:
  *                 quality = self.calc_q_metric(sq_distances, labels)
  */
   }
 
-  /* "KKMeans.py":481
+  /* "KKMeans.py":480
  *             converged = True
  * 
  *         return quality, converged             # <<<<<<<<<<<<<<
  * 
  *     def calc_q_metric(self, sq_distances, labels):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_converged); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_converged); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 481, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_quality);
   __Pyx_GIVEREF(__pyx_v_quality);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_quality);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":441
+  /* "KKMeans.py":440
  * 
  * 
  *     def _measure_iter(self, sq_distances, labels, labels_old, quality):             # <<<<<<<<<<<<<<
  *         '''
  *         Measures quality of iteration and checks for convergence
  */
 
@@ -10637,15 +10520,15 @@
   __Pyx_XDECREF(__pyx_v_quality_old);
   __Pyx_XDECREF(__pyx_v_quality);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":483
+/* "KKMeans.py":482
  *         return quality, converged
  * 
  *     def calc_q_metric(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Calculates quality metric
  */
 
@@ -10694,49 +10577,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 482, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sq_distances)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 482, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("calc_q_metric", 1, 3, 3, 1); __PYX_ERR(0, 483, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calc_q_metric", 1, 3, 3, 1); __PYX_ERR(0, 482, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 482, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("calc_q_metric", 1, 3, 3, 2); __PYX_ERR(0, 483, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calc_q_metric", 1, 3, 3, 2); __PYX_ERR(0, 482, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_q_metric") < 0)) __PYX_ERR(0, 483, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_q_metric") < 0)) __PYX_ERR(0, 482, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_sq_distances = values[1];
     __pyx_v_labels = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calc_q_metric", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 483, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calc_q_metric", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 482, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.calc_q_metric", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_42calc_q_metric(__pyx_self, __pyx_v_self, __pyx_v_sq_distances, __pyx_v_labels);
 
@@ -10754,55 +10637,55 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calc_q_metric", 0);
 
-  /* "KKMeans.py":506
+  /* "KKMeans.py":505
  *         float, the calculated quality score
  *         '''
  *         if self.q_metric == "inertia":             # <<<<<<<<<<<<<<
  *             return sq_distances[range(sq_distances.shape[0]), labels].sum()
  *         elif self.q_metric == "silhouette":
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_inertia, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_inertia, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "KKMeans.py":507
+    /* "KKMeans.py":506
  *         '''
  *         if self.q_metric == "inertia":
  *             return sq_distances[range(sq_distances.shape[0]), labels].sum()             # <<<<<<<<<<<<<<
  *         elif self.q_metric == "silhouette":
  *             return self.calc_silhouette(sq_distances, labels)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_sq_distances, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_sq_distances, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_labels);
     __Pyx_GIVEREF(__pyx_v_labels);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_labels);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_sq_distances, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_sq_distances, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sum); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sum); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
@@ -10813,53 +10696,53 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[1] = {__pyx_t_3, };
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":506
+    /* "KKMeans.py":505
  *         float, the calculated quality score
  *         '''
  *         if self.q_metric == "inertia":             # <<<<<<<<<<<<<<
  *             return sq_distances[range(sq_distances.shape[0]), labels].sum()
  *         elif self.q_metric == "silhouette":
  */
   }
 
-  /* "KKMeans.py":508
+  /* "KKMeans.py":507
  *         if self.q_metric == "inertia":
  *             return sq_distances[range(sq_distances.shape[0]), labels].sum()
  *         elif self.q_metric == "silhouette":             # <<<<<<<<<<<<<<
  *             return self.calc_silhouette(sq_distances, labels)
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_silhouette, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_silhouette, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 507, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (likely(__pyx_t_2)) {
 
-    /* "KKMeans.py":509
+    /* "KKMeans.py":508
  *             return sq_distances[range(sq_distances.shape[0]), labels].sum()
  *         elif self.q_metric == "silhouette":
  *             return self.calc_silhouette(sq_distances, labels)             # <<<<<<<<<<<<<<
  *         else:
  *             raise NotImplementedError(str(self.q_metric) + " quality metric not implemented")
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calc_silhouette); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 509, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_calc_silhouette); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -10869,56 +10752,56 @@
         __pyx_t_5 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_sq_distances, __pyx_v_labels};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 509, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 508, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "KKMeans.py":508
+    /* "KKMeans.py":507
  *         if self.q_metric == "inertia":
  *             return sq_distances[range(sq_distances.shape[0]), labels].sum()
  *         elif self.q_metric == "silhouette":             # <<<<<<<<<<<<<<
  *             return self.calc_silhouette(sq_distances, labels)
  *         else:
  */
   }
 
-  /* "KKMeans.py":511
+  /* "KKMeans.py":510
  *             return self.calc_silhouette(sq_distances, labels)
  *         else:
  *             raise NotImplementedError(str(self.q_metric) + " quality metric not implemented")             # <<<<<<<<<<<<<<
  * 
  *     def calc_silhouette(self, sq_distances, labels):
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_q_metric); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_quality_metric_not_implemented); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_t_4, __pyx_kp_u_quality_metric_not_implemented); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 511, __pyx_L1_error)
+    __PYX_ERR(0, 510, __pyx_L1_error)
   }
 
-  /* "KKMeans.py":483
+  /* "KKMeans.py":482
  *         return quality, converged
  * 
  *     def calc_q_metric(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Calculates quality metric
  */
 
@@ -10931,15 +10814,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":513
+/* "KKMeans.py":512
  *             raise NotImplementedError(str(self.q_metric) + " quality metric not implemented")
  * 
  *     def calc_silhouette(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''Calculates average silhouette of clustering
  * 
  */
 
@@ -10988,49 +10871,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sq_distances)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("calc_silhouette", 1, 3, 3, 1); __PYX_ERR(0, 513, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calc_silhouette", 1, 3, 3, 1); __PYX_ERR(0, 512, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("calc_silhouette", 1, 3, 3, 2); __PYX_ERR(0, 513, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calc_silhouette", 1, 3, 3, 2); __PYX_ERR(0, 512, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_silhouette") < 0)) __PYX_ERR(0, 513, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_silhouette") < 0)) __PYX_ERR(0, 512, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_sq_distances = values[1];
     __pyx_v_labels = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calc_silhouette", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 513, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calc_silhouette", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 512, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.calc_silhouette", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_44calc_silhouette(__pyx_self, __pyx_v_self, __pyx_v_sq_distances, __pyx_v_labels);
 
@@ -11047,23 +10930,23 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calc_silhouette", 0);
 
-  /* "KKMeans.py":530
+  /* "KKMeans.py":529
  *         Average silhouette of each datapoint
  *         '''
  *         return avg_silhouette(sq_distances, labels)             # <<<<<<<<<<<<<<
  * 
  *     def _build_starting_distance(self, kernel_matrix):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_avg_silhouette); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 530, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_avg_silhouette); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 529, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -11073,23 +10956,23 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_sq_distances, __pyx_v_labels};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 530, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 529, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":513
+  /* "KKMeans.py":512
  *             raise NotImplementedError(str(self.q_metric) + " quality metric not implemented")
  * 
  *     def calc_silhouette(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''Calculates average silhouette of clustering
  * 
  */
 
@@ -11102,15 +10985,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":532
+/* "KKMeans.py":531
  *         return avg_silhouette(sq_distances, labels)
  * 
  *     def _build_starting_distance(self, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Builds basis for computing square distances
  */
 
@@ -11156,40 +11039,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 532, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 532, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 531, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_build_starting_distance", 1, 2, 2, 1); __PYX_ERR(0, 532, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_build_starting_distance", 1, 2, 2, 1); __PYX_ERR(0, 531, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_build_starting_distance") < 0)) __PYX_ERR(0, 532, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_build_starting_distance") < 0)) __PYX_ERR(0, 531, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_kernel_matrix = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_build_starting_distance", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 532, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_build_starting_distance", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 531, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans._build_starting_distance", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_46_build_starting_distance(__pyx_self, __pyx_v_self, __pyx_v_kernel_matrix);
 
@@ -11209,35 +11092,35 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_build_starting_distance", 0);
 
-  /* "KKMeans.py":545
+  /* "KKMeans.py":544
  *         # ascontiguousarray is necessary as by transposing ndarray becomes f-ordered
  *         # c-order is necessary for cython.
  *         return np.ascontiguousarray(np.tile(np.diag(kernel_matrix), (self.n_clusters, 1)).T, dtype=np.double)             # <<<<<<<<<<<<<<
  * 
  *     def elkan(self, kernel_matrix, labels):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_tile); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_tile); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_diag); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_diag); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
@@ -11248,21 +11131,21 @@
       __pyx_t_7 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_kernel_matrix};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_int_1);
   __pyx_t_6 = 0;
@@ -11280,45 +11163,45 @@
   }
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_3, __pyx_t_5};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 545, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_T); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_T); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_double); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 545, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 544, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":532
+  /* "KKMeans.py":531
  *         return avg_silhouette(sq_distances, labels)
  * 
  *     def _build_starting_distance(self, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Builds basis for computing square distances
  */
 
@@ -11334,15 +11217,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":547
+/* "KKMeans.py":546
  *         return np.ascontiguousarray(np.tile(np.diag(kernel_matrix), (self.n_clusters, 1)).T, dtype=np.double)
  * 
  *     def elkan(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a slightly optimized Kernel-Kmeans heuristic
  */
 
@@ -11391,49 +11274,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 547, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 546, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 547, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 546, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("elkan", 1, 3, 3, 1); __PYX_ERR(0, 547, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("elkan", 1, 3, 3, 1); __PYX_ERR(0, 546, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 547, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 546, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("elkan", 1, 3, 3, 2); __PYX_ERR(0, 547, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("elkan", 1, 3, 3, 2); __PYX_ERR(0, 546, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elkan") < 0)) __PYX_ERR(0, 547, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "elkan") < 0)) __PYX_ERR(0, 546, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_kernel_matrix = values[1];
     __pyx_v_labels = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("elkan", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 547, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("elkan", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 546, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.elkan", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_48elkan(__pyx_self, __pyx_v_self, __pyx_v_kernel_matrix, __pyx_v_labels);
 
@@ -11469,56 +11352,56 @@
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("elkan", 0);
   __Pyx_INCREF(__pyx_v_labels);
 
-  /* "KKMeans.py":575
+  /* "KKMeans.py":574
  *                 returned to ease prediction
  *         '''
  *         labels = np.array(labels, dtype=np.int_)             # <<<<<<<<<<<<<<
  *         start_dists = self._build_starting_distance(kernel_matrix)
  *         center_dists = np.zeros((kernel_matrix.shape[0], self.n_clusters))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_labels);
   __Pyx_GIVEREF(__pyx_v_labels);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_labels);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 574, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":576
+  /* "KKMeans.py":575
  *         '''
  *         labels = np.array(labels, dtype=np.int_)
  *         start_dists = self._build_starting_distance(kernel_matrix)             # <<<<<<<<<<<<<<
  *         center_dists = np.zeros((kernel_matrix.shape[0], self.n_clusters))
  *         quality = 0
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_build_starting_distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_build_starting_distance); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11528,41 +11411,41 @@
       __pyx_t_6 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_kernel_matrix};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 576, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 575, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_start_dists = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":577
+  /* "KKMeans.py":576
  *         labels = np.array(labels, dtype=np.int_)
  *         start_dists = self._build_starting_distance(kernel_matrix)
  *         center_dists = np.zeros((kernel_matrix.shape[0], self.n_clusters))             # <<<<<<<<<<<<<<
  *         quality = 0
  *         for it in range(self.max_iter):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_kernel_matrix, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_kernel_matrix, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
@@ -11579,195 +11462,195 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 577, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 576, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_v_center_dists = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "KKMeans.py":578
+  /* "KKMeans.py":577
  *         start_dists = self._build_starting_distance(kernel_matrix)
  *         center_dists = np.zeros((kernel_matrix.shape[0], self.n_clusters))
  *         quality = 0             # <<<<<<<<<<<<<<
  *         for it in range(self.max_iter):
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_quality = __pyx_int_0;
 
-  /* "KKMeans.py":579
+  /* "KKMeans.py":578
  *         center_dists = np.zeros((kernel_matrix.shape[0], self.n_clusters))
  *         quality = 0
  *         for it in range(self.max_iter):             # <<<<<<<<<<<<<<
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             if it == 0:
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 579, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_iter); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_5 = __pyx_t_1; __Pyx_INCREF(__pyx_t_5); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 578, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 579, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 578, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 578, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 579, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_1); __pyx_t_7++; if (unlikely((0 < 0))) __PYX_ERR(0, 578, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 578, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_8(__pyx_t_5);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 579, __pyx_L1_error)
+          else __PYX_ERR(0, 578, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_it, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":580
+    /* "KKMeans.py":579
  *         quality = 0
  *         for it in range(self.max_iter):
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)             # <<<<<<<<<<<<<<
  *             if it == 0:
  *                 l_bounds, inner_sums, sizes = start_elkan(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_fill_empty_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_fill_empty_clusters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 580, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_labels);
     __Pyx_GIVEREF(__pyx_v_labels);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_labels);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_rng, __pyx_t_2) < 0) __PYX_ERR(0, 580, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_rng, __pyx_t_2) < 0) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
       PyObject* sequence = __pyx_t_2;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 580, __pyx_L1_error)
+        __PYX_ERR(0, 579, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 579, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 580, __pyx_L1_error)
+      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 579, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       #endif
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
+      __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1);
       index = 0; __pyx_t_4 = __pyx_t_9(__pyx_t_1); if (unlikely(!__pyx_t_4)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
       index = 1; __pyx_t_3 = __pyx_t_9(__pyx_t_1); if (unlikely(!__pyx_t_3)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_3);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_1), 2) < 0) __PYX_ERR(0, 580, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_1), 2) < 0) __PYX_ERR(0, 579, __pyx_L1_error)
       __pyx_t_9 = NULL;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_9 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 580, __pyx_L1_error)
+      __PYX_ERR(0, 579, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
     __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_sizes, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "KKMeans.py":581
+    /* "KKMeans.py":580
  *         for it in range(self.max_iter):
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             if it == 0:             # <<<<<<<<<<<<<<
  *                 l_bounds, inner_sums, sizes = start_elkan(
  *                     start_dists, kernel_matrix, labels,
  */
-    __pyx_t_10 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_it, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 581, __pyx_L1_error)
+    __pyx_t_10 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_it, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 580, __pyx_L1_error)
     if (__pyx_t_10) {
 
-      /* "KKMeans.py":582
+      /* "KKMeans.py":581
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             if it == 0:
  *                 l_bounds, inner_sums, sizes = start_elkan(             # <<<<<<<<<<<<<<
  *                     start_dists, kernel_matrix, labels,
  *                     self.n_clusters, sizes)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_start_elkan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_start_elkan); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 581, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
 
-      /* "KKMeans.py":584
+      /* "KKMeans.py":583
  *                 l_bounds, inner_sums, sizes = start_elkan(
  *                     start_dists, kernel_matrix, labels,
  *                     self.n_clusters, sizes)             # <<<<<<<<<<<<<<
  *             else:
  *                 l_bounds, inner_sums, sizes, center_dists = update_elkan(
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 584, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 583, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_1 = NULL;
       __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11778,25 +11661,25 @@
         }
       }
       {
         PyObject *__pyx_callargs[6] = {__pyx_t_1, __pyx_v_start_dists, __pyx_v_kernel_matrix, __pyx_v_labels, __pyx_t_4, __pyx_v_sizes};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 5+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 581, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
         PyObject* sequence = __pyx_t_2;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 3)) {
           if (size > 3) __Pyx_RaiseTooManyValuesError(3);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 582, __pyx_L1_error)
+          __PYX_ERR(0, 581, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_1 = PyTuple_GET_ITEM(sequence, 2); 
         } else {
@@ -11804,109 +11687,109 @@
           __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
           __pyx_t_1 = PyList_GET_ITEM(sequence, 2); 
         }
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         #else
-        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 581, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 582, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 581, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 582, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 581, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_11 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 582, __pyx_L1_error)
+        __pyx_t_11 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 581, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_11);
         index = 0; __pyx_t_3 = __pyx_t_9(__pyx_t_11); if (unlikely(!__pyx_t_3)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_3);
         index = 1; __pyx_t_4 = __pyx_t_9(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_4);
         index = 2; __pyx_t_1 = __pyx_t_9(__pyx_t_11); if (unlikely(!__pyx_t_1)) goto __pyx_L8_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_1);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_11), 3) < 0) __PYX_ERR(0, 582, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_11), 3) < 0) __PYX_ERR(0, 581, __pyx_L1_error)
         __pyx_t_9 = NULL;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         goto __pyx_L9_unpacking_done;
         __pyx_L8_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __pyx_t_9 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 582, __pyx_L1_error)
+        __PYX_ERR(0, 581, __pyx_L1_error)
         __pyx_L9_unpacking_done:;
       }
 
-      /* "KKMeans.py":582
+      /* "KKMeans.py":581
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             if it == 0:
  *                 l_bounds, inner_sums, sizes = start_elkan(             # <<<<<<<<<<<<<<
  *                     start_dists, kernel_matrix, labels,
  *                     self.n_clusters, sizes)
  */
       __Pyx_XDECREF_SET(__pyx_v_l_bounds, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_inner_sums, __pyx_t_4);
       __pyx_t_4 = 0;
       __Pyx_DECREF_SET(__pyx_v_sizes, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "KKMeans.py":581
+      /* "KKMeans.py":580
  *         for it in range(self.max_iter):
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             if it == 0:             # <<<<<<<<<<<<<<
  *                 l_bounds, inner_sums, sizes = start_elkan(
  *                     start_dists, kernel_matrix, labels,
  */
       goto __pyx_L7;
     }
 
-    /* "KKMeans.py":586
+    /* "KKMeans.py":585
  *                     self.n_clusters, sizes)
  *             else:
  *                 l_bounds, inner_sums, sizes, center_dists = update_elkan(             # <<<<<<<<<<<<<<
  *                     kernel_matrix, l_bounds, center_dists,
  *                     labels, labels_old, sizes, sizes_old,
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_update_elkan); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_update_elkan); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 585, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "KKMeans.py":587
+      /* "KKMeans.py":586
  *             else:
  *                 l_bounds, inner_sums, sizes, center_dists = update_elkan(
  *                     kernel_matrix, l_bounds, center_dists,             # <<<<<<<<<<<<<<
  *                     labels, labels_old, sizes, sizes_old,
  *                     inner_sums, self.n_clusters)
  */
-      if (unlikely(!__pyx_v_l_bounds)) { __Pyx_RaiseUnboundLocalError("l_bounds"); __PYX_ERR(0, 587, __pyx_L1_error) }
+      if (unlikely(!__pyx_v_l_bounds)) { __Pyx_RaiseUnboundLocalError("l_bounds"); __PYX_ERR(0, 586, __pyx_L1_error) }
 
-      /* "KKMeans.py":588
+      /* "KKMeans.py":587
  *                 l_bounds, inner_sums, sizes, center_dists = update_elkan(
  *                     kernel_matrix, l_bounds, center_dists,
  *                     labels, labels_old, sizes, sizes_old,             # <<<<<<<<<<<<<<
  *                     inner_sums, self.n_clusters)
  * 
  */
-      if (unlikely(!__pyx_v_labels_old)) { __Pyx_RaiseUnboundLocalError("labels_old"); __PYX_ERR(0, 588, __pyx_L1_error) }
-      if (unlikely(!__pyx_v_sizes_old)) { __Pyx_RaiseUnboundLocalError("sizes_old"); __PYX_ERR(0, 588, __pyx_L1_error) }
+      if (unlikely(!__pyx_v_labels_old)) { __Pyx_RaiseUnboundLocalError("labels_old"); __PYX_ERR(0, 587, __pyx_L1_error) }
+      if (unlikely(!__pyx_v_sizes_old)) { __Pyx_RaiseUnboundLocalError("sizes_old"); __PYX_ERR(0, 587, __pyx_L1_error) }
 
-      /* "KKMeans.py":589
+      /* "KKMeans.py":588
  *                     kernel_matrix, l_bounds, center_dists,
  *                     labels, labels_old, sizes, sizes_old,
  *                     inner_sums, self.n_clusters)             # <<<<<<<<<<<<<<
  * 
  *             labels_old = labels
  */
-      if (unlikely(!__pyx_v_inner_sums)) { __Pyx_RaiseUnboundLocalError("inner_sums"); __PYX_ERR(0, 589, __pyx_L1_error) }
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 589, __pyx_L1_error)
+      if (unlikely(!__pyx_v_inner_sums)) { __Pyx_RaiseUnboundLocalError("inner_sums"); __PYX_ERR(0, 588, __pyx_L1_error) }
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 588, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_3 = NULL;
       __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -11917,25 +11800,25 @@
         }
       }
       {
         PyObject *__pyx_callargs[10] = {__pyx_t_3, __pyx_v_kernel_matrix, __pyx_v_l_bounds, __pyx_v_center_dists, __pyx_v_labels, __pyx_v_labels_old, __pyx_v_sizes, __pyx_v_sizes_old, __pyx_v_inner_sums, __pyx_t_4};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_6, 9+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 585, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
         PyObject* sequence = __pyx_t_2;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 4)) {
           if (size > 4) __Pyx_RaiseTooManyValuesError(4);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 586, __pyx_L1_error)
+          __PYX_ERR(0, 585, __pyx_L1_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
           __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
           __pyx_t_11 = PyTuple_GET_ITEM(sequence, 3); 
@@ -11950,46 +11833,46 @@
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_11);
         #else
         {
           Py_ssize_t i;
           PyObject** temps[4] = {&__pyx_t_1,&__pyx_t_4,&__pyx_t_3,&__pyx_t_11};
           for (i=0; i < 4; i++) {
-            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 586, __pyx_L1_error)
+            PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(0, 585, __pyx_L1_error)
             __Pyx_GOTREF(item);
             *(temps[i]) = item;
           }
         }
         #endif
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else {
         Py_ssize_t index = -1;
         PyObject** temps[4] = {&__pyx_t_1,&__pyx_t_4,&__pyx_t_3,&__pyx_t_11};
-        __pyx_t_12 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 586, __pyx_L1_error)
+        __pyx_t_12 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 585, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_12);
         for (index=0; index < 4; index++) {
           PyObject* item = __pyx_t_9(__pyx_t_12); if (unlikely(!item)) goto __pyx_L10_unpacking_failed;
           __Pyx_GOTREF(item);
           *(temps[index]) = item;
         }
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_12), 4) < 0) __PYX_ERR(0, 586, __pyx_L1_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_12), 4) < 0) __PYX_ERR(0, 585, __pyx_L1_error)
         __pyx_t_9 = NULL;
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         goto __pyx_L11_unpacking_done;
         __pyx_L10_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __pyx_t_9 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 586, __pyx_L1_error)
+        __PYX_ERR(0, 585, __pyx_L1_error)
         __pyx_L11_unpacking_done:;
       }
 
-      /* "KKMeans.py":586
+      /* "KKMeans.py":585
  *                     self.n_clusters, sizes)
  *             else:
  *                 l_bounds, inner_sums, sizes, center_dists = update_elkan(             # <<<<<<<<<<<<<<
  *                     kernel_matrix, l_bounds, center_dists,
  *                     labels, labels_old, sizes, sizes_old,
  */
       __Pyx_XDECREF_SET(__pyx_v_l_bounds, __pyx_t_1);
@@ -11999,84 +11882,84 @@
       __Pyx_DECREF_SET(__pyx_v_sizes, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_DECREF_SET(__pyx_v_center_dists, __pyx_t_11);
       __pyx_t_11 = 0;
     }
     __pyx_L7:;
 
-    /* "KKMeans.py":591
+    /* "KKMeans.py":590
  *                     inner_sums, self.n_clusters)
  * 
  *             labels_old = labels             # <<<<<<<<<<<<<<
  *             labels = np.array(np.argmin(l_bounds, axis=1), dtype=np.int_)
  *             quality, converged = self._measure_iter(l_bounds, labels, labels_old, quality)
  */
     __Pyx_INCREF(__pyx_v_labels);
     __Pyx_XDECREF_SET(__pyx_v_labels_old, __pyx_v_labels);
 
-    /* "KKMeans.py":592
+    /* "KKMeans.py":591
  * 
  *             labels_old = labels
  *             labels = np.array(np.argmin(l_bounds, axis=1), dtype=np.int_)             # <<<<<<<<<<<<<<
  *             quality, converged = self._measure_iter(l_bounds, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_argmin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_argmin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_l_bounds);
     __Pyx_GIVEREF(__pyx_v_l_bounds);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_l_bounds);
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 591, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_labels, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "KKMeans.py":593
+    /* "KKMeans.py":592
  *             labels_old = labels
  *             labels = np.array(np.argmin(l_bounds, axis=1), dtype=np.int_)
  *             quality, converged = self._measure_iter(l_bounds, labels, labels_old, quality)             # <<<<<<<<<<<<<<
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_measure_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_measure_iter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -12086,160 +11969,160 @@
         __pyx_t_6 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[5] = {__pyx_t_4, __pyx_v_l_bounds, __pyx_v_labels, __pyx_v_labels_old, __pyx_v_quality};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 593, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 593, __pyx_L1_error)
+        __PYX_ERR(0, 592, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_4);
       #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 593, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_11 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 593, __pyx_L1_error)
+      __pyx_t_11 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 592, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_11);
       index = 0; __pyx_t_1 = __pyx_t_9(__pyx_t_11); if (unlikely(!__pyx_t_1)) goto __pyx_L12_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_1);
       index = 1; __pyx_t_4 = __pyx_t_9(__pyx_t_11); if (unlikely(!__pyx_t_4)) goto __pyx_L12_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_11), 2) < 0) __PYX_ERR(0, 593, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_11), 2) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
       __pyx_t_9 = NULL;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       goto __pyx_L13_unpacking_done;
       __pyx_L12_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_9 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 593, __pyx_L1_error)
+      __PYX_ERR(0, 592, __pyx_L1_error)
       __pyx_L13_unpacking_done:;
     }
     __Pyx_DECREF_SET(__pyx_v_quality, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_XDECREF_SET(__pyx_v_converged, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "KKMeans.py":594
+    /* "KKMeans.py":593
  *             labels = np.array(np.argmin(l_bounds, axis=1), dtype=np.int_)
  *             quality, converged = self._measure_iter(l_bounds, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)             # <<<<<<<<<<<<<<
  *             if converged:
  *                 break
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_out_verbose); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 594, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_out_verbose); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 594, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_it);
     __Pyx_GIVEREF(__pyx_v_it);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_it);
     __Pyx_INCREF(__pyx_v_quality);
     __Pyx_GIVEREF(__pyx_v_quality);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_quality);
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 594, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_converged, __pyx_v_converged) < 0) __PYX_ERR(0, 594, __pyx_L1_error)
-    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 594, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_converged, __pyx_v_converged) < 0) __PYX_ERR(0, 593, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-    /* "KKMeans.py":595
+    /* "KKMeans.py":594
  *             quality, converged = self._measure_iter(l_bounds, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:             # <<<<<<<<<<<<<<
  *                 break
  *             sizes_old = sizes
  */
-    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_v_converged); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 595, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_v_converged); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 594, __pyx_L1_error)
     if (__pyx_t_10) {
 
-      /* "KKMeans.py":596
+      /* "KKMeans.py":595
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:
  *                 break             # <<<<<<<<<<<<<<
  *             sizes_old = sizes
  *         return labels, quality, inner_sums, sizes
  */
       goto __pyx_L4_break;
 
-      /* "KKMeans.py":595
+      /* "KKMeans.py":594
  *             quality, converged = self._measure_iter(l_bounds, labels, labels_old, quality)
  *             self._out_verbose(it, quality, converged=converged)
  *             if converged:             # <<<<<<<<<<<<<<
  *                 break
  *             sizes_old = sizes
  */
     }
 
-    /* "KKMeans.py":597
+    /* "KKMeans.py":596
  *             if converged:
  *                 break
  *             sizes_old = sizes             # <<<<<<<<<<<<<<
  *         return labels, quality, inner_sums, sizes
  * 
  */
     __Pyx_INCREF(__pyx_v_sizes);
     __Pyx_XDECREF_SET(__pyx_v_sizes_old, __pyx_v_sizes);
 
-    /* "KKMeans.py":579
+    /* "KKMeans.py":578
  *         center_dists = np.zeros((kernel_matrix.shape[0], self.n_clusters))
  *         quality = 0
  *         for it in range(self.max_iter):             # <<<<<<<<<<<<<<
  *             labels, sizes = fill_empty_clusters(labels, self.n_clusters, rng=self.rng)
  *             if it == 0:
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   goto __pyx_L15_for_end;
   __pyx_L4_break:;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   goto __pyx_L15_for_end;
   __pyx_L15_for_end:;
 
-  /* "KKMeans.py":598
+  /* "KKMeans.py":597
  *                 break
  *             sizes_old = sizes
  *         return labels, quality, inner_sums, sizes             # <<<<<<<<<<<<<<
  * 
  *     def kmeanspp(self, X, kernel_matrix):
  */
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_inner_sums)) { __Pyx_RaiseUnboundLocalError("inner_sums"); __PYX_ERR(0, 598, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_sizes)) { __Pyx_RaiseUnboundLocalError("sizes"); __PYX_ERR(0, 598, __pyx_L1_error) }
-  __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 598, __pyx_L1_error)
+  if (unlikely(!__pyx_v_inner_sums)) { __Pyx_RaiseUnboundLocalError("inner_sums"); __PYX_ERR(0, 597, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_sizes)) { __Pyx_RaiseUnboundLocalError("sizes"); __PYX_ERR(0, 597, __pyx_L1_error) }
+  __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 597, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_labels);
   __Pyx_GIVEREF(__pyx_v_labels);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_labels);
   __Pyx_INCREF(__pyx_v_quality);
   __Pyx_GIVEREF(__pyx_v_quality);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_quality);
@@ -12249,15 +12132,15 @@
   __Pyx_INCREF(__pyx_v_sizes);
   __Pyx_GIVEREF(__pyx_v_sizes);
   PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_v_sizes);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":547
+  /* "KKMeans.py":546
  *         return np.ascontiguousarray(np.tile(np.diag(kernel_matrix), (self.n_clusters, 1)).T, dtype=np.double)
  * 
  *     def elkan(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a slightly optimized Kernel-Kmeans heuristic
  */
 
@@ -12285,15 +12168,15 @@
   __Pyx_XDECREF(__pyx_v_sizes_old);
   __Pyx_XDECREF(__pyx_v_labels);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":600
+/* "KKMeans.py":599
  *         return labels, quality, inner_sums, sizes
  * 
  *     def kmeanspp(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes heuristic to get good initial centers
  */
 
@@ -12342,49 +12225,49 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 600, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 599, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_X_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 600, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 599, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("kmeanspp", 1, 3, 3, 1); __PYX_ERR(0, 600, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("kmeanspp", 1, 3, 3, 1); __PYX_ERR(0, 599, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kernel_matrix)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 600, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 599, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("kmeanspp", 1, 3, 3, 2); __PYX_ERR(0, 600, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("kmeanspp", 1, 3, 3, 2); __PYX_ERR(0, 599, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "kmeanspp") < 0)) __PYX_ERR(0, 600, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "kmeanspp") < 0)) __PYX_ERR(0, 599, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v_self = values[0];
     __pyx_v_X = values[1];
     __pyx_v_kernel_matrix = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("kmeanspp", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 600, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("kmeanspp", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 599, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.kmeanspp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_50kmeanspp(__pyx_self, __pyx_v_self, __pyx_v_X, __pyx_v_kernel_matrix);
 
@@ -12416,22 +12299,22 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("kmeanspp", 0);
 
-  /* "KKMeans.py":633
+  /* "KKMeans.py":632
  *         '''
  *         #those will be square dists
  *         dists_to_centers = self._build_starting_distance(kernel_matrix)             # <<<<<<<<<<<<<<
  *         n_samples = X.shape[0]
  *         for cluster in range(self.n_clusters):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_build_starting_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_build_starting_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12441,187 +12324,187 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_kernel_matrix};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 632, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_dists_to_centers = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "KKMeans.py":634
+  /* "KKMeans.py":633
  *         #those will be square dists
  *         dists_to_centers = self._build_starting_distance(kernel_matrix)
  *         n_samples = X.shape[0]             # <<<<<<<<<<<<<<
  *         for cluster in range(self.n_clusters):
  *             if cluster == 0:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_X, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 633, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_n_samples = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "KKMeans.py":635
+  /* "KKMeans.py":634
  *         dists_to_centers = self._build_starting_distance(kernel_matrix)
  *         n_samples = X.shape[0]
  *         for cluster in range(self.n_clusters):             # <<<<<<<<<<<<<<
  *             if cluster == 0:
  *                 # choose first center randomly
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 635, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 634, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 635, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 634, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 635, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 634, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 635, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_6(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 635, __pyx_L1_error)
+          else __PYX_ERR(0, 634, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_cluster, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":636
+    /* "KKMeans.py":635
  *         n_samples = X.shape[0]
  *         for cluster in range(self.n_clusters):
  *             if cluster == 0:             # <<<<<<<<<<<<<<
  *                 # choose first center randomly
  *                 index = self.rng.integers(low=0, high=n_samples)
  */
-    __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_cluster, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 636, __pyx_L1_error)
+    __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_v_cluster, __pyx_int_0, 0, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 635, __pyx_L1_error)
     if (__pyx_t_7) {
 
-      /* "KKMeans.py":638
+      /* "KKMeans.py":637
  *             if cluster == 0:
  *                 # choose first center randomly
  *                 index = self.rng.integers(low=0, high=n_samples)             # <<<<<<<<<<<<<<
  *             else:
  *                 # careful, dists_to_centers not initialized with 0
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 638, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_integers); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 638, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_integers); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 637, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 638, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_low, __pyx_int_0) < 0) __PYX_ERR(0, 638, __pyx_L1_error)
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_high, __pyx_v_n_samples) < 0) __PYX_ERR(0, 638, __pyx_L1_error)
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 638, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_low, __pyx_int_0) < 0) __PYX_ERR(0, 637, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_high, __pyx_v_n_samples) < 0) __PYX_ERR(0, 637, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 637, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_8);
       __pyx_t_8 = 0;
 
-      /* "KKMeans.py":636
+      /* "KKMeans.py":635
  *         n_samples = X.shape[0]
  *         for cluster in range(self.n_clusters):
  *             if cluster == 0:             # <<<<<<<<<<<<<<
  *                 # choose first center randomly
  *                 index = self.rng.integers(low=0, high=n_samples)
  */
       goto __pyx_L5;
     }
 
-    /* "KKMeans.py":641
+    /* "KKMeans.py":640
  *             else:
  *                 # careful, dists_to_centers not initialized with 0
  *                 min_dist_each = np.amin(dists_to_centers[:, :cluster + 1], axis = 1)             # <<<<<<<<<<<<<<
  *                 probs = min_dist_each/min_dist_each.sum()
  *                 index = self.rng.choice(n_samples, size=1, p=probs)
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_amin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_amin); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_PyInt_AddObjC(__pyx_v_cluster, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_AddObjC(__pyx_v_cluster, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_3 = PySlice_New(Py_None, __pyx_t_8, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_3 = PySlice_New(Py_None, __pyx_t_8, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_slice__21);
       __Pyx_GIVEREF(__pyx_slice__21);
       PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_slice__21);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_3);
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_dists_to_centers, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_dists_to_centers, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3);
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 641, __pyx_L1_error)
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_8, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 641, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_8, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 640, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF_SET(__pyx_v_min_dist_each, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "KKMeans.py":642
+      /* "KKMeans.py":641
  *                 # careful, dists_to_centers not initialized with 0
  *                 min_dist_each = np.amin(dists_to_centers[:, :cluster + 1], axis = 1)
  *                 probs = min_dist_each/min_dist_each.sum()             # <<<<<<<<<<<<<<
  *                 index = self.rng.choice(n_samples, size=1, p=probs)
  *             center = X[index]
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_min_dist_each, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_min_dist_each, __pyx_n_s_sum); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_8 = NULL;
       __pyx_t_4 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -12631,75 +12514,75 @@
           __pyx_t_4 = 1;
         }
       }
       {
         PyObject *__pyx_callargs[1] = {__pyx_t_8, };
         __pyx_t_9 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 642, __pyx_L1_error)
+        if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 641, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_v_min_dist_each, __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_v_min_dist_each, __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_XDECREF_SET(__pyx_v_probs, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "KKMeans.py":643
+      /* "KKMeans.py":642
  *                 min_dist_each = np.amin(dists_to_centers[:, :cluster + 1], axis = 1)
  *                 probs = min_dist_each/min_dist_each.sum()
  *                 index = self.rng.choice(n_samples, size=1, p=probs)             # <<<<<<<<<<<<<<
  *             center = X[index]
  *             inner_sum = self.kernel_wrapper(center)
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 643, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rng); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 643, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_choice); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 642, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 643, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_INCREF(__pyx_v_n_samples);
       __Pyx_GIVEREF(__pyx_v_n_samples);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_n_samples);
-      __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 643, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 642, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_size, __pyx_int_1) < 0) __PYX_ERR(0, 643, __pyx_L1_error)
-      if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_p, __pyx_v_probs) < 0) __PYX_ERR(0, 643, __pyx_L1_error)
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_3, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 643, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_size, __pyx_int_1) < 0) __PYX_ERR(0, 642, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_p, __pyx_v_probs) < 0) __PYX_ERR(0, 642, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_3, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_1);
       __pyx_t_1 = 0;
     }
     __pyx_L5:;
 
-    /* "KKMeans.py":644
+    /* "KKMeans.py":643
  *                 probs = min_dist_each/min_dist_each.sum()
  *                 index = self.rng.choice(n_samples, size=1, p=probs)
  *             center = X[index]             # <<<<<<<<<<<<<<
  *             inner_sum = self.kernel_wrapper(center)
  *             outer_sum = self.kernel_wrapper(X, center)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_X, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 644, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_X, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 643, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_center, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":645
+    /* "KKMeans.py":644
  *                 index = self.rng.choice(n_samples, size=1, p=probs)
  *             center = X[index]
  *             inner_sum = self.kernel_wrapper(center)             # <<<<<<<<<<<<<<
  *             outer_sum = self.kernel_wrapper(X, center)
  *             # reshape necessary as kernel_wrapper has 2dim array output
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 645, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 644, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -12709,29 +12592,29 @@
         __pyx_t_4 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_center};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 644, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_inner_sum, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":646
+    /* "KKMeans.py":645
  *             center = X[index]
  *             inner_sum = self.kernel_wrapper(center)
  *             outer_sum = self.kernel_wrapper(X, center)             # <<<<<<<<<<<<<<
  *             # reshape necessary as kernel_wrapper has 2dim array output
  *             dists_to_centers[:, cluster] += (-2 * outer_sum + inner_sum).reshape(n_samples,)
  */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 646, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 645, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
@@ -12741,44 +12624,44 @@
         __pyx_t_4 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_X, __pyx_v_center};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 646, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v_outer_sum, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "KKMeans.py":648
+    /* "KKMeans.py":647
  *             outer_sum = self.kernel_wrapper(X, center)
  *             # reshape necessary as kernel_wrapper has 2dim array output
  *             dists_to_centers[:, cluster] += (-2 * outer_sum + inner_sum).reshape(n_samples,)             # <<<<<<<<<<<<<<
  *             # eliminate flop errors
  *             dists_to_centers[np.isclose(dists_to_centers, 0)] = 0
  */
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 647, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_slice__21);
     __Pyx_GIVEREF(__pyx_slice__21);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_slice__21);
     __Pyx_INCREF(__pyx_v_cluster);
     __Pyx_GIVEREF(__pyx_v_cluster);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_cluster);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_dists_to_centers, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_dists_to_centers, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 647, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_2, __pyx_v_outer_sum, -2L, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyInt_MultiplyCObj(__pyx_int_neg_2, __pyx_v_outer_sum, -2L, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 647, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = PyNumber_Add(__pyx_t_9, __pyx_v_inner_sum); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_10 = PyNumber_Add(__pyx_t_9, __pyx_v_inner_sum); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 647, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_reshape); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_reshape); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 647, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_t_10 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_10)) {
@@ -12789,36 +12672,36 @@
         __pyx_t_4 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_v_n_samples};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 648, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 647, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
-    __pyx_t_9 = PyNumber_InPlaceAdd(__pyx_t_8, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 648, __pyx_L1_error)
+    __pyx_t_9 = PyNumber_InPlaceAdd(__pyx_t_8, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 647, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely((PyObject_SetItem(__pyx_v_dists_to_centers, __pyx_t_1, __pyx_t_9) < 0))) __PYX_ERR(0, 648, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_dists_to_centers, __pyx_t_1, __pyx_t_9) < 0))) __PYX_ERR(0, 647, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "KKMeans.py":650
+    /* "KKMeans.py":649
  *             dists_to_centers[:, cluster] += (-2 * outer_sum + inner_sum).reshape(n_samples,)
  *             # eliminate flop errors
  *             dists_to_centers[np.isclose(dists_to_centers, 0)] = 0             # <<<<<<<<<<<<<<
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 650, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 649, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isclose); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 650, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_isclose); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 649, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = NULL;
     __pyx_t_4 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_9)) {
@@ -12829,86 +12712,86 @@
         __pyx_t_4 = 1;
       }
     }
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_9, __pyx_v_dists_to_centers, __pyx_int_0};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 649, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    if (unlikely((PyObject_SetItem(__pyx_v_dists_to_centers, __pyx_t_1, __pyx_int_0) < 0))) __PYX_ERR(0, 650, __pyx_L1_error)
+    if (unlikely((PyObject_SetItem(__pyx_v_dists_to_centers, __pyx_t_1, __pyx_int_0) < 0))) __PYX_ERR(0, 649, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "KKMeans.py":635
+    /* "KKMeans.py":634
  *         dists_to_centers = self._build_starting_distance(kernel_matrix)
  *         n_samples = X.shape[0]
  *         for cluster in range(self.n_clusters):             # <<<<<<<<<<<<<<
  *             if cluster == 0:
  *                 # choose first center randomly
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":651
+  /* "KKMeans.py":650
  *             # eliminate flop errors
  *             dists_to_centers[np.isclose(dists_to_centers, 0)] = 0
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_asarray); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_argmin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_argmin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_dists_to_centers);
   __Pyx_GIVEREF(__pyx_v_dists_to_centers);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_dists_to_centers);
-  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 651, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 651, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, __pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 651, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 651, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":600
+  /* "KKMeans.py":599
  *         return labels, quality, inner_sums, sizes
  * 
  *     def kmeanspp(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes heuristic to get good initial centers
  */
 
@@ -12933,15 +12816,15 @@
   __Pyx_XDECREF(__pyx_v_inner_sum);
   __Pyx_XDECREF(__pyx_v_outer_sum);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":654
+/* "KKMeans.py":653
  * 
  * 
  *     def predict(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes the closest cluster center for each x in X
  */
 
@@ -12987,40 +12870,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 654, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 653, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_X_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 654, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 653, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("predict", 1, 2, 2, 1); __PYX_ERR(0, 654, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("predict", 1, 2, 2, 1); __PYX_ERR(0, 653, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "predict") < 0)) __PYX_ERR(0, 654, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "predict") < 0)) __PYX_ERR(0, 653, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_X = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("predict", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 654, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("predict", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 653, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("KKMeans.KKMeans.predict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7KKMeans_7KKMeans_52predict(__pyx_self, __pyx_v_self, __pyx_v_X);
 
@@ -13044,59 +12927,59 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("predict", 0);
 
-  /* "KKMeans.py":678
+  /* "KKMeans.py":677
  *             labels for each datapoint in X
  *         '''
  *         if self.X_ is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("KKMeans instance is not fitted!")
  *         kernel_matrix = self.kernel_wrapper(X, self.X_)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_X); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_X); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 677, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 == Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "KKMeans.py":679
+    /* "KKMeans.py":678
  *         '''
  *         if self.X_ is None:
  *             raise ValueError("KKMeans instance is not fitted!")             # <<<<<<<<<<<<<<
  *         kernel_matrix = self.kernel_wrapper(X, self.X_)
  *         sq_distances = calc_sq_distances(
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 678, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 679, __pyx_L1_error)
+    __PYX_ERR(0, 678, __pyx_L1_error)
 
-    /* "KKMeans.py":678
+    /* "KKMeans.py":677
  *             labels for each datapoint in X
  *         '''
  *         if self.X_ is None:             # <<<<<<<<<<<<<<
  *             raise ValueError("KKMeans instance is not fitted!")
  *         kernel_matrix = self.kernel_wrapper(X, self.X_)
  */
   }
 
-  /* "KKMeans.py":680
+  /* "KKMeans.py":679
  *         if self.X_ is None:
  *             raise ValueError("KKMeans instance is not fitted!")
  *         kernel_matrix = self.kernel_wrapper(X, self.X_)             # <<<<<<<<<<<<<<
  *         sq_distances = calc_sq_distances(
  *             self.inner_sums_, self.cluster_sizes_,
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_kernel_wrapper); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_X); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_X); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -13107,61 +12990,60 @@
     }
   }
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_v_X, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 680, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_kernel_matrix = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "KKMeans.py":681
+  /* "KKMeans.py":680
  *             raise ValueError("KKMeans instance is not fitted!")
  *         kernel_matrix = self.kernel_wrapper(X, self.X_)
  *         sq_distances = calc_sq_distances(             # <<<<<<<<<<<<<<
  *             self.inner_sums_, self.cluster_sizes_,
  *             kernel_matrix, self.labels_,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_sq_distances); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_calc_sq_distances); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "KKMeans.py":682
+  /* "KKMeans.py":681
  *         kernel_matrix = self.kernel_wrapper(X, self.X_)
  *         sq_distances = calc_sq_distances(
  *             self.inner_sums_, self.cluster_sizes_,             # <<<<<<<<<<<<<<
  *             kernel_matrix, self.labels_,
  *             self.n_clusters)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_inner_sums); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_inner_sums); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cluster_sizes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cluster_sizes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "KKMeans.py":683
+  /* "KKMeans.py":682
  *         sq_distances = calc_sq_distances(
  *             self.inner_sums_, self.cluster_sizes_,
  *             kernel_matrix, self.labels_,             # <<<<<<<<<<<<<<
  *             self.n_clusters)
  *         return np.argmin(sq_distances, axis=1)
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_labels); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 682, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
 
-  /* "KKMeans.py":684
+  /* "KKMeans.py":683
  *             self.inner_sums_, self.cluster_sizes_,
  *             kernel_matrix, self.labels_,
  *             self.n_clusters)             # <<<<<<<<<<<<<<
  *         return np.argmin(sq_distances, axis=1)
- * 
  */
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_n_clusters); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 683, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_9 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -13175,52 +13057,50 @@
     PyObject *__pyx_callargs[6] = {__pyx_t_9, __pyx_t_4, __pyx_t_5, __pyx_v_kernel_matrix, __pyx_t_7, __pyx_t_8};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 5+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 680, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_sq_distances = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "KKMeans.py":685
+  /* "KKMeans.py":684
  *             kernel_matrix, self.labels_,
  *             self.n_clusters)
  *         return np.argmin(sq_distances, axis=1)             # <<<<<<<<<<<<<<
- * 
- * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_argmin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_argmin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_sq_distances);
   __Pyx_GIVEREF(__pyx_v_sq_distances);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_sq_distances);
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 685, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 685, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans.py":654
+  /* "KKMeans.py":653
  * 
  * 
  *     def predict(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes the closest cluster center for each x in X
  */
 
@@ -13239,422 +13119,14 @@
   __Pyx_XDECREF(__pyx_v_kernel_matrix);
   __Pyx_XDECREF(__pyx_v_sq_distances);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans.py":689
- * 
- * 
- * def visualize_kkm(data, labels):             # <<<<<<<<<<<<<<
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_7KKMeans_1visualize_kkm(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_7KKMeans_1visualize_kkm = {"visualize_kkm", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7KKMeans_1visualize_kkm, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7KKMeans_1visualize_kkm(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_data = 0;
-  PyObject *__pyx_v_labels = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("visualize_kkm (wrapper)", 0);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,&__pyx_n_s_labels_2,0};
-    PyObject* values[2] = {0,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 689, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels_2)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 689, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("visualize_kkm", 1, 2, 2, 1); __PYX_ERR(0, 689, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "visualize_kkm") < 0)) __PYX_ERR(0, 689, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 2)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-    }
-    __pyx_v_data = values[0];
-    __pyx_v_labels = values[1];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("visualize_kkm", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 689, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("KKMeans.visualize_kkm", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7KKMeans_visualize_kkm(__pyx_self, __pyx_v_data, __pyx_v_labels);
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_7KKMeans_visualize_kkm(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data, PyObject *__pyx_v_labels) {
-  PyObject *__pyx_v_fig = NULL;
-  PyObject *__pyx_v_ax = NULL;
-  CYTHON_UNUSED Py_ssize_t __pyx_7genexpr__pyx_v_x;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  int __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
-  Py_ssize_t __pyx_t_5;
-  Py_ssize_t __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
-  PyObject *__pyx_t_10 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("visualize_kkm", 0);
-
-  /* "KKMeans.py":690
- * 
- * def visualize_kkm(data, labels):
- *     if len(data[0]) > 3:             # <<<<<<<<<<<<<<
- *         raise Exception("Dimensionality is too high for visualization")
- *     elif len(data[0]) == 1:
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_data, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 690, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 690, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__pyx_t_2 > 3);
-  if (unlikely(__pyx_t_3)) {
-
-    /* "KKMeans.py":691
- * def visualize_kkm(data, labels):
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")             # <<<<<<<<<<<<<<
- *     elif len(data[0]) == 1:
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 691, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 691, __pyx_L1_error)
-
-    /* "KKMeans.py":690
- * 
- * def visualize_kkm(data, labels):
- *     if len(data[0]) > 3:             # <<<<<<<<<<<<<<
- *         raise Exception("Dimensionality is too high for visualization")
- *     elif len(data[0]) == 1:
- */
-  }
-
-  /* "KKMeans.py":692
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")
- *     elif len(data[0]) == 1:             # <<<<<<<<<<<<<<
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- *     elif len(data[0]) == 2:
- */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_data, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 692, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__pyx_t_2 == 1);
-  if (__pyx_t_3) {
-
-    /* "KKMeans.py":693
- *         raise Exception("Dimensionality is too high for visualization")
- *     elif len(data[0]) == 1:
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)             # <<<<<<<<<<<<<<
- *     elif len(data[0]) == 2:
- *         plt.scatter(data[:,0], data[:,1], c = labels)
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_plt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_scatter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 693, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    { /* enter inner scope */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 693, __pyx_L1_error)
-      __pyx_t_5 = __pyx_t_2;
-      for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
-        __pyx_7genexpr__pyx_v_x = __pyx_t_6;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_int_0))) __PYX_ERR(0, 693, __pyx_L1_error)
-      }
-    } /* exit inner scope */
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 693, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_INCREF(__pyx_v_data);
-    __Pyx_GIVEREF(__pyx_v_data);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_v_data);
-    __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
-    __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_c, __pyx_v_labels) < 0) __PYX_ERR(0, 693, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 693, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-
-    /* "KKMeans.py":692
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")
- *     elif len(data[0]) == 1:             # <<<<<<<<<<<<<<
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- *     elif len(data[0]) == 2:
- */
-    goto __pyx_L3;
-  }
-
-  /* "KKMeans.py":694
- *     elif len(data[0]) == 1:
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- *     elif len(data[0]) == 2:             # <<<<<<<<<<<<<<
- *         plt.scatter(data[:,0], data[:,1], c = labels)
- *     elif len(data[0]) == 3:
- */
-  __pyx_t_8 = __Pyx_GetItemInt(__pyx_v_data, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 694, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_2 = PyObject_Length(__pyx_t_8); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 694, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_3 = (__pyx_t_2 == 2);
-  if (__pyx_t_3) {
-
-    /* "KKMeans.py":695
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- *     elif len(data[0]) == 2:
- *         plt.scatter(data[:,0], data[:,1], c = labels)             # <<<<<<<<<<<<<<
- *     elif len(data[0]) == 3:
- *         fig = plt.figure()
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_plt); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 695, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_scatter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_data, __pyx_tuple__24); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 695, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_data, __pyx_tuple__25); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 695, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 695, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
-    __pyx_t_8 = 0;
-    __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 695, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_c, __pyx_v_labels) < 0) __PYX_ERR(0, 695, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 695, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-
-    /* "KKMeans.py":694
- *     elif len(data[0]) == 1:
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- *     elif len(data[0]) == 2:             # <<<<<<<<<<<<<<
- *         plt.scatter(data[:,0], data[:,1], c = labels)
- *     elif len(data[0]) == 3:
- */
-    goto __pyx_L3;
-  }
-
-  /* "KKMeans.py":696
- *     elif len(data[0]) == 2:
- *         plt.scatter(data[:,0], data[:,1], c = labels)
- *     elif len(data[0]) == 3:             # <<<<<<<<<<<<<<
- *         fig = plt.figure()
- *         ax = fig.add_subplot(projection = "3d")
- */
-  __pyx_t_8 = __Pyx_GetItemInt(__pyx_v_data, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 696, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_2 = PyObject_Length(__pyx_t_8); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 696, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_3 = (__pyx_t_2 == 3);
-  if (__pyx_t_3) {
-
-    /* "KKMeans.py":697
- *         plt.scatter(data[:,0], data[:,1], c = labels)
- *     elif len(data[0]) == 3:
- *         fig = plt.figure()             # <<<<<<<<<<<<<<
- *         ax = fig.add_subplot(projection = "3d")
- *         ax.scatter(data[:,0], data[:,1], data[:,2], c = labels)
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_plt); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 697, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_figure); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 697, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = NULL;
-    __pyx_t_9 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_7);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-        __pyx_t_9 = 1;
-      }
-    }
-    {
-      PyObject *__pyx_callargs[1] = {__pyx_t_7, };
-      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_9, 0+__pyx_t_9);
-      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 697, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    }
-    __pyx_v_fig = __pyx_t_8;
-    __pyx_t_8 = 0;
-
-    /* "KKMeans.py":698
- *     elif len(data[0]) == 3:
- *         fig = plt.figure()
- *         ax = fig.add_subplot(projection = "3d")             # <<<<<<<<<<<<<<
- *         ax.scatter(data[:,0], data[:,1], data[:,2], c = labels)
- */
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_fig, __pyx_n_s_add_subplot); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 698, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 698, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_projection, __pyx_kp_u_3d) < 0) __PYX_ERR(0, 698, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 698, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_v_ax = __pyx_t_7;
-    __pyx_t_7 = 0;
-
-    /* "KKMeans.py":699
- *         fig = plt.figure()
- *         ax = fig.add_subplot(projection = "3d")
- *         ax.scatter(data[:,0], data[:,1], data[:,2], c = labels)             # <<<<<<<<<<<<<<
- */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_ax, __pyx_n_s_scatter); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 699, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_data, __pyx_tuple__24); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 699, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_data, __pyx_tuple__25); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 699, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_data, __pyx_tuple__26); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 699, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 699, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_1);
-    __pyx_t_4 = 0;
-    __pyx_t_8 = 0;
-    __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 699, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_c, __pyx_v_labels) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 699, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-
-    /* "KKMeans.py":696
- *     elif len(data[0]) == 2:
- *         plt.scatter(data[:,0], data[:,1], c = labels)
- *     elif len(data[0]) == 3:             # <<<<<<<<<<<<<<
- *         fig = plt.figure()
- *         ax = fig.add_subplot(projection = "3d")
- */
-  }
-  __pyx_L3:;
-
-  /* "KKMeans.py":689
- * 
- * 
- * def visualize_kkm(data, labels):             # <<<<<<<<<<<<<<
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")
- */
-
-  /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("KKMeans.visualize_kkm", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_fig);
-  __Pyx_XDECREF(__pyx_v_ax);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
@@ -13663,19 +13135,17 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_u_3d, __pyx_k_3d, sizeof(__pyx_k_3d), 0, 1, 0, 0},
     {&__pyx_kp_u_Amount_of_given_centers_must_be, __pyx_k_Amount_of_given_centers_must_be, sizeof(__pyx_k_Amount_of_given_centers_must_be), 0, 1, 0, 0},
     {&__pyx_kp_u_Best, __pyx_k_Best, sizeof(__pyx_k_Best), 0, 1, 0, 0},
     {&__pyx_kp_u_Converged_at_iteration, __pyx_k_Converged_at_iteration, sizeof(__pyx_k_Converged_at_iteration), 0, 1, 0, 0},
-    {&__pyx_kp_u_Dimensionality_is_too_high_for_v, __pyx_k_Dimensionality_is_too_high_for_v, sizeof(__pyx_k_Dimensionality_is_too_high_for_v), 0, 1, 0, 0},
     {&__pyx_kp_u_Found_at_init, __pyx_k_Found_at_init, sizeof(__pyx_k_Found_at_init), 0, 1, 0, 0},
     {&__pyx_kp_u_Given_centers_are_empty, __pyx_k_Given_centers_are_empty, sizeof(__pyx_k_Given_centers_are_empty), 0, 1, 0, 0},
     {&__pyx_kp_u_Given_centers_need_to_be_2_d_arr, __pyx_k_Given_centers_need_to_be_2_d_arr, sizeof(__pyx_k_Given_centers_need_to_be_2_d_arr), 0, 1, 0, 0},
     {&__pyx_kp_u_Initialisation_method_not_implem, __pyx_k_Initialisation_method_not_implem, sizeof(__pyx_k_Initialisation_method_not_implem), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_kernel_provided, __pyx_k_Invalid_kernel_provided, sizeof(__pyx_k_Invalid_kernel_provided), 0, 1, 0, 0},
     {&__pyx_kp_u_Iteration, __pyx_k_Iteration, sizeof(__pyx_k_Iteration), 0, 1, 0, 0},
     {&__pyx_n_s_KKMeans, __pyx_k_KKMeans, sizeof(__pyx_k_KKMeans), 0, 0, 1, 1},
@@ -13732,61 +13202,55 @@
     {&__pyx_n_s_X, __pyx_k_X, sizeof(__pyx_k_X), 0, 0, 1, 1},
     {&__pyx_n_s_X_2, __pyx_k_X_2, sizeof(__pyx_k_X_2), 0, 0, 1, 1},
     {&__pyx_n_s_X_center_kernel, __pyx_k_X_center_kernel, sizeof(__pyx_k_X_center_kernel), 0, 0, 1, 1},
     {&__pyx_kp_u_X_is_empty, __pyx_k_X_is_empty, sizeof(__pyx_k_X_is_empty), 0, 1, 0, 0},
     {&__pyx_kp_u_X_needs_to_be_2_d_Array, __pyx_k_X_needs_to_be_2_d_Array, sizeof(__pyx_k_X_needs_to_be_2_d_Array), 0, 1, 0, 0},
     {&__pyx_n_s_Y, __pyx_k_Y, sizeof(__pyx_k_Y), 0, 0, 1, 1},
     {&__pyx_kp_u__16, __pyx_k__16, sizeof(__pyx_k__16), 0, 1, 0, 0},
-    {&__pyx_n_s__27, __pyx_k__27, sizeof(__pyx_k__27), 0, 0, 1, 1},
-    {&__pyx_kp_u__28, __pyx_k__28, sizeof(__pyx_k__28), 0, 1, 0, 0},
-    {&__pyx_n_s__77, __pyx_k__77, sizeof(__pyx_k__77), 0, 0, 1, 1},
-    {&__pyx_n_s_add_subplot, __pyx_k_add_subplot, sizeof(__pyx_k_add_subplot), 0, 0, 1, 1},
+    {&__pyx_n_s__23, __pyx_k__23, sizeof(__pyx_k__23), 0, 0, 1, 1},
+    {&__pyx_kp_u__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 1, 0, 0},
+    {&__pyx_n_s__71, __pyx_k__71, sizeof(__pyx_k__71), 0, 0, 1, 1},
     {&__pyx_n_s_algorithm, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
     {&__pyx_kp_u_algorithm_not_implemented_this, __pyx_k_algorithm_not_implemented_this, sizeof(__pyx_k_algorithm_not_implemented_this), 0, 1, 0, 0},
     {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
     {&__pyx_n_s_amin, __pyx_k_amin, sizeof(__pyx_k_amin), 0, 0, 1, 1},
     {&__pyx_n_s_argmax, __pyx_k_argmax, sizeof(__pyx_k_argmax), 0, 0, 1, 1},
     {&__pyx_n_s_argmin, __pyx_k_argmin, sizeof(__pyx_k_argmin), 0, 0, 1, 1},
     {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
     {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
     {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
     {&__pyx_n_s_assign_to_centers, __pyx_k_assign_to_centers, sizeof(__pyx_k_assign_to_centers), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_avg_silhouette, __pyx_k_avg_silhouette, sizeof(__pyx_k_avg_silhouette), 0, 0, 1, 1},
-    {&__pyx_n_s_ax, __pyx_k_ax, sizeof(__pyx_k_ax), 0, 0, 1, 1},
     {&__pyx_n_s_axis, __pyx_k_axis, sizeof(__pyx_k_axis), 0, 0, 1, 1},
     {&__pyx_n_s_best_init, __pyx_k_best_init, sizeof(__pyx_k_best_init), 0, 0, 1, 1},
     {&__pyx_n_s_build_kernel_matrix, __pyx_k_build_kernel_matrix, sizeof(__pyx_k_build_kernel_matrix), 0, 0, 1, 1},
     {&__pyx_n_s_build_starting_distance, __pyx_k_build_starting_distance, sizeof(__pyx_k_build_starting_distance), 0, 0, 1, 1},
-    {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
     {&__pyx_n_s_calc_q_metric, __pyx_k_calc_q_metric, sizeof(__pyx_k_calc_q_metric), 0, 0, 1, 1},
     {&__pyx_n_s_calc_silhouette, __pyx_k_calc_silhouette, sizeof(__pyx_k_calc_silhouette), 0, 0, 1, 1},
     {&__pyx_n_s_calc_sq_distances, __pyx_k_calc_sq_distances, sizeof(__pyx_k_calc_sq_distances), 0, 0, 1, 1},
     {&__pyx_n_s_center, __pyx_k_center, sizeof(__pyx_k_center), 0, 0, 1, 1},
     {&__pyx_n_s_center_dists, __pyx_k_center_dists, sizeof(__pyx_k_center_dists), 0, 0, 1, 1},
     {&__pyx_n_s_centers, __pyx_k_centers, sizeof(__pyx_k_centers), 0, 0, 1, 1},
     {&__pyx_n_s_choice, __pyx_k_choice, sizeof(__pyx_k_choice), 0, 0, 1, 1},
     {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_cluster, __pyx_k_cluster, sizeof(__pyx_k_cluster), 0, 0, 1, 1},
     {&__pyx_n_s_cluster_sizes, __pyx_k_cluster_sizes, sizeof(__pyx_k_cluster_sizes), 0, 0, 1, 1},
     {&__pyx_n_s_cluster_sizes_2, __pyx_k_cluster_sizes_2, sizeof(__pyx_k_cluster_sizes_2), 0, 0, 1, 1},
     {&__pyx_n_s_converged, __pyx_k_converged, sizeof(__pyx_k_converged), 0, 0, 1, 1},
-    {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_s_default_rng, __pyx_k_default_rng, sizeof(__pyx_k_default_rng), 0, 0, 1, 1},
     {&__pyx_n_s_diag, __pyx_k_diag, sizeof(__pyx_k_diag), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_dists_to_centers, __pyx_k_dists_to_centers, sizeof(__pyx_k_dists_to_centers), 0, 0, 1, 1},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
     {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
     {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
     {&__pyx_n_s_elkan, __pyx_k_elkan, sizeof(__pyx_k_elkan), 0, 0, 1, 1},
     {&__pyx_n_u_elkan, __pyx_k_elkan, sizeof(__pyx_k_elkan), 0, 1, 0, 1},
-    {&__pyx_n_s_fig, __pyx_k_fig, sizeof(__pyx_k_fig), 0, 0, 1, 1},
-    {&__pyx_n_s_figure, __pyx_k_figure, sizeof(__pyx_k_figure), 0, 0, 1, 1},
     {&__pyx_n_s_fill_empty_clusters, __pyx_k_fill_empty_clusters, sizeof(__pyx_k_fill_empty_clusters), 0, 0, 1, 1},
     {&__pyx_n_s_fit, __pyx_k_fit, sizeof(__pyx_k_fit), 0, 0, 1, 1},
     {&__pyx_n_u_gaussian, __pyx_k_gaussian, sizeof(__pyx_k_gaussian), 0, 1, 0, 1},
     {&__pyx_n_s_get_best_init, __pyx_k_get_best_init, sizeof(__pyx_k_get_best_init), 0, 0, 1, 1},
     {&__pyx_n_s_high, __pyx_k_high, sizeof(__pyx_k_high), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
@@ -13821,15 +13285,14 @@
     {&__pyx_n_s_labels_store, __pyx_k_labels_store, sizeof(__pyx_k_labels_store), 0, 0, 1, 1},
     {&__pyx_n_u_laplacian, __pyx_k_laplacian, sizeof(__pyx_k_laplacian), 0, 1, 0, 1},
     {&__pyx_n_u_linear, __pyx_k_linear, sizeof(__pyx_k_linear), 0, 1, 0, 1},
     {&__pyx_n_s_lloyd, __pyx_k_lloyd, sizeof(__pyx_k_lloyd), 0, 0, 1, 1},
     {&__pyx_n_u_lloyd, __pyx_k_lloyd, sizeof(__pyx_k_lloyd), 0, 1, 0, 1},
     {&__pyx_n_s_low, __pyx_k_low, sizeof(__pyx_k_low), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-    {&__pyx_n_s_matplotlib, __pyx_k_matplotlib, sizeof(__pyx_k_matplotlib), 0, 0, 1, 1},
     {&__pyx_n_s_max_iter, __pyx_k_max_iter, sizeof(__pyx_k_max_iter), 0, 0, 1, 1},
     {&__pyx_kp_u_max_iter_must_be_1, __pyx_k_max_iter_must_be_1, sizeof(__pyx_k_max_iter_must_be_1), 0, 1, 0, 0},
     {&__pyx_kp_u_max_iter_must_be_int, __pyx_k_max_iter_must_be_int, sizeof(__pyx_k_max_iter_must_be_int), 0, 1, 0, 0},
     {&__pyx_n_s_measure_iter, __pyx_k_measure_iter, sizeof(__pyx_k_measure_iter), 0, 0, 1, 1},
     {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
     {&__pyx_kp_u_metric_not_implemented_this_sho, __pyx_k_metric_not_implemented_this_sho, sizeof(__pyx_k_metric_not_implemented_this_sho), 0, 1, 0, 0},
     {&__pyx_n_s_min_dist_each, __pyx_k_min_dist_each, sizeof(__pyx_k_min_dist_each), 0, 0, 1, 1},
@@ -13847,37 +13310,33 @@
     {&__pyx_kp_u_not_implemented, __pyx_k_not_implemented, sizeof(__pyx_k_not_implemented), 0, 1, 0, 0},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
     {&__pyx_n_s_out_finish, __pyx_k_out_finish, sizeof(__pyx_k_out_finish), 0, 0, 1, 1},
     {&__pyx_n_s_out_verbose, __pyx_k_out_verbose, sizeof(__pyx_k_out_verbose), 0, 0, 1, 1},
     {&__pyx_n_s_outer_sum, __pyx_k_outer_sum, sizeof(__pyx_k_outer_sum), 0, 0, 1, 1},
     {&__pyx_n_s_p, __pyx_k_p, sizeof(__pyx_k_p), 0, 0, 1, 1},
-    {&__pyx_n_s_plt, __pyx_k_plt, sizeof(__pyx_k_plt), 0, 0, 1, 1},
     {&__pyx_n_u_polynomial, __pyx_k_polynomial, sizeof(__pyx_k_polynomial), 0, 1, 0, 1},
     {&__pyx_n_s_predict, __pyx_k_predict, sizeof(__pyx_k_predict), 0, 0, 1, 1},
     {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
     {&__pyx_n_s_print, __pyx_k_print, sizeof(__pyx_k_print), 0, 0, 1, 1},
     {&__pyx_n_s_probs, __pyx_k_probs, sizeof(__pyx_k_probs), 0, 0, 1, 1},
-    {&__pyx_n_s_projection, __pyx_k_projection, sizeof(__pyx_k_projection), 0, 0, 1, 1},
-    {&__pyx_n_s_pyplot, __pyx_k_pyplot, sizeof(__pyx_k_pyplot), 0, 0, 1, 1},
     {&__pyx_n_s_q_metric, __pyx_k_q_metric, sizeof(__pyx_k_q_metric), 0, 0, 1, 1},
     {&__pyx_n_s_quality, __pyx_k_quality, sizeof(__pyx_k_quality), 0, 0, 1, 1},
     {&__pyx_n_s_quality_2, __pyx_k_quality_2, sizeof(__pyx_k_quality_2), 0, 0, 1, 1},
     {&__pyx_kp_u_quality_metric_not_implemented, __pyx_k_quality_metric_not_implemented, sizeof(__pyx_k_quality_metric_not_implemented), 0, 1, 0, 0},
     {&__pyx_n_s_quality_old, __pyx_k_quality_old, sizeof(__pyx_k_quality_old), 0, 0, 1, 1},
     {&__pyx_n_s_quality_store, __pyx_k_quality_store, sizeof(__pyx_k_quality_store), 0, 0, 1, 1},
     {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
     {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
     {&__pyx_n_u_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 1, 0, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_u_rbf, __pyx_k_rbf, sizeof(__pyx_k_rbf), 0, 1, 0, 1},
     {&__pyx_n_s_reshape, __pyx_k_reshape, sizeof(__pyx_k_reshape), 0, 0, 1, 1},
     {&__pyx_n_s_rng, __pyx_k_rng, sizeof(__pyx_k_rng), 0, 0, 1, 1},
     {&__pyx_kp_u_sample_cluster_ratio_needs_to_be, __pyx_k_sample_cluster_ratio_needs_to_be, sizeof(__pyx_k_sample_cluster_ratio_needs_to_be), 0, 1, 0, 0},
-    {&__pyx_n_s_scatter, __pyx_k_scatter, sizeof(__pyx_k_scatter), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
     {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
     {&__pyx_n_u_silhouette, __pyx_k_silhouette, sizeof(__pyx_k_silhouette), 0, 1, 0, 1},
     {&__pyx_kp_u_silhouette_inertia, __pyx_k_silhouette_inertia, sizeof(__pyx_k_silhouette_inertia), 0, 1, 0, 0},
     {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
     {&__pyx_n_s_sizes, __pyx_k_sizes, sizeof(__pyx_k_sizes), 0, 0, 1, 1},
@@ -13906,614 +13365,566 @@
     {&__pyx_n_s_validate_max_iter, __pyx_k_validate_max_iter, sizeof(__pyx_k_validate_max_iter), 0, 0, 1, 1},
     {&__pyx_n_s_validate_n_clusters, __pyx_k_validate_n_clusters, sizeof(__pyx_k_validate_n_clusters), 0, 0, 1, 1},
     {&__pyx_n_s_validate_n_init, __pyx_k_validate_n_init, sizeof(__pyx_k_validate_n_init), 0, 0, 1, 1},
     {&__pyx_n_s_validate_params, __pyx_k_validate_params, sizeof(__pyx_k_validate_params), 0, 0, 1, 1},
     {&__pyx_n_s_validate_q_metric, __pyx_k_validate_q_metric, sizeof(__pyx_k_validate_q_metric), 0, 0, 1, 1},
     {&__pyx_n_s_validate_tol, __pyx_k_validate_tol, sizeof(__pyx_k_validate_tol), 0, 0, 1, 1},
     {&__pyx_n_s_verbose, __pyx_k_verbose, sizeof(__pyx_k_verbose), 0, 0, 1, 1},
-    {&__pyx_n_s_visualize_kkm, __pyx_k_visualize_kkm, sizeof(__pyx_k_visualize_kkm), 0, 0, 1, 1},
-    {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
     {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 173, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 178, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 186, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 276, __pyx_L1_error)
-  __pyx_builtin_all = __Pyx_GetBuiltinName(__pyx_n_s_all); if (!__pyx_builtin_all) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 275, __pyx_L1_error)
+  __pyx_builtin_all = __Pyx_GetBuiltinName(__pyx_n_s_all); if (!__pyx_builtin_all) __PYX_ERR(0, 475, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "KKMeans.py":173
+  /* "KKMeans.py":172
  *         self.__validate_kernel()
  *         if self.algorithm == "elkan" and self.q_metric == "silhouette":
  *             print("WARNING: using silhouette with elkan will most likely be inaccurate\             # <<<<<<<<<<<<<<
  *                   as elkan does not calculate exact distances to every center")
  * 
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_WARNING_using_silhouette_with_el); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_WARNING_using_silhouette_with_el); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "KKMeans.py":178
+  /* "KKMeans.py":177
  *     def __validate_n_clusters(self):
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")             # <<<<<<<<<<<<<<
  *         if self.n_clusters < 1:
  *             raise ValueError("n_cluster must be >= 1")
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_n_clusters_must_be_int); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_n_clusters_must_be_int); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "KKMeans.py":180
+  /* "KKMeans.py":179
  *             raise ValueError("n_clusters must be int")
  *         if self.n_clusters < 1:
  *             raise ValueError("n_cluster must be >= 1")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_init(self):
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_n_cluster_must_be_1); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_n_cluster_must_be_1); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "KKMeans.py":186
+  /* "KKMeans.py":185
  *             self.__validate_centers()
  *         elif self.init not in ("kmeans++", "random", "truerandom") :
  *             raise NotImplementedError("Initialisation method not implemented")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_centers(self):
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Initialisation_method_not_implem); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Initialisation_method_not_implem); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "KKMeans.py":192
+  /* "KKMeans.py":191
  *         self.init = np.asarray(self.init, dtype=np.double)
  *         if self.init.ndim != 2:
  *             raise ValueError("Given centers need to be 2-d array")             # <<<<<<<<<<<<<<
  *         if 0 in self.init.shape:
  *             raise ValueError("Given centers are empty")
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Given_centers_need_to_be_2_d_arr); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Given_centers_need_to_be_2_d_arr); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "KKMeans.py":194
+  /* "KKMeans.py":193
  *             raise ValueError("Given centers need to be 2-d array")
  *         if 0 in self.init.shape:
  *             raise ValueError("Given centers are empty")             # <<<<<<<<<<<<<<
  *         if self.init.shape[0] != self.n_clusters:
  *             raise ValueError("Amount of given centers must be equal to n_clusters")
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Given_centers_are_empty); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Given_centers_are_empty); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "KKMeans.py":196
+  /* "KKMeans.py":195
  *             raise ValueError("Given centers are empty")
  *         if self.init.shape[0] != self.n_clusters:
  *             raise ValueError("Amount of given centers must be equal to n_clusters")             # <<<<<<<<<<<<<<
  *         return self.init
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Amount_of_given_centers_must_be); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Amount_of_given_centers_must_be); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "KKMeans.py":201
+  /* "KKMeans.py":200
  *     def __validate_n_init(self):
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")             # <<<<<<<<<<<<<<
  *         if self.n_init <= 0:
  *             raise ValueError("n_inits must be => 1")
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_n_init_must_be_int); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_n_init_must_be_int); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "KKMeans.py":203
+  /* "KKMeans.py":202
  *             raise ValueError("n_init must be int")
  *         if self.n_init <= 0:
  *             raise ValueError("n_inits must be => 1")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_max_iter(self):
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_n_inits_must_be_1); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_n_inits_must_be_1); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "KKMeans.py":207
+  /* "KKMeans.py":206
  *     def __validate_max_iter(self):
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")             # <<<<<<<<<<<<<<
  *         if self.max_iter <= 0:
  *             raise ValueError("max_iter must be => 1")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_max_iter_must_be_int); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_max_iter_must_be_int); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "KKMeans.py":209
+  /* "KKMeans.py":208
  *             raise ValueError("max_iter must be int")
  *         if self.max_iter <= 0:
  *             raise ValueError("max_iter must be => 1")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_algorithm(self):
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_max_iter_must_be_1); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_max_iter_must_be_1); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "KKMeans.py":217
+  /* "KKMeans.py":216
  *     def __validate_q_metric(self):
  *         if self.q_metric not in ("silhouette, inertia"):
  *             raise NotImplementedError("Quality metric not implemented")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_tol(self):
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_Quality_metric_not_implemented); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_Quality_metric_not_implemented); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "KKMeans.py":221
+  /* "KKMeans.py":220
  *     def __validate_tol(self):
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")             # <<<<<<<<<<<<<<
  *         if self.tol < 0:
  *             self.tol = 0
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_tol_must_be_numeric); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_tol_must_be_numeric); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "KKMeans.py":224
+  /* "KKMeans.py":223
  *         if self.tol < 0:
  *             self.tol = 0
  *             print("Warning! tol < 0 passed, tol set to 0")             # <<<<<<<<<<<<<<
  * 
  *     def __validate_kernel(self):
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_Warning_tol_0_passed_tol_set_to); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_Warning_tol_0_passed_tol_set_to); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "KKMeans.py":230
+  /* "KKMeans.py":229
  *                 "linear", "rbf", "polynomial",
  *                 "gaussian", "laplacian"]:
  *             raise ValueError("Invalid kernel provided.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_Invalid_kernel_provided); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_Invalid_kernel_provided); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "KKMeans.py":319
+  /* "KKMeans.py":318
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:
  *             raise ValueError("X needs to be 2-d Array")             # <<<<<<<<<<<<<<
  *         if 0 in X.shape:
  *             raise ValueError("X is empty")
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_X_needs_to_be_2_d_Array); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_X_needs_to_be_2_d_Array); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 318, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "KKMeans.py":321
+  /* "KKMeans.py":320
  *             raise ValueError("X needs to be 2-d Array")
  *         if 0 in X.shape:
  *             raise ValueError("X is empty")             # <<<<<<<<<<<<<<
  *         if X.shape[0] <  self.n_clusters:
  *             raise ValueError("sample:cluster ratio needs to be at least one")
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_X_is_empty); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_X_is_empty); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "KKMeans.py":323
+  /* "KKMeans.py":322
  *             raise ValueError("X is empty")
  *         if X.shape[0] <  self.n_clusters:
  *             raise ValueError("sample:cluster ratio needs to be at least one")             # <<<<<<<<<<<<<<
  *         return X
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_sample_cluster_ratio_needs_to_be); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_sample_cluster_ratio_needs_to_be); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "KKMeans.py":344
+  /* "KKMeans.py":343
  *             return self.kmeanspp(X, kernel_matrix)
  * 
  *         raise NotImplementedError("Unknown initialisation method")             # <<<<<<<<<<<<<<
  * 
  *     def _assign_to_centers(self, X, centers):
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_Unknown_initialisation_method); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_Unknown_initialisation_method); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "KKMeans.py":373
+  /* "KKMeans.py":372
  *         dists_to_centers = np.zeros((len(X), self.n_clusters))
  *         for cluster in range(self.n_clusters):
  *             dists_to_centers[:, cluster] = (-2 * X_center_kernel[:, cluster]             # <<<<<<<<<<<<<<
  *                                          + self.kernel_wrapper(centers[cluster]))
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  */
-  __pyx_slice__21 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__21)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_slice__21 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__21)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__21);
   __Pyx_GIVEREF(__pyx_slice__21);
 
-  /* "KKMeans.py":679
+  /* "KKMeans.py":678
  *         '''
  *         if self.X_ is None:
  *             raise ValueError("KKMeans instance is not fitted!")             # <<<<<<<<<<<<<<
  *         kernel_matrix = self.kernel_wrapper(X, self.X_)
  *         sq_distances = calc_sq_distances(
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_u_KKMeans_instance_is_not_fitted); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_u_KKMeans_instance_is_not_fitted); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
 
-  /* "KKMeans.py":691
- * def visualize_kkm(data, labels):
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")             # <<<<<<<<<<<<<<
- *     elif len(data[0]) == 1:
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_u_Dimensionality_is_too_high_for_v); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 691, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
-
-  /* "KKMeans.py":695
- *         plt.scatter(data, [0 for x in range(len(data))], c = labels)
- *     elif len(data[0]) == 2:
- *         plt.scatter(data[:,0], data[:,1], c = labels)             # <<<<<<<<<<<<<<
- *     elif len(data[0]) == 3:
- *         fig = plt.figure()
- */
-  __pyx_tuple__24 = PyTuple_Pack(2, __pyx_slice__21, __pyx_int_0); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 695, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_tuple__25 = PyTuple_Pack(2, __pyx_slice__21, __pyx_int_1); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 695, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-
-  /* "KKMeans.py":699
- *         fig = plt.figure()
- *         ax = fig.add_subplot(projection = "3d")
- *         ax.scatter(data[:,0], data[:,1], data[:,2], c = labels)             # <<<<<<<<<<<<<<
- */
-  __pyx_tuple__26 = PyTuple_Pack(2, __pyx_slice__21, __pyx_int_2); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 699, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-
-  /* "KKMeans.py":117
+  /* "KKMeans.py":116
  * 
  *     '''
  *     def __init__(self, n_clusters=8, init="kmeans++", n_init=3,             # <<<<<<<<<<<<<<
  *                  max_iter=300, tol=1e-4, q_metric="inertia", verbose=False,
  *                  rng=None, algorithm="lloyd", kernel="linear", **kwargs):
  */
-  __pyx_tuple__29 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_n_clusters, __pyx_n_s_init, __pyx_n_s_n_init, __pyx_n_s_max_iter, __pyx_n_s_tol, __pyx_n_s_q_metric, __pyx_n_s_verbose, __pyx_n_s_rng, __pyx_n_s_algorithm, __pyx_n_s_kernel, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 117, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(11, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_init_2, 117, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 117, __pyx_L1_error)
-  __pyx_tuple__31 = PyTuple_Pack(10, ((PyObject *)__pyx_int_8), ((PyObject*)__pyx_kp_u_kmeans), ((PyObject *)__pyx_int_3), ((PyObject *)__pyx_int_300), ((PyObject*)__pyx_float_1eneg_4), ((PyObject*)__pyx_n_u_inertia), ((PyObject *)Py_False), ((PyObject *)Py_None), ((PyObject*)__pyx_n_u_lloyd), ((PyObject*)__pyx_n_u_linear)); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 117, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__25 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_n_clusters, __pyx_n_s_init, __pyx_n_s_n_init, __pyx_n_s_max_iter, __pyx_n_s_tol, __pyx_n_s_q_metric, __pyx_n_s_verbose, __pyx_n_s_rng, __pyx_n_s_algorithm, __pyx_n_s_kernel, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(11, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_init_2, 116, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(10, ((PyObject *)__pyx_int_8), ((PyObject*)__pyx_kp_u_kmeans), ((PyObject *)__pyx_int_3), ((PyObject *)__pyx_int_300), ((PyObject*)__pyx_float_1eneg_4), ((PyObject*)__pyx_n_u_inertia), ((PyObject *)Py_False), ((PyObject *)Py_None), ((PyObject*)__pyx_n_u_lloyd), ((PyObject*)__pyx_n_u_linear)); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
-  /* "KKMeans.py":162
+  /* "KKMeans.py":161
  * 
  * 
  *     def _validate_params(self):             # <<<<<<<<<<<<<<
  *         '''Checks for possible errors in the parameters, can raise exceptions'''
  *         self.__validate_n_clusters()
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_params, 162, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_params, 161, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 161, __pyx_L1_error)
 
-  /* "KKMeans.py":176
+  /* "KKMeans.py":175
  *                   as elkan does not calculate exact distances to every center")
  * 
  *     def __validate_n_clusters(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")
  */
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_n_clusters, 176, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_n_clusters, 175, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 175, __pyx_L1_error)
 
-  /* "KKMeans.py":182
+  /* "KKMeans.py":181
  *             raise ValueError("n_cluster must be >= 1")
  * 
  *     def __validate_init(self):             # <<<<<<<<<<<<<<
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *             self.__validate_centers()
  */
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_init, 182, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_init, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 181, __pyx_L1_error)
 
-  /* "KKMeans.py":188
+  /* "KKMeans.py":187
  *             raise NotImplementedError("Initialisation method not implemented")
  * 
  *     def __validate_centers(self):             # <<<<<<<<<<<<<<
  *         '''checks for invalid centers, can raise exceptions.'''
  *         self.init = np.asarray(self.init, dtype=np.double)
  */
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_centers, 188, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 188, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_centers, 187, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 187, __pyx_L1_error)
 
-  /* "KKMeans.py":199
+  /* "KKMeans.py":198
  *         return self.init
  * 
  *     def __validate_n_init(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")
  */
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_n_init, 199, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_n_init, 198, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 198, __pyx_L1_error)
 
-  /* "KKMeans.py":205
+  /* "KKMeans.py":204
  *             raise ValueError("n_inits must be => 1")
  * 
  *     def __validate_max_iter(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")
  */
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_max_iter, 205, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 205, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_max_iter, 204, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 204, __pyx_L1_error)
 
-  /* "KKMeans.py":211
+  /* "KKMeans.py":210
  *             raise ValueError("max_iter must be => 1")
  * 
  *     def __validate_algorithm(self):             # <<<<<<<<<<<<<<
  *         if self.algorithm not in ("lloyd", "elkan"):
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  */
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_algorithm, 211, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_algorithm, 210, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 210, __pyx_L1_error)
 
-  /* "KKMeans.py":215
+  /* "KKMeans.py":214
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  * 
  *     def __validate_q_metric(self):             # <<<<<<<<<<<<<<
  *         if self.q_metric not in ("silhouette, inertia"):
  *             raise NotImplementedError("Quality metric not implemented")
  */
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_q_metric, 215, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_q_metric, 214, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 214, __pyx_L1_error)
 
-  /* "KKMeans.py":219
+  /* "KKMeans.py":218
  *             raise NotImplementedError("Quality metric not implemented")
  * 
  *     def __validate_tol(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")
  */
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_tol, 219, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_tol, 218, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 218, __pyx_L1_error)
 
-  /* "KKMeans.py":226
+  /* "KKMeans.py":225
  *             print("Warning! tol < 0 passed, tol set to 0")
  * 
  *     def __validate_kernel(self):             # <<<<<<<<<<<<<<
  *         if self.kernel not in [
  *                 "linear", "rbf", "polynomial",
  */
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_kernel, 226, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_kernel, 225, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 225, __pyx_L1_error)
 
-  /* "KKMeans.py":234
+  /* "KKMeans.py":233
  * 
  * 
  *     def kernel_wrapper(self, X, Y=None):             # <<<<<<<<<<<<<<
  *         '''
  *         Wrapper function to compute kernel matrix
  */
-  __pyx_tuple__43 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_Y); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_kernel_wrapper, 234, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 234, __pyx_L1_error)
-  __pyx_tuple__45 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
+  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_Y); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_kernel_wrapper, 233, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
 
-  /* "KKMeans.py":253
+  /* "KKMeans.py":252
  *         return build_kernel_matrix(X, Y, kernel=self.kernel, **self.kwargs)
  * 
  *     def fit(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Fits the data X with the given parameters.
  */
-  __pyx_tuple__46 = PyTuple_Pack(14, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_labels_store, __pyx_n_s_quality_store, __pyx_n_s_inner_sums_store, __pyx_n_s_sizes_store, __pyx_n_s_init, __pyx_n_s_start_labels, __pyx_n_s_labels_2, __pyx_n_s_quality_2, __pyx_n_s_inner_sums_2, __pyx_n_s_sizes, __pyx_n_s_best_init); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 253, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__46);
-  __Pyx_GIVEREF(__pyx_tuple__46);
-  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_fit, 253, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_tuple__42 = PyTuple_Pack(14, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_labels_store, __pyx_n_s_quality_store, __pyx_n_s_inner_sums_store, __pyx_n_s_sizes_store, __pyx_n_s_init, __pyx_n_s_start_labels, __pyx_n_s_labels_2, __pyx_n_s_quality_2, __pyx_n_s_inner_sums_2, __pyx_n_s_sizes, __pyx_n_s_best_init); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_fit, 252, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 252, __pyx_L1_error)
 
-  /* "KKMeans.py":299
+  /* "KKMeans.py":298
  *         self._out_finish(best_init)
  * 
  *     def _get_best_init(self, quality_store):             # <<<<<<<<<<<<<<
  *         """Returns best quality score given self.q_metric"""
  *         if self.q_metric == "inertia": # smalles is better
  */
-  __pyx_tuple__48 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_quality_store); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 299, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
-  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_get_best_init, 299, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_tuple__44 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_quality_store); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_get_best_init, 298, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 298, __pyx_L1_error)
 
-  /* "KKMeans.py":311
+  /* "KKMeans.py":310
  *                 this should have been caught in _validate_params")
  * 
  *     def _out_finish(self, best_init):             # <<<<<<<<<<<<<<
  *         '''output at the end of self.fit'''
  *         print("Best " + self.q_metric +":", self.quality_,
  */
-  __pyx_tuple__50 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_best_init); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 311, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__50);
-  __Pyx_GIVEREF(__pyx_tuple__50);
-  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_out_finish, 311, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_best_init); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_out_finish, 310, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 310, __pyx_L1_error)
 
-  /* "KKMeans.py":316
+  /* "KKMeans.py":315
  *               "Found at init:", best_init + 1)
  * 
  *     def _validate_data(self, X):             # <<<<<<<<<<<<<<
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:
  */
-  __pyx_tuple__52 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_X_2); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 316, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__52);
-  __Pyx_GIVEREF(__pyx_tuple__52);
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_data, 316, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_X_2); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_validate_data, 315, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 315, __pyx_L1_error)
 
-  /* "KKMeans.py":326
+  /* "KKMeans.py":325
  *         return X
  * 
  *     def _init_labels(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''Assign labels to each datapoint by given method'''
  * 
  */
-  __pyx_tuple__54 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_centers); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 326, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__54);
-  __Pyx_GIVEREF(__pyx_tuple__54);
-  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_init_labels, 326, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_centers); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_init_labels, 325, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 325, __pyx_L1_error)
 
-  /* "KKMeans.py":346
+  /* "KKMeans.py":345
  *         raise NotImplementedError("Unknown initialisation method")
  * 
  *     def _assign_to_centers(self, X, centers):             # <<<<<<<<<<<<<<
  *         '''
  *         Assigns each datapoint to the closest given center.
  */
-  __pyx_tuple__56 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_centers, __pyx_n_s_X_center_kernel, __pyx_n_s_dists_to_centers, __pyx_n_s_cluster); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 346, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__56);
-  __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_assign_to_centers, 346, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_centers, __pyx_n_s_X_center_kernel, __pyx_n_s_dists_to_centers, __pyx_n_s_cluster); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_assign_to_centers, 345, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 345, __pyx_L1_error)
 
-  /* "KKMeans.py":377
+  /* "KKMeans.py":376
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  * 
  *     def lloyd(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a run of lloyd's algorithm
  */
-  __pyx_tuple__58 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_kernel_matrix, __pyx_n_s_labels_2, __pyx_n_s_quality_2, __pyx_n_s_it, __pyx_n_s_cluster_sizes_2, __pyx_n_s_sq_distances, __pyx_n_s_inner_sums_2, __pyx_n_s_labels_old, __pyx_n_s_converged); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 377, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__58);
-  __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_lloyd, 377, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_kernel_matrix, __pyx_n_s_labels_2, __pyx_n_s_quality_2, __pyx_n_s_it, __pyx_n_s_cluster_sizes_2, __pyx_n_s_sq_distances, __pyx_n_s_inner_sums_2, __pyx_n_s_labels_old, __pyx_n_s_converged); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_lloyd, 376, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 376, __pyx_L1_error)
 
-  /* "KKMeans.py":429
+  /* "KKMeans.py":428
  * 
  * 
  *     def _out_verbose(self, iter, quality, converged):             # <<<<<<<<<<<<<<
  *         '''Checks if self.verbose and prints accordingly'''
  *         if not self.verbose:
  */
-  __pyx_tuple__60 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_iter_2, __pyx_n_s_quality_2, __pyx_n_s_converged); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 429, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__60);
-  __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_out_verbose, 429, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_iter_2, __pyx_n_s_quality_2, __pyx_n_s_converged); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_out_verbose, 428, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 428, __pyx_L1_error)
 
-  /* "KKMeans.py":441
+  /* "KKMeans.py":440
  * 
  * 
  *     def _measure_iter(self, sq_distances, labels, labels_old, quality):             # <<<<<<<<<<<<<<
  *         '''
  *         Measures quality of iteration and checks for convergence
  */
-  __pyx_tuple__62 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_sq_distances, __pyx_n_s_labels_2, __pyx_n_s_labels_old, __pyx_n_s_quality_2, __pyx_n_s_converged, __pyx_n_s_quality_old); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 441, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__62);
-  __Pyx_GIVEREF(__pyx_tuple__62);
-  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_measure_iter, 441, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_sq_distances, __pyx_n_s_labels_2, __pyx_n_s_labels_old, __pyx_n_s_quality_2, __pyx_n_s_converged, __pyx_n_s_quality_old); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_measure_iter, 440, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 440, __pyx_L1_error)
 
-  /* "KKMeans.py":483
+  /* "KKMeans.py":482
  *         return quality, converged
  * 
  *     def calc_q_metric(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Calculates quality metric
  */
-  __pyx_tuple__64 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_sq_distances, __pyx_n_s_labels_2); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 483, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__64);
-  __Pyx_GIVEREF(__pyx_tuple__64);
-  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_calc_q_metric, 483, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_sq_distances, __pyx_n_s_labels_2); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__60);
+  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_calc_q_metric, 482, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 482, __pyx_L1_error)
 
-  /* "KKMeans.py":513
+  /* "KKMeans.py":512
  *             raise NotImplementedError(str(self.q_metric) + " quality metric not implemented")
  * 
  *     def calc_silhouette(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''Calculates average silhouette of clustering
  * 
  */
-  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_calc_silhouette, 513, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_calc_silhouette, 512, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 512, __pyx_L1_error)
 
-  /* "KKMeans.py":532
+  /* "KKMeans.py":531
  *         return avg_silhouette(sq_distances, labels)
  * 
  *     def _build_starting_distance(self, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Builds basis for computing square distances
  */
-  __pyx_tuple__67 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kernel_matrix); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 532, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
-  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_build_starting_distance, 532, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_kernel_matrix); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 531, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__63);
+  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_build_starting_distance, 531, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(0, 531, __pyx_L1_error)
 
-  /* "KKMeans.py":547
+  /* "KKMeans.py":546
  *         return np.ascontiguousarray(np.tile(np.diag(kernel_matrix), (self.n_clusters, 1)).T, dtype=np.double)
  * 
  *     def elkan(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a slightly optimized Kernel-Kmeans heuristic
  */
-  __pyx_tuple__69 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_kernel_matrix, __pyx_n_s_labels_2, __pyx_n_s_start_dists, __pyx_n_s_center_dists, __pyx_n_s_quality_2, __pyx_n_s_it, __pyx_n_s_sizes, __pyx_n_s_l_bounds, __pyx_n_s_inner_sums_2, __pyx_n_s_labels_old, __pyx_n_s_converged, __pyx_n_s_sizes_old); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 547, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__69);
-  __Pyx_GIVEREF(__pyx_tuple__69);
-  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_elkan, 547, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __pyx_tuple__65 = PyTuple_Pack(13, __pyx_n_s_self, __pyx_n_s_kernel_matrix, __pyx_n_s_labels_2, __pyx_n_s_start_dists, __pyx_n_s_center_dists, __pyx_n_s_quality_2, __pyx_n_s_it, __pyx_n_s_sizes, __pyx_n_s_l_bounds, __pyx_n_s_inner_sums_2, __pyx_n_s_labels_old, __pyx_n_s_converged, __pyx_n_s_sizes_old); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__65);
+  __Pyx_GIVEREF(__pyx_tuple__65);
+  __pyx_codeobj__66 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__65, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_elkan, 546, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__66)) __PYX_ERR(0, 546, __pyx_L1_error)
 
-  /* "KKMeans.py":600
+  /* "KKMeans.py":599
  *         return labels, quality, inner_sums, sizes
  * 
  *     def kmeanspp(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes heuristic to get good initial centers
  */
-  __pyx_tuple__71 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_dists_to_centers, __pyx_n_s_n_samples, __pyx_n_s_cluster, __pyx_n_s_index, __pyx_n_s_min_dist_each, __pyx_n_s_probs, __pyx_n_s_center, __pyx_n_s_inner_sum, __pyx_n_s_outer_sum); if (unlikely(!__pyx_tuple__71)) __PYX_ERR(0, 600, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__71);
-  __Pyx_GIVEREF(__pyx_tuple__71);
-  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__71, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_kmeanspp, 600, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_tuple__67 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_dists_to_centers, __pyx_n_s_n_samples, __pyx_n_s_cluster, __pyx_n_s_index, __pyx_n_s_min_dist_each, __pyx_n_s_probs, __pyx_n_s_center, __pyx_n_s_inner_sum, __pyx_n_s_outer_sum); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__67);
+  __Pyx_GIVEREF(__pyx_tuple__67);
+  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_kmeanspp, 599, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 599, __pyx_L1_error)
 
-  /* "KKMeans.py":654
+  /* "KKMeans.py":653
  * 
  * 
  *     def predict(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes the closest cluster center for each x in X
  */
-  __pyx_tuple__73 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_sq_distances); if (unlikely(!__pyx_tuple__73)) __PYX_ERR(0, 654, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__73);
-  __Pyx_GIVEREF(__pyx_tuple__73);
-  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__73, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_predict, 654, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(0, 654, __pyx_L1_error)
-
-  /* "KKMeans.py":689
- * 
- * 
- * def visualize_kkm(data, labels):             # <<<<<<<<<<<<<<
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")
- */
-  __pyx_tuple__75 = PyTuple_Pack(5, __pyx_n_s_data, __pyx_n_s_labels_2, __pyx_n_s_fig, __pyx_n_s_ax, __pyx_n_s_x); if (unlikely(!__pyx_tuple__75)) __PYX_ERR(0, 689, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__75);
-  __Pyx_GIVEREF(__pyx_tuple__75);
-  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__75, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_visualize_kkm, 689, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_tuple__69 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_X_2, __pyx_n_s_kernel_matrix, __pyx_n_s_sq_distances); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 653, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__69);
+  __Pyx_GIVEREF(__pyx_tuple__69);
+  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_KKMeans_py, __pyx_n_s_predict, 653, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 653, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -14964,15 +14375,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "KKMeans.py":5
  * from KKMeans.utils import calc_sq_distances, fill_empty_clusters
  * from KKMeans.kernels import build_kernel_matrix
  * from KKMeans.quality import avg_silhouette             # <<<<<<<<<<<<<<
  * from KKMeans.elkan import update_elkan, start_elkan
- * from matplotlib import pyplot as plt
+ * 
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_avg_silhouette);
   __Pyx_GIVEREF(__pyx_n_s_avg_silhouette);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_avg_silhouette);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_KKMeans_quality, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
@@ -14984,16 +14395,16 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "KKMeans.py":6
  * from KKMeans.kernels import build_kernel_matrix
  * from KKMeans.quality import avg_silhouette
  * from KKMeans.elkan import update_elkan, start_elkan             # <<<<<<<<<<<<<<
- * from matplotlib import pyplot as plt
  * 
+ * class KKMeans():
  */
   __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_update_elkan);
   __Pyx_GIVEREF(__pyx_n_s_update_elkan);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_update_elkan);
   __Pyx_INCREF(__pyx_n_s_start_elkan);
@@ -15008,405 +14419,372 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_start_elkan); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_start_elkan, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "KKMeans.py":7
- * from KKMeans.quality import avg_silhouette
+  /* "KKMeans.py":8
  * from KKMeans.elkan import update_elkan, start_elkan
- * from matplotlib import pyplot as plt             # <<<<<<<<<<<<<<
- * 
- * class KKMeans():
- */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_INCREF(__pyx_n_s_pyplot);
-  __Pyx_GIVEREF(__pyx_n_s_pyplot);
-  PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_pyplot);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_matplotlib, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_pyplot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_plt, __pyx_t_3) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "KKMeans.py":9
- * from matplotlib import pyplot as plt
  * 
  * class KKMeans():             # <<<<<<<<<<<<<<
  *     '''
  *     Kernel K-Means Clustering.
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_KKMeans, __pyx_n_s_KKMeans, (PyObject *) NULL, __pyx_n_s_KKMeans, __pyx_kp_s_Kernel_K_Means_Clustering_Read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_KKMeans, __pyx_n_s_KKMeans, (PyObject *) NULL, __pyx_n_s_KKMeans, __pyx_kp_s_Kernel_K_Means_Clustering_Read); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
 
-  /* "KKMeans.py":117
+  /* "KKMeans.py":116
  * 
  *     '''
  *     def __init__(self, n_clusters=8, init="kmeans++", n_init=3,             # <<<<<<<<<<<<<<
  *                  max_iter=300, tol=1e-4, q_metric="inertia", verbose=False,
  *                  rng=None, algorithm="lloyd", kernel="linear", **kwargs):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_1__init__, 0, __pyx_n_s_KKMeans___init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__31);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init_2, __pyx_t_3) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_1__init__, 0, __pyx_n_s_KKMeans___init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__27);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init_2, __pyx_t_2) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":162
+  /* "KKMeans.py":161
  * 
  * 
  *     def _validate_params(self):             # <<<<<<<<<<<<<<
  *         '''Checks for possible errors in the parameters, can raise exceptions'''
  *         self.__validate_n_clusters()
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_3_validate_params, 0, __pyx_n_s_KKMeans__validate_params, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_validate_params, __pyx_t_3) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_3_validate_params, 0, __pyx_n_s_KKMeans__validate_params, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_validate_params, __pyx_t_2) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":176
+  /* "KKMeans.py":175
  *                   as elkan does not calculate exact distances to every center")
  * 
  *     def __validate_n_clusters(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_clusters, int):
  *             raise ValueError("n_clusters must be int")
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_5__validate_n_clusters, 0, __pyx_n_s_KKMeans___validate_n_clusters, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_n_clusters, __pyx_t_3) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_5__validate_n_clusters, 0, __pyx_n_s_KKMeans___validate_n_clusters, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_n_clusters, __pyx_t_2) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":182
+  /* "KKMeans.py":181
  *             raise ValueError("n_cluster must be >= 1")
  * 
  *     def __validate_init(self):             # <<<<<<<<<<<<<<
  *         if hasattr(self.init, "__iter__") and not isinstance(self.init, str):
  *             self.__validate_centers()
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_7__validate_init, 0, __pyx_n_s_KKMeans___validate_init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_init, __pyx_t_3) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_7__validate_init, 0, __pyx_n_s_KKMeans___validate_init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_init, __pyx_t_2) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":188
+  /* "KKMeans.py":187
  *             raise NotImplementedError("Initialisation method not implemented")
  * 
  *     def __validate_centers(self):             # <<<<<<<<<<<<<<
  *         '''checks for invalid centers, can raise exceptions.'''
  *         self.init = np.asarray(self.init, dtype=np.double)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_9__validate_centers, 0, __pyx_n_s_KKMeans___validate_centers, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_centers, __pyx_t_3) < 0) __PYX_ERR(0, 188, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_9__validate_centers, 0, __pyx_n_s_KKMeans___validate_centers, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_centers, __pyx_t_2) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":199
+  /* "KKMeans.py":198
  *         return self.init
  * 
  *     def __validate_n_init(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.n_init, int):
  *             raise ValueError("n_init must be int")
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_11__validate_n_init, 0, __pyx_n_s_KKMeans___validate_n_init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_n_init, __pyx_t_3) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_11__validate_n_init, 0, __pyx_n_s_KKMeans___validate_n_init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_n_init, __pyx_t_2) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":205
+  /* "KKMeans.py":204
  *             raise ValueError("n_inits must be => 1")
  * 
  *     def __validate_max_iter(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.max_iter, int):
  *             raise ValueError("max_iter must be int")
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_13__validate_max_iter, 0, __pyx_n_s_KKMeans___validate_max_iter, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_max_iter, __pyx_t_3) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_13__validate_max_iter, 0, __pyx_n_s_KKMeans___validate_max_iter, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_max_iter, __pyx_t_2) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":211
+  /* "KKMeans.py":210
  *             raise ValueError("max_iter must be => 1")
  * 
  *     def __validate_algorithm(self):             # <<<<<<<<<<<<<<
  *         if self.algorithm not in ("lloyd", "elkan"):
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_15__validate_algorithm, 0, __pyx_n_s_KKMeans___validate_algorithm, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_algorithm, __pyx_t_3) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_15__validate_algorithm, 0, __pyx_n_s_KKMeans___validate_algorithm, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_algorithm, __pyx_t_2) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":215
+  /* "KKMeans.py":214
  *             raise NotImplementedError(str(self.algorithm)+ " not implemented")
  * 
  *     def __validate_q_metric(self):             # <<<<<<<<<<<<<<
  *         if self.q_metric not in ("silhouette, inertia"):
  *             raise NotImplementedError("Quality metric not implemented")
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_17__validate_q_metric, 0, __pyx_n_s_KKMeans___validate_q_metric, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_q_metric, __pyx_t_3) < 0) __PYX_ERR(0, 215, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_17__validate_q_metric, 0, __pyx_n_s_KKMeans___validate_q_metric, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_q_metric, __pyx_t_2) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":219
+  /* "KKMeans.py":218
  *             raise NotImplementedError("Quality metric not implemented")
  * 
  *     def __validate_tol(self):             # <<<<<<<<<<<<<<
  *         if not isinstance(self.tol, (int, float)):
  *             raise ValueError("tol must be numeric")
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_19__validate_tol, 0, __pyx_n_s_KKMeans___validate_tol, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_tol, __pyx_t_3) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_19__validate_tol, 0, __pyx_n_s_KKMeans___validate_tol, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_tol, __pyx_t_2) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":226
+  /* "KKMeans.py":225
  *             print("Warning! tol < 0 passed, tol set to 0")
  * 
  *     def __validate_kernel(self):             # <<<<<<<<<<<<<<
  *         if self.kernel not in [
  *                 "linear", "rbf", "polynomial",
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_21__validate_kernel, 0, __pyx_n_s_KKMeans___validate_kernel, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_KKMeans__validate_kernel, __pyx_t_3) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_21__validate_kernel, 0, __pyx_n_s_KKMeans___validate_kernel, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_KKMeans__validate_kernel, __pyx_t_2) < 0) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":234
+  /* "KKMeans.py":233
  * 
  * 
  *     def kernel_wrapper(self, X, Y=None):             # <<<<<<<<<<<<<<
  *         '''
  *         Wrapper function to compute kernel matrix
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_23kernel_wrapper, 0, __pyx_n_s_KKMeans_kernel_wrapper, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__45);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_kernel_wrapper, __pyx_t_3) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_23kernel_wrapper, 0, __pyx_n_s_KKMeans_kernel_wrapper, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__41);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_kernel_wrapper, __pyx_t_2) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":253
+  /* "KKMeans.py":252
  *         return build_kernel_matrix(X, Y, kernel=self.kernel, **self.kwargs)
  * 
  *     def fit(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Fits the data X with the given parameters.
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_25fit, 0, __pyx_n_s_KKMeans_fit, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_fit, __pyx_t_3) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_25fit, 0, __pyx_n_s_KKMeans_fit, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_fit, __pyx_t_2) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":299
+  /* "KKMeans.py":298
  *         self._out_finish(best_init)
  * 
  *     def _get_best_init(self, quality_store):             # <<<<<<<<<<<<<<
  *         """Returns best quality score given self.q_metric"""
  *         if self.q_metric == "inertia": # smalles is better
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_27_get_best_init, 0, __pyx_n_s_KKMeans__get_best_init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_best_init, __pyx_t_3) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_27_get_best_init, 0, __pyx_n_s_KKMeans__get_best_init, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_get_best_init, __pyx_t_2) < 0) __PYX_ERR(0, 298, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":311
+  /* "KKMeans.py":310
  *                 this should have been caught in _validate_params")
  * 
  *     def _out_finish(self, best_init):             # <<<<<<<<<<<<<<
  *         '''output at the end of self.fit'''
  *         print("Best " + self.q_metric +":", self.quality_,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_29_out_finish, 0, __pyx_n_s_KKMeans__out_finish, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 311, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_out_finish, __pyx_t_3) < 0) __PYX_ERR(0, 311, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_29_out_finish, 0, __pyx_n_s_KKMeans__out_finish, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_out_finish, __pyx_t_2) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":316
+  /* "KKMeans.py":315
  *               "Found at init:", best_init + 1)
  * 
  *     def _validate_data(self, X):             # <<<<<<<<<<<<<<
  *         """checks for invalidate data, can raise exceptions."""
  *         if len(X.shape) != 2:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_31_validate_data, 0, __pyx_n_s_KKMeans__validate_data, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 316, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_validate_data, __pyx_t_3) < 0) __PYX_ERR(0, 316, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_31_validate_data, 0, __pyx_n_s_KKMeans__validate_data, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_validate_data, __pyx_t_2) < 0) __PYX_ERR(0, 315, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":326
+  /* "KKMeans.py":325
  *         return X
  * 
  *     def _init_labels(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''Assign labels to each datapoint by given method'''
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_33_init_labels, 0, __pyx_n_s_KKMeans__init_labels, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 326, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init_labels, __pyx_t_3) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_33_init_labels, 0, __pyx_n_s_KKMeans__init_labels, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init_labels, __pyx_t_2) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":346
+  /* "KKMeans.py":345
  *         raise NotImplementedError("Unknown initialisation method")
  * 
  *     def _assign_to_centers(self, X, centers):             # <<<<<<<<<<<<<<
  *         '''
  *         Assigns each datapoint to the closest given center.
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_35_assign_to_centers, 0, __pyx_n_s_KKMeans__assign_to_centers, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_assign_to_centers, __pyx_t_3) < 0) __PYX_ERR(0, 346, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_35_assign_to_centers, 0, __pyx_n_s_KKMeans__assign_to_centers, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_assign_to_centers, __pyx_t_2) < 0) __PYX_ERR(0, 345, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":377
+  /* "KKMeans.py":376
  *         return np.asarray(np.argmin(dists_to_centers, axis=1), dtype=np.int_)
  * 
  *     def lloyd(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a run of lloyd's algorithm
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_37lloyd, 0, __pyx_n_s_KKMeans_lloyd, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_lloyd, __pyx_t_3) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_37lloyd, 0, __pyx_n_s_KKMeans_lloyd, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__55)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_lloyd, __pyx_t_2) < 0) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":429
+  /* "KKMeans.py":428
  * 
  * 
  *     def _out_verbose(self, iter, quality, converged):             # <<<<<<<<<<<<<<
  *         '''Checks if self.verbose and prints accordingly'''
  *         if not self.verbose:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_39_out_verbose, 0, __pyx_n_s_KKMeans__out_verbose, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 429, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_out_verbose, __pyx_t_3) < 0) __PYX_ERR(0, 429, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_39_out_verbose, 0, __pyx_n_s_KKMeans__out_verbose, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_out_verbose, __pyx_t_2) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":441
+  /* "KKMeans.py":440
  * 
  * 
  *     def _measure_iter(self, sq_distances, labels, labels_old, quality):             # <<<<<<<<<<<<<<
  *         '''
  *         Measures quality of iteration and checks for convergence
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_41_measure_iter, 0, __pyx_n_s_KKMeans__measure_iter, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__63)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_measure_iter, __pyx_t_3) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_41_measure_iter, 0, __pyx_n_s_KKMeans__measure_iter, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_measure_iter, __pyx_t_2) < 0) __PYX_ERR(0, 440, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":483
+  /* "KKMeans.py":482
  *         return quality, converged
  * 
  *     def calc_q_metric(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Calculates quality metric
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_43calc_q_metric, 0, __pyx_n_s_KKMeans_calc_q_metric, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 483, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calc_q_metric, __pyx_t_3) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_43calc_q_metric, 0, __pyx_n_s_KKMeans_calc_q_metric, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_calc_q_metric, __pyx_t_2) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":513
+  /* "KKMeans.py":512
  *             raise NotImplementedError(str(self.q_metric) + " quality metric not implemented")
  * 
  *     def calc_silhouette(self, sq_distances, labels):             # <<<<<<<<<<<<<<
  *         '''Calculates average silhouette of clustering
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_45calc_silhouette, 0, __pyx_n_s_KKMeans_calc_silhouette, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 513, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_calc_silhouette, __pyx_t_3) < 0) __PYX_ERR(0, 513, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_45calc_silhouette, 0, __pyx_n_s_KKMeans_calc_silhouette, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_calc_silhouette, __pyx_t_2) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":532
+  /* "KKMeans.py":531
  *         return avg_silhouette(sq_distances, labels)
  * 
  *     def _build_starting_distance(self, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Builds basis for computing square distances
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_47_build_starting_distance, 0, __pyx_n_s_KKMeans__build_starting_distance, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 532, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_build_starting_distance, __pyx_t_3) < 0) __PYX_ERR(0, 532, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_47_build_starting_distance, 0, __pyx_n_s_KKMeans__build_starting_distance, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 531, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_build_starting_distance, __pyx_t_2) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":547
+  /* "KKMeans.py":546
  *         return np.ascontiguousarray(np.tile(np.diag(kernel_matrix), (self.n_clusters, 1)).T, dtype=np.double)
  * 
  *     def elkan(self, kernel_matrix, labels):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes a slightly optimized Kernel-Kmeans heuristic
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_49elkan, 0, __pyx_n_s_KKMeans_elkan, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 547, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_elkan, __pyx_t_3) < 0) __PYX_ERR(0, 547, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_49elkan, 0, __pyx_n_s_KKMeans_elkan, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_elkan, __pyx_t_2) < 0) __PYX_ERR(0, 546, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":600
+  /* "KKMeans.py":599
  *         return labels, quality, inner_sums, sizes
  * 
  *     def kmeanspp(self, X, kernel_matrix):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes heuristic to get good initial centers
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_51kmeanspp, 0, __pyx_n_s_KKMeans_kmeanspp, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 600, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_kmeanspp, __pyx_t_3) < 0) __PYX_ERR(0, 600, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_51kmeanspp, 0, __pyx_n_s_KKMeans_kmeanspp, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_kmeanspp, __pyx_t_2) < 0) __PYX_ERR(0, 599, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":654
+  /* "KKMeans.py":653
  * 
  * 
  *     def predict(self, X):             # <<<<<<<<<<<<<<
  *         '''
  *         Computes the closest cluster center for each x in X
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_53predict, 0, __pyx_n_s_KKMeans_predict, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__74)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 654, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_predict, __pyx_t_3) < 0) __PYX_ERR(0, 654, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7KKMeans_53predict, 0, __pyx_n_s_KKMeans_predict, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 653, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_predict, __pyx_t_2) < 0) __PYX_ERR(0, 653, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "KKMeans.py":9
- * from matplotlib import pyplot as plt
+  /* "KKMeans.py":8
+ * from KKMeans.elkan import update_elkan, start_elkan
  * 
  * class KKMeans():             # <<<<<<<<<<<<<<
  *     '''
  *     Kernel K-Means Clustering.
  */
-  __pyx_t_3 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_KKMeans, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_KKMeans, __pyx_t_3) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "KKMeans.py":689
- * 
- * 
- * def visualize_kkm(data, labels):             # <<<<<<<<<<<<<<
- *     if len(data[0]) > 3:
- *         raise Exception("Dimensionality is too high for visualization")
- */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_1visualize_kkm, 0, __pyx_n_s_visualize_kkm, NULL, __pyx_n_s_KKMeans, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_KKMeans, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_visualize_kkm, __pyx_t_2) < 0) __PYX_ERR(0, 689, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_KKMeans, __pyx_t_2) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "KKMeans.py":1
  * import numpy as np             # <<<<<<<<<<<<<<
  * from KKMeans.lloyd import update_lloyd
  * from KKMeans.utils import calc_sq_distances, fill_empty_clusters
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -17628,15 +17006,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__27;
+    PyObject *module, *from_list, *star = __pyx_n_s__23;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -17691,15 +17069,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__28);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__24);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -19410,15 +18788,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__77));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__71));
     }
     return name;
 }
 #endif
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
```

### Comparing `KKMeans-0.0.3/src/KKMeans/KKMeans.py` & `KKMeans-0.0.4/src/KKMeans/KKMeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from KKMeans.lloyd import update_lloyd
 from KKMeans.utils import calc_sq_distances, fill_empty_clusters
 from KKMeans.kernels import build_kernel_matrix
 from KKMeans.quality import avg_silhouette
 from KKMeans.elkan import update_elkan, start_elkan
-from matplotlib import pyplot as plt
 
 class KKMeans():
     '''
     Kernel K-Means Clustering.
 
     Read more in the thesis. TODO
     Designed to mimic sklearn.cluster.KMeans
@@ -678,22 +677,8 @@
         if self.X_ is None:
             raise ValueError("KKMeans instance is not fitted!")
         kernel_matrix = self.kernel_wrapper(X, self.X_)
         sq_distances = calc_sq_distances(
             self.inner_sums_, self.cluster_sizes_,
             kernel_matrix, self.labels_, 
             self.n_clusters)
-        return np.argmin(sq_distances, axis=1)
-
-
-
-def visualize_kkm(data, labels):
-    if len(data[0]) > 3:
-        raise Exception("Dimensionality is too high for visualization")
-    elif len(data[0]) == 1:
-        plt.scatter(data, [0 for x in range(len(data))], c = labels)
-    elif len(data[0]) == 2:
-        plt.scatter(data[:,0], data[:,1], c = labels)
-    elif len(data[0]) == 3:
-        fig = plt.figure()
-        ax = fig.add_subplot(projection = "3d")
-        ax.scatter(data[:,0], data[:,1], data[:,2], c = labels)
+        return np.argmin(sq_distances, axis=1)
```

### Comparing `KKMeans-0.0.3/src/KKMeans/elkan.c` & `KKMeans-0.0.4/src/KKMeans/elkan.c`

 * *Files 0% similar despite different names*

```diff
@@ -18246,15 +18246,15 @@
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
                             }
                             __pyx_parallel_why = 4;
                             goto __pyx_L13;
                             __pyx_L13:;
                             #ifdef _OPENMP
-                            #pragma omp critical(__pyx_parallel_lastprivates0)
+                            #pragma omp critical(__pyx_parallel_lastprivates1)
                             #endif /* _OPENMP */
                             {
                                 __pyx_parallel_temp0 = __pyx_v_i;
                                 __pyx_parallel_temp1 = __pyx_v_j;
                                 __pyx_parallel_temp2 = __pyx_v_labels_i;
                                 __pyx_parallel_temp3 = __pyx_v_outer_sum;
                             }
```

### Comparing `KKMeans-0.0.3/src/KKMeans/elkan.pyx` & `KKMeans-0.0.4/src/KKMeans/elkan.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.3/src/KKMeans/kernels.c` & `KKMeans-0.0.4/src/KKMeans/kernels.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.3/src/KKMeans/kernels.pyx` & `KKMeans-0.0.4/src/KKMeans/kernels.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.3/src/KKMeans/lloyd.c` & `KKMeans-0.0.4/src/KKMeans/lloyd.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.3/src/KKMeans/lloyd.pyx` & `KKMeans-0.0.4/src/KKMeans/lloyd.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.3/src/KKMeans/quality.c` & `KKMeans-0.0.4/src/KKMeans/quality.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
-            "/O2",
-            "-DCYTHON_WITHOUT_ASSERTIONS",
-            "/openmp"
+            "-DCYTHON_WITHOUT_ASSERTIONS"
         ],
         "name": "KKMeans.quality",
         "sources": [
             "src/KKMeans/quality.pyx"
         ]
     },
     "module_name": "KKMeans.quality"
@@ -2447,21 +2445,25 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_long(PyObject *, int writable_flag);
 
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *, int writable_flag);
-
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj);
 
+/* MemviewDtypeToObject.proto */
+static CYTHON_INLINE PyObject *__pyx_memview_get_long(const char *itemp);
+static CYTHON_INLINE int __pyx_memview_set_long(const char *itemp, PyObject *obj);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *, int writable_flag);
+
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object);
 
@@ -2486,25 +2488,25 @@
     __pyx_atomic_int_type *acquisition_count, PyThread_type_lock lock);
 #define __pyx_get_slice_count_pointer(memview) (&memview->acquisition_count)
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XCLEAR_MEMVIEW(slice, have_gil) __Pyx_XCLEAR_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XCLEAR_MEMVIEW(__Pyx_memviewslice *, int, int);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+/* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
@@ -2614,15 +2616,15 @@
 static const char __pyx_k__2[] = ".";
 static const char __pyx_k__3[] = "*";
 static const char __pyx_k__6[] = "'";
 static const char __pyx_k__7[] = ")";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
-static const char __pyx_k__24[] = "?";
+static const char __pyx_k__25[] = "?";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_got[] = " (got ";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_sys[] = "sys";
@@ -2855,15 +2857,15 @@
   PyObject *__pyx_n_s_Sequence;
   PyObject *__pyx_kp_s_Step_may_not_be_zero_axis_d;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_View_MemoryView;
   PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_n_s__24;
+  PyObject *__pyx_n_s__25;
   PyObject *__pyx_n_s__3;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_s_abc;
   PyObject *__pyx_n_s_allocate_buffer;
   PyObject *__pyx_kp_u_and;
@@ -2981,17 +2983,18 @@
   PyObject *__pyx_tuple__14;
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__16;
   PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__18;
   PyObject *__pyx_tuple__19;
   PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__23;
   PyObject *__pyx_codeobj__20;
   PyObject *__pyx_codeobj__22;
-  PyObject *__pyx_codeobj__23;
+  PyObject *__pyx_codeobj__24;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -3068,15 +3071,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Sequence);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_View_MemoryView);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_n_s__24);
+  Py_CLEAR(clear_module_state->__pyx_n_s__25);
   Py_CLEAR(clear_module_state->__pyx_n_s__3);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_abc);
   Py_CLEAR(clear_module_state->__pyx_n_s_allocate_buffer);
   Py_CLEAR(clear_module_state->__pyx_kp_u_and);
@@ -3194,17 +3197,18 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__14);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
   Py_CLEAR(clear_module_state->__pyx_tuple__19);
   Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__23);
   Py_CLEAR(clear_module_state->__pyx_codeobj__20);
   Py_CLEAR(clear_module_state->__pyx_codeobj__22);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3259,15 +3263,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Sequence);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_View_MemoryView);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_n_s__24);
+  Py_VISIT(traverse_module_state->__pyx_n_s__25);
   Py_VISIT(traverse_module_state->__pyx_n_s__3);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_abc);
   Py_VISIT(traverse_module_state->__pyx_n_s_allocate_buffer);
   Py_VISIT(traverse_module_state->__pyx_kp_u_and);
@@ -3385,17 +3389,18 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__14);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
   Py_VISIT(traverse_module_state->__pyx_tuple__19);
   Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__23);
   Py_VISIT(traverse_module_state->__pyx_codeobj__20);
   Py_VISIT(traverse_module_state->__pyx_codeobj__22);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3460,15 +3465,15 @@
 #define __pyx_n_s_Sequence __pyx_mstate_global->__pyx_n_s_Sequence
 #define __pyx_kp_s_Step_may_not_be_zero_axis_d __pyx_mstate_global->__pyx_kp_s_Step_may_not_be_zero_axis_d
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_s_Unable_to_convert_item_to_object __pyx_mstate_global->__pyx_kp_s_Unable_to_convert_item_to_object
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_View_MemoryView __pyx_mstate_global->__pyx_n_s_View_MemoryView
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_n_s__24 __pyx_mstate_global->__pyx_n_s__24
+#define __pyx_n_s__25 __pyx_mstate_global->__pyx_n_s__25
 #define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_s_abc __pyx_mstate_global->__pyx_n_s_abc
 #define __pyx_n_s_allocate_buffer __pyx_mstate_global->__pyx_n_s_allocate_buffer
 #define __pyx_kp_u_and __pyx_mstate_global->__pyx_kp_u_and
@@ -3586,17 +3591,18 @@
 #define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
 #define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
 #define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
 #define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
-#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
 /* #### Code section: module_code ### */
 
 /* "View.MemoryView":131
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
@@ -16901,27 +16907,27 @@
   return __pyx_r;
 }
 
 /* "KKMeans/quality.pyx":7
  *     cdef double DBL_MAX
  * 
  * def avg_silhouette(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
- *     '''returns the average silhouette of a dataset
- *     '''
+ *     '''returns the average silhouette of a dataset'''
+ *     silhouettes = calc_silhouettes(distances, labels)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_7KKMeans_7quality_1avg_silhouette(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7KKMeans_7quality_avg_silhouette, "returns the average silhouette of a dataset\n    ");
+PyDoc_STRVAR(__pyx_doc_7KKMeans_7quality_avg_silhouette, "returns the average silhouette of a dataset");
 static PyMethodDef __pyx_mdef_7KKMeans_7quality_1avg_silhouette = {"avg_silhouette", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7KKMeans_7quality_1avg_silhouette, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7KKMeans_7quality_avg_silhouette};
 static PyObject *__pyx_pw_7KKMeans_7quality_1avg_silhouette(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
@@ -16994,530 +17000,136 @@
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_distances, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7KKMeans_7quality_avg_silhouette(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_distances, __Pyx_memviewslice __pyx_v_labels) {
-  Py_ssize_t __pyx_v_n_samples;
-  Py_ssize_t __pyx_v_n_clusters;
-  __Pyx_memviewslice __pyx_v_silhouettes = { 0, 0, { 0 }, { 0 }, { 0 } };
-  Py_ssize_t __pyx_v_i;
-  Py_ssize_t __pyx_v_j;
-  long __pyx_v_labels_i;
-  double __pyx_v_a;
-  double __pyx_v_b;
-  double __pyx_v_max_a_b;
+  PyObject *__pyx_v_silhouettes = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  int __pyx_t_7;
-  Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
-  Py_ssize_t __pyx_t_12;
-  Py_ssize_t __pyx_t_13;
-  Py_ssize_t __pyx_t_14;
-  Py_ssize_t __pyx_t_15;
-  double __pyx_t_16;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("avg_silhouette", 0);
 
-  /* "KKMeans/quality.pyx":11
- *     '''
- *     cdef:
- *         Py_ssize_t n_samples = distances.shape[0]             # <<<<<<<<<<<<<<
- *         Py_ssize_t n_clusters = distances.shape[1]
- *         double[::1] silhouettes = np.zeros(n_samples)
- */
-  __pyx_v_n_samples = (__pyx_v_distances.shape[0]);
-
-  /* "KKMeans/quality.pyx":12
- *     cdef:
- *         Py_ssize_t n_samples = distances.shape[0]
- *         Py_ssize_t n_clusters = distances.shape[1]             # <<<<<<<<<<<<<<
- *         double[::1] silhouettes = np.zeros(n_samples)
- *         Py_ssize_t i, j
- */
-  __pyx_v_n_clusters = (__pyx_v_distances.shape[1]);
-
-  /* "KKMeans/quality.pyx":13
- *         Py_ssize_t n_samples = distances.shape[0]
- *         Py_ssize_t n_clusters = distances.shape[1]
- *         double[::1] silhouettes = np.zeros(n_samples)             # <<<<<<<<<<<<<<
- *         Py_ssize_t i, j
- *         long labels_i
+  /* "KKMeans/quality.pyx":9
+ * def avg_silhouette(double[:, ::1] distances, long[::1] labels):
+ *     '''returns the average silhouette of a dataset'''
+ *     silhouettes = calc_silhouettes(distances, labels)             # <<<<<<<<<<<<<<
+ *     return np.sum(silhouettes)/len(silhouettes)
+ * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_calc_silhouettes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_distances, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_n_samples); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_labels, 1, (PyObject *(*)(char *)) __pyx_memview_get_long, (int (*)(char *, PyObject *)) __pyx_memview_set_long, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = NULL;
+  __pyx_t_6 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_5 = 1;
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_6 = 1;
     }
   }
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_silhouettes = __pyx_t_6;
-  __pyx_t_6.memview = NULL;
-  __pyx_t_6.data = NULL;
-
-  /* "KKMeans/quality.pyx":18
- *         double a, b, max_a_b
- * 
- *     if n_clusters <= 1:             # <<<<<<<<<<<<<<
- *         raise ValueError("Must have at least two clusters for silhouette")
- *     for i in prange(n_samples, nogil=True):
- */
-  __pyx_t_7 = (__pyx_v_n_clusters <= 1);
-  if (unlikely(__pyx_t_7)) {
-
-    /* "KKMeans/quality.pyx":19
- * 
- *     if n_clusters <= 1:
- *         raise ValueError("Must have at least two clusters for silhouette")             # <<<<<<<<<<<<<<
- *     for i in prange(n_samples, nogil=True):
- *         labels_i = labels[i]
- */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 19, __pyx_L1_error)
-
-    /* "KKMeans/quality.pyx":18
- *         double a, b, max_a_b
- * 
- *     if n_clusters <= 1:             # <<<<<<<<<<<<<<
- *         raise ValueError("Must have at least two clusters for silhouette")
- *     for i in prange(n_samples, nogil=True):
- */
-  }
-
-  /* "KKMeans/quality.pyx":20
- *     if n_clusters <= 1:
- *         raise ValueError("Must have at least two clusters for silhouette")
- *     for i in prange(n_samples, nogil=True):             # <<<<<<<<<<<<<<
- *         labels_i = labels[i]
- *         a = distances[i, labels_i]
- */
-  {
-      #ifdef WITH_THREAD
-      PyThreadState *_save;
-      _save = NULL;
-      Py_UNBLOCK_THREADS
-      __Pyx_FastGIL_Remember();
-      #endif
-      /*try:*/ {
-        __pyx_t_8 = __pyx_v_n_samples;
-        {
-            double __pyx_parallel_temp0 = ((double)__PYX_NAN());
-            double __pyx_parallel_temp1 = ((double)__PYX_NAN());
-            Py_ssize_t __pyx_parallel_temp2 = ((Py_ssize_t)0xbad0bad0);
-            Py_ssize_t __pyx_parallel_temp3 = ((Py_ssize_t)0xbad0bad0);
-            long __pyx_parallel_temp4 = ((long)0xbad0bad0);
-            double __pyx_parallel_temp5 = ((double)__PYX_NAN());
-            const char *__pyx_parallel_filename = NULL; int __pyx_parallel_lineno = 0, __pyx_parallel_clineno = 0;
-            PyObject *__pyx_parallel_exc_type = NULL, *__pyx_parallel_exc_value = NULL, *__pyx_parallel_exc_tb = NULL;
-            int __pyx_parallel_why;
-            __pyx_parallel_why = 0;
-            #if ((defined(__APPLE__) || defined(__OSX__)) && (defined(__GNUC__) && (__GNUC__ > 2 || (__GNUC__ == 2 && (__GNUC_MINOR__ > 95)))))
-                #undef likely
-                #undef unlikely
-                #define likely(x)   (x)
-                #define unlikely(x) (x)
-            #endif
-            __pyx_t_10 = (__pyx_t_8 - 0 + 1 - 1/abs(1)) / 1;
-            if (__pyx_t_10 > 0)
-            {
-                #ifdef _OPENMP
-                #pragma omp parallel private(__pyx_t_11, __pyx_t_12, __pyx_t_13, __pyx_t_14, __pyx_t_15, __pyx_t_16, __pyx_t_7) private(__pyx_filename, __pyx_lineno, __pyx_clineno) shared(__pyx_parallel_why, __pyx_parallel_exc_type, __pyx_parallel_exc_value, __pyx_parallel_exc_tb)
-                #endif /* _OPENMP */
-                {
-                    #ifdef _OPENMP
-                    #ifdef WITH_THREAD
-                    PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-                    #endif
-                    Py_BEGIN_ALLOW_THREADS
-                    #endif /* _OPENMP */
-                    #ifdef _OPENMP
-                    #pragma omp for lastprivate(__pyx_v_a) lastprivate(__pyx_v_b) firstprivate(__pyx_v_i) lastprivate(__pyx_v_i) lastprivate(__pyx_v_j) lastprivate(__pyx_v_labels_i) lastprivate(__pyx_v_max_a_b)
-                    #endif /* _OPENMP */
-                    for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_10; __pyx_t_9++){
-                        if (__pyx_parallel_why < 2)
-                        {
-                            __pyx_v_i = (Py_ssize_t)(0 + 1 * __pyx_t_9);
-                            /* Initialize private variables to invalid values */
-                            __pyx_v_a = ((double)__PYX_NAN());
-                            __pyx_v_b = ((double)__PYX_NAN());
-                            __pyx_v_j = ((Py_ssize_t)0xbad0bad0);
-                            __pyx_v_labels_i = ((long)0xbad0bad0);
-                            __pyx_v_max_a_b = ((double)__PYX_NAN());
-
-                            /* "KKMeans/quality.pyx":21
- *         raise ValueError("Must have at least two clusters for silhouette")
- *     for i in prange(n_samples, nogil=True):
- *         labels_i = labels[i]             # <<<<<<<<<<<<<<
- *         a = distances[i, labels_i]
- *         b = DBL_MAX
- */
-                            __pyx_t_11 = __pyx_v_i;
-                            __pyx_v_labels_i = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_11)) )));
-
-                            /* "KKMeans/quality.pyx":22
- *     for i in prange(n_samples, nogil=True):
- *         labels_i = labels[i]
- *         a = distances[i, labels_i]             # <<<<<<<<<<<<<<
- *         b = DBL_MAX
- *         for j in range(n_clusters):
- */
-                            __pyx_t_11 = __pyx_v_i;
-                            __pyx_t_12 = __pyx_v_labels_i;
-                            __pyx_v_a = (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_distances.data + __pyx_t_11 * __pyx_v_distances.strides[0]) )) + __pyx_t_12)) )));
-
-                            /* "KKMeans/quality.pyx":23
- *         labels_i = labels[i]
- *         a = distances[i, labels_i]
- *         b = DBL_MAX             # <<<<<<<<<<<<<<
- *         for j in range(n_clusters):
- *             if j == labels_i:
- */
-                            __pyx_v_b = DBL_MAX;
-
-                            /* "KKMeans/quality.pyx":24
- *         a = distances[i, labels_i]
- *         b = DBL_MAX
- *         for j in range(n_clusters):             # <<<<<<<<<<<<<<
- *             if j == labels_i:
- *                 continue
- */
-                            __pyx_t_13 = __pyx_v_n_clusters;
-                            __pyx_t_14 = __pyx_t_13;
-                            for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
-                              __pyx_v_j = __pyx_t_15;
-
-                              /* "KKMeans/quality.pyx":25
- *         b = DBL_MAX
- *         for j in range(n_clusters):
- *             if j == labels_i:             # <<<<<<<<<<<<<<
- *                 continue
- *             b = min(distances[i, j], b)
- */
-                              __pyx_t_7 = (__pyx_v_j == __pyx_v_labels_i);
-                              if (__pyx_t_7) {
-
-                                /* "KKMeans/quality.pyx":26
- *         for j in range(n_clusters):
- *             if j == labels_i:
- *                 continue             # <<<<<<<<<<<<<<
- *             b = min(distances[i, j], b)
- *         max_a_b = max(a,b)
- */
-                                goto __pyx_L11_continue;
-
-                                /* "KKMeans/quality.pyx":25
- *         b = DBL_MAX
- *         for j in range(n_clusters):
- *             if j == labels_i:             # <<<<<<<<<<<<<<
- *                 continue
- *             b = min(distances[i, j], b)
- */
-                              }
-
-                              /* "KKMeans/quality.pyx":27
- *             if j == labels_i:
- *                 continue
- *             b = min(distances[i, j], b)             # <<<<<<<<<<<<<<
- *         max_a_b = max(a,b)
- *         if max_a_b == 0:
- */
-                              __pyx_t_12 = __pyx_v_i;
-                              __pyx_t_11 = __pyx_v_j;
-                              __pyx_t_16 = __pyx_f_7KKMeans_7quality_min((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_distances.data + __pyx_t_12 * __pyx_v_distances.strides[0]) )) + __pyx_t_11)) ))), __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 27, __pyx_L9_error)
-                              __pyx_v_b = __pyx_t_16;
-                              __pyx_L11_continue:;
-                            }
-
-                            /* "KKMeans/quality.pyx":28
- *                 continue
- *             b = min(distances[i, j], b)
- *         max_a_b = max(a,b)             # <<<<<<<<<<<<<<
- *         if max_a_b == 0:
- *             # if max_a_b = 0, a == b == 0 as dists always positive
- */
-                            __pyx_t_16 = __pyx_f_7KKMeans_7quality_max(__pyx_v_a, __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 28, __pyx_L9_error)
-                            __pyx_v_max_a_b = __pyx_t_16;
-
-                            /* "KKMeans/quality.pyx":29
- *             b = min(distances[i, j], b)
- *         max_a_b = max(a,b)
- *         if max_a_b == 0:             # <<<<<<<<<<<<<<
- *             # if max_a_b = 0, a == b == 0 as dists always positive
- *             silhouettes[i] = 0
- */
-                            __pyx_t_7 = (__pyx_v_max_a_b == 0.0);
-                            if (__pyx_t_7) {
-
-                              /* "KKMeans/quality.pyx":31
- *         if max_a_b == 0:
- *             # if max_a_b = 0, a == b == 0 as dists always positive
- *             silhouettes[i] = 0             # <<<<<<<<<<<<<<
- *             continue
- *         silhouettes[i] = (b - a) / max(a,b)
- */
-                              __pyx_t_11 = __pyx_v_i;
-                              *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_silhouettes.data) + __pyx_t_11)) )) = 0.0;
-
-                              /* "KKMeans/quality.pyx":32
- *             # if max_a_b = 0, a == b == 0 as dists always positive
- *             silhouettes[i] = 0
- *             continue             # <<<<<<<<<<<<<<
- *         silhouettes[i] = (b - a) / max(a,b)
- *     return np.sum(silhouettes)/len(silhouettes)
- */
-                              goto __pyx_L7_continue;
-
-                              /* "KKMeans/quality.pyx":29
- *             b = min(distances[i, j], b)
- *         max_a_b = max(a,b)
- *         if max_a_b == 0:             # <<<<<<<<<<<<<<
- *             # if max_a_b = 0, a == b == 0 as dists always positive
- *             silhouettes[i] = 0
- */
-                            }
-
-                            /* "KKMeans/quality.pyx":33
- *             silhouettes[i] = 0
- *             continue
- *         silhouettes[i] = (b - a) / max(a,b)             # <<<<<<<<<<<<<<
- *     return np.sum(silhouettes)/len(silhouettes)
- * 
- */
-                            __pyx_t_16 = __pyx_f_7KKMeans_7quality_max(__pyx_v_a, __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 33, __pyx_L9_error)
-                            __pyx_t_11 = __pyx_v_i;
-                            *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_silhouettes.data) + __pyx_t_11)) )) = ((__pyx_v_b - __pyx_v_a) / __pyx_t_16);
-                            goto __pyx_L16;
-                            __pyx_L7_continue:;
-                            goto __pyx_L16;
-                            __pyx_L9_error:;
-                            {
-                                #ifdef WITH_THREAD
-                                PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-                                #endif
-                                #ifdef _OPENMP
-                                #pragma omp flush(__pyx_parallel_exc_type)
-                                #endif /* _OPENMP */
-                                if (!__pyx_parallel_exc_type) {
-                                  __Pyx_ErrFetchWithState(&__pyx_parallel_exc_type, &__pyx_parallel_exc_value, &__pyx_parallel_exc_tb);
-                                  __pyx_parallel_filename = __pyx_filename; __pyx_parallel_lineno = __pyx_lineno; __pyx_parallel_clineno = __pyx_clineno;
-                                  __Pyx_GOTREF(__pyx_parallel_exc_type);
-                                }
-                                #ifdef WITH_THREAD
-                                __Pyx_PyGILState_Release(__pyx_gilstate_save);
-                                #endif
-                            }
-                            __pyx_parallel_why = 4;
-                            goto __pyx_L15;
-                            __pyx_L15:;
-                            #ifdef _OPENMP
-                            #pragma omp critical(__pyx_parallel_lastprivates1)
-                            #endif /* _OPENMP */
-                            {
-                                __pyx_parallel_temp0 = __pyx_v_a;
-                                __pyx_parallel_temp1 = __pyx_v_b;
-                                __pyx_parallel_temp2 = __pyx_v_i;
-                                __pyx_parallel_temp3 = __pyx_v_j;
-                                __pyx_parallel_temp4 = __pyx_v_labels_i;
-                                __pyx_parallel_temp5 = __pyx_v_max_a_b;
-                            }
-                            __pyx_L16:;
-                            #ifdef _OPENMP
-                            #pragma omp flush(__pyx_parallel_why)
-                            #endif /* _OPENMP */
-                        }
-                    }
-                    #ifdef _OPENMP
-                    Py_END_ALLOW_THREADS
-                    #else
-{
-#ifdef WITH_THREAD
-                    PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-                    #endif
-                    #endif /* _OPENMP */
-                    /* Clean up any temporaries */
-                    #ifdef WITH_THREAD
-                    __Pyx_PyGILState_Release(__pyx_gilstate_save);
-                    #endif
-                    #ifndef _OPENMP
-}
-#endif /* _OPENMP */
-                }
-            }
-            if (__pyx_parallel_exc_type) {
-              /* This may have been overridden by a continue, break or return in another thread. Prefer the error. */
-              __pyx_parallel_why = 4;
-            }
-            if (__pyx_parallel_why) {
-              __pyx_v_a = __pyx_parallel_temp0;
-              __pyx_v_b = __pyx_parallel_temp1;
-              __pyx_v_i = __pyx_parallel_temp2;
-              __pyx_v_j = __pyx_parallel_temp3;
-              __pyx_v_labels_i = __pyx_parallel_temp4;
-              __pyx_v_max_a_b = __pyx_parallel_temp5;
-              switch (__pyx_parallel_why) {
-                    case 4:
-                {
-                    #ifdef WITH_THREAD
-                    PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
-                    #endif
-                    __Pyx_GIVEREF(__pyx_parallel_exc_type);
-                    __Pyx_ErrRestoreWithState(__pyx_parallel_exc_type, __pyx_parallel_exc_value, __pyx_parallel_exc_tb);
-                    __pyx_filename = __pyx_parallel_filename; __pyx_lineno = __pyx_parallel_lineno; __pyx_clineno = __pyx_parallel_clineno;
-                    #ifdef WITH_THREAD
-                    __Pyx_PyGILState_Release(__pyx_gilstate_save);
-                    #endif
-                }
-                goto __pyx_L5_error;
-              }
-            }
-        }
-        #if ((defined(__APPLE__) || defined(__OSX__)) && (defined(__GNUC__) && (__GNUC__ > 2 || (__GNUC__ == 2 && (__GNUC_MINOR__ > 95)))))
-            #undef likely
-            #undef unlikely
-            #define likely(x)   __builtin_expect(!!(x), 1)
-            #define unlikely(x) __builtin_expect(!!(x), 0)
-        #endif
-      }
-
-      /* "KKMeans/quality.pyx":20
- *     if n_clusters <= 1:
- *         raise ValueError("Must have at least two clusters for silhouette")
- *     for i in prange(n_samples, nogil=True):             # <<<<<<<<<<<<<<
- *         labels_i = labels[i]
- *         a = distances[i, labels_i]
- */
-      /*finally:*/ {
-        /*normal exit:*/{
-          #ifdef WITH_THREAD
-          __Pyx_FastGIL_Forget();
-          Py_BLOCK_THREADS
-          #endif
-          goto __pyx_L6;
-        }
-        __pyx_L5_error: {
-          #ifdef WITH_THREAD
-          __Pyx_FastGIL_Forget();
-          Py_BLOCK_THREADS
-          #endif
-          goto __pyx_L1_error;
-        }
-        __pyx_L6:;
-      }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
+  __pyx_v_silhouettes = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-  /* "KKMeans/quality.pyx":34
- *             continue
- *         silhouettes[i] = (b - a) / max(a,b)
+  /* "KKMeans/quality.pyx":10
+ *     '''returns the average silhouette of a dataset'''
+ *     silhouettes = calc_silhouettes(distances, labels)
  *     return np.sum(silhouettes)/len(silhouettes)             # <<<<<<<<<<<<<<
  * 
  * def calc_silhouettes(double[:, ::1] distances, long[::1] labels):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_sum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_silhouettes, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = NULL;
-  __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sum); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_6 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_5 = 1;
+      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __pyx_t_6 = 1;
     }
   }
   {
-    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+    PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_silhouettes};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_10 = __Pyx_MemoryView_Len(__pyx_v_silhouettes); 
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_v_silhouettes); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "KKMeans/quality.pyx":7
  *     cdef double DBL_MAX
  * 
  * def avg_silhouette(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
- *     '''returns the average silhouette of a dataset
- *     '''
+ *     '''returns the average silhouette of a dataset'''
+ *     silhouettes = calc_silhouettes(distances, labels)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __PYX_XCLEAR_MEMVIEW(&__pyx_t_6, 1);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("KKMeans.quality.avg_silhouette", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __PYX_XCLEAR_MEMVIEW(&__pyx_v_silhouettes, 1);
+  __Pyx_XDECREF(__pyx_v_silhouettes);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/quality.pyx":36
+/* "KKMeans/quality.pyx":12
  *     return np.sum(silhouettes)/len(silhouettes)
  * 
  * def calc_silhouettes(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
  *     '''
  *     calculates the silhouette of each datapoint
  */
 
@@ -17563,40 +17175,40 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_distances)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 12, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 36, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 12, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("calc_silhouettes", 1, 2, 2, 1); __PYX_ERR(0, 36, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("calc_silhouettes", 1, 2, 2, 1); __PYX_ERR(0, 12, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_silhouettes") < 0)) __PYX_ERR(0, 36, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_silhouettes") < 0)) __PYX_ERR(0, 12, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_distances = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_distances.memview)) __PYX_ERR(0, 36, __pyx_L3_error)
-    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 36, __pyx_L3_error)
+    __pyx_v_distances = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_distances.memview)) __PYX_ERR(0, 12, __pyx_L3_error)
+    __pyx_v_labels = __Pyx_PyObject_to_MemoryviewSlice_dc_long(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_labels.memview)) __PYX_ERR(0, 12, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("calc_silhouettes", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 36, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("calc_silhouettes", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 12, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_distances, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_labels, 1);
   __Pyx_AddTraceback("KKMeans.quality.calc_silhouettes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -17638,45 +17250,45 @@
   Py_ssize_t __pyx_t_15;
   double __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calc_silhouettes", 0);
 
-  /* "KKMeans/quality.pyx":55
+  /* "KKMeans/quality.pyx":31
  *     '''
  *     cdef:
  *         Py_ssize_t n_samples = distances.shape[0]             # <<<<<<<<<<<<<<
  *         Py_ssize_t n_clusters = distances.shape[1]
  *         double[::1] silhouettes = np.zeros(n_samples)
  */
   __pyx_v_n_samples = (__pyx_v_distances.shape[0]);
 
-  /* "KKMeans/quality.pyx":56
+  /* "KKMeans/quality.pyx":32
  *     cdef:
  *         Py_ssize_t n_samples = distances.shape[0]
  *         Py_ssize_t n_clusters = distances.shape[1]             # <<<<<<<<<<<<<<
  *         double[::1] silhouettes = np.zeros(n_samples)
  *         Py_ssize_t i, j
  */
   __pyx_v_n_clusters = (__pyx_v_distances.shape[1]);
 
-  /* "KKMeans/quality.pyx":57
+  /* "KKMeans/quality.pyx":33
  *         Py_ssize_t n_samples = distances.shape[0]
  *         Py_ssize_t n_clusters = distances.shape[1]
  *         double[::1] silhouettes = np.zeros(n_samples)             # <<<<<<<<<<<<<<
  *         Py_ssize_t i, j
  *         long labels_i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_n_samples); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_n_samples); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -17687,57 +17299,57 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_silhouettes = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "KKMeans/quality.pyx":62
+  /* "KKMeans/quality.pyx":38
  *         double a, b, max_a_b
  * 
  *     if n_clusters <= 1:             # <<<<<<<<<<<<<<
  *         raise ValueError("Must have at least two clusters for silhouette")
  *     for i in prange(n_samples, nogil=True):
  */
   __pyx_t_7 = (__pyx_v_n_clusters <= 1);
   if (unlikely(__pyx_t_7)) {
 
-    /* "KKMeans/quality.pyx":63
+    /* "KKMeans/quality.pyx":39
  * 
  *     if n_clusters <= 1:
  *         raise ValueError("Must have at least two clusters for silhouette")             # <<<<<<<<<<<<<<
  *     for i in prange(n_samples, nogil=True):
  *         labels_i = labels[i]
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 63, __pyx_L1_error)
+    __PYX_ERR(0, 39, __pyx_L1_error)
 
-    /* "KKMeans/quality.pyx":62
+    /* "KKMeans/quality.pyx":38
  *         double a, b, max_a_b
  * 
  *     if n_clusters <= 1:             # <<<<<<<<<<<<<<
  *         raise ValueError("Must have at least two clusters for silhouette")
  *     for i in prange(n_samples, nogil=True):
  */
   }
 
-  /* "KKMeans/quality.pyx":64
+  /* "KKMeans/quality.pyx":40
  *     if n_clusters <= 1:
  *         raise ValueError("Must have at least two clusters for silhouette")
  *     for i in prange(n_samples, nogil=True):             # <<<<<<<<<<<<<<
  *         labels_i = labels[i]
  *         a = distances[i, labels_i]
  */
   {
@@ -17789,154 +17401,154 @@
                             /* Initialize private variables to invalid values */
                             __pyx_v_a = ((double)__PYX_NAN());
                             __pyx_v_b = ((double)__PYX_NAN());
                             __pyx_v_j = ((Py_ssize_t)0xbad0bad0);
                             __pyx_v_labels_i = ((long)0xbad0bad0);
                             __pyx_v_max_a_b = ((double)__PYX_NAN());
 
-                            /* "KKMeans/quality.pyx":65
+                            /* "KKMeans/quality.pyx":41
  *         raise ValueError("Must have at least two clusters for silhouette")
  *     for i in prange(n_samples, nogil=True):
  *         labels_i = labels[i]             # <<<<<<<<<<<<<<
  *         a = distances[i, labels_i]
  *         b = DBL_MAX
  */
                             __pyx_t_11 = __pyx_v_i;
                             __pyx_v_labels_i = (*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_labels.data) + __pyx_t_11)) )));
 
-                            /* "KKMeans/quality.pyx":66
+                            /* "KKMeans/quality.pyx":42
  *     for i in prange(n_samples, nogil=True):
  *         labels_i = labels[i]
  *         a = distances[i, labels_i]             # <<<<<<<<<<<<<<
  *         b = DBL_MAX
  *         for j in range(n_clusters):
  */
                             __pyx_t_11 = __pyx_v_i;
                             __pyx_t_12 = __pyx_v_labels_i;
                             __pyx_v_a = (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_distances.data + __pyx_t_11 * __pyx_v_distances.strides[0]) )) + __pyx_t_12)) )));
 
-                            /* "KKMeans/quality.pyx":67
+                            /* "KKMeans/quality.pyx":43
  *         labels_i = labels[i]
  *         a = distances[i, labels_i]
  *         b = DBL_MAX             # <<<<<<<<<<<<<<
  *         for j in range(n_clusters):
  *             if j == labels_i:
  */
                             __pyx_v_b = DBL_MAX;
 
-                            /* "KKMeans/quality.pyx":68
+                            /* "KKMeans/quality.pyx":44
  *         a = distances[i, labels_i]
  *         b = DBL_MAX
  *         for j in range(n_clusters):             # <<<<<<<<<<<<<<
  *             if j == labels_i:
  *                 continue
  */
                             __pyx_t_13 = __pyx_v_n_clusters;
                             __pyx_t_14 = __pyx_t_13;
                             for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
                               __pyx_v_j = __pyx_t_15;
 
-                              /* "KKMeans/quality.pyx":69
+                              /* "KKMeans/quality.pyx":45
  *         b = DBL_MAX
  *         for j in range(n_clusters):
  *             if j == labels_i:             # <<<<<<<<<<<<<<
  *                 continue
  *             b = min(distances[i, j], b)
  */
                               __pyx_t_7 = (__pyx_v_j == __pyx_v_labels_i);
                               if (__pyx_t_7) {
 
-                                /* "KKMeans/quality.pyx":70
+                                /* "KKMeans/quality.pyx":46
  *         for j in range(n_clusters):
  *             if j == labels_i:
  *                 continue             # <<<<<<<<<<<<<<
  *             b = min(distances[i, j], b)
  *         max_a_b = max(a,b)
  */
                                 goto __pyx_L11_continue;
 
-                                /* "KKMeans/quality.pyx":69
+                                /* "KKMeans/quality.pyx":45
  *         b = DBL_MAX
  *         for j in range(n_clusters):
  *             if j == labels_i:             # <<<<<<<<<<<<<<
  *                 continue
  *             b = min(distances[i, j], b)
  */
                               }
 
-                              /* "KKMeans/quality.pyx":71
+                              /* "KKMeans/quality.pyx":47
  *             if j == labels_i:
  *                 continue
  *             b = min(distances[i, j], b)             # <<<<<<<<<<<<<<
  *         max_a_b = max(a,b)
  *         if max_a_b == 0:
  */
                               __pyx_t_12 = __pyx_v_i;
                               __pyx_t_11 = __pyx_v_j;
-                              __pyx_t_16 = __pyx_f_7KKMeans_7quality_min((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_distances.data + __pyx_t_12 * __pyx_v_distances.strides[0]) )) + __pyx_t_11)) ))), __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 71, __pyx_L9_error)
+                              __pyx_t_16 = __pyx_f_7KKMeans_7quality_min((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_distances.data + __pyx_t_12 * __pyx_v_distances.strides[0]) )) + __pyx_t_11)) ))), __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 47, __pyx_L9_error)
                               __pyx_v_b = __pyx_t_16;
                               __pyx_L11_continue:;
                             }
 
-                            /* "KKMeans/quality.pyx":72
+                            /* "KKMeans/quality.pyx":48
  *                 continue
  *             b = min(distances[i, j], b)
  *         max_a_b = max(a,b)             # <<<<<<<<<<<<<<
  *         if max_a_b == 0:
  *             # if max_a_b = 0, a == b == 0 as dists always positive
  */
-                            __pyx_t_16 = __pyx_f_7KKMeans_7quality_max(__pyx_v_a, __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 72, __pyx_L9_error)
+                            __pyx_t_16 = __pyx_f_7KKMeans_7quality_max(__pyx_v_a, __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 48, __pyx_L9_error)
                             __pyx_v_max_a_b = __pyx_t_16;
 
-                            /* "KKMeans/quality.pyx":73
+                            /* "KKMeans/quality.pyx":49
  *             b = min(distances[i, j], b)
  *         max_a_b = max(a,b)
  *         if max_a_b == 0:             # <<<<<<<<<<<<<<
  *             # if max_a_b = 0, a == b == 0 as dists always positive
  *             silhouettes[i] = 0
  */
                             __pyx_t_7 = (__pyx_v_max_a_b == 0.0);
                             if (__pyx_t_7) {
 
-                              /* "KKMeans/quality.pyx":75
+                              /* "KKMeans/quality.pyx":51
  *         if max_a_b == 0:
  *             # if max_a_b = 0, a == b == 0 as dists always positive
  *             silhouettes[i] = 0             # <<<<<<<<<<<<<<
  *             continue
  *         silhouettes[i] = (b - a) / max(a,b)
  */
                               __pyx_t_11 = __pyx_v_i;
                               *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_silhouettes.data) + __pyx_t_11)) )) = 0.0;
 
-                              /* "KKMeans/quality.pyx":76
+                              /* "KKMeans/quality.pyx":52
  *             # if max_a_b = 0, a == b == 0 as dists always positive
  *             silhouettes[i] = 0
  *             continue             # <<<<<<<<<<<<<<
  *         silhouettes[i] = (b - a) / max(a,b)
  * 
  */
                               goto __pyx_L7_continue;
 
-                              /* "KKMeans/quality.pyx":73
+                              /* "KKMeans/quality.pyx":49
  *             b = min(distances[i, j], b)
  *         max_a_b = max(a,b)
  *         if max_a_b == 0:             # <<<<<<<<<<<<<<
  *             # if max_a_b = 0, a == b == 0 as dists always positive
  *             silhouettes[i] = 0
  */
                             }
 
-                            /* "KKMeans/quality.pyx":77
+                            /* "KKMeans/quality.pyx":53
  *             silhouettes[i] = 0
  *             continue
  *         silhouettes[i] = (b - a) / max(a,b)             # <<<<<<<<<<<<<<
  * 
  *     return np.asarray(silhouettes)
  */
-                            __pyx_t_16 = __pyx_f_7KKMeans_7quality_max(__pyx_v_a, __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 77, __pyx_L9_error)
+                            __pyx_t_16 = __pyx_f_7KKMeans_7quality_max(__pyx_v_a, __pyx_v_b); if (unlikely(__pyx_t_16 == ((double)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 53, __pyx_L9_error)
                             __pyx_t_11 = __pyx_v_i;
                             *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_silhouettes.data) + __pyx_t_11)) )) = ((__pyx_v_b - __pyx_v_a) / __pyx_t_16);
                             goto __pyx_L16;
                             __pyx_L7_continue:;
                             goto __pyx_L16;
                             __pyx_L9_error:;
                             {
@@ -17955,15 +17567,15 @@
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
                             }
                             __pyx_parallel_why = 4;
                             goto __pyx_L15;
                             __pyx_L15:;
                             #ifdef _OPENMP
-                            #pragma omp critical(__pyx_parallel_lastprivates2)
+                            #pragma omp critical(__pyx_parallel_lastprivates0)
                             #endif /* _OPENMP */
                             {
                                 __pyx_parallel_temp0 = __pyx_v_a;
                                 __pyx_parallel_temp1 = __pyx_v_b;
                                 __pyx_parallel_temp2 = __pyx_v_i;
                                 __pyx_parallel_temp3 = __pyx_v_j;
                                 __pyx_parallel_temp4 = __pyx_v_labels_i;
@@ -18024,15 +17636,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "KKMeans/quality.pyx":64
+      /* "KKMeans/quality.pyx":40
  *     if n_clusters <= 1:
  *         raise ValueError("Must have at least two clusters for silhouette")
  *     for i in prange(n_samples, nogil=True):             # <<<<<<<<<<<<<<
  *         labels_i = labels[i]
  *         a = distances[i, labels_i]
  */
       /*finally:*/ {
@@ -18050,28 +17662,28 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L6:;
       }
   }
 
-  /* "KKMeans/quality.pyx":79
+  /* "KKMeans/quality.pyx":55
  *         silhouettes[i] = (b - a) / max(a,b)
  * 
  *     return np.asarray(silhouettes)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_asarray); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_silhouettes, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_silhouettes, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -18082,23 +17694,23 @@
     }
   }
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "KKMeans/quality.pyx":36
+  /* "KKMeans/quality.pyx":12
  *     return np.sum(silhouettes)/len(silhouettes)
  * 
  * def calc_silhouettes(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
  *     '''
  *     calculates the silhouette of each datapoint
  */
 
@@ -18114,130 +17726,130 @@
   __pyx_L0:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_silhouettes, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "KKMeans/quality.pyx":82
+/* "KKMeans/quality.pyx":58
  * 
  * 
  * cdef double max(double a, double b) nogil:             # <<<<<<<<<<<<<<
  *     if a > b:
  *         return a
  */
 
 static double __pyx_f_7KKMeans_7quality_max(double __pyx_v_a, double __pyx_v_b) {
   double __pyx_r;
   int __pyx_t_1;
 
-  /* "KKMeans/quality.pyx":83
+  /* "KKMeans/quality.pyx":59
  * 
  * cdef double max(double a, double b) nogil:
  *     if a > b:             # <<<<<<<<<<<<<<
  *         return a
  *     return b
  */
   __pyx_t_1 = (__pyx_v_a > __pyx_v_b);
   if (__pyx_t_1) {
 
-    /* "KKMeans/quality.pyx":84
+    /* "KKMeans/quality.pyx":60
  * cdef double max(double a, double b) nogil:
  *     if a > b:
  *         return a             # <<<<<<<<<<<<<<
  *     return b
  * 
  */
     __pyx_r = __pyx_v_a;
     goto __pyx_L0;
 
-    /* "KKMeans/quality.pyx":83
+    /* "KKMeans/quality.pyx":59
  * 
  * cdef double max(double a, double b) nogil:
  *     if a > b:             # <<<<<<<<<<<<<<
  *         return a
  *     return b
  */
   }
 
-  /* "KKMeans/quality.pyx":85
+  /* "KKMeans/quality.pyx":61
  *     if a > b:
  *         return a
  *     return b             # <<<<<<<<<<<<<<
  * 
  * cdef double min(double a, double b) nogil:
  */
   __pyx_r = __pyx_v_b;
   goto __pyx_L0;
 
-  /* "KKMeans/quality.pyx":82
+  /* "KKMeans/quality.pyx":58
  * 
  * 
  * cdef double max(double a, double b) nogil:             # <<<<<<<<<<<<<<
  *     if a > b:
  *         return a
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "KKMeans/quality.pyx":87
+/* "KKMeans/quality.pyx":63
  *     return b
  * 
  * cdef double min(double a, double b) nogil:             # <<<<<<<<<<<<<<
  *     if a < b:
  *         return a
  */
 
 static double __pyx_f_7KKMeans_7quality_min(double __pyx_v_a, double __pyx_v_b) {
   double __pyx_r;
   int __pyx_t_1;
 
-  /* "KKMeans/quality.pyx":88
+  /* "KKMeans/quality.pyx":64
  * 
  * cdef double min(double a, double b) nogil:
  *     if a < b:             # <<<<<<<<<<<<<<
  *         return a
  *     return b
  */
   __pyx_t_1 = (__pyx_v_a < __pyx_v_b);
   if (__pyx_t_1) {
 
-    /* "KKMeans/quality.pyx":89
+    /* "KKMeans/quality.pyx":65
  * cdef double min(double a, double b) nogil:
  *     if a < b:
  *         return a             # <<<<<<<<<<<<<<
  *     return b
  * 
  */
     __pyx_r = __pyx_v_a;
     goto __pyx_L0;
 
-    /* "KKMeans/quality.pyx":88
+    /* "KKMeans/quality.pyx":64
  * 
  * cdef double min(double a, double b) nogil:
  *     if a < b:             # <<<<<<<<<<<<<<
  *         return a
  *     return b
  */
   }
 
-  /* "KKMeans/quality.pyx":90
+  /* "KKMeans/quality.pyx":66
  *     if a < b:
  *         return a
  *     return b             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_b;
   goto __pyx_L0;
 
-  /* "KKMeans/quality.pyx":87
+  /* "KKMeans/quality.pyx":63
  *     return b
  * 
  * cdef double min(double a, double b) nogil:             # <<<<<<<<<<<<<<
  *     if a < b:
  *         return a
  */
 
@@ -19217,15 +18829,15 @@
     {&__pyx_n_s_Sequence, __pyx_k_Sequence, sizeof(__pyx_k_Sequence), 0, 0, 1, 1},
     {&__pyx_kp_s_Step_may_not_be_zero_axis_d, __pyx_k_Step_may_not_be_zero_axis_d, sizeof(__pyx_k_Step_may_not_be_zero_axis_d), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_n_s__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 0, 1, 1},
+    {&__pyx_n_s__25, __pyx_k__25, sizeof(__pyx_k__25), 0, 0, 1, 1},
     {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
     {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
     {&__pyx_kp_u_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 1, 0, 0},
@@ -19327,16 +18939,16 @@
     {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 44, __pyx_L1_error)
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 373, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
@@ -19383,22 +18995,22 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "KKMeans/quality.pyx":19
+  /* "KKMeans/quality.pyx":39
  * 
  *     if n_clusters <= 1:
  *         raise ValueError("Must have at least two clusters for silhouette")             # <<<<<<<<<<<<<<
  *     for i in prange(n_samples, nogil=True):
  *         labels_i = labels[i]
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Must_have_at_least_two_clusters); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Must_have_at_least_two_clusters); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "View.MemoryView":100
  * cdef object __pyx_collections_abc_Sequence "__pyx_collections_abc_Sequence"
  * try:
  *     if __import__("sys").version_info >= (3, 3):             # <<<<<<<<<<<<<<
@@ -19499,30 +19111,33 @@
   __Pyx_GIVEREF(__pyx_tuple__19);
   __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "KKMeans/quality.pyx":7
  *     cdef double DBL_MAX
  * 
  * def avg_silhouette(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
- *     '''returns the average silhouette of a dataset
- *     '''
+ *     '''returns the average silhouette of a dataset'''
+ *     silhouettes = calc_silhouettes(distances, labels)
  */
-  __pyx_tuple__21 = PyTuple_Pack(11, __pyx_n_s_distances, __pyx_n_s_labels, __pyx_n_s_n_samples, __pyx_n_s_n_clusters, __pyx_n_s_silhouettes, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_labels_i, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_max_a_b); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_n_s_distances, __pyx_n_s_labels, __pyx_n_s_silhouettes); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_quality_pyx, __pyx_n_s_avg_silhouette, 7, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_quality_pyx, __pyx_n_s_avg_silhouette, 7, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 7, __pyx_L1_error)
 
-  /* "KKMeans/quality.pyx":36
+  /* "KKMeans/quality.pyx":12
  *     return np.sum(silhouettes)/len(silhouettes)
  * 
  * def calc_silhouettes(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
  *     '''
  *     calculates the silhouette of each datapoint
  */
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_quality_pyx, __pyx_n_s_calc_silhouettes, 36, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(11, __pyx_n_s_distances, __pyx_n_s_labels, __pyx_n_s_n_samples, __pyx_n_s_n_clusters, __pyx_n_s_silhouettes, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_labels_i, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_max_a_b); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_KKMeans_quality_pyx, __pyx_n_s_calc_silhouettes, 12, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -20588,32 +20203,32 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_7) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "KKMeans/quality.pyx":7
  *     cdef double DBL_MAX
  * 
  * def avg_silhouette(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
- *     '''returns the average silhouette of a dataset
- *     '''
+ *     '''returns the average silhouette of a dataset'''
+ *     silhouettes = calc_silhouettes(distances, labels)
  */
   __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7quality_1avg_silhouette, 0, __pyx_n_s_avg_silhouette, NULL, __pyx_n_s_KKMeans_quality, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_avg_silhouette, __pyx_t_7) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "KKMeans/quality.pyx":36
+  /* "KKMeans/quality.pyx":12
  *     return np.sum(silhouettes)/len(silhouettes)
  * 
  * def calc_silhouettes(double[:, ::1] distances, long[::1] labels):             # <<<<<<<<<<<<<<
  *     '''
  *     calculates the silhouette of each datapoint
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7quality_3calc_silhouettes, 0, __pyx_n_s_calc_silhouettes, NULL, __pyx_n_s_KKMeans_quality, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7KKMeans_7quality_3calc_silhouettes, 0, __pyx_n_s_calc_silhouettes, NULL, __pyx_n_s_KKMeans_quality, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_silhouettes, __pyx_t_7) < 0) __PYX_ERR(0, 36, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_calc_silhouettes, __pyx_t_7) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "KKMeans/quality.pyx":1
  * import numpy as np             # <<<<<<<<<<<<<<
  * from cython.parallel import prange
  * 
  */
@@ -25763,14 +25378,60 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* MemviewDtypeToObject */
+  static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp) {
+    return (PyObject *) PyFloat_FromDouble(*(double *) itemp);
+}
+static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj) {
+    double value = __pyx_PyFloat_AsDouble(obj);
+    if (unlikely((value == (double)-1) && PyErr_Occurred()))
+        return 0;
+    *(double *) itemp = value;
+    return 1;
+}
+
+/* CIntFromPyVerify */
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
+/* MemviewDtypeToObject */
+  static CYTHON_INLINE PyObject *__pyx_memview_get_long(const char *itemp) {
+    return (PyObject *) __Pyx_PyInt_From_long(*(long *) itemp);
+}
+static CYTHON_INLINE int __pyx_memview_set_long(const char *itemp, PyObject *obj) {
+    long value = __Pyx_PyInt_As_long(obj);
+    if (unlikely((value == (long)-1) && PyErr_Occurred()))
+        return 0;
+    *(long *) itemp = value;
+    return 1;
+}
+
 /* ObjectToMemviewSlice */
   static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_double(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
     int retcode;
     if (obj == Py_None) {
@@ -25786,26 +25447,14 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
-/* MemviewDtypeToObject */
-  static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp) {
-    return (PyObject *) PyFloat_FromDouble(*(double *) itemp);
-}
-static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj) {
-    double value = __pyx_PyFloat_AsDouble(obj);
-    if (unlikely((value == (double)-1) && PyErr_Occurred()))
-        return 0;
-    *(double *) itemp = value;
-    return 1;
-}
-
 /* MemviewSliceCopyTemplate */
   static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object)
 {
@@ -26000,196 +25649,212 @@
         }
     } else {
         __pyx_fatalerror("Acquisition count is %d (line %d)",
                          old_acquisition_count-1, lineno);
     }
 }
 
-/* CIntFromPyVerify */
-  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
     }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
 
 /* CIntFromPy */
-  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(int) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
+        if ((sizeof(long) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (int) val;
+            return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (unlikely(__Pyx_PyLong_IsNeg(x))) {
                 goto raise_neg_overflow;
             } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_DigitCount(x)) {
                     case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
-                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
-                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
-                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                 }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (int) -1;
+                    return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(int) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
+            if ((sizeof(long) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_SignedDigitCount(x)) {
                     case -2:
-                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case -3:
-                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case -4:
-                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                 }
             }
 #endif
-            if ((sizeof(int) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
+            if ((sizeof(long) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-            int val;
+            long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
 #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -26208,261 +25873,261 @@
                 long idigit;
                 int chunk_size = (sizeof(long) < 8) ? 30 : 62;
                 if (unlikely(!PyLong_CheckExact(v))) {
                     PyObject *tmp = v;
                     v = PyNumber_Long(v);
                     assert(PyLong_CheckExact(v));
                     Py_DECREF(tmp);
-                    if (unlikely(!v)) return (int) -1;
+                    if (unlikely(!v)) return (long) -1;
                 }
 #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                 if (Py_SIZE(x) == 0)
-                    return (int) 0;
+                    return (long) 0;
                 is_negative = Py_SIZE(x) < 0;
 #else
                 {
                     int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                     if (unlikely(result < 0))
-                        return (int) -1;
+                        return (long) -1;
                     is_negative = result == 1;
                 }
 #endif
                 if (is_unsigned && unlikely(is_negative)) {
                     goto raise_neg_overflow;
                 } else if (is_negative) {
                     stepval = PyNumber_Invert(v);
                     if (unlikely(!stepval))
-                        return (int) -1;
+                        return (long) -1;
                 } else {
                     stepval = __Pyx_NewRef(v);
                 }
-                val = (int) 0;
+                val = (long) 0;
                 mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
                 shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
                     PyObject *tmp, *digit;
                     digit = PyNumber_And(stepval, mask);
                     if (unlikely(!digit)) goto done;
                     idigit = PyLong_AsLong(digit);
                     Py_DECREF(digit);
                     if (unlikely(idigit < 0)) goto done;
                     tmp = PyNumber_Rshift(stepval, shift);
                     if (unlikely(!tmp)) goto done;
                     Py_DECREF(stepval); stepval = tmp;
-                    val |= ((int) idigit) << bits;
+                    val |= ((long) idigit) << bits;
                     #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                     if (Py_SIZE(stepval) == 0)
                         goto unpacking_done;
                     #endif
                 }
                 idigit = PyLong_AsLong(stepval);
                 if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
                 if (unlikely(idigit >= (1L << remaining_bits)))
                     goto raise_overflow;
-                val |= ((int) idigit) << bits;
+                val |= ((long) idigit) << bits;
             #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
             unpacking_done:
             #endif
                 if (!is_unsigned) {
-                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
                         goto raise_overflow;
                     if (is_negative)
                         val = ~val;
                 }
                 ret = 0;
             done:
                 Py_XDECREF(shift);
                 Py_XDECREF(mask);
                 Py_XDECREF(stepval);
 #endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-            return (int) -1;
+            return (long) -1;
         }
     } else {
-        int val;
+        long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (int) -1;
-        val = __Pyx_PyInt_As_int(tmp);
+        if (!tmp) return (long) -1;
+        val = __Pyx_PyInt_As_long(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to int");
-    return (int) -1;
+        "value too large to convert to long");
+    return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to int");
-    return (int) -1;
+        "can't convert negative value to long");
+    return (long) -1;
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(long) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
+        if ((sizeof(int) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (long) val;
+            return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (unlikely(__Pyx_PyLong_IsNeg(x))) {
                 goto raise_neg_overflow;
             } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_DigitCount(x)) {
                     case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
-                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
-                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
-                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                 }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (long) -1;
+                    return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(long) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
+            if ((sizeof(int) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_SignedDigitCount(x)) {
                     case -2:
-                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case -3:
-                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case -4:
-                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                 }
             }
 #endif
-            if ((sizeof(long) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
+            if ((sizeof(int) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-            long val;
+            int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
 #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -26481,99 +26146,99 @@
                 long idigit;
                 int chunk_size = (sizeof(long) < 8) ? 30 : 62;
                 if (unlikely(!PyLong_CheckExact(v))) {
                     PyObject *tmp = v;
                     v = PyNumber_Long(v);
                     assert(PyLong_CheckExact(v));
                     Py_DECREF(tmp);
-                    if (unlikely(!v)) return (long) -1;
+                    if (unlikely(!v)) return (int) -1;
                 }
 #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                 if (Py_SIZE(x) == 0)
-                    return (long) 0;
+                    return (int) 0;
                 is_negative = Py_SIZE(x) < 0;
 #else
                 {
                     int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                     if (unlikely(result < 0))
-                        return (long) -1;
+                        return (int) -1;
                     is_negative = result == 1;
                 }
 #endif
                 if (is_unsigned && unlikely(is_negative)) {
                     goto raise_neg_overflow;
                 } else if (is_negative) {
                     stepval = PyNumber_Invert(v);
                     if (unlikely(!stepval))
-                        return (long) -1;
+                        return (int) -1;
                 } else {
                     stepval = __Pyx_NewRef(v);
                 }
-                val = (long) 0;
+                val = (int) 0;
                 mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
                 shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
                     PyObject *tmp, *digit;
                     digit = PyNumber_And(stepval, mask);
                     if (unlikely(!digit)) goto done;
                     idigit = PyLong_AsLong(digit);
                     Py_DECREF(digit);
                     if (unlikely(idigit < 0)) goto done;
                     tmp = PyNumber_Rshift(stepval, shift);
                     if (unlikely(!tmp)) goto done;
                     Py_DECREF(stepval); stepval = tmp;
-                    val |= ((long) idigit) << bits;
+                    val |= ((int) idigit) << bits;
                     #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                     if (Py_SIZE(stepval) == 0)
                         goto unpacking_done;
                     #endif
                 }
                 idigit = PyLong_AsLong(stepval);
                 if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
                 if (unlikely(idigit >= (1L << remaining_bits)))
                     goto raise_overflow;
-                val |= ((long) idigit) << bits;
+                val |= ((int) idigit) << bits;
             #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
             unpacking_done:
             #endif
                 if (!is_unsigned) {
-                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
                         goto raise_overflow;
                     if (is_negative)
                         val = ~val;
                 }
                 ret = 0;
             done:
                 Py_XDECREF(shift);
                 Py_XDECREF(mask);
                 Py_XDECREF(stepval);
 #endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-            return (long) -1;
+            return (int) -1;
         }
     } else {
-        long val;
+        int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (long) -1;
-        val = __Pyx_PyInt_As_long(tmp);
+        if (!tmp) return (int) -1;
+        val = __Pyx_PyInt_As_int(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to long");
-    return (long) -1;
+        "value too large to convert to int");
+    return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to long");
-    return (long) -1;
+        "can't convert negative value to int");
+    return (int) -1;
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
@@ -26606,52 +26271,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
@@ -26926,15 +26553,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__24));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__25));
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
```

### Comparing `KKMeans-0.0.3/src/KKMeans/quality.pyx` & `KKMeans-0.0.4/src/KKMeans/quality.pyx`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,16 @@
 import numpy as np
 from cython.parallel import prange
 
 cdef extern from "float.h":
     cdef double DBL_MAX
 
 def avg_silhouette(double[:, ::1] distances, long[::1] labels):
-    '''returns the average silhouette of a dataset
-    '''
-    cdef:
-        Py_ssize_t n_samples = distances.shape[0]
-        Py_ssize_t n_clusters = distances.shape[1]
-        double[::1] silhouettes = np.zeros(n_samples)
-        Py_ssize_t i, j
-        long labels_i
-        double a, b, max_a_b
-
-    if n_clusters <= 1:
-        raise ValueError("Must have at least two clusters for silhouette")
-    for i in prange(n_samples, nogil=True):
-        labels_i = labels[i]
-        a = distances[i, labels_i]
-        b = DBL_MAX
-        for j in range(n_clusters):
-            if j == labels_i:
-                continue
-            b = min(distances[i, j], b)
-        max_a_b = max(a,b)
-        if max_a_b == 0:
-            # if max_a_b = 0, a == b == 0 as dists always positive 
-            silhouettes[i] = 0
-            continue
-        silhouettes[i] = (b - a) / max(a,b) 
+    '''returns the average silhouette of a dataset'''
+    silhouettes = calc_silhouettes(distances, labels)
     return np.sum(silhouettes)/len(silhouettes)
 
 def calc_silhouettes(double[:, ::1] distances, long[::1] labels):
     '''
     calculates the silhouette of each datapoint
 
     For more details see KKMeans class docstring
```

### Comparing `KKMeans-0.0.3/src/KKMeans/utils.c` & `KKMeans-0.0.4/src/KKMeans/utils.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.3/src/KKMeans/utils.pyx` & `KKMeans-0.0.4/src/KKMeans/utils.pyx`

 * *Files identical despite different names*

