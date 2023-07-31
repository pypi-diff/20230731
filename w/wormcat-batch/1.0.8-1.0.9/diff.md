# Comparing `tmp/wormcat_batch-1.0.8.tar.gz` & `tmp/wormcat_batch-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormcat_batch-1.0.8.tar", last modified: Fri Jun 30 16:42:32 2023, max compression
+gzip compressed data, was "wormcat_batch-1.0.9.tar", last modified: Mon Jul 31 12:07:09 2023, max compression
```

## Comparing `wormcat_batch-1.0.8.tar` & `wormcat_batch-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 16:42:32.390137 wormcat_batch-1.0.8/
--rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.0.8/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-30 16:42:32.390027 wormcat_batch-1.0.8/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2346 2023-06-28 11:53:36.000000 wormcat_batch-1.0.8/README.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-06-30 16:42:32.390171 wormcat_batch-1.0.8/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      676 2023-06-30 16:39:58.000000 wormcat_batch-1.0.8/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 16:42:32.389143 wormcat_batch-1.0.8/wormcat_batch/
--rw-r--r--   0 dan        (501) staff       (20)     2024 2022-08-16 12:41:26.000000 wormcat_batch-1.0.8/wormcat_batch/create_wormcat_xlsx.py
--rw-r--r--   0 dan        (501) staff       (20)     2486 2023-06-27 18:05:20.000000 wormcat_batch-1.0.8/wormcat_batch/execute_r.py
--rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.0.8/wormcat_batch/is_wormcat_installed.R
--rwxr-xr-x   0 dan        (501) staff       (20)     8360 2023-06-30 16:41:09.000000 wormcat_batch-1.0.8/wormcat_batch/run_wormcat_batch.py
--rwxr-xr-x   0 dan        (501) staff       (20)     1446 2022-08-16 12:41:26.000000 wormcat_batch-1.0.8/wormcat_batch/worm_cat.R
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-06-30 16:42:32.389891 wormcat_batch-1.0.8/wormcat_batch.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-06-30 16:42:32.000000 wormcat_batch-1.0.8/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      451 2023-06-30 16:42:32.000000 wormcat_batch-1.0.8/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-30 16:42:32.000000 wormcat_batch-1.0.8/wormcat_batch.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2023-06-30 16:42:32.000000 wormcat_batch-1.0.8/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-06-30 14:14:54.000000 wormcat_batch-1.0.8/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       23 2023-06-30 16:42:32.000000 wormcat_batch-1.0.8/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       14 2023-06-30 16:42:32.000000 wormcat_batch-1.0.8/wormcat_batch.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 12:07:09.574432 wormcat_batch-1.0.9/
+-rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 12:07:09.574281 wormcat_batch-1.0.9/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2346 2023-06-28 11:53:36.000000 wormcat_batch-1.0.9/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-31 12:07:09.574518 wormcat_batch-1.0.9/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      691 2023-07-31 12:06:10.000000 wormcat_batch-1.0.9/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 12:07:09.573091 wormcat_batch-1.0.9/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     2024 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2486 2023-06-27 18:05:20.000000 wormcat_batch-1.0.9/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     8365 2023-07-31 11:42:52.000000 wormcat_batch-1.0.9/wormcat_batch/run_wormcat_batch.py
+-rwxr-xr-x   0 dan        (501) staff       (20)     1446 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 12:07:09.574113 wormcat_batch-1.0.9/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      451 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       23 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/top_level.txt
```

### Comparing `wormcat_batch-1.0.8/README.md` & `wormcat_batch-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.8/setup.py` & `wormcat_batch-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup
 
-#python setup.py sdist
+# rm -rf dist
+# python setup.py sdist
 #pip install dist/wormcat_batch-1.0.1.tar.gz
 # twine check dist/*
 # twine upload --repository pypi dist/*
 
 setup(name='wormcat_batch',
-      version='1.0.8',
+      version='1.0.9',
       description='Batch processing for Wormcat data',
       url='https://github.com/dphiggs01/Wormcat_batch',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
       license='MIT',
 
       packages=['wormcat_batch'],
```

### Comparing `wormcat_batch-1.0.8/wormcat_batch/create_wormcat_xlsx.py` & `wormcat_batch-1.0.9/wormcat_batch/create_wormcat_xlsx.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.8/wormcat_batch/execute_r.py` & `wormcat_batch-1.0.9/wormcat_batch/execute_r.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.0.8/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.0.9/wormcat_batch/run_wormcat_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,24 +91,26 @@
             print("ERROR: You must provide column names with either 'Sequence ID' or 'Wormbase ID")
             exit(-1)
 
         call_wormcat(sheet, gene_id_all, output_dir, annotation_file, input_type)
 
 def files_to_process(output_dir):
     '''
-    After all the sheet on the Excel have been executed create a dataframe that can be used to summarize the results
+    After all the sheets on the Excel have been executed create a dataframe that can be used to summarize the results
     this dataframe is used to create the output Excel
     '''
-    df_process = pd.DataFrame(columns=['sheet', 'category', 'file','label'])
+    process_lst = []
     for dir_nm in os.listdir(output_dir):
         for cat_num in [1,2,3]:
             rgs_fisher = f"{output_dir}{os.path.sep}{dir_nm}{os.path.sep}rgs_fisher_cat{cat_num}.csv"
             cat_nm = f"Cat{cat_num}"
             row = {'sheet': cat_nm, 'category': cat_num, 'file': rgs_fisher,'label': dir_nm}
-            df_process = df_process.append(row, ignore_index=True)
+            process_lst.append(row)
+
+    df_process = pd.DataFrame(process_lst, columns=['sheet', 'category', 'file','label'])
     return df_process
 
 ##########################################################
 ## Utility functions
 
 def move_file_to_output_directory(file_path, output_directory,copy=False):
     '''
```

### Comparing `wormcat_batch-1.0.8/wormcat_batch/worm_cat.R` & `wormcat_batch-1.0.9/wormcat_batch/worm_cat.R`

 * *Files identical despite different names*

