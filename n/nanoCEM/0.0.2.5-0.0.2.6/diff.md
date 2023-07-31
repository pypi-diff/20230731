# Comparing `tmp/nanoCEM-0.0.2.5.tar.gz` & `tmp/nanoCEM-0.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.2.5.tar", last modified: Mon Jul 24 04:49:01 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.2.6.tar", last modified: Mon Jul 31 02:10:04 2023, max compression
```

## Comparing `nanoCEM-0.0.2.5.tar` & `nanoCEM-0.0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.5/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10233 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9650 2023-07-24 02:19:07.000000 nanoCEM-0.0.2.5/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10148 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.5/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.5/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.5/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8385 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.5/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.5/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.2.5/nanoCEM/extract_sub_fastq_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.5/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.5/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.5/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.5/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10233 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      458 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-24 04:49:01.000000 nanoCEM-0.0.2.5/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-24 04:49:01.183662 nanoCEM-0.0.2.5/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1192 2023-07-24 04:48:56.000000 nanoCEM-0.0.2.5/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-31 02:10:04.648263 nanoCEM-0.0.2.6/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.6/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10519 2023-07-31 02:10:04.648263 nanoCEM-0.0.2.6/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9936 2023-07-31 02:09:46.000000 nanoCEM-0.0.2.6/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-31 02:10:04.648263 nanoCEM-0.0.2.6/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10148 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.6/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.6/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.6/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8385 2023-07-21 02:50:56.000000 nanoCEM-0.0.2.6/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.6/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.2.6/nanoCEM/extract_sub_fastq_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.6/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.6/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.6/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.6/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-31 02:10:04.648263 nanoCEM-0.0.2.6/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10519 2023-07-31 02:10:04.000000 nanoCEM-0.0.2.6/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      458 2023-07-31 02:10:04.000000 nanoCEM-0.0.2.6/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-31 02:10:04.000000 nanoCEM-0.0.2.6/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-31 02:10:04.000000 nanoCEM-0.0.2.6/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-31 02:10:04.000000 nanoCEM-0.0.2.6/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-31 02:10:04.648263 nanoCEM-0.0.2.6/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1192 2023-07-31 02:10:03.000000 nanoCEM-0.0.2.6/setup.py
```

### Comparing `nanoCEM-0.0.2.5/LICENSE` & `nanoCEM-0.0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/PKG-INFO` & `nanoCEM-0.0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: nanoCEM
-Version: 0.0.2.5
-Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
-Home-page: https://github.com/lrslab/nanoCEM
-Author: GUO Zhihao
-Author-email: qhuozhihao@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 NanoCEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
@@ -69,15 +55,15 @@
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.2.4
+pip install nanoCEM==0.0.2.6
 ```
 
 Other tools if you needed
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
@@ -209,12 +195,16 @@
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 ```
+### 4 Result files
+
+Merged_violin.pdf and Merged_boxplot.pdf will be generated in the output folder if compared two groups, while will obtain Merged_single.pdf if applied single mode 
+And result table included all statistical feature called feature.csv will be added to the output file
```

### Comparing `nanoCEM-0.0.2.5/README.md` & `nanoCEM-0.0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: nanoCEM
+Version: 0.0.2.6
+Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
+Home-page: https://github.com/lrslab/nanoCEM
+Author: GUO Zhihao
+Author-email: qhuozhihao@icloud.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7,<3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 NanoCEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
@@ -55,15 +69,15 @@
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.2.4
+pip install nanoCEM==0.0.2.6
 ```
 
 Other tools if you needed
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
@@ -195,12 +209,16 @@
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 ```
+### 4 Result files
+
+Merged_violin.pdf and Merged_boxplot.pdf will be generated in the output folder if compared two groups, while will obtain Merged_single.pdf if applied single mode 
+And result table included all statistical feature called feature.csv will be added to the output file
```

### Comparing `nanoCEM-0.0.2.5/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.2.6/nanoCEM/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/cem_utils.py` & `nanoCEM-0.0.2.6/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.2.6/nanoCEM/current_events_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.2.6/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/extract_sub_fastq_from_bam` & `nanoCEM-0.0.2.6/nanoCEM/extract_sub_fastq_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/normalization.py` & `nanoCEM-0.0.2.6/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/plot.py` & `nanoCEM-0.0.2.6/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.2.6/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.2.6/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.5/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.2.6/nanoCEM.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.5
+Version: 0.0.2.6
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -69,15 +69,15 @@
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
 In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.2.4
+pip install nanoCEM==0.0.2.6
 ```
 
 Other tools if you needed
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
@@ -209,12 +209,16 @@
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
 current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 ```
+### 4 Result files
+
+Merged_violin.pdf and Merged_boxplot.pdf will be generated in the output folder if compared two groups, while will obtain Merged_single.pdf if applied single mode 
+And result table included all statistical feature called feature.csv will be added to the output file
```

### Comparing `nanoCEM-0.0.2.5/setup.py` & `nanoCEM-0.0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.2.5",
+    version="0.0.2.6",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

