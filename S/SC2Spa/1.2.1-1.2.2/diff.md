# Comparing `tmp/SC2Spa-1.2.1.tar.gz` & `tmp/SC2Spa-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC2Spa-1.2.1.tar", last modified: Mon Jul 31 15:40:30 2023, max compression
+gzip compressed data, was "SC2Spa-1.2.2.tar", last modified: Mon Jul 31 15:49:56 2023, max compression
```

## Comparing `SC2Spa-1.2.1.tar` & `SC2Spa-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:40:30.140468 SC2Spa-1.2.1/
--rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.2.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 15:40:30.139878 SC2Spa-1.2.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.2.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:40:30.135188 SC2Spa-1.2.1/SC2Spa/
--rwxrwxrwx   0 root         (0) root         (0)    20229 2023-07-17 14:46:02.000000 SC2Spa-1.2.1/SC2Spa/BM.py
--rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.2.1/SC2Spa/ME.py
--rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.2.1/SC2Spa/PP.py
--rwxrwxrwx   0 root         (0) root         (0)    50744 2023-07-11 14:10:24.000000 SC2Spa-1.2.1/SC2Spa/SI.py
--rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.2.1/SC2Spa/SVA.py
--rwxrwxrwx   0 root         (0) root         (0)    23478 2023-07-14 16:52:28.000000 SC2Spa-1.2.1/SC2Spa/Vis.py
--rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.2.1/SC2Spa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-07-31 15:40:12.000000 SC2Spa-1.2.1/SC2Spa/__metadata__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:40:30.138794 SC2Spa-1.2.1/SC2Spa.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      274 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-07-31 15:40:30.000000 SC2Spa-1.2.1/SC2Spa.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      691 2023-07-31 15:40:00.000000 SC2Spa-1.2.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-31 15:40:30.140691 SC2Spa-1.2.1/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:49:56.431387 SC2Spa-1.2.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.2.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 15:49:56.430981 SC2Spa-1.2.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.2.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:49:56.427482 SC2Spa-1.2.2/SC2Spa/
+-rwxrwxrwx   0 root         (0) root         (0)    20229 2023-07-17 14:46:02.000000 SC2Spa-1.2.2/SC2Spa/BM.py
+-rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.2.2/SC2Spa/ME.py
+-rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.2.2/SC2Spa/PP.py
+-rwxrwxrwx   0 root         (0) root         (0)    50744 2023-07-11 14:10:24.000000 SC2Spa-1.2.2/SC2Spa/SI.py
+-rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.2.2/SC2Spa/SVA.py
+-rwxrwxrwx   0 root         (0) root         (0)    23478 2023-07-31 15:48:59.000000 SC2Spa-1.2.2/SC2Spa/Vis.py
+-rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.2.2/SC2Spa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      460 2023-07-31 15:49:40.000000 SC2Spa-1.2.2/SC2Spa/__metadata__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-31 15:49:56.430128 SC2Spa-1.2.2/SC2Spa.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-31 15:49:56.000000 SC2Spa-1.2.2/SC2Spa.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      274 2023-07-31 15:49:56.000000 SC2Spa-1.2.2/SC2Spa.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-31 15:49:56.000000 SC2Spa-1.2.2/SC2Spa.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-07-31 15:49:56.000000 SC2Spa-1.2.2/SC2Spa.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      691 2023-07-31 15:49:23.000000 SC2Spa-1.2.2/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-31 15:49:56.431561 SC2Spa-1.2.2/setup.cfg
```

### Comparing `SC2Spa-1.2.1/LICENSE` & `SC2Spa-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.1/PKG-INFO` & `SC2Spa-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.1
+Version: 1.2.2
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.2.1/README.md` & `SC2Spa-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.1/SC2Spa/BM.py` & `SC2Spa-1.2.2/SC2Spa/BM.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.1/SC2Spa/ME.py` & `SC2Spa-1.2.2/SC2Spa/ME.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.1/SC2Spa/PP.py` & `SC2Spa-1.2.2/SC2Spa/PP.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.1/SC2Spa/SI.py` & `SC2Spa-1.2.2/SC2Spa/SI.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.1/SC2Spa/SVA.py` & `SC2Spa-1.2.2/SC2Spa/SVA.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.2.1/SC2Spa/Vis.py` & `SC2Spa-1.2.2/SC2Spa/Vis.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
                 plt.savefig(root + Genes[i] + '_' + CT + '.png', )
             else:
                 plt.savefig(root + Genes[i] + '.png', )
         plt.show()
 
 
 def DrawGenes2(adata:anndata.AnnData, gene:str, coords_name='spatial', lim = False,
-               xlim = [650, 5750], ylim = [650, 5750], figsize = (10,10), alpha = 0.7.
+               xlim = [650, 5750], ylim = [650, 5750], figsize = (10,10), alpha = 0.7,
                cmap = cmap, FM = True, scST = False, CTL = None, c_name = 'simp_name',
                root = 'transfer2/FM_Valid1/', s = 2, Sparse = True, title = False, save = None):
 
     '''
     Show the expression of a gene in cells or ST beads
 
     The figure will be saved as `root + save + '_' + gene + '.png'`
```

### Comparing `SC2Spa-1.2.1/SC2Spa.egg-info/PKG-INFO` & `SC2Spa-1.2.2/SC2Spa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.1
+Version: 1.2.2
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.2.1/pyproject.toml` & `SC2Spa-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

