# Comparing `tmp/cs2star-0.5.5.tar.gz` & `tmp/cs2star-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2star-0.5.5.tar", last modified: Sun Jul  2 08:26:12 2023, max compression
+gzip compressed data, was "cs2star-0.6.0.tar", last modified: Mon Jul 31 12:48:57 2023, max compression
```

## Comparing `cs2star-0.5.5.tar` & `cs2star-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brisvag   (1000) brisvag   (1000)        0 2023-07-02 08:26:12.132649 cs2star-0.5.5/
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)       12 2023-07-01 16:41:09.000000 cs2star-0.5.5/.gitignore
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)    35149 2023-07-01 16:41:09.000000 cs2star-0.5.5/LICENSE
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)     2692 2023-07-02 08:26:12.129315 cs2star-0.5.5/PKG-INFO
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)     2167 2023-07-01 16:41:09.000000 cs2star-0.5.5/README.md
-drwxr-xr-x   0 brisvag   (1000) brisvag   (1000)        0 2023-07-02 08:26:12.129315 cs2star-0.5.5/cs2star/
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)        0 2023-07-01 16:41:09.000000 cs2star-0.5.5/cs2star/__init__.py
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)      160 2023-07-02 08:26:11.000000 cs2star-0.5.5/cs2star/_version.py
--rwxr-xr-x   0 brisvag   (1000) brisvag   (1000)    11036 2023-07-02 08:22:29.000000 cs2star-0.5.5/cs2star/cs2star.py
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)     3422 2023-07-01 16:41:09.000000 cs2star-0.5.5/cs2star/job_parser.py
-drwxr-xr-x   0 brisvag   (1000) brisvag   (1000)        0 2023-07-02 08:26:12.129315 cs2star-0.5.5/cs2star.egg-info/
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)     2692 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/PKG-INFO
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)      312 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/SOURCES.txt
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)        1 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/dependency_links.txt
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)       49 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/entry_points.txt
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)       24 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/requires.txt
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)        8 2023-07-02 08:26:12.000000 cs2star-0.5.5/cs2star.egg-info/top_level.txt
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)      841 2023-07-01 16:41:09.000000 cs2star-0.5.5/pyproject.toml
--rw-r--r--   0 brisvag   (1000) brisvag   (1000)       38 2023-07-02 08:26:12.132649 cs2star-0.5.5/setup.cfg
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 12:48:57.801122 cs2star-0.6.0/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.6.0/.gitignore
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.6.0/LICENSE
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 12:48:57.801122 cs2star-0.6.0/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.6.0/README.md
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 12:48:57.801122 cs2star-0.6.0/cs2star/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.6.0/cs2star/__init__.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star/_version.py
+-rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    11001 2023-07-31 12:48:00.000000 cs2star-0.6.0/cs2star/cs2star.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3422 2023-03-29 12:13:31.000000 cs2star-0.6.0/cs2star/job_parser.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 12:48:57.801122 cs2star-0.6.0/cs2star.egg-info/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/entry_points.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/requires.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2023-07-31 12:44:31.000000 cs2star-0.6.0/pyproject.toml
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-07-31 12:48:57.801122 cs2star-0.6.0/setup.cfg
```

### Comparing `cs2star-0.5.5/LICENSE` & `cs2star-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2star-0.5.5/PKG-INFO` & `cs2star-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.5.5
+Version: 0.6.0
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.5.5/README.md` & `cs2star-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cs2star-0.5.5/cs2star/cs2star.py` & `cs2star-0.6.0/cs2star/cs2star.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,17 +166,17 @@
             classes = classes.split(',')
             print(f'selecting classes: {", ".join(classes)}')
             df_part = pyem.star.select_classes(df_part, classes)
 
         df_mic = pd.DataFrame()
         for f, p in progress.track(list(zip(micrographs, micrographs_passthrough)), description='Loading micrograph data...'):
             data = np.load(f)
-            df_mic_i = pyem.metadata.parse_cryosparc_2_cs(
-                data, passthroughs=[p],
-                minphic=0, boxsize=None, swapxy=swapxy, invertx=invertx, inverty=inverty)
+            df_mic_i = pyem.metadata.cryosparc_2_cs_movie_parameters(
+                data, passthroughs=[p], trajdir=str(f.parent.parent),
+            )
             df_mic = pd.concat([df_mic, df_mic_i], ignore_index=True)
 
         # clean up
         cleaning = progress.add_task('Cleaning up data...', total=2)
         df_part = pyem.star.check_defaults(df_part, inplace=True)
         progress.update(cleaning, advance=1)
         df_part = pyem.star.remove_deprecated_relion2(df_part, inplace=True)
```

### Comparing `cs2star-0.5.5/cs2star/job_parser.py` & `cs2star-0.6.0/cs2star/job_parser.py`

 * *Files identical despite different names*

### Comparing `cs2star-0.5.5/cs2star.egg-info/PKG-INFO` & `cs2star-0.6.0/cs2star.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.5.5
+Version: 0.6.0
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.5.5/pyproject.toml` & `cs2star-0.6.0/pyproject.toml`

 * *Files identical despite different names*

