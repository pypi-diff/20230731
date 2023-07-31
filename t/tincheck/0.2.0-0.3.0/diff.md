# Comparing `tmp/tincheck-0.2.0.tar.gz` & `tmp/tincheck-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tincheck-0.2.0.tar", last modified: Mon Jul 24 22:24:37 2023, max compression
+gzip compressed data, was "tincheck-0.3.0.tar", last modified: Mon Jul 31 03:37:59 2023, max compression
```

## Comparing `tincheck-0.2.0.tar` & `tincheck-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:24:37.484785 tincheck-0.2.0/
--rw-r--r--   0 asebastian   (501) staff       (20)     3797 2023-07-24 22:24:37.484411 tincheck-0.2.0/PKG-INFO
--rw-r--r--   0 asebastian   (501) staff       (20)     3406 2023-07-24 22:21:00.000000 tincheck-0.2.0/README.md
--rw-r--r--   0 asebastian   (501) staff       (20)       38 2023-07-24 22:24:37.484957 tincheck-0.2.0/setup.cfg
--rw-r--r--   0 asebastian   (501) staff       (20)      846 2023-07-24 21:20:53.000000 tincheck-0.2.0/setup.py
-drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:24:37.481673 tincheck-0.2.0/tincheck.egg-info/
--rw-r--r--   0 asebastian   (501) staff       (20)     3797 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/PKG-INFO
--rw-r--r--   0 asebastian   (501) staff       (20)      315 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/SOURCES.txt
--rw-r--r--   0 asebastian   (501) staff       (20)        1 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/dependency_links.txt
--rw-r--r--   0 asebastian   (501) staff       (20)       50 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/entry_points.txt
--rw-r--r--   0 asebastian   (501) staff       (20)        5 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/requires.txt
--rw-r--r--   0 asebastian   (501) staff       (20)        7 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/top_level.txt
-drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:24:37.483900 tincheck-0.2.0/tinrun/
--rw-r--r--   0 asebastian   (501) staff       (20)       37 2023-07-24 22:21:35.000000 tincheck-0.2.0/tinrun/__init__.py
--rw-r--r--   0 asebastian   (501) staff       (20)      248 2023-07-24 21:20:53.000000 tincheck-0.2.0/tinrun/__main__.py
--rw-r--r--   0 asebastian   (501) staff       (20)     2518 2023-07-24 21:28:42.000000 tincheck-0.2.0/tinrun/bam2gtf.py
--rw-r--r--   0 asebastian   (501) staff       (20)      995 2023-07-24 21:28:42.000000 tincheck-0.2.0/tinrun/main.py
--rw-r--r--   0 asebastian   (501) staff       (20)    27276 2023-07-24 21:47:58.000000 tincheck-0.2.0/tinrun/overlap.py
--rw-r--r--   0 asebastian   (501) staff       (20)    23448 2023-07-24 21:47:58.000000 tincheck-0.2.0/tinrun/tin.py
+drwxr-xr-x   0 aswathyseb   (501) staff       (20)        0 2023-07-31 03:37:59.021806 tincheck-0.3.0/
+-rw-r--r--   0 aswathyseb   (501) staff       (20)     4108 2023-07-31 03:37:59.020916 tincheck-0.3.0/PKG-INFO
+-rw-r--r--   0 aswathyseb   (501) staff       (20)     3717 2023-07-31 02:13:29.000000 tincheck-0.3.0/README.md
+-rw-r--r--   0 aswathyseb   (501) staff       (20)       38 2023-07-31 03:37:59.022050 tincheck-0.3.0/setup.cfg
+-rw-r--r--   0 aswathyseb   (501) staff       (20)      846 2023-07-31 02:13:29.000000 tincheck-0.3.0/setup.py
+drwxr-xr-x   0 aswathyseb   (501) staff       (20)        0 2023-07-31 03:37:59.010490 tincheck-0.3.0/tincheck.egg-info/
+-rw-r--r--   0 aswathyseb   (501) staff       (20)     4108 2023-07-31 03:37:58.000000 tincheck-0.3.0/tincheck.egg-info/PKG-INFO
+-rw-r--r--   0 aswathyseb   (501) staff       (20)      315 2023-07-31 03:37:58.000000 tincheck-0.3.0/tincheck.egg-info/SOURCES.txt
+-rw-r--r--   0 aswathyseb   (501) staff       (20)        1 2023-07-31 03:37:58.000000 tincheck-0.3.0/tincheck.egg-info/dependency_links.txt
+-rw-r--r--   0 aswathyseb   (501) staff       (20)       50 2023-07-31 03:37:58.000000 tincheck-0.3.0/tincheck.egg-info/entry_points.txt
+-rw-r--r--   0 aswathyseb   (501) staff       (20)        5 2023-07-31 03:37:58.000000 tincheck-0.3.0/tincheck.egg-info/requires.txt
+-rw-r--r--   0 aswathyseb   (501) staff       (20)        7 2023-07-31 03:37:58.000000 tincheck-0.3.0/tincheck.egg-info/top_level.txt
+drwxr-xr-x   0 aswathyseb   (501) staff       (20)        0 2023-07-31 03:37:59.019360 tincheck-0.3.0/tinrun/
+-rw-r--r--   0 aswathyseb   (501) staff       (20)       37 2023-07-31 03:35:15.000000 tincheck-0.3.0/tinrun/__init__.py
+-rw-r--r--   0 aswathyseb   (501) staff       (20)      248 2023-07-31 02:13:29.000000 tincheck-0.3.0/tinrun/__main__.py
+-rw-r--r--   0 aswathyseb   (501) staff       (20)     2518 2023-07-31 02:13:29.000000 tincheck-0.3.0/tinrun/bam2gtf.py
+-rw-r--r--   0 aswathyseb   (501) staff       (20)      995 2023-07-31 02:13:29.000000 tincheck-0.3.0/tinrun/main.py
+-rw-r--r--   0 aswathyseb   (501) staff       (20)    27276 2023-07-31 02:13:29.000000 tincheck-0.3.0/tinrun/overlap.py
+-rw-r--r--   0 aswathyseb   (501) staff       (20)    23475 2023-07-31 03:23:40.000000 tincheck-0.3.0/tinrun/tin.py
```

### Comparing `tincheck-0.2.0/PKG-INFO` & `tincheck-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,98 @@
 Metadata-Version: 2.1
 Name: tincheck
-Version: 0.2.0
+Version: 0.3.0
 Summary: tincheck
 Home-page: https://github.com/aswathyseb/tincheck
 Author: Aswathy Sebastian
 Author-email: aswathyseb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Tincheck
 
 Tincheck is a python package to calculate transcript Integrity Number (TIN) and Transcription overlap.
 
-Transcripts with transcription overlap or uneven coverage can result in false positives in differential expression analysis.
+Transcripts with uneven coverage or transcription overlap can result in false positives in differential expression analysis.
 Transcript Integrity Number is a metric that calculates coverage evenness and can be used as a filtering criteria in RNA-Seq studies to improve the accuracy of results.
 
+### Quick Start
 
-**Transcript Integrity Number (TIN)** calculation
-
-TIN denotes how evenly a feature is covered by reads. By default, the script calculate the coverage evenness across a 
-gene by considering the coverage across all exons. However, the script can calculate coverage evenness across a transcript or any other feature that is in the annotation file.
-
+Test data and annotation file is in `data` folder.
 
+**How to run**
+    
+    tincheck tin -a data/ann.gtf data/sample.bam
+    
 **Inputs**
+
 1. Alignment file in bam format
-2. Annotation file in GTFor GFF3 format
+2. Annotation file in GTF/GFF3 format
 
 **Output**
 
 Tab delimited textfile  with TIN score calculated for each gene/transcript/any other feature specified in the input.
 An example is given below.
 
-    target_id       eff_length  S1_count    S1_exp_tin  S1_obs_tin
+    target_id       eff_length  S1_count S1_exp_tin  S1_obs_tin
     PF3D7_0102700	1683	    670	        100.0	    70.9
     PF3D7_0103700	1624	    135	        100.0	    72.8
     PF3D7_0107300	1581	    4508        100.0	    70.4
     PF3D7_0107600	5702	    4979        100.0	    74.9
     PF3D7_0107800	4424	    924	        100.0	    78.8
 
 
 **How to install the script?**
-    
+
+Step1: Install script
+
     pip install tincheck --upgrade
 
-Install additional requirements
+Step2 :Install additional requirements
     
     conda install --file conda-requirements.txt
 
-**How to run the script?**
+### Additional details
 
-The required inputs to the script is bam file(s) and annotation file in GTF or GFF format.
- 
+
+TIN denotes how evenly a feature is covered by reads. By default, the script calculate the coverage evenness across a 
+gene by considering the coverage across all exons. However, the script can calculate coverage evenness across a transcript or any other feature that is in the annotation file.
 The annotation file should have a gene feature row present in it.
 
-Given a bam file and an annotation file, the simplest way to run the script is
+**How to calculate tin for each gene?**
+
+    tincheck tin --a data/ann.gtf data/sample.bam 
+
+**How to calculate tin for each transcript?**
+
+    tincheck tin -g transcript_id -a data/ann.gtf data/sample.bam 
+
+Here -g option should be the transcript grouping attribute present in the annotation file. 
 
-    tincheck tin --ann data/ann.gtf data/sample.bam 
 
 **How to calculate TIN across coding regions of a gene?**
     
-    tincheck tin  --ann data/ann.gtf --feat CDS data/sample.bam
+    tincheck tin -f CDS -a data/ann.gtf data/sample.bam
 
+
+**How to calculate TIN across coding regions of a transcript?**
     
+    tincheck tin -f CDS -g transcript_id -a data/ann.gtf data/sample.bam
+
+
 **How is tin calculated**
 
 Overlapping features specified by `--feat` are merged together and coverage evenness is captured using Shannon's entropy formula  (H).
-This is then convered into TIN Score as
 
-    TIN = (100*exp(H))⁄length  where H= Shannon's entropy formula.
+This is then converted into TIN score as
 
+    TIN = (100*exp(H))⁄length  where H= Shannon's entropy formula.
 
 **Transcription overlaps**
 
 Transcription overlaps are flagged using `overlap.py` script.
 
 	tincheck overlap --ann data/ann.gtf data/sample.bam >sample_overlap.txt
 
@@ -89,11 +106,10 @@
 
 In stranded mode, if the count and tin values of neighboring genes and the intergenic region in the gene sense strand is 
 comparable to the gene count and tin, then that gene is considered to have an overlap from neighboring transcripts.
 
 
 More specifically in stranded mode, a gene is considered to have a neighboring transcript overlap, if **either of** the following conditions are satisfied.
 
-    
     1. left gene tin in gene sense strand >= gene tin and left intergenic tin in gene sense strand >=gene-tin
     2. right gene tin in gene sense strand >= gene tin and right intergenic tin in gene sense strand >=gene-tin
```

### Comparing `tincheck-0.2.0/README.md` & `tincheck-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,85 @@
 # Tincheck
 
 Tincheck is a python package to calculate transcript Integrity Number (TIN) and Transcription overlap.
 
-Transcripts with transcription overlap or uneven coverage can result in false positives in differential expression analysis.
+Transcripts with uneven coverage or transcription overlap can result in false positives in differential expression analysis.
 Transcript Integrity Number is a metric that calculates coverage evenness and can be used as a filtering criteria in RNA-Seq studies to improve the accuracy of results.
 
+### Quick Start
 
-**Transcript Integrity Number (TIN)** calculation
-
-TIN denotes how evenly a feature is covered by reads. By default, the script calculate the coverage evenness across a 
-gene by considering the coverage across all exons. However, the script can calculate coverage evenness across a transcript or any other feature that is in the annotation file.
-
+Test data and annotation file is in `data` folder.
 
+**How to run**
+    
+    tincheck tin -a data/ann.gtf data/sample.bam
+    
 **Inputs**
+
 1. Alignment file in bam format
-2. Annotation file in GTFor GFF3 format
+2. Annotation file in GTF/GFF3 format
 
 **Output**
 
 Tab delimited textfile  with TIN score calculated for each gene/transcript/any other feature specified in the input.
 An example is given below.
 
-    target_id       eff_length  S1_count    S1_exp_tin  S1_obs_tin
+    target_id       eff_length  S1_count S1_exp_tin  S1_obs_tin
     PF3D7_0102700	1683	    670	        100.0	    70.9
     PF3D7_0103700	1624	    135	        100.0	    72.8
     PF3D7_0107300	1581	    4508        100.0	    70.4
     PF3D7_0107600	5702	    4979        100.0	    74.9
     PF3D7_0107800	4424	    924	        100.0	    78.8
 
 
 **How to install the script?**
-    
+
+Step1: Install script
+
     pip install tincheck --upgrade
 
-Install additional requirements
+Step2 :Install additional requirements
     
     conda install --file conda-requirements.txt
 
-**How to run the script?**
+### Additional details
 
-The required inputs to the script is bam file(s) and annotation file in GTF or GFF format.
- 
+
+TIN denotes how evenly a feature is covered by reads. By default, the script calculate the coverage evenness across a 
+gene by considering the coverage across all exons. However, the script can calculate coverage evenness across a transcript or any other feature that is in the annotation file.
 The annotation file should have a gene feature row present in it.
 
-Given a bam file and an annotation file, the simplest way to run the script is
+**How to calculate tin for each gene?**
+
+    tincheck tin --a data/ann.gtf data/sample.bam 
+
+**How to calculate tin for each transcript?**
+
+    tincheck tin -g transcript_id -a data/ann.gtf data/sample.bam 
+
+Here -g option should be the transcript grouping attribute present in the annotation file. 
 
-    tincheck tin --ann data/ann.gtf data/sample.bam 
 
 **How to calculate TIN across coding regions of a gene?**
     
-    tincheck tin  --ann data/ann.gtf --feat CDS data/sample.bam
+    tincheck tin -f CDS -a data/ann.gtf data/sample.bam
 
+
+**How to calculate TIN across coding regions of a transcript?**
     
+    tincheck tin -f CDS -g transcript_id -a data/ann.gtf data/sample.bam
+
+
 **How is tin calculated**
 
 Overlapping features specified by `--feat` are merged together and coverage evenness is captured using Shannon's entropy formula  (H).
-This is then convered into TIN Score as
 
-    TIN = (100*exp(H))⁄length  where H= Shannon's entropy formula.
+This is then converted into TIN score as
 
+    TIN = (100*exp(H))⁄length  where H= Shannon's entropy formula.
 
 **Transcription overlaps**
 
 Transcription overlaps are flagged using `overlap.py` script.
 
 	tincheck overlap --ann data/ann.gtf data/sample.bam >sample_overlap.txt
 
@@ -76,11 +93,10 @@
 
 In stranded mode, if the count and tin values of neighboring genes and the intergenic region in the gene sense strand is 
 comparable to the gene count and tin, then that gene is considered to have an overlap from neighboring transcripts.
 
 
 More specifically in stranded mode, a gene is considered to have a neighboring transcript overlap, if **either of** the following conditions are satisfied.
 
-    
     1. left gene tin in gene sense strand >= gene tin and left intergenic tin in gene sense strand >=gene-tin
     2. right gene tin in gene sense strand >= gene tin and right intergenic tin in gene sense strand >=gene-tin
```

### Comparing `tincheck-0.2.0/setup.py` & `tincheck-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.2.0/tincheck.egg-info/PKG-INFO` & `tincheck-0.3.0/tincheck.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,98 @@
 Metadata-Version: 2.1
 Name: tincheck
-Version: 0.2.0
+Version: 0.3.0
 Summary: tincheck
 Home-page: https://github.com/aswathyseb/tincheck
 Author: Aswathy Sebastian
 Author-email: aswathyseb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Tincheck
 
 Tincheck is a python package to calculate transcript Integrity Number (TIN) and Transcription overlap.
 
-Transcripts with transcription overlap or uneven coverage can result in false positives in differential expression analysis.
+Transcripts with uneven coverage or transcription overlap can result in false positives in differential expression analysis.
 Transcript Integrity Number is a metric that calculates coverage evenness and can be used as a filtering criteria in RNA-Seq studies to improve the accuracy of results.
 
+### Quick Start
 
-**Transcript Integrity Number (TIN)** calculation
-
-TIN denotes how evenly a feature is covered by reads. By default, the script calculate the coverage evenness across a 
-gene by considering the coverage across all exons. However, the script can calculate coverage evenness across a transcript or any other feature that is in the annotation file.
-
+Test data and annotation file is in `data` folder.
 
+**How to run**
+    
+    tincheck tin -a data/ann.gtf data/sample.bam
+    
 **Inputs**
+
 1. Alignment file in bam format
-2. Annotation file in GTFor GFF3 format
+2. Annotation file in GTF/GFF3 format
 
 **Output**
 
 Tab delimited textfile  with TIN score calculated for each gene/transcript/any other feature specified in the input.
 An example is given below.
 
-    target_id       eff_length  S1_count    S1_exp_tin  S1_obs_tin
+    target_id       eff_length  S1_count S1_exp_tin  S1_obs_tin
     PF3D7_0102700	1683	    670	        100.0	    70.9
     PF3D7_0103700	1624	    135	        100.0	    72.8
     PF3D7_0107300	1581	    4508        100.0	    70.4
     PF3D7_0107600	5702	    4979        100.0	    74.9
     PF3D7_0107800	4424	    924	        100.0	    78.8
 
 
 **How to install the script?**
-    
+
+Step1: Install script
+
     pip install tincheck --upgrade
 
-Install additional requirements
+Step2 :Install additional requirements
     
     conda install --file conda-requirements.txt
 
-**How to run the script?**
+### Additional details
 
-The required inputs to the script is bam file(s) and annotation file in GTF or GFF format.
- 
+
+TIN denotes how evenly a feature is covered by reads. By default, the script calculate the coverage evenness across a 
+gene by considering the coverage across all exons. However, the script can calculate coverage evenness across a transcript or any other feature that is in the annotation file.
 The annotation file should have a gene feature row present in it.
 
-Given a bam file and an annotation file, the simplest way to run the script is
+**How to calculate tin for each gene?**
+
+    tincheck tin --a data/ann.gtf data/sample.bam 
+
+**How to calculate tin for each transcript?**
+
+    tincheck tin -g transcript_id -a data/ann.gtf data/sample.bam 
+
+Here -g option should be the transcript grouping attribute present in the annotation file. 
 
-    tincheck tin --ann data/ann.gtf data/sample.bam 
 
 **How to calculate TIN across coding regions of a gene?**
     
-    tincheck tin  --ann data/ann.gtf --feat CDS data/sample.bam
+    tincheck tin -f CDS -a data/ann.gtf data/sample.bam
 
+
+**How to calculate TIN across coding regions of a transcript?**
     
+    tincheck tin -f CDS -g transcript_id -a data/ann.gtf data/sample.bam
+
+
 **How is tin calculated**
 
 Overlapping features specified by `--feat` are merged together and coverage evenness is captured using Shannon's entropy formula  (H).
-This is then convered into TIN Score as
 
-    TIN = (100*exp(H))⁄length  where H= Shannon's entropy formula.
+This is then converted into TIN score as
 
+    TIN = (100*exp(H))⁄length  where H= Shannon's entropy formula.
 
 **Transcription overlaps**
 
 Transcription overlaps are flagged using `overlap.py` script.
 
 	tincheck overlap --ann data/ann.gtf data/sample.bam >sample_overlap.txt
 
@@ -89,11 +106,10 @@
 
 In stranded mode, if the count and tin values of neighboring genes and the intergenic region in the gene sense strand is 
 comparable to the gene count and tin, then that gene is considered to have an overlap from neighboring transcripts.
 
 
 More specifically in stranded mode, a gene is considered to have a neighboring transcript overlap, if **either of** the following conditions are satisfied.
 
-    
     1. left gene tin in gene sense strand >= gene tin and left intergenic tin in gene sense strand >=gene-tin
     2. right gene tin in gene sense strand >= gene tin and right intergenic tin in gene sense strand >=gene-tin
```

### Comparing `tincheck-0.2.0/tinrun/bam2gtf.py` & `tincheck-0.3.0/tinrun/bam2gtf.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.2.0/tinrun/main.py` & `tincheck-0.3.0/tinrun/main.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.2.0/tinrun/overlap.py` & `tincheck-0.3.0/tinrun/overlap.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.2.0/tinrun/tin.py` & `tincheck-0.3.0/tinrun/tin.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,26 +81,26 @@
     """
 
     countsfile = f"counts_{flag}.txt" if len(bam.split(' ')) > 1 else get_filename(bam) + "_counts.txt"
     countsfile = countsfile.replace("_counts.txt", f'_{flag}_counts.txt') if flag else countsfile
     countsfile = os.path.join(TMP, countsfile)
 
     # Set paired end or single end.
-    pflag = '-p' if paired else ""
+    pflag = '-p --countReadPairs' if paired else ""
 
     group_attr = "gene_id" if feat == "intergenic" else groupby
 
     # Set strandedness.
     if strand == "unstranded":
         sflag = ""
     else:
         sflag = '-s 2' if strand == "sense" else '-s 1'
 
     # Make the command.
-    cmd = f'featureCounts --primary -M {pflag} {sflag} -t {feat} -O -g {group_attr} -a {ann} -o {countsfile} {bam} 2>>{log}'
+    cmd = f'featureCounts --primary -O -M {pflag} {sflag} -t {feat}  -g {group_attr} -a {ann} -o {countsfile} {bam} 2>>{log}'
 
     # print(cmd)
 
     # Run command and get counts.
     out = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True,
                          universal_newlines=True)
 
@@ -404,15 +404,15 @@
     suffix1 = "depth.txt"
     outfile = get_filename(bam)
     suffix = f"_{flag}_{suffix1}" if flag else f"_{suffix1}"
     outfile = outfile.replace("_primary", "") + suffix
     outfile = os.path.join(TMP, outfile)
 
     # Command to get the depth.
-    cmd2 = f'bedtools coverage -d -a {bed} -b {bam} {lib_strand} | cut -f 4,8 > {outfile}'
+    cmd2 = f'bedtools coverage -split -d -a {bed} -b {bam} {lib_strand} | cut -f 4,8 > {outfile}'
     # print(cmd2)
 
     d = subprocess.run(cmd2, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True,
                        universal_newlines=True)
     # Exit on error.
     exit_on_error(d.stderr) if d.stderr and d.returncode != 0 else None
 
@@ -455,20 +455,22 @@
 
         # The very first time
         if not curr:
             curr = uid
 
         if uid != curr:
             fid, tlen, bg, obs_tin, exp_tin = calculate_tin(coverages=covs, background=background, uid=curr, size=size)
+
             store[fid] = (tlen, bg, obs_tin, exp_tin)
             curr = uid
             covs = dict()
 
         covs.setdefault(uid, []).append(depth)
 
+
     # Print the last element
     fid, tlen, bg, obs_tin, exp_tin = calculate_tin(coverages=covs, background=background, uid=uid, size=size)
 
     store[fid] = (tlen, bg, obs_tin, exp_tin)
 
     return store
 
@@ -531,15 +533,15 @@
     cvg = list(map(float, cvg))
 
     # Remove zeros
     cvg = list(filter(None, cvg))
 
     if not cvg:
         tin = 0.0
-        return tin, eff_len, 0
+        return tin, 0, eff_len
 
     # Calculate shannon's entropy
     ent = shannon_entropy(cvg)
 
     # Calculate uniformity
     uni = math.exp(ent)
```

