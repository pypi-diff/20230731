# Comparing `tmp/hypyp-0.5.0b0.tar.gz` & `tmp/hypyp-0.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypyp-0.5.0b0.tar", max compression
+gzip compressed data, was "hypyp-0.5.0b1.tar", max compression
```

## Comparing `hypyp-0.5.0b0.tar` & `hypyp-0.5.0b1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1524 2023-05-12 13:18:38.310986 hypyp-0.5.0b0/LICENSE
--rw-r--r--   0        0        0     3566 2023-07-23 00:30:33.560601 hypyp-0.5.0b0/README.md
--rw-r--r--   0        0        0      179 2023-07-22 23:20:29.348412 hypyp-0.5.0b0/hypyp/__init__.py
--rw-r--r--   0        0        0    35843 2023-07-22 20:11:20.545731 hypyp-0.5.0b0/hypyp/analyses.py
--rw-r--r--   0        0        0    13770 2023-05-12 13:18:38.588050 hypyp-0.5.0b0/hypyp/data/Basehead.obj
--rw-r--r--   0        0        0        1 2023-05-12 13:18:38.588445 hypyp-0.5.0b0/hypyp/ext/mpl3d/__init__.py
--rw-r--r--   0        0        0     4511 2023-05-12 13:18:38.588628 hypyp-0.5.0b0/hypyp/ext/mpl3d/camera.py
--rw-r--r--   0        0        0     7705 2023-05-12 13:18:38.589183 hypyp-0.5.0b0/hypyp/ext/mpl3d/glm.py
--rw-r--r--   0        0        0     3147 2023-05-12 13:18:38.589330 hypyp-0.5.0b0/hypyp/ext/mpl3d/lighting.py
--rw-r--r--   0        0        0     2990 2023-05-12 13:18:38.589460 hypyp-0.5.0b0/hypyp/ext/mpl3d/mesh.py
--rw-r--r--   0        0        0     9205 2023-05-12 13:18:38.589643 hypyp-0.5.0b0/hypyp/ext/mpl3d/trackball.py
--rw-r--r--   0        0        0     9887 2023-05-12 13:18:38.589827 hypyp-0.5.0b0/hypyp/fnirs_tools.py
--rw-r--r--   0        0        0        1 2023-05-12 13:18:38.589947 hypyp-0.5.0b0/hypyp/io.py
--rw-r--r--   0        0        0     9148 2023-05-12 13:18:38.590193 hypyp-0.5.0b0/hypyp/mvarica.py
--rw-r--r--   0        0        0    12650 2023-07-22 19:35:17.847420 hypyp-0.5.0b0/hypyp/prep.py
--rw-r--r--   0        0        0    21562 2023-05-12 13:18:38.590649 hypyp-0.5.0b0/hypyp/stats.py
--rw-r--r--   0        0        0    15121 2023-05-12 13:18:38.590859 hypyp-0.5.0b0/hypyp/utils.py
--rw-r--r--   0        0        0    69995 2023-07-23 00:26:53.243713 hypyp-0.5.0b0/hypyp/viz.py
--rw-r--r--   0        0        0     1808 2023-07-23 00:29:41.394603 hypyp-0.5.0b0/pyproject.toml
--rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 hypyp-0.5.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2023-05-12 13:18:38.310986 hypyp-0.5.0b1/LICENSE
+-rw-r--r--   0        0        0     3566 2023-07-23 00:30:33.560601 hypyp-0.5.0b1/README.md
+-rw-r--r--   0        0        0      179 2023-07-22 23:20:29.348412 hypyp-0.5.0b1/hypyp/__init__.py
+-rw-r--r--   0        0        0    35843 2023-07-22 20:11:20.545731 hypyp-0.5.0b1/hypyp/analyses.py
+-rw-r--r--   0        0        0    13770 2023-05-12 13:18:38.588050 hypyp-0.5.0b1/hypyp/data/Basehead.obj
+-rw-r--r--   0        0        0        1 2023-05-12 13:18:38.588445 hypyp-0.5.0b1/hypyp/ext/mpl3d/__init__.py
+-rw-r--r--   0        0        0     4511 2023-05-12 13:18:38.588628 hypyp-0.5.0b1/hypyp/ext/mpl3d/camera.py
+-rw-r--r--   0        0        0     7705 2023-05-12 13:18:38.589183 hypyp-0.5.0b1/hypyp/ext/mpl3d/glm.py
+-rw-r--r--   0        0        0     3147 2023-05-12 13:18:38.589330 hypyp-0.5.0b1/hypyp/ext/mpl3d/lighting.py
+-rw-r--r--   0        0        0     2990 2023-05-12 13:18:38.589460 hypyp-0.5.0b1/hypyp/ext/mpl3d/mesh.py
+-rw-r--r--   0        0        0     9205 2023-05-12 13:18:38.589643 hypyp-0.5.0b1/hypyp/ext/mpl3d/trackball.py
+-rw-r--r--   0        0        0     9887 2023-05-12 13:18:38.589827 hypyp-0.5.0b1/hypyp/fnirs_tools.py
+-rw-r--r--   0        0        0        1 2023-05-12 13:18:38.589947 hypyp-0.5.0b1/hypyp/io.py
+-rw-r--r--   0        0        0     9148 2023-05-12 13:18:38.590193 hypyp-0.5.0b1/hypyp/mvarica.py
+-rw-r--r--   0        0        0    12650 2023-07-22 19:35:17.847420 hypyp-0.5.0b1/hypyp/prep.py
+-rw-r--r--   0        0        0    21479 2023-07-31 17:05:53.375387 hypyp-0.5.0b1/hypyp/stats.py
+-rw-r--r--   0        0        0    15121 2023-05-12 13:18:38.590859 hypyp-0.5.0b1/hypyp/utils.py
+-rw-r--r--   0        0        0    69995 2023-07-23 00:26:53.243713 hypyp-0.5.0b1/hypyp/viz.py
+-rw-r--r--   0        0        0     1810 2023-07-31 17:06:19.188776 hypyp-0.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 hypyp-0.5.0b1/PKG-INFO
```

### Comparing `hypyp-0.5.0b0/LICENSE` & `hypyp-0.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/README.md` & `hypyp-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/analyses.py` & `hypyp-0.5.0b1/hypyp/analyses.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/data/Basehead.obj` & `hypyp-0.5.0b1/hypyp/data/Basehead.obj`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/ext/mpl3d/camera.py` & `hypyp-0.5.0b1/hypyp/ext/mpl3d/camera.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/ext/mpl3d/glm.py` & `hypyp-0.5.0b1/hypyp/ext/mpl3d/glm.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/ext/mpl3d/lighting.py` & `hypyp-0.5.0b1/hypyp/ext/mpl3d/lighting.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/ext/mpl3d/mesh.py` & `hypyp-0.5.0b1/hypyp/ext/mpl3d/mesh.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/ext/mpl3d/trackball.py` & `hypyp-0.5.0b1/hypyp/ext/mpl3d/trackball.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/fnirs_tools.py` & `hypyp-0.5.0b1/hypyp/fnirs_tools.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/mvarica.py` & `hypyp-0.5.0b1/hypyp/mvarica.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/prep.py` & `hypyp-0.5.0b1/hypyp/prep.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/stats.py` & `hypyp-0.5.0b1/hypyp/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,22 +446,22 @@
                                        return_pvals=False)[0])
         alpha = mne.stats.f_threshold_mway_rm(n_subjects=data.shape[1],
                                               factor_levels=factor_levels,
                                               effects='all',
                                               pvalue=0.05)
 
     # computing the cluster permutation t test
-    Stat_obs, clusters, cluster_p_values, H0 = mne.stats.permutation_cluster_test(data,
-                                                                                  stat_fun=stat_fun,
-                                                                                  threshold=alpha,
-                                                                                  tail=tail,
-                                                                                  n_permutations=n_permutations,
-                                                                                  connectivity=ch_con_freq,
-                                                                                  t_power=1,
-                                                                                  out_type='mask')
+    Stat_obs, clusters, cluster_p_values, H0 = permutation_cluster_test(data,
+                                                                        stat_fun=stat_fun,
+                                                                        threshold=alpha,
+                                                                        tail=tail,
+                                                                        n_permutations=n_permutations,
+                                                                        adjacency=ch_con_freq,
+                                                                        t_power=1,
+                                                                        out_type='mask')
     # getting F values for sensors belonging to a significant cluster
     Stat_obs_plot = np.zeros(Stat_obs.shape)
     for cluster_p in cluster_p_values:
         if cluster_p <= 0.05:
             sensors_plot = clusters[np.where(cluster_p_values == cluster_p)[
                 0][0]].astype('uint8')
             Stat_values = sensors_plot*Stat_obs
```

### Comparing `hypyp-0.5.0b0/hypyp/utils.py` & `hypyp-0.5.0b1/hypyp/utils.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/hypyp/viz.py` & `hypyp-0.5.0b1/hypyp/viz.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.5.0b0/pyproject.toml` & `hypyp-0.5.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hypyp"
-version = "0.5.0-beta"
+version = "0.5.0-beta.1"
 description = "The Hyperscanning Python Pipeline."
 readme = "README.md"
 authors = [
     "Anaël AYROLLLES <anael.ayrollles@pasteur.fr>",
     "Florence BRUN <florence.brun@pasteur.fr>",
     "Phoebe CHEN <phoebe.chen1117@gmail.com>",
     "Amir DJALOVSKI <amir.djv@gmail.com>",
```

### Comparing `hypyp-0.5.0b0/PKG-INFO` & `hypyp-0.5.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypyp
-Version: 0.5.0b0
+Version: 0.5.0b1
 Summary: The Hyperscanning Python Pipeline.
 Home-page: https://github.com/ppsp-team/HyPyP
 License: BSD-3-Clause
 Keywords: hyperscanning,neuroscience,pipeline,statistics,visualization
 Author: Anaël AYROLLLES
 Author-email: anael.ayrollles@pasteur.fr
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hypyp Version: 0.5.0b0 Summary: The Hyperscanning
+Metadata-Version: 2.1 Name: hypyp Version: 0.5.0b1 Summary: The Hyperscanning
 Python Pipeline. Home-page: https://github.com/ppsp-team/HyPyP License: BSD-3-
 Clause Keywords: hyperscanning,neuroscience,pipeline,statistics,visualization
 Author: AnaÃ«l AYROLLLES Author-email: anael.ayrollles@pasteur.fr Requires-
 Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

