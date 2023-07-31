# Comparing `tmp/pheno-utils-0.3.7.7.tar.gz` & `tmp/pheno-utils-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.7.7.tar", last modified: Thu Jul 27 12:53:44 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.8.tar", last modified: Mon Jul 31 07:54:31 2023, max compression
```

## Comparing `pheno-utils-0.3.7.7.tar` & `pheno-utils-0.3.8.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:53:44.210536 pheno-utils-0.3.7.7/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-27 12:53:44.209557 pheno-utils-0.3.7.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.7.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:53:44.158715 pheno-utils-0.3.7.7/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19064 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20118 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-07-27 12:50:49.000000 pheno-utils-0.3.7.7/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:53:44.203677 pheno-utils-0.3.7.7/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-27 12:53:43.000000 pheno-utils-0.3.7.7/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-27 12:50:42.000000 pheno-utils-0.3.7.7/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 12:53:44.211037 pheno-utils-0.3.7.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2591 2023-07-26 08:46:36.000000 pheno-utils-0.3.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:54:31.915063 pheno-utils-0.3.8/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-07-31 07:54:31.909947 pheno-utils-0.3.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:54:31.836060 pheno-utils-0.3.8/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19682 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20194 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/questionnaires_handler.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-31 07:53:24.000000 pheno-utils-0.3.8/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:54:31.897398 pheno-utils-0.3.8/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.8/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-31 07:54:31.000000 pheno-utils-0.3.8/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      942 2023-07-31 07:53:20.000000 pheno-utils-0.3.8/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 07:54:31.923758 pheno-utils-0.3.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-07-26 08:46:36.000000 pheno-utils-0.3.8/setup.py
```

### Comparing `pheno-utils-0.3.7.7/LICENSE` & `pheno-utils-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/PKG-INFO` & `pheno-utils-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.7
+Version: 0.3.8
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.7/README.md` & `pheno-utils-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/_modidx.py` & `pheno-utils-0.3.8/pheno_utils/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,18 @@
                                                                                                    'pheno_utils/pheno_loader.py'),
                                           'pheno_utils.pheno_loader.PhenoLoader.get': ( 'pheno_loader.html#phenoloader.get',
                                                                                         'pheno_utils/pheno_loader.py'),
                                           'pheno_utils.pheno_loader.PhenoLoader.load_sample_data': ( 'pheno_loader.html#phenoloader.load_sample_data',
                                                                                                      'pheno_utils/pheno_loader.py'),
                                           'pheno_utils.pheno_loader.PhenoLoader.replace_bulk_data_path': ( 'pheno_loader.html#phenoloader.replace_bulk_data_path',
                                                                                                            'pheno_utils/pheno_loader.py')},
+            'pheno_utils.questionnaires_handler': { 'pheno_utils.questionnaires_handler.convert_to_string': ( 'questionnaire_handler.html#convert_to_string',
+                                                                                                              'pheno_utils/questionnaires_handler.py'),
+                                                    'pheno_utils.questionnaires_handler.tranform_answers': ( 'questionnaire_handler.html#tranform_answers',
+                                                                                                             'pheno_utils/questionnaires_handler.py')},
             'pheno_utils.sleep_plots': { 'pheno_utils.sleep_plots.format_xticks': ( 'sleep_plots.html#format_xticks',
                                                                                     'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.get_legend_colors': ( 'sleep_plots.html#get_legend_colors',
                                                                                         'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_channels': ( 'sleep_plots.html#plot_channels',
                                                                                     'pheno_utils/sleep_plots.py'),
                                          'pheno_utils.sleep_plots.plot_events': ( 'sleep_plots.html#plot_events',
```

### Comparing `pheno-utils-0.3.7.7/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.8/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.8/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/basic_plots.py` & `pheno-utils-0.3.8/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.8/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.8/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.8/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/config.py` & `pheno-utils-0.3.8/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/dates_plots.py` & `pheno-utils-0.3.8/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.8/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/meta_loader.py` & `pheno-utils-0.3.8/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.8/pheno_utils/pheno_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,17 @@
         parent_dict = self.dict.loc[self.dict.index.isin(fields), 'parent_dataframe'].dropna().to_dict()
         fields = [parent_dict.get(field, field) for field in fields]
         fields = [field for field in fields if field not in seen_fields and not seen_fields.add(field)]
         # fields += has_parent.unique().tolist()
         flexi_fields = list()
 
         data = pd.DataFrame()
-        for df in self.dfs.values():
+        for table_name, df in self.dfs.items():
+            if 'mapping' in table_name:
+                continue
             if flexible:
                 # use fuzzy matching including regex to find fields
                 fields_in_col = np.unique([col for f in fields for col in df.columns if re.search(f, col)])
                 flexi_fields += fields_in_col.tolist()
             else:
                 fields_in_col = df.columns.intersection(fields).difference(data.columns)
             if len(fields_in_col):
```

### Comparing `pheno-utils-0.3.7.7/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.8/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.7/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.8/pheno_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.7
+Version: 0.3.8
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.7/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.8/pheno_utils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pheno_utils/cgm_plots.py
 pheno_utils/cohort_selector.py
 pheno_utils/config.py
 pheno_utils/dates_plots.py
 pheno_utils/ecg_analysis.py
 pheno_utils/meta_loader.py
 pheno_utils/pheno_loader.py
+pheno_utils/questionnaires_handler.py
 pheno_utils/sleep_plots.py
 pheno_utils.egg-info/PKG-INFO
 pheno_utils.egg-info/SOURCES.txt
 pheno_utils.egg-info/dependency_links.txt
 pheno_utils.egg-info/entry_points.txt
 pheno_utils.egg-info/not-zip-safe
 pheno_utils.egg-info/requires.txt
```

### Comparing `pheno-utils-0.3.7.7/settings.ini` & `pheno-utils-0.3.8/settings.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.7.7
+version = 0.3.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

### Comparing `pheno-utils-0.3.7.7/setup.py` & `pheno-utils-0.3.8/setup.py`

 * *Files identical despite different names*

