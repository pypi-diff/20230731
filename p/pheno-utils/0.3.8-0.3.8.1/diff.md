# Comparing `tmp/pheno-utils-0.3.8.tar.gz` & `tmp/pheno-utils-0.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.8.tar", last modified: Mon Jul 31 07:54:31 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.8.1.tar", last modified: Mon Jul 31 08:31:44 2023, max compression
```

## Comparing `pheno-utils-0.3.8.tar` & `pheno-utils-0.3.8.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:54:31.915063 pheno-utils-0.3.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2359 2023-07-31 07:54:31.909947 pheno-utils-0.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:54:31.836060 pheno-utils-0.3.8/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19682 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20194 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)     1267 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/questionnaires_handler.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:54:31.897398 pheno-utils-0.3.8/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2359 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      722 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.8/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      942 2023-07-31 07:53:20.000000 pheno-utils-0.3.8/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 07:54:31.923758 pheno-utils-0.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2591 2023-07-26 08:46:36.000000 pheno-utils-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:31:44.730141 pheno-utils-0.3.8.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-31 08:31:44.708176 pheno-utils-0.3.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:31:44.598493 pheno-utils-0.3.8.1/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19682 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20194 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/questionnaires_handler.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-31 08:30:08.000000 pheno-utils-0.3.8.1/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:31:44.663848 pheno-utils-0.3.8.1/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-31 08:31:44.000000 pheno-utils-0.3.8.1/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-31 08:31:44.000000 pheno-utils-0.3.8.1/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 08:31:44.000000 pheno-utils-0.3.8.1/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-31 08:31:44.000000 pheno-utils-0.3.8.1/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.8.1/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-31 08:31:44.000000 pheno-utils-0.3.8.1/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-31 08:31:44.000000 pheno-utils-0.3.8.1/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-31 08:16:28.000000 pheno-utils-0.3.8.1/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 08:31:44.764871 pheno-utils-0.3.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-26 08:46:36.000000 pheno-utils-0.3.8.1/setup.py
```

### Comparing `pheno-utils-0.3.8/LICENSE` & `pheno-utils-0.3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/PKG-INFO` & `pheno-utils-0.3.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.8/README.md` & `pheno-utils-0.3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/_modidx.py` & `pheno-utils-0.3.8.1/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.8.1/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.8.1/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/basic_plots.py` & `pheno-utils-0.3.8.1/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.8.1/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.8.1/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.8.1/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/config.py` & `pheno-utils-0.3.8.1/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/dates_plots.py` & `pheno-utils-0.3.8.1/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.8.1/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/meta_loader.py` & `pheno-utils-0.3.8.1/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.8.1/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils/questionnaires_handler.py` & `pheno-utils-0.3.8.1/pheno_utils/questionnaires_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,12 +21,15 @@
                      dict_df: pd.DataFrame, mapping_df: pd.DataFrame) -> pd.Series:
     code_from = transform_from.lower()
     code_to = transform_to.lower()
     assert code_from in ['hebrew', 'english', 'coding']
     assert code_to in ['hebrew', 'english', 'coding']
     
     # the index of the dict_df is the tabular_field_name
-    code_string = convert_to_string(dict_df.loc[tab_field_name]['data_coding'])
+    if isinstance(dict_df.loc[tab_field_name]['data_coding'], pd.Series):
+        code_string = convert_to_string(dict_df.loc[tab_field_name]['data_coding'][0] )
+    else: 
+        code_string = convert_to_string(dict_df.loc[tab_field_name]['data_coding'])
     code_df = mapping_df[mapping_df['code_number'] == code_string].copy()
     coding = dict(zip(code_df[code_from].astype(int).astype(str), code_df[code_to]))
     return orig_answer.astype(str).replace(coding)
```

### Comparing `pheno-utils-0.3.8/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.8.1/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.8.1/pheno_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.8/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.8.1/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8/settings.ini` & `pheno-utils-0.3.8.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.8
+version = 0.3.8.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

### Comparing `pheno-utils-0.3.8/setup.py` & `pheno-utils-0.3.8.1/setup.py`

 * *Files identical despite different names*

