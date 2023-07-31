# Comparing `tmp/iseqcbioportal-0.0.2.tar.gz` & `tmp/iseqcbioportal-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iseqcbioportal-0.0.2.tar", last modified: Thu Jul 27 14:31:44 2023, max compression
+gzip compressed data, was "iseqcbioportal-0.0.3.tar", last modified: Mon Jul 31 09:47:32 2023, max compression
```

## Comparing `iseqcbioportal-0.0.2.tar` & `iseqcbioportal-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3078 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/.gitignore
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1067 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/LICENSE
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      868 2023-07-26 10:19:46.000000 iseqcbioportal-0.0.2/README.md
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/cbioportal/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/cbioportal/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1419 2023-07-27 14:30:28.000000 iseqcbioportal-0.0.2/cbioportal/create_cbioportal_database.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/cbioportal/test/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/cbioportal/test/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1034 2023-07-25 16:44:42.000000 iseqcbioportal-0.0.2/cbioportal/test/create_cbioportal_database_test.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2081 2023-07-27 14:30:48.000000 iseqcbioportal-0.0.2/cbioportal/vcf_annotate_cbioportal.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      719 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      156 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/entry_points.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       90 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-07-27 14:31:43.000000 iseqcbioportal-0.0.2/iseqcbioportal.egg-info/top_level.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      957 2023-07-27 14:31:44.010106 iseqcbioportal-0.0.2/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       69 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/setup.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-27 14:31:44.006106 iseqcbioportal-0.0.2/utils/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.2/utils/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2360 2023-07-27 14:30:10.000000 iseqcbioportal-0.0.2/utils/utils.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-31 09:47:32.968659 iseqcbioportal-0.0.3/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     3078 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.3/.gitignore
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1067 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.3/LICENSE
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-31 09:47:32.968659 iseqcbioportal-0.0.3/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      868 2023-07-26 10:19:46.000000 iseqcbioportal-0.0.3/README.md
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-31 09:47:32.964659 iseqcbioportal-0.0.3/cbioportal/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.3/cbioportal/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1419 2023-07-31 09:45:23.000000 iseqcbioportal-0.0.3/cbioportal/create_cbioportal_database.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-31 09:47:32.964659 iseqcbioportal-0.0.3/cbioportal/test/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.3/cbioportal/test/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1034 2023-07-25 16:44:42.000000 iseqcbioportal-0.0.3/cbioportal/test/create_cbioportal_database_test.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2196 2023-07-31 09:45:20.000000 iseqcbioportal-0.0.3/cbioportal/vcf_annotate_cbioportal.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-31 09:47:32.968659 iseqcbioportal-0.0.3/iseqcbioportal.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     1399 2023-07-31 09:47:32.000000 iseqcbioportal-0.0.3/iseqcbioportal.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      719 2023-07-31 09:47:32.000000 iseqcbioportal-0.0.3/iseqcbioportal.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        1 2023-07-31 09:47:32.000000 iseqcbioportal-0.0.3/iseqcbioportal.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      156 2023-07-31 09:47:32.000000 iseqcbioportal-0.0.3/iseqcbioportal.egg-info/entry_points.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       90 2023-07-31 09:47:32.000000 iseqcbioportal-0.0.3/iseqcbioportal.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       17 2023-07-31 09:47:32.000000 iseqcbioportal-0.0.3/iseqcbioportal.egg-info/top_level.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)      957 2023-07-31 09:47:32.968659 iseqcbioportal-0.0.3/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)       69 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.3/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1000)        0 2023-07-31 09:47:32.968659 iseqcbioportal-0.0.3/utils/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)        0 2023-07-25 15:09:40.000000 iseqcbioportal-0.0.3/utils/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1000)     2360 2023-07-27 14:30:10.000000 iseqcbioportal-0.0.3/utils/utils.py
```

### Comparing `iseqcbioportal-0.0.2/.gitignore` & `iseqcbioportal-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.2/LICENSE` & `iseqcbioportal-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.2/PKG-INFO` & `iseqcbioportal-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iseqcbioportal
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for creating database from cBioPortal and annotating VCF with information from this database
 Home-page: https://gitlab.com/intelliseq/iseqcbioportal
 Author: Mateusz Marynowski
 Author-email: mateusz.marynowski@intelliseq.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iseqcbioportal-0.0.2/README.md` & `iseqcbioportal-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.2/cbioportal/create_cbioportal_database.py` & `iseqcbioportal-0.0.3/cbioportal/create_cbioportal_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 from utils import utils
 from typing import List
 from typing import Dict
 from tqdm import tqdm
 
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 def create_cbioportal_database(all_studies: List[Dict]):
     engine = utils.create_sqlite_engine("cbioportal.db")
     for study in tqdm(all_studies):
         studyId = {
             "studyIds": [
```

### Comparing `iseqcbioportal-0.0.2/cbioportal/test/create_cbioportal_database_test.py` & `iseqcbioportal-0.0.3/cbioportal/test/create_cbioportal_database_test.py`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.2/cbioportal/vcf_annotate_cbioportal.py` & `iseqcbioportal-0.0.3/cbioportal/vcf_annotate_cbioportal.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 import argparse
 import pandas as pd
 import sqlite3
 import pysam
 from utils import utils
 
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 def annotate_vcf(record: pysam.libcbcf.VariantRecord, vcf: pysam.VariantFile, studies: list, database: sqlite3.Connection):
-    gene_name = record.info.get("ISEQ_GENES_NAMES")[0]
-    cases_for_gene = 0
-    all_cases = 0
-    for study_id in studies:
-        df = pd.read_sql(f'''SELECT * FROM {study_id} 
-            WHERE hugoGeneSymbol LIKE "{gene_name}"''' , database)
-        if not df.empty:
-            cases_for_gene += int(df["numberOfAlteredCases"].tolist()[0])
-            all_cases += int(df["numberOfProfiledCases"].tolist()[0])
-    if cases_for_gene > 0:
-        frequency = round(int(cases_for_gene)/int(all_cases)*100, 1)
-        record.info["ISEQ_CBIOPORTAL_CASES"] = str(cases_for_gene)
-        record.info["ISEQ_CBIOPORTAL_FREQUENCY"] = str(frequency)
+    gene_name = record.info.get("ISEQ_GENES_NAMES")[0] if record.info.get("ISEQ_GENES_NAMES") else None
+    if gene_name:
+        cases_for_gene = 0
+        all_cases = 0
+        for study_id in studies:
+            df = pd.read_sql(f'''SELECT * FROM {study_id} 
+                WHERE hugoGeneSymbol LIKE "{gene_name}"''' , database)
+            if not df.empty:
+                cases_for_gene += int(df["numberOfAlteredCases"].tolist()[0])
+                all_cases += int(df["numberOfProfiledCases"].tolist()[0])
+        if cases_for_gene > 0:
+            frequency = round(int(cases_for_gene)/int(all_cases)*100, 1)
+            record.info["ISEQ_CBIOPORTAL_CASES"] = str(cases_for_gene)
+            record.info["ISEQ_CBIOPORTAL_FREQUENCY"] = str(frequency)
     vcf.write(record)          
 
 
 def main():
     parser = argparse.ArgumentParser(description='Annotate VCF with number of samples with one or more mutations \
                                      and percentage of samples with one or more mutations')
     parser.add_argument('-v', '--version', action='version', version='%(prog)s {}'.format(__version__))
```

### Comparing `iseqcbioportal-0.0.2/iseqcbioportal.egg-info/PKG-INFO` & `iseqcbioportal-0.0.3/iseqcbioportal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iseqcbioportal
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for creating database from cBioPortal and annotating VCF with information from this database
 Home-page: https://gitlab.com/intelliseq/iseqcbioportal
 Author: Mateusz Marynowski
 Author-email: mateusz.marynowski@intelliseq.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iseqcbioportal-0.0.2/iseqcbioportal.egg-info/SOURCES.txt` & `iseqcbioportal-0.0.3/iseqcbioportal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iseqcbioportal-0.0.2/setup.cfg` & `iseqcbioportal-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iseqcbioportal
-version = 0.0.2
+version = 0.0.3
 author = Mateusz Marynowski
 author_email = mateusz.marynowski@intelliseq.pl
 description = Package for creating database from cBioPortal and annotating VCF with information from this database
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/intelliseq/iseqcbioportal
 classifiers =
```

### Comparing `iseqcbioportal-0.0.2/utils/utils.py` & `iseqcbioportal-0.0.3/utils/utils.py`

 * *Files identical despite different names*

