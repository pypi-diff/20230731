# Comparing `tmp/pelc-0.5.2.tar.gz` & `tmp/pelc-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelc-0.5.2.tar", max compression
+gzip compressed data, was "pelc-0.5.3.tar", max compression
```

## Comparing `pelc-0.5.2.tar` & `pelc-0.5.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      153 2023-01-23 15:17:57.130463 pelc-0.5.2/pelc/__init__.py
--rw-r--r--   0        0        0     2124 2023-04-20 20:27:25.207099 pelc-0.5.2/pelc/_input_sanity_check.py
--rw-r--r--   0        0        0     2370 2023-04-03 06:26:08.645035 pelc-0.5.2/pelc/_open_epregistry_databases.py
--rw-r--r--   0        0        0     2380 2023-03-29 12:31:04.739936 pelc-0.5.2/pelc/_unexpected_alleles.py
--rw-r--r--   0        0        0    10287 2023-07-21 13:34:31.293683 pelc-0.5.2/pelc/batch_eplet_comp.py
--rw-r--r--   0        0        0     7935 2023-03-29 12:27:43.032924 pelc-0.5.2/pelc/batch_eplet_comp_aux.py
--rw-r--r--   0        0        0   115455 2023-01-11 14:48:35.472443 pelc-0.5.2/pelc/data/A.csv
--rw-r--r--   0        0        0   138339 2023-04-03 06:26:57.877645 pelc-0.5.2/pelc/data/A_False_A_.pickle
--rw-r--r--   0        0        0     6382 2023-04-03 06:27:12.022395 pelc-0.5.2/pelc/data/A_True_A_.pickle
--rw-r--r--   0        0        0   160035 2023-01-11 14:48:35.523080 pelc-0.5.2/pelc/data/B.csv
--rw-r--r--   0        0        0   209729 2023-04-03 06:26:57.893263 pelc-0.5.2/pelc/data/B_False_B_.pickle
--rw-r--r--   0        0        0    10304 2023-04-03 06:27:12.022395 pelc-0.5.2/pelc/data/B_True_B_.pickle
--rw-r--r--   0        0        0    46142 2023-01-11 14:48:35.546441 pelc-0.5.2/pelc/data/C.csv
--rw-r--r--   0        0        0    62050 2023-04-03 06:26:57.908987 pelc-0.5.2/pelc/data/C_False_C_.pickle
--rw-r--r--   0        0        0     3777 2023-04-03 06:27:12.022395 pelc-0.5.2/pelc/data/C_True_C_.pickle
--rw-r--r--   0        0        0    61100 2023-01-11 14:48:35.675866 pelc-0.5.2/pelc/data/DP.csv
--rw-r--r--   0        0        0   104070 2023-04-03 06:26:57.956271 pelc-0.5.2/pelc/data/DP_False_DPB1_.pickle
--rw-r--r--   0        0        0     9774 2023-04-03 06:27:08.976536 pelc-0.5.2/pelc/data/DP_True_DPB1_.pickle
--rw-r--r--   0        0        0    18294 2023-01-11 14:48:35.718263 pelc-0.5.2/pelc/data/DQ.csv
--rw-r--r--   0        0        0    34476 2023-04-03 06:26:57.940645 pelc-0.5.2/pelc/data/DQ_False_DQB1_.pickle
--rw-r--r--   0        0        0     2479 2023-04-03 06:27:08.976536 pelc-0.5.2/pelc/data/DQ_True_DQB1_.pickle
--rw-r--r--   0        0        0   169376 2023-01-11 14:48:35.855944 pelc-0.5.2/pelc/data/DR.csv
--rw-r--r--   0        0        0   320839 2023-04-03 06:26:57.925016 pelc-0.5.2/pelc/data/DR_False_DRB1_.pickle
--rw-r--r--   0        0        0    12678 2023-04-03 06:27:08.960909 pelc-0.5.2/pelc/data/DR_True_DRB1_.pickle
--rw-r--r--   0        0        0    13281 2023-01-11 15:29:16.746377 pelc-0.5.2/pelc/data/ep_data.csv
--rw-r--r--   0        0        0    16515 2023-04-03 06:26:57.956271 pelc-0.5.2/pelc/data/ep_data.pickle
--rw-r--r--   0        0        0      146 2023-01-09 17:00:55.194758 pelc-0.5.2/pelc/output_type.py
--rw-r--r--   0        0        0     3265 2023-04-03 06:35:26.318686 pelc-0.5.2/pelc/simple_comparison.py
--rw-r--r--   0        0        0      511 2023-07-21 14:35:10.888718 pelc-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     9114 2023-07-21 14:35:10.891723 pelc-0.5.2/README.md
--rw-r--r--   0        0        0     9864 1970-01-01 00:00:00.000000 pelc-0.5.2/setup.py
--rw-r--r--   0        0        0     9420 1970-01-01 00:00:00.000000 pelc-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      153 2023-01-23 15:17:57.130463 pelc-0.5.3/pelc/__init__.py
+-rw-r--r--   0        0        0     2124 2023-04-20 20:27:25.207099 pelc-0.5.3/pelc/_input_sanity_check.py
+-rw-r--r--   0        0        0     2370 2023-04-03 06:26:08.645035 pelc-0.5.3/pelc/_open_epregistry_databases.py
+-rw-r--r--   0        0        0     2380 2023-03-29 12:31:04.739936 pelc-0.5.3/pelc/_unexpected_alleles.py
+-rw-r--r--   0        0        0    10584 2023-07-31 20:33:09.987159 pelc-0.5.3/pelc/batch_eplet_comp.py
+-rw-r--r--   0        0        0     8226 2023-07-31 20:37:55.410565 pelc-0.5.3/pelc/batch_eplet_comp_aux.py
+-rw-r--r--   0        0        0   115455 2023-01-11 14:48:35.472443 pelc-0.5.3/pelc/data/A.csv
+-rw-r--r--   0        0        0   138339 2023-04-03 06:26:57.877645 pelc-0.5.3/pelc/data/A_False_A_.pickle
+-rw-r--r--   0        0        0     6382 2023-04-03 06:27:12.022395 pelc-0.5.3/pelc/data/A_True_A_.pickle
+-rw-r--r--   0        0        0   160035 2023-01-11 14:48:35.523080 pelc-0.5.3/pelc/data/B.csv
+-rw-r--r--   0        0        0   209729 2023-04-03 06:26:57.893263 pelc-0.5.3/pelc/data/B_False_B_.pickle
+-rw-r--r--   0        0        0    10304 2023-04-03 06:27:12.022395 pelc-0.5.3/pelc/data/B_True_B_.pickle
+-rw-r--r--   0        0        0    46142 2023-01-11 14:48:35.546441 pelc-0.5.3/pelc/data/C.csv
+-rw-r--r--   0        0        0    62050 2023-04-03 06:26:57.908987 pelc-0.5.3/pelc/data/C_False_C_.pickle
+-rw-r--r--   0        0        0     3777 2023-04-03 06:27:12.022395 pelc-0.5.3/pelc/data/C_True_C_.pickle
+-rw-r--r--   0        0        0    61100 2023-01-11 14:48:35.675866 pelc-0.5.3/pelc/data/DP.csv
+-rw-r--r--   0        0        0   104070 2023-04-03 06:26:57.956271 pelc-0.5.3/pelc/data/DP_False_DPB1_.pickle
+-rw-r--r--   0        0        0     9774 2023-04-03 06:27:08.976536 pelc-0.5.3/pelc/data/DP_True_DPB1_.pickle
+-rw-r--r--   0        0        0    18294 2023-01-11 14:48:35.718263 pelc-0.5.3/pelc/data/DQ.csv
+-rw-r--r--   0        0        0    34476 2023-04-03 06:26:57.940645 pelc-0.5.3/pelc/data/DQ_False_DQB1_.pickle
+-rw-r--r--   0        0        0     2479 2023-04-03 06:27:08.976536 pelc-0.5.3/pelc/data/DQ_True_DQB1_.pickle
+-rw-r--r--   0        0        0   169376 2023-01-11 14:48:35.855944 pelc-0.5.3/pelc/data/DR.csv
+-rw-r--r--   0        0        0   320839 2023-04-03 06:26:57.925016 pelc-0.5.3/pelc/data/DR_False_DRB1_.pickle
+-rw-r--r--   0        0        0    12678 2023-04-03 06:27:08.960909 pelc-0.5.3/pelc/data/DR_True_DRB1_.pickle
+-rw-r--r--   0        0        0    13281 2023-01-11 15:29:16.746377 pelc-0.5.3/pelc/data/ep_data.csv
+-rw-r--r--   0        0        0    16515 2023-04-03 06:26:57.956271 pelc-0.5.3/pelc/data/ep_data.pickle
+-rw-r--r--   0        0        0      146 2023-01-09 17:00:55.194758 pelc-0.5.3/pelc/output_type.py
+-rw-r--r--   0        0        0     3263 2023-07-31 20:24:27.250728 pelc-0.5.3/pelc/simple_comparison.py
+-rw-r--r--   0        0        0      511 2023-07-31 20:55:28.727194 pelc-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     9101 2023-07-31 20:55:28.727194 pelc-0.5.3/README.md
+-rw-r--r--   0        0        0     9851 1970-01-01 00:00:00.000000 pelc-0.5.3/setup.py
+-rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pelc-0.5.3/PKG-INFO
```

### Comparing `pelc-0.5.2/pelc/_input_sanity_check.py` & `pelc-0.5.3/pelc/_input_sanity_check.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/_open_epregistry_databases.py` & `pelc-0.5.3/pelc/_open_epregistry_databases.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/_unexpected_alleles.py` & `pelc-0.5.3/pelc/_unexpected_alleles.py`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/batch_eplet_comp.py` & `pelc-0.5.3/pelc/batch_eplet_comp.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 )
 from pelc._unexpected_alleles import (
     _delete_unexpected_alleles,
     _remove_unexpected_other_individual,
 )
 from pelc.batch_eplet_comp_aux import (
     _allele_df_to_eplets_df,
-    _transform_eplet_load_detail
+    _replace_null_alleles,
+    _transform_eplet_load_detail,
 )
 from pelc.output_type import OutputType
 
 
 # MAIN
 def compute_epletic_load(
     input_df_donor: pd.DataFrame,
@@ -132,14 +133,19 @@
             df_c = _open_epregistry_database(
                 f"{this_file_directory_path}/data/C.csv", ["C*"], no_eplets=True
             )
 
 
     df_data = open_ep_data(this_file_directory_path)
 
+    # Replace Null alleles with ghost alleles in input_df_donors and input_df_recipients
+    _replace_null_alleles(input_df_donor)
+    _replace_null_alleles(input_df_recipient)
+
+    # Delete unexpected alleles (those who are not found in the EpRegistry database)
     input_df_donor, removed_donors = _delete_unexpected_alleles(
         input_df_donor, df_a, df_b, df_c, df_dr, df_dq, df_dp
     )
     input_df_recipient, removed_recipients = _delete_unexpected_alleles(
         input_df_recipient, df_a, df_b, df_c, df_dr, df_dq, df_dp
     )
```

### Comparing `pelc-0.5.2/pelc/batch_eplet_comp_aux.py` & `pelc-0.5.3/pelc/batch_eplet_comp_aux.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,7 +231,20 @@
         eplet_load_detail.replace("[]", "None")  # no regex no need to escape
         .replace("\\[", "", regex=True)
         .replace("\\]", "", regex=True)
         .replace("'", "", regex=True)
     )
 
     return eplet_load_detail
+
+
+def _replace_null_alleles(df: pd.DataFrame) -> None:
+    """
+    :param df: pd.DataFrame with the typing details
+    :return: None, the dataframe is modified inplace
+    """
+    df.replace(
+        r'^(.*\*).*N$',
+        r"\1",
+        regex=True,
+        inplace=True
+    )
```

### Comparing `pelc-0.5.2/pelc/data/A.csv` & `pelc-0.5.3/pelc/data/A.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/A_False_A_.pickle` & `pelc-0.5.3/pelc/data/A_False_A_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/A_True_A_.pickle` & `pelc-0.5.3/pelc/data/A_True_A_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/B.csv` & `pelc-0.5.3/pelc/data/B.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/B_False_B_.pickle` & `pelc-0.5.3/pelc/data/B_False_B_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/B_True_B_.pickle` & `pelc-0.5.3/pelc/data/B_True_B_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/C.csv` & `pelc-0.5.3/pelc/data/C.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/C_False_C_.pickle` & `pelc-0.5.3/pelc/data/C_False_C_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/C_True_C_.pickle` & `pelc-0.5.3/pelc/data/C_True_C_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DP.csv` & `pelc-0.5.3/pelc/data/DP.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DP_False_DPB1_.pickle` & `pelc-0.5.3/pelc/data/DP_False_DPB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DP_True_DPB1_.pickle` & `pelc-0.5.3/pelc/data/DP_True_DPB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DQ.csv` & `pelc-0.5.3/pelc/data/DQ.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DQ_False_DQB1_.pickle` & `pelc-0.5.3/pelc/data/DQ_False_DQB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DQ_True_DQB1_.pickle` & `pelc-0.5.3/pelc/data/DQ_True_DQB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DR.csv` & `pelc-0.5.3/pelc/data/DR.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DR_False_DRB1_.pickle` & `pelc-0.5.3/pelc/data/DR_False_DRB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/DR_True_DRB1_.pickle` & `pelc-0.5.3/pelc/data/DR_True_DRB1_.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/ep_data.csv` & `pelc-0.5.3/pelc/data/ep_data.csv`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/data/ep_data.pickle` & `pelc-0.5.3/pelc/data/ep_data.pickle`

 * *Files identical despite different names*

### Comparing `pelc-0.5.2/pelc/simple_comparison.py` & `pelc-0.5.3/pelc/simple_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 
 def _is_valid_allele(allele: str) -> bool:
     """
     :param allele: allele to check
     :return: whether or not the allele is valid
     """
-
     return "*" in allele and ":" in allele
 
 
 def _same_locus(allele1: str, allele2: str) -> bool:
     """
     :param allele1: First allele to compare
     :param allele2: Second allele to compare
```

### Comparing `pelc-0.5.2/README.md` & `pelc-0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -85,18 +85,18 @@
 ```
 - 55: an eplet did not match the regular expression '^\d+' (ABC, DR, DQ or DP) and it also did not match the regular
 expression '^.[pqr]*(\d+)' (interlocus2) either.
 ```
 
 
 #### Unit tests
-Tested on `Python 3.10.2` & `Python 3.11.1`.
+Tested on `Python 3.10.6` & `Python 3.11.1`.
 ```
-platform win32 -- Python 3.10.2, pytest-7.2.0, pluggy-1.0.0
-plugins: anyio-3.6.2, mypy-0.10.3
+platform win32 -- Python 3.10.6, pytest-7.4.0, pluggy-1.2.0
+plugins: mypy-0.10.3
 collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
 unit_tests_simple.py .                                                   [  7%]
 pelc\__init__.py .                                                       [ 10%]
 pelc\_input_sanity_check.py .                                            [ 12%]
 pelc\_open_epregistry_databases.py .                                     [ 15%]
@@ -114,19 +114,19 @@
 tests\test_pelc.py ..                                                    [ 76%]
 tests\test_same_locus.py ..                                              [ 82%]
 tests\test_simple_comparison.py .....                                    [ 94%]
 tests\test_unexpected_alleles.py ..                                      [100%]
 ==================================== mypy =====================================
 
 Success: no issues found in 20 source files
-============================= 39 passed in 32.56s =============================
+============================= 39 passed in 34.42s =============================
 ```
 
 ```
-platform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0
+platform win32 -- Python 3.11.1, pytest-7.2.2, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
 collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
 unit_tests_simple.py .                                                   [  7%]
 pelc\__init__.py .                                                       [ 10%]
 pelc\_input_sanity_check.py .                                            [ 12%]
@@ -173,26 +173,26 @@
 If you use this software, please cite it as below.
 
 - APA:
 ```
 If you use this software, please cite it as below. 
 
 Lhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). 
-Python Eplet Load Calculator (PELC) package (Version 0.5.2) [Computer software].
+Python Eplet Load Calculator (PELC) package (Version 0.5.3) [Computer software].
 https://doi.org/10.5281/zenodo.7254809
 ```
 
 - BibTeX:
 ```
 @software{lhotte_romain_2022_7526198,
   author       = {Lhotte, Romain and
                   Clichet, Valentin and
                   Usureau, Cédric and
                   Taupin, Jean-Luc},
   title        = {Python Eplet Load Calculator},
   month        = oct,
   year         = 2022,
   publisher    = {Zenodo},
-  version      = {0.5.2},
+  version      = {0.5.3},
   doi          = {10.5281/zenodo.7526198},
 }
 ```
```

### Comparing `pelc-0.5.2/setup.py` & `pelc-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['openpyxl>=3.0.10,<4.0.0',
  'pandas-stubs>=2.0.0.230412,<3.0.0.0',
  'pandas>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'pelc',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'Python Eplet Load Calculator',
-    'long_description': '[![DOI](https://zenodo.org/badge/555576588.svg)](https://zenodo.org/badge/latestdoi/555576588)\n[![Downloads](https://pepy.tech/badge/pelc)](https://pepy.tech/project/pelc)\n# PELC (Python Eplet Load Calculator)\n\n### Overview\nPELC is a Python package designed to calculate efficiently the HLA Eplet Load (based on the\n[EpRegistry database](https://www.epregistry.com.br/)) between donors and recipients by loading in a pandas.DataFrame\nin `eplet_comparison.compute_epletic_load` the recipients\' and donors\' typings.  See minimal reproducible example for\nmore details.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pelc`, run `pip install pelc` in your terminal.\n\n\n#### Usage\n\n##### a. Comparing two alleles\nHere is a minimal example of how to use `pelc` to compare two alleles:\n```py\nfrom pelc.simple_comparison import simple_comparison\n\nsimple_comparison(\n    "A*68:01",\n    "A*68:02",\n    "output",  # file will be saved as output.csv in the current directory\n    verifiedonly=False,  # if True, only verified eplets will be considered, otherwise all eplets will be considered\n    interlocus2=True  # doesn\'t matter for class I alleles\n)\n```\nIn the `output.csv` file created in the current directory, you will find two rows: "In A&ast;68:02 but not in \nA&ast;68:01" and "In A&ast;68:01 but not in A&ast;68:02".\n\n##### b. Batch mode\nHere is a minimal example with the file [Template.xlsx](https://github.com/MICS-Lab/pelc/raw/main/Template.xlsx)\n(click to download):\n```py\nimport pandas as pd\n\nfrom pelc import batch_eplet_comp, batch_eplet_comp_aux, output_type\n\nif __name__ == "__main__":\n    input_path: str = "Template.xlsx"\n\n    output_path: str = "MyOutput"\n    input_df: pd.DataFrame = pd.read_excel(\n        input_path,\n        sheet_name="My Sheet",\n        index_col=0,\n    )\n\n    donordf: pd.DataFrame\n    recipientdf: pd.DataFrame\n    donordf, recipientdf = batch_eplet_comp_aux.split_dataframe(input_df)\n\n    batch_eplet_comp.compute_epletic_load(\n        donordf,\n        recipientdf,\n        output_path,\n        output_type.OutputType.DETAILS_AND_COUNT,\n        class_i=True,  # Compute class I eplets comparison?\n        class_ii=True,  # Compute class II eplets comparison?\n        verifiedonly=False,  # How should the epletic charge be computed? Verified eplets only? Or all eplets?\n        exclude=None,  # list of indices to exclude\n        interlocus2=True  # whether or not to take into account interlocus eplets for HLA of class II\n    )\n```\nNote that if a typing is unknown, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for **both** recipients and\ndonors. If the allele is unknown for only of the two individuals, it is necessary to use `A*`, `B*`, ..., `DPB1*` for\nboth individuals otherwise the eplet mismatch computation will not be performed for this donor / recipient pair.\n\n#### Advanced usage:\n##### a. Not taking into account all loci (if they are not typed for example)\nIf one wants to determine the eplet mismatches between a donor and a recipient but without taking into account\na certain locus, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for both recipients and donors on this locus\nand the eplet mismatch computation will only take into account the loci filled in.\n\n##### b. Not creating a file but generating a pandas.DataFrame\nIf one wants to generate a `pandas.DataFrame` directly, the `output_path` argument of `simple_comparison` can be \nset to `None`. The `pandas.DataFrame` will be returned by the function. Same goes for `compute_epletic_load`.\n\n\n#### Exit codes:\n```\n- 55: an eplet did not match the regular expression \'^\\d+\' (ABC, DR, DQ or DP) and it also did not match the regular\nexpression \'^.[pqr]*(\\d+)\' (interlocus2) either.\n```\n\n\n#### Unit tests\nTested on `Python 3.10.2` & `Python 3.11.1`.\n```\nplatform win32 -- Python 3.10.2, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 39 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  7%]\npelc\\__init__.py .                                                       [ 10%]\npelc\\_input_sanity_check.py .                                            [ 12%]\npelc\\_open_epregistry_databases.py .                                     [ 15%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 25%]\npelc\\simple_comparison.py .                                              [ 28%]\ntests\\__init__.py .                                                      [ 30%]\ntests\\base_loading_for_tests.py .                                        [ 33%]\ntests\\test_eplet_mismatches.py .........                                 [ 56%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 66%]\ntests\\test_only_one_chromosome.py ..                                     [ 71%]\ntests\\test_pelc.py ..                                                    [ 76%]\ntests\\test_same_locus.py ..                                              [ 82%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n==================================== mypy =====================================\n\nSuccess: no issues found in 20 source files\n============================= 39 passed in 32.56s =============================\n```\n\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 39 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  7%]\npelc\\__init__.py .                                                       [ 10%]\npelc\\_input_sanity_check.py .                                            [ 12%]\npelc\\_open_epregistry_databases.py .                                     [ 15%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 25%]\npelc\\simple_comparison.py .                                              [ 28%]\ntests\\__init__.py .                                                      [ 30%]\ntests\\base_loading_for_tests.py .                                        [ 33%]\ntests\\test_eplet_mismatches.py .........                                 [ 56%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 66%]\ntests\\test_only_one_chromosome.py ..                                     [ 71%]\ntests\\test_pelc.py ..                                                    [ 76%]\ntests\\test_same_locus.py ..                                              [ 82%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n==================================== mypy =====================================\n\nSuccess: no issues found in 20 source files\n============================= 39 passed in 32.56s =============================\n```\n\n\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pelc)\n- [Corresponding PyPI page](https://pypi.org/project/pelc)\n\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n```\nIf you use this software, please cite it as below. \n\nLhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). \nPython Eplet Load Calculator (PELC) package (Version 0.5.2) [Computer software].\nhttps://doi.org/10.5281/zenodo.7254809\n```\n\n- BibTeX:\n```\n@software{lhotte_romain_2022_7526198,\n  author       = {Lhotte, Romain and\n                  Clichet, Valentin and\n                  Usureau, Cédric and\n                  Taupin, Jean-Luc},\n  title        = {Python Eplet Load Calculator},\n  month        = oct,\n  year         = 2022,\n  publisher    = {Zenodo},\n  version      = {0.5.2},\n  doi          = {10.5281/zenodo.7526198},\n}\n```\n',
+    'long_description': '[![DOI](https://zenodo.org/badge/555576588.svg)](https://zenodo.org/badge/latestdoi/555576588)\n[![Downloads](https://pepy.tech/badge/pelc)](https://pepy.tech/project/pelc)\n# PELC (Python Eplet Load Calculator)\n\n### Overview\nPELC is a Python package designed to calculate efficiently the HLA Eplet Load (based on the\n[EpRegistry database](https://www.epregistry.com.br/)) between donors and recipients by loading in a pandas.DataFrame\nin `eplet_comparison.compute_epletic_load` the recipients\' and donors\' typings.  See minimal reproducible example for\nmore details.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pelc`, run `pip install pelc` in your terminal.\n\n\n#### Usage\n\n##### a. Comparing two alleles\nHere is a minimal example of how to use `pelc` to compare two alleles:\n```py\nfrom pelc.simple_comparison import simple_comparison\n\nsimple_comparison(\n    "A*68:01",\n    "A*68:02",\n    "output",  # file will be saved as output.csv in the current directory\n    verifiedonly=False,  # if True, only verified eplets will be considered, otherwise all eplets will be considered\n    interlocus2=True  # doesn\'t matter for class I alleles\n)\n```\nIn the `output.csv` file created in the current directory, you will find two rows: "In A&ast;68:02 but not in \nA&ast;68:01" and "In A&ast;68:01 but not in A&ast;68:02".\n\n##### b. Batch mode\nHere is a minimal example with the file [Template.xlsx](https://github.com/MICS-Lab/pelc/raw/main/Template.xlsx)\n(click to download):\n```py\nimport pandas as pd\n\nfrom pelc import batch_eplet_comp, batch_eplet_comp_aux, output_type\n\nif __name__ == "__main__":\n    input_path: str = "Template.xlsx"\n\n    output_path: str = "MyOutput"\n    input_df: pd.DataFrame = pd.read_excel(\n        input_path,\n        sheet_name="My Sheet",\n        index_col=0,\n    )\n\n    donordf: pd.DataFrame\n    recipientdf: pd.DataFrame\n    donordf, recipientdf = batch_eplet_comp_aux.split_dataframe(input_df)\n\n    batch_eplet_comp.compute_epletic_load(\n        donordf,\n        recipientdf,\n        output_path,\n        output_type.OutputType.DETAILS_AND_COUNT,\n        class_i=True,  # Compute class I eplets comparison?\n        class_ii=True,  # Compute class II eplets comparison?\n        verifiedonly=False,  # How should the epletic charge be computed? Verified eplets only? Or all eplets?\n        exclude=None,  # list of indices to exclude\n        interlocus2=True  # whether or not to take into account interlocus eplets for HLA of class II\n    )\n```\nNote that if a typing is unknown, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for **both** recipients and\ndonors. If the allele is unknown for only of the two individuals, it is necessary to use `A*`, `B*`, ..., `DPB1*` for\nboth individuals otherwise the eplet mismatch computation will not be performed for this donor / recipient pair.\n\n#### Advanced usage:\n##### a. Not taking into account all loci (if they are not typed for example)\nIf one wants to determine the eplet mismatches between a donor and a recipient but without taking into account\na certain locus, one can use `A*`, `B*`, ..., `DPB1*` as the allele name for both recipients and donors on this locus\nand the eplet mismatch computation will only take into account the loci filled in.\n\n##### b. Not creating a file but generating a pandas.DataFrame\nIf one wants to generate a `pandas.DataFrame` directly, the `output_path` argument of `simple_comparison` can be \nset to `None`. The `pandas.DataFrame` will be returned by the function. Same goes for `compute_epletic_load`.\n\n\n#### Exit codes:\n```\n- 55: an eplet did not match the regular expression \'^\\d+\' (ABC, DR, DQ or DP) and it also did not match the regular\nexpression \'^.[pqr]*(\\d+)\' (interlocus2) either.\n```\n\n\n#### Unit tests\nTested on `Python 3.10.6` & `Python 3.11.1`.\n```\nplatform win32 -- Python 3.10.6, pytest-7.4.0, pluggy-1.2.0\nplugins: mypy-0.10.3\ncollected 39 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  7%]\npelc\\__init__.py .                                                       [ 10%]\npelc\\_input_sanity_check.py .                                            [ 12%]\npelc\\_open_epregistry_databases.py .                                     [ 15%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 25%]\npelc\\simple_comparison.py .                                              [ 28%]\ntests\\__init__.py .                                                      [ 30%]\ntests\\base_loading_for_tests.py .                                        [ 33%]\ntests\\test_eplet_mismatches.py .........                                 [ 56%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 66%]\ntests\\test_only_one_chromosome.py ..                                     [ 71%]\ntests\\test_pelc.py ..                                                    [ 76%]\ntests\\test_same_locus.py ..                                              [ 82%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n==================================== mypy =====================================\n\nSuccess: no issues found in 20 source files\n============================= 39 passed in 34.42s =============================\n```\n\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.2, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 39 items\n\nunit_tests_mypy.py ..                                                    [  5%]\nunit_tests_simple.py .                                                   [  7%]\npelc\\__init__.py .                                                       [ 10%]\npelc\\_input_sanity_check.py .                                            [ 12%]\npelc\\_open_epregistry_databases.py .                                     [ 15%]\npelc\\_unexpected_alleles.py .                                            [ 17%]\npelc\\batch_eplet_comp.py .                                               [ 20%]\npelc\\batch_eplet_comp_aux.py .                                           [ 23%]\npelc\\output_type.py .                                                    [ 25%]\npelc\\simple_comparison.py .                                              [ 28%]\ntests\\__init__.py .                                                      [ 30%]\ntests\\base_loading_for_tests.py .                                        [ 33%]\ntests\\test_eplet_mismatches.py .........                                 [ 56%]\ntests\\test_extract_key_to_rank_epletes.py ..                             [ 61%]\ntests\\test_is_valid_allele.py ..                                         [ 66%]\ntests\\test_only_one_chromosome.py ..                                     [ 71%]\ntests\\test_pelc.py ..                                                    [ 76%]\ntests\\test_same_locus.py ..                                              [ 82%]\ntests\\test_simple_comparison.py .....                                    [ 94%]\ntests\\test_unexpected_alleles.py ..                                      [100%]\n==================================== mypy =====================================\n\nSuccess: no issues found in 20 source files\n============================= 39 passed in 32.56s =============================\n```\n\n\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pelc)\n- [Corresponding PyPI page](https://pypi.org/project/pelc)\n\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n```\nIf you use this software, please cite it as below. \n\nLhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). \nPython Eplet Load Calculator (PELC) package (Version 0.5.3) [Computer software].\nhttps://doi.org/10.5281/zenodo.7254809\n```\n\n- BibTeX:\n```\n@software{lhotte_romain_2022_7526198,\n  author       = {Lhotte, Romain and\n                  Clichet, Valentin and\n                  Usureau, Cédric and\n                  Taupin, Jean-Luc},\n  title        = {Python Eplet Load Calculator},\n  month        = oct,\n  year         = 2022,\n  publisher    = {Zenodo},\n  version      = {0.5.3},\n  doi          = {10.5281/zenodo.7526198},\n}\n```\n',
     'author': 'JasonMendoza2008',
     'author_email': 'lhotteromain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pelc-0.5.2/PKG-INFO` & `pelc-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelc
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python Eplet Load Calculator
 Author: JasonMendoza2008
 Author-email: lhotteromain@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -100,18 +100,18 @@
 ```
 - 55: an eplet did not match the regular expression '^\d+' (ABC, DR, DQ or DP) and it also did not match the regular
 expression '^.[pqr]*(\d+)' (interlocus2) either.
 ```
 
 
 #### Unit tests
-Tested on `Python 3.10.2` & `Python 3.11.1`.
+Tested on `Python 3.10.6` & `Python 3.11.1`.
 ```
-platform win32 -- Python 3.10.2, pytest-7.2.0, pluggy-1.0.0
-plugins: anyio-3.6.2, mypy-0.10.3
+platform win32 -- Python 3.10.6, pytest-7.4.0, pluggy-1.2.0
+plugins: mypy-0.10.3
 collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
 unit_tests_simple.py .                                                   [  7%]
 pelc\__init__.py .                                                       [ 10%]
 pelc\_input_sanity_check.py .                                            [ 12%]
 pelc\_open_epregistry_databases.py .                                     [ 15%]
@@ -129,19 +129,19 @@
 tests\test_pelc.py ..                                                    [ 76%]
 tests\test_same_locus.py ..                                              [ 82%]
 tests\test_simple_comparison.py .....                                    [ 94%]
 tests\test_unexpected_alleles.py ..                                      [100%]
 ==================================== mypy =====================================
 
 Success: no issues found in 20 source files
-============================= 39 passed in 32.56s =============================
+============================= 39 passed in 34.42s =============================
 ```
 
 ```
-platform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0
+platform win32 -- Python 3.11.1, pytest-7.2.2, pluggy-1.0.0
 plugins: anyio-3.6.2, mypy-0.10.3
 collected 39 items
 
 unit_tests_mypy.py ..                                                    [  5%]
 unit_tests_simple.py .                                                   [  7%]
 pelc\__init__.py .                                                       [ 10%]
 pelc\_input_sanity_check.py .                                            [ 12%]
@@ -188,27 +188,27 @@
 If you use this software, please cite it as below.
 
 - APA:
 ```
 If you use this software, please cite it as below. 
 
 Lhotte, R., Clichet, V., Usureau, C. & Taupin, J. (2022). 
-Python Eplet Load Calculator (PELC) package (Version 0.5.2) [Computer software].
+Python Eplet Load Calculator (PELC) package (Version 0.5.3) [Computer software].
 https://doi.org/10.5281/zenodo.7254809
 ```
 
 - BibTeX:
 ```
 @software{lhotte_romain_2022_7526198,
   author       = {Lhotte, Romain and
                   Clichet, Valentin and
                   Usureau, Cédric and
                   Taupin, Jean-Luc},
   title        = {Python Eplet Load Calculator},
   month        = oct,
   year         = 2022,
   publisher    = {Zenodo},
-  version      = {0.5.2},
+  version      = {0.5.3},
   doi          = {10.5281/zenodo.7526198},
 }
 ```
```

