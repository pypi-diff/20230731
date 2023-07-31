# Comparing `tmp/sumt-3.2.3.tar.gz` & `tmp/sumt-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumt-3.2.3.tar", last modified: Fri Mar 31 06:49:39 2023, max compression
+gzip compressed data, was "sumt-3.2.4.tar", last modified: Mon Jul 31 08:46:44 2023, max compression
```

## Comparing `sumt-3.2.3.tar` & `sumt-3.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-03-31 06:49:39.707934 sumt-3.2.3/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.3/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)    20742 2023-03-31 06:49:39.708015 sumt-3.2.3/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)    20267 2023-03-31 06:48:06.000000 sumt-3.2.3/README.md
--rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.3/pyproject.toml
--rw-r--r--   0 agpe       (502) staff       (20)      650 2023-03-31 06:49:39.708312 sumt-3.2.3/setup.cfg
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-03-31 06:49:39.707827 sumt-3.2.3/sumt.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)    20742 2023-03-31 06:49:39.000000 sumt-3.2.3/sumt.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      220 2023-03-31 06:49:39.000000 sumt-3.2.3/sumt.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2023-03-31 06:49:39.000000 sumt-3.2.3/sumt.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       35 2023-03-31 06:49:39.000000 sumt-3.2.3/sumt.egg-info/entry_points.txt
--rw-r--r--   0 agpe       (502) staff       (20)       28 2023-03-31 06:49:39.000000 sumt-3.2.3/sumt.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)        5 2023-03-31 06:49:39.000000 sumt-3.2.3/sumt.egg-info/top_level.txt
--rwxr-xr-x   0 agpe       (502) staff       (20)    31927 2023-03-31 06:47:39.000000 sumt-3.2.3/sumt.py
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 08:46:44.404968 sumt-3.2.4/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.4/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)    20816 2023-07-31 08:46:44.405054 sumt-3.2.4/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)    20341 2023-07-31 08:44:47.000000 sumt-3.2.4/README.md
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.4/pyproject.toml
+-rw-r--r--   0 agpe       (502) staff       (20)      650 2023-07-31 08:46:44.405363 sumt-3.2.4/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 08:46:44.404864 sumt-3.2.4/sumt.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)    20816 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      220 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       35 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/entry_points.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       28 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        5 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/top_level.txt
+-rwxr-xr-x   0 agpe       (502) staff       (20)    31927 2023-03-31 06:47:39.000000 sumt-3.2.4/sumt.py
```

### Comparing `sumt-3.2.3/LICENSE` & `sumt-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sumt-3.2.3/PKG-INFO` & `sumt-3.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.2.3
+Version: 3.2.4
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.3-blue)
+![](https://img.shields.io/badge/version-3.2.4-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
@@ -84,62 +84,65 @@
 	* Indication of whether summary tree has been explicitly rooted
 	* Log bipartition credibility (sum of logs of bipartition frequencies in summary tree)
 	* Report of maximum memory usage during processing
 
 ## Usage
 
 ```
-usage: sumt    [-h] [--con | --all | --mbc] [-b NUM] [-t NUM] [-s] [-f NUM] [-n] [-v] [-q]
-               [--basename NAME] [--rootmid | --rootminvar | -r TAXON [TAXON ...] | --rootfile
-               FILE] [-w WEIGHT INFILE] [--autow] [-i FORMAT]
-               [INFILE ...]
+usage: sumt [-h] [--con | --all | --mbc] [-b NUM] [-t NUM] [-s] [-f NUM] [-n] [-v] [-q]
+            [--basename NAME] [--rootmid | --rootminvar | -r TAXON [TAXON ...] | --rootfile
+            FILE] [--autow] [--informat FORMAT] [-i FILE | -w WEIGHT FILE]
 
 Computes summary tree and statistics from set of phylogenetic trees
 
 options:
   -h, --help            show this help message and exit
 
 Type of summary tree:
   --con                 majority rule consensus tree [default]
   --all                 majority rule consensus tree with all compatible bipartitions added
   --mbc                 Maximum Bipartition Credibility (MBC) tree. MBC is similar to MCC
-                        (Maximum Clade Credibility) tree but counting bipartitions instead of
-                        clades, i.e. ignoring rooting. Additionally, branch lengths are
-                        estimated from branch lengths of bipartitions and not from node depths
-                        (i.e., again ignoring rooting)
+                        (Maximum Clade Credibility) tree but counting bipartitions instead
+                        of clades, i.e. ignoring rooting. Additionally, branch lengths are
+                        estimated from branch lengths of bipartitions and not from node
+                        depths (i.e., again ignoring rooting)
 
 Bayesian phylogeny options:
   -b NUM                burnin: fraction of trees to discard [0 - 1; default: 0.25]
-  -t NUM                compute tree probabilities, report NUM percent credible interval [0 -
-                        1]
+  -t NUM                compute tree probabilities, report NUM percent credible interval [0
+                        - 1]
   -s                    compute average standard deviation of split frequencies (ASDSF)
   -f NUM                Minimum frequency for including bipartitions in report and in
                         computation of ASDSF [default: 0.1]
 
 Output to terminal and files:
   -n                    no warning when overwriting files
   -v                    verbose: more information, longer error messages
-  -q                    quiet: don't print progress indication to terminal window. NOTE: also
-                        turns on the -n option
+  -q                    quiet: don't print progress indication to terminal window. NOTE:
+                        also turns on the -n option
   --basename NAME       base name of output files (default: derived from input file)
 
 Rooting of summary tree:
   --rootmid             perform midpoint rooting of tree
   --rootminvar          perform minimum variance rooting of tree
   -r TAXON [TAXON ...]  root consensus tree on specified outgroup taxon/taxa
-  --rootfile FILE       root consensus tree on outgroup taxa listed in file (one name per line)
+  --rootfile FILE       root consensus tree on outgroup taxa listed in file (one name per
+                        line)
 
-Input tree files:
-  INFILE                input FILE(s) containing phylogenetic trees (can list several files)
-  -w WEIGHT INFILE      input FILEs with specified weights (repeat -w option for each input
-                        file)
+Other options:
   --autow               automatically assign file weights based on tree counts, so all files
-                        have equal impact (default is for all trees, not files, to be equally
-                        important)
-  -i FORMAT             format of input files: nexus, newick [default: nexus]
+                        have equal impact (default is for all trees, not files, to be
+                        equally important)
+  --informat FORMAT     format of input files: nexus, newick [default: nexus]
+
+Input tree files:
+  -i FILE               input FILE(s) containing phylogenetic trees (repeat -i FILE option
+                        for each input file)
+  -w WEIGHT FILE        input FILEs with specified weights (repeat -w WEIGHT FILE option for
+                        each input file)
 ```
 
 ## Usage examples
 
 ### Example 1: 
 #### Majority rule consensus tree, bipartition summary, topology summary, computation of average standard deviation of split frequencies, midpoint rooting
```

### Comparing `sumt-3.2.3/README.md` & `sumt-3.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.3-blue)
+![](https://img.shields.io/badge/version-3.2.4-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
@@ -70,62 +70,65 @@
 	* Indication of whether summary tree has been explicitly rooted
 	* Log bipartition credibility (sum of logs of bipartition frequencies in summary tree)
 	* Report of maximum memory usage during processing
 
 ## Usage
 
 ```
-usage: sumt    [-h] [--con | --all | --mbc] [-b NUM] [-t NUM] [-s] [-f NUM] [-n] [-v] [-q]
-               [--basename NAME] [--rootmid | --rootminvar | -r TAXON [TAXON ...] | --rootfile
-               FILE] [-w WEIGHT INFILE] [--autow] [-i FORMAT]
-               [INFILE ...]
+usage: sumt [-h] [--con | --all | --mbc] [-b NUM] [-t NUM] [-s] [-f NUM] [-n] [-v] [-q]
+            [--basename NAME] [--rootmid | --rootminvar | -r TAXON [TAXON ...] | --rootfile
+            FILE] [--autow] [--informat FORMAT] [-i FILE | -w WEIGHT FILE]
 
 Computes summary tree and statistics from set of phylogenetic trees
 
 options:
   -h, --help            show this help message and exit
 
 Type of summary tree:
   --con                 majority rule consensus tree [default]
   --all                 majority rule consensus tree with all compatible bipartitions added
   --mbc                 Maximum Bipartition Credibility (MBC) tree. MBC is similar to MCC
-                        (Maximum Clade Credibility) tree but counting bipartitions instead of
-                        clades, i.e. ignoring rooting. Additionally, branch lengths are
-                        estimated from branch lengths of bipartitions and not from node depths
-                        (i.e., again ignoring rooting)
+                        (Maximum Clade Credibility) tree but counting bipartitions instead
+                        of clades, i.e. ignoring rooting. Additionally, branch lengths are
+                        estimated from branch lengths of bipartitions and not from node
+                        depths (i.e., again ignoring rooting)
 
 Bayesian phylogeny options:
   -b NUM                burnin: fraction of trees to discard [0 - 1; default: 0.25]
-  -t NUM                compute tree probabilities, report NUM percent credible interval [0 -
-                        1]
+  -t NUM                compute tree probabilities, report NUM percent credible interval [0
+                        - 1]
   -s                    compute average standard deviation of split frequencies (ASDSF)
   -f NUM                Minimum frequency for including bipartitions in report and in
                         computation of ASDSF [default: 0.1]
 
 Output to terminal and files:
   -n                    no warning when overwriting files
   -v                    verbose: more information, longer error messages
-  -q                    quiet: don't print progress indication to terminal window. NOTE: also
-                        turns on the -n option
+  -q                    quiet: don't print progress indication to terminal window. NOTE:
+                        also turns on the -n option
   --basename NAME       base name of output files (default: derived from input file)
 
 Rooting of summary tree:
   --rootmid             perform midpoint rooting of tree
   --rootminvar          perform minimum variance rooting of tree
   -r TAXON [TAXON ...]  root consensus tree on specified outgroup taxon/taxa
-  --rootfile FILE       root consensus tree on outgroup taxa listed in file (one name per line)
+  --rootfile FILE       root consensus tree on outgroup taxa listed in file (one name per
+                        line)
 
-Input tree files:
-  INFILE                input FILE(s) containing phylogenetic trees (can list several files)
-  -w WEIGHT INFILE      input FILEs with specified weights (repeat -w option for each input
-                        file)
+Other options:
   --autow               automatically assign file weights based on tree counts, so all files
-                        have equal impact (default is for all trees, not files, to be equally
-                        important)
-  -i FORMAT             format of input files: nexus, newick [default: nexus]
+                        have equal impact (default is for all trees, not files, to be
+                        equally important)
+  --informat FORMAT     format of input files: nexus, newick [default: nexus]
+
+Input tree files:
+  -i FILE               input FILE(s) containing phylogenetic trees (repeat -i FILE option
+                        for each input file)
+  -w WEIGHT FILE        input FILEs with specified weights (repeat -w WEIGHT FILE option for
+                        each input file)
 ```
 
 ## Usage examples
 
 ### Example 1: 
 #### Majority rule consensus tree, bipartition summary, topology summary, computation of average standard deviation of split frequencies, midpoint rooting
```

### Comparing `sumt-3.2.3/setup.cfg` & `sumt-3.2.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumt
-version = 3.2.3
+version = 3.2.4
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = Computes consensus trees and other phylogenetic tree summaries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/sumt
 classifiers =
```

### Comparing `sumt-3.2.3/sumt.egg-info/PKG-INFO` & `sumt-3.2.4/sumt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.2.3
+Version: 3.2.4
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.3-blue)
+![](https://img.shields.io/badge/version-3.2.4-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
@@ -84,62 +84,65 @@
 	* Indication of whether summary tree has been explicitly rooted
 	* Log bipartition credibility (sum of logs of bipartition frequencies in summary tree)
 	* Report of maximum memory usage during processing
 
 ## Usage
 
 ```
-usage: sumt    [-h] [--con | --all | --mbc] [-b NUM] [-t NUM] [-s] [-f NUM] [-n] [-v] [-q]
-               [--basename NAME] [--rootmid | --rootminvar | -r TAXON [TAXON ...] | --rootfile
-               FILE] [-w WEIGHT INFILE] [--autow] [-i FORMAT]
-               [INFILE ...]
+usage: sumt [-h] [--con | --all | --mbc] [-b NUM] [-t NUM] [-s] [-f NUM] [-n] [-v] [-q]
+            [--basename NAME] [--rootmid | --rootminvar | -r TAXON [TAXON ...] | --rootfile
+            FILE] [--autow] [--informat FORMAT] [-i FILE | -w WEIGHT FILE]
 
 Computes summary tree and statistics from set of phylogenetic trees
 
 options:
   -h, --help            show this help message and exit
 
 Type of summary tree:
   --con                 majority rule consensus tree [default]
   --all                 majority rule consensus tree with all compatible bipartitions added
   --mbc                 Maximum Bipartition Credibility (MBC) tree. MBC is similar to MCC
-                        (Maximum Clade Credibility) tree but counting bipartitions instead of
-                        clades, i.e. ignoring rooting. Additionally, branch lengths are
-                        estimated from branch lengths of bipartitions and not from node depths
-                        (i.e., again ignoring rooting)
+                        (Maximum Clade Credibility) tree but counting bipartitions instead
+                        of clades, i.e. ignoring rooting. Additionally, branch lengths are
+                        estimated from branch lengths of bipartitions and not from node
+                        depths (i.e., again ignoring rooting)
 
 Bayesian phylogeny options:
   -b NUM                burnin: fraction of trees to discard [0 - 1; default: 0.25]
-  -t NUM                compute tree probabilities, report NUM percent credible interval [0 -
-                        1]
+  -t NUM                compute tree probabilities, report NUM percent credible interval [0
+                        - 1]
   -s                    compute average standard deviation of split frequencies (ASDSF)
   -f NUM                Minimum frequency for including bipartitions in report and in
                         computation of ASDSF [default: 0.1]
 
 Output to terminal and files:
   -n                    no warning when overwriting files
   -v                    verbose: more information, longer error messages
-  -q                    quiet: don't print progress indication to terminal window. NOTE: also
-                        turns on the -n option
+  -q                    quiet: don't print progress indication to terminal window. NOTE:
+                        also turns on the -n option
   --basename NAME       base name of output files (default: derived from input file)
 
 Rooting of summary tree:
   --rootmid             perform midpoint rooting of tree
   --rootminvar          perform minimum variance rooting of tree
   -r TAXON [TAXON ...]  root consensus tree on specified outgroup taxon/taxa
-  --rootfile FILE       root consensus tree on outgroup taxa listed in file (one name per line)
+  --rootfile FILE       root consensus tree on outgroup taxa listed in file (one name per
+                        line)
 
-Input tree files:
-  INFILE                input FILE(s) containing phylogenetic trees (can list several files)
-  -w WEIGHT INFILE      input FILEs with specified weights (repeat -w option for each input
-                        file)
+Other options:
   --autow               automatically assign file weights based on tree counts, so all files
-                        have equal impact (default is for all trees, not files, to be equally
-                        important)
-  -i FORMAT             format of input files: nexus, newick [default: nexus]
+                        have equal impact (default is for all trees, not files, to be
+                        equally important)
+  --informat FORMAT     format of input files: nexus, newick [default: nexus]
+
+Input tree files:
+  -i FILE               input FILE(s) containing phylogenetic trees (repeat -i FILE option
+                        for each input file)
+  -w WEIGHT FILE        input FILEs with specified weights (repeat -w WEIGHT FILE option for
+                        each input file)
 ```
 
 ## Usage examples
 
 ### Example 1: 
 #### Majority rule consensus tree, bipartition summary, topology summary, computation of average standard deviation of split frequencies, midpoint rooting
```

### Comparing `sumt-3.2.3/sumt.py` & `sumt-3.2.4/sumt.py`

 * *Files identical despite different names*

