# Comparing `tmp/cs2star-0.6.0.tar.gz` & `tmp/cs2star-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2star-0.6.0.tar", last modified: Mon Jul 31 12:48:57 2023, max compression
+gzip compressed data, was "cs2star-0.6.1.tar", last modified: Mon Jul 31 13:52:17 2023, max compression
```

## Comparing `cs2star-0.6.0.tar` & `cs2star-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 12:48:57.801122 cs2star-0.6.0/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.6.0/.gitignore
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.6.0/LICENSE
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 12:48:57.801122 cs2star-0.6.0/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.6.0/README.md
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 12:48:57.801122 cs2star-0.6.0/cs2star/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.6.0/cs2star/__init__.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star/_version.py
--rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    11001 2023-07-31 12:48:00.000000 cs2star-0.6.0/cs2star/cs2star.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3422 2023-03-29 12:13:31.000000 cs2star-0.6.0/cs2star/job_parser.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 12:48:57.801122 cs2star-0.6.0/cs2star.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/entry_points.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-07-31 12:48:57.000000 cs2star-0.6.0/cs2star.egg-info/top_level.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2023-07-31 12:44:31.000000 cs2star-0.6.0/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-07-31 12:48:57.801122 cs2star-0.6.0/setup.cfg
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 13:52:17.174568 cs2star-0.6.1/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       12 2022-05-03 16:46:56.000000 cs2star-0.6.1/.gitignore
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    35149 2022-05-03 16:12:49.000000 cs2star-0.6.1/LICENSE
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 13:52:17.171235 cs2star-0.6.1/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2167 2023-03-16 10:09:28.000000 cs2star-0.6.1/README.md
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 13:52:17.171235 cs2star-0.6.1/cs2star/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        0 2021-02-26 10:09:35.000000 cs2star-0.6.1/cs2star/__init__.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      160 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star/_version.py
+-rwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)    11537 2023-07-31 13:49:43.000000 cs2star-0.6.1/cs2star/cs2star.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3422 2023-03-29 12:13:31.000000 cs2star-0.6.1/cs2star/job_parser.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-07-31 13:52:17.171235 cs2star-0.6.1/cs2star.egg-info/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2692 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      312 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       49 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/entry_points.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       24 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/requires.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        8 2023-07-31 13:52:17.000000 cs2star-0.6.1/cs2star.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      841 2023-07-31 12:44:31.000000 cs2star-0.6.1/pyproject.toml
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-07-31 13:52:17.174568 cs2star-0.6.1/setup.cfg
```

### Comparing `cs2star-0.6.0/LICENSE` & `cs2star-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.0/PKG-INFO` & `cs2star-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.6.0
+Version: 0.6.1
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.6.0/README.md` & `cs2star-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.0/cs2star/cs2star.py` & `cs2star-0.6.1/cs2star/cs2star.py`

 * *Files 5% similar despite different names*

```diff
@@ -185,14 +185,22 @@
         # clean up
         cleaning = progress.add_task('Cleaning up data...', total=2)
         df_mic = pyem.star.check_defaults(df_mic, inplace=True)
         progress.update(cleaning, advance=1)
         df_mic = pyem.star.remove_deprecated_relion2(df_mic, inplace=True)
         progress.update(cleaning, advance=1)
 
+        # need to fix the micrographs optics because pyem is missing some things that relion wants
+        # also, optics are changed to 1-based indexing by pyem in parse_cryosparc_2_cs!!
+        df_mic['rlnOpticsGroup'] += 1
+        optics = ['rlnOpticsGroup'] + [head for head in ('rlnVoltage', 'rlnSphericalAberration') if head in df_part and head not in df_mic]
+        opt = df_part.get(optics).drop_duplicates()
+        df_mic = df_mic.loc[:, ~df_mic.columns.duplicated()]
+        df_mic = df_mic.merge(opt, on='rlnOpticsGroup')
+
         # symlink/copy images
         def copy_images(paths, to_dir, label='micrographs', copy=False, add_s=False):
             exists = False
             for img in progress.track(paths, description=f'{"Copying" if copy else "Linking"} {label} to {to_dir}...'):
                 orig = job_dir.parent / img
                 # new path + add s to extension for relion
                 moved = Path(to_dir / (orig.name + ('s' if add_s else '')))
```

### Comparing `cs2star-0.6.0/cs2star/job_parser.py` & `cs2star-0.6.1/cs2star/job_parser.py`

 * *Files identical despite different names*

### Comparing `cs2star-0.6.0/cs2star.egg-info/PKG-INFO` & `cs2star-0.6.1/cs2star.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2star
-Version: 0.6.0
+Version: 0.6.1
 Summary: A simple utility to convert cryosparc particle positions to relion star format.
 Author-email: Lorenzo Gaifas <brisvag@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/brisvag/cs2star/
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `cs2star-0.6.0/pyproject.toml` & `cs2star-0.6.1/pyproject.toml`

 * *Files identical despite different names*

