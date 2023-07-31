# Comparing `tmp/sumt-3.2.4.tar.gz` & `tmp/sumt-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumt-3.2.4.tar", last modified: Mon Jul 31 08:46:44 2023, max compression
+gzip compressed data, was "sumt-3.2.5.tar", last modified: Mon Jul 31 09:22:29 2023, max compression
```

## Comparing `sumt-3.2.4.tar` & `sumt-3.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 08:46:44.404968 sumt-3.2.4/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.4/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)    20816 2023-07-31 08:46:44.405054 sumt-3.2.4/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)    20341 2023-07-31 08:44:47.000000 sumt-3.2.4/README.md
--rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.4/pyproject.toml
--rw-r--r--   0 agpe       (502) staff       (20)      650 2023-07-31 08:46:44.405363 sumt-3.2.4/setup.cfg
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 08:46:44.404864 sumt-3.2.4/sumt.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)    20816 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      220 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       35 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/entry_points.txt
--rw-r--r--   0 agpe       (502) staff       (20)       28 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)        5 2023-07-31 08:46:44.000000 sumt-3.2.4/sumt.egg-info/top_level.txt
--rwxr-xr-x   0 agpe       (502) staff       (20)    31927 2023-03-31 06:47:39.000000 sumt-3.2.4/sumt.py
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 09:22:29.719376 sumt-3.2.5/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.5/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-07-31 09:22:29.719806 sumt-3.2.5/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)    20838 2023-07-31 09:18:33.000000 sumt-3.2.5/README.md
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.5/pyproject.toml
+-rw-r--r--   0 agpe       (502) staff       (20)      650 2023-07-31 09:22:29.720859 sumt-3.2.5/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 09:22:29.718740 sumt-3.2.5/sumt.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      220 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       35 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/entry_points.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       28 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        5 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/top_level.txt
+-rwxr-xr-x   0 agpe       (502) staff       (20)    32428 2023-07-31 09:16:44.000000 sumt-3.2.5/sumt.py
```

### Comparing `sumt-3.2.4/LICENSE` & `sumt-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sumt-3.2.4/PKG-INFO` & `sumt-3.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,11 @@
-Metadata-Version: 2.1
-Name: sumt
-Version: 3.2.4
-Summary: Computes consensus trees and other phylogenetic tree summaries
-Home-page: https://github.com/agormp/sumt
-Author: Anders Gorm Pedersen
-Author-email: agpe@dtu.dk
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.4-blue)
-[![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/sumt)
+![](https://img.shields.io/badge/version-3.2.5-blue)
+[![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
 * Majority rule consensus tree, with all compatible bipartitions added
@@ -96,19 +82,24 @@
 
 options:
   -h, --help            show this help message and exit
 
 Type of summary tree:
   --con                 majority rule consensus tree [default]
   --all                 majority rule consensus tree with all compatible bipartitions added
-  --mbc                 Maximum Bipartition Credibility (MBC) tree. MBC is similar to MCC
-                        (Maximum Clade Credibility) tree but counting bipartitions instead
-                        of clades, i.e. ignoring rooting. Additionally, branch lengths are
-                        estimated from branch lengths of bipartitions and not from node
-                        depths (i.e., again ignoring rooting)
+  --mbc                 Maximum Bipartition Credibility (MBC) tree. The MBC is similar to
+                        the MCC (Maximum Clade Credibility) tree but counting bipartitions
+                        instead of clades, i.e. ignoring rooting. Specifically, the MBC tree
+                        is determined by inspecting tree samples and selecting the tree that
+                        has the highest sum of log of bipartition frequencies. Hence, the
+                        MBC tree is an actual observed tree from the pool of tree samples,
+                        differing from the consensus tree which typically does not match any
+                        individual sample. Furthermore, branch lengths are estimated from
+                        branch lengths of bipartitions and not from node depths (i.e., again
+                        ignoring rooting).
 
 Bayesian phylogeny options:
   -b NUM                burnin: fraction of trees to discard [0 - 1; default: 0.25]
   -t NUM                compute tree probabilities, report NUM percent credible interval [0
                         - 1]
   -s                    compute average standard deviation of split frequencies (ASDSF)
   -f NUM                Minimum frequency for including bipartitions in report and in
@@ -147,18 +138,18 @@
 #### Majority rule consensus tree, bipartition summary, topology summary, computation of average standard deviation of split frequencies, midpoint rooting
 
 The command below causes `sumt` to do the following:
 
 * `--con`: Compute majority rule consensus tree (this is default and could have been omitted)
 * `-b 0.25`: Discard 25% of tree samples as burn-in
 * `-t 0.99`: Keep track of topology probabilities, report 99% credible set
-* `-s`: Compute average standard deviation of split frequencies as a measure of MCMC convergence
-* `-f 0.1`: Report mean, variance, and standard error of the mean, for branch lengths for all bipartitions seen in more than 10% of input trees
+* `-s`: Compute average standard deviation of split frequencies as a measure of MCMC convergence (asdsf)
+* `-f 0.1`: Include bipartitions seen in more than 10% of input trees for computations of (1) asdsf and of (2) branch lengt mean, variance, and standard error of the mean
 * `--rootmid`: Perform midpoint rooting
-* `-i primates.nexus.run1.t -i primates.nexus.run2.t `: Summarise the tree samples in the files `hiv.nexus.run1.t` and `hiv.nexus.run2.t`
+* `-i primates.nexus.run1.t -i primates.nexus.run2.t `: Summarise the tree samples in the files `primates.nexus.run1.t` and `primates.nexus.run2.t`
 
 ```
 sumt --con -b 0.25 -t 0.99 -f 0.1 --rootmid -i primates.nexus.run1.t -i primates.nexus.run2.t 
 ```
 
 #### Screen output
```

### Comparing `sumt-3.2.4/README.md` & `sumt-3.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,25 @@
+Metadata-Version: 2.1
+Name: sumt
+Version: 3.2.5
+Summary: Computes consensus trees and other phylogenetic tree summaries
+Home-page: https://github.com/agormp/sumt
+Author: Anders Gorm Pedersen
+Author-email: agpe@dtu.dk
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.4-blue)
-[![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/sumt)
+![](https://img.shields.io/badge/version-3.2.5-blue)
+[![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
 * Majority rule consensus tree, with all compatible bipartitions added
@@ -82,19 +96,24 @@
 
 options:
   -h, --help            show this help message and exit
 
 Type of summary tree:
   --con                 majority rule consensus tree [default]
   --all                 majority rule consensus tree with all compatible bipartitions added
-  --mbc                 Maximum Bipartition Credibility (MBC) tree. MBC is similar to MCC
-                        (Maximum Clade Credibility) tree but counting bipartitions instead
-                        of clades, i.e. ignoring rooting. Additionally, branch lengths are
-                        estimated from branch lengths of bipartitions and not from node
-                        depths (i.e., again ignoring rooting)
+  --mbc                 Maximum Bipartition Credibility (MBC) tree. The MBC is similar to
+                        the MCC (Maximum Clade Credibility) tree but counting bipartitions
+                        instead of clades, i.e. ignoring rooting. Specifically, the MBC tree
+                        is determined by inspecting tree samples and selecting the tree that
+                        has the highest sum of log of bipartition frequencies. Hence, the
+                        MBC tree is an actual observed tree from the pool of tree samples,
+                        differing from the consensus tree which typically does not match any
+                        individual sample. Furthermore, branch lengths are estimated from
+                        branch lengths of bipartitions and not from node depths (i.e., again
+                        ignoring rooting).
 
 Bayesian phylogeny options:
   -b NUM                burnin: fraction of trees to discard [0 - 1; default: 0.25]
   -t NUM                compute tree probabilities, report NUM percent credible interval [0
                         - 1]
   -s                    compute average standard deviation of split frequencies (ASDSF)
   -f NUM                Minimum frequency for including bipartitions in report and in
@@ -133,18 +152,18 @@
 #### Majority rule consensus tree, bipartition summary, topology summary, computation of average standard deviation of split frequencies, midpoint rooting
 
 The command below causes `sumt` to do the following:
 
 * `--con`: Compute majority rule consensus tree (this is default and could have been omitted)
 * `-b 0.25`: Discard 25% of tree samples as burn-in
 * `-t 0.99`: Keep track of topology probabilities, report 99% credible set
-* `-s`: Compute average standard deviation of split frequencies as a measure of MCMC convergence
-* `-f 0.1`: Report mean, variance, and standard error of the mean, for branch lengths for all bipartitions seen in more than 10% of input trees
+* `-s`: Compute average standard deviation of split frequencies as a measure of MCMC convergence (asdsf)
+* `-f 0.1`: Include bipartitions seen in more than 10% of input trees for computations of (1) asdsf and of (2) branch lengt mean, variance, and standard error of the mean
 * `--rootmid`: Perform midpoint rooting
-* `-i primates.nexus.run1.t -i primates.nexus.run2.t `: Summarise the tree samples in the files `hiv.nexus.run1.t` and `hiv.nexus.run2.t`
+* `-i primates.nexus.run1.t -i primates.nexus.run2.t `: Summarise the tree samples in the files `primates.nexus.run1.t` and `primates.nexus.run2.t`
 
 ```
 sumt --con -b 0.25 -t 0.99 -f 0.1 --rootmid -i primates.nexus.run1.t -i primates.nexus.run2.t 
 ```
 
 #### Screen output
```

### Comparing `sumt-3.2.4/setup.cfg` & `sumt-3.2.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumt
-version = 3.2.4
+version = 3.2.5
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = Computes consensus trees and other phylogenetic tree summaries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/sumt
 classifiers =
```

### Comparing `sumt-3.2.4/sumt.egg-info/PKG-INFO` & `sumt-3.2.5/sumt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.2.4
+Version: 3.2.5
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
 
-![](https://img.shields.io/badge/version-3.2.4-blue)
-[![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=downloads&service=github)](https://pepy.tech/project/sumt)
+![](https://img.shields.io/badge/version-3.2.5-blue)
+[![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
 * Majority rule consensus tree, with all compatible bipartitions added
@@ -96,19 +96,24 @@
 
 options:
   -h, --help            show this help message and exit
 
 Type of summary tree:
   --con                 majority rule consensus tree [default]
   --all                 majority rule consensus tree with all compatible bipartitions added
-  --mbc                 Maximum Bipartition Credibility (MBC) tree. MBC is similar to MCC
-                        (Maximum Clade Credibility) tree but counting bipartitions instead
-                        of clades, i.e. ignoring rooting. Additionally, branch lengths are
-                        estimated from branch lengths of bipartitions and not from node
-                        depths (i.e., again ignoring rooting)
+  --mbc                 Maximum Bipartition Credibility (MBC) tree. The MBC is similar to
+                        the MCC (Maximum Clade Credibility) tree but counting bipartitions
+                        instead of clades, i.e. ignoring rooting. Specifically, the MBC tree
+                        is determined by inspecting tree samples and selecting the tree that
+                        has the highest sum of log of bipartition frequencies. Hence, the
+                        MBC tree is an actual observed tree from the pool of tree samples,
+                        differing from the consensus tree which typically does not match any
+                        individual sample. Furthermore, branch lengths are estimated from
+                        branch lengths of bipartitions and not from node depths (i.e., again
+                        ignoring rooting).
 
 Bayesian phylogeny options:
   -b NUM                burnin: fraction of trees to discard [0 - 1; default: 0.25]
   -t NUM                compute tree probabilities, report NUM percent credible interval [0
                         - 1]
   -s                    compute average standard deviation of split frequencies (ASDSF)
   -f NUM                Minimum frequency for including bipartitions in report and in
@@ -147,18 +152,18 @@
 #### Majority rule consensus tree, bipartition summary, topology summary, computation of average standard deviation of split frequencies, midpoint rooting
 
 The command below causes `sumt` to do the following:
 
 * `--con`: Compute majority rule consensus tree (this is default and could have been omitted)
 * `-b 0.25`: Discard 25% of tree samples as burn-in
 * `-t 0.99`: Keep track of topology probabilities, report 99% credible set
-* `-s`: Compute average standard deviation of split frequencies as a measure of MCMC convergence
-* `-f 0.1`: Report mean, variance, and standard error of the mean, for branch lengths for all bipartitions seen in more than 10% of input trees
+* `-s`: Compute average standard deviation of split frequencies as a measure of MCMC convergence (asdsf)
+* `-f 0.1`: Include bipartitions seen in more than 10% of input trees for computations of (1) asdsf and of (2) branch lengt mean, variance, and standard error of the mean
 * `--rootmid`: Perform midpoint rooting
-* `-i primates.nexus.run1.t -i primates.nexus.run2.t `: Summarise the tree samples in the files `hiv.nexus.run1.t` and `hiv.nexus.run2.t`
+* `-i primates.nexus.run1.t -i primates.nexus.run2.t `: Summarise the tree samples in the files `primates.nexus.run1.t` and `primates.nexus.run2.t`
 
 ```
 sumt --con -b 0.25 -t 0.99 -f 0.1 --rootmid -i primates.nexus.run1.t -i primates.nexus.run2.t 
 ```
 
 #### Screen output
```

### Comparing `sumt-3.2.4/sumt.py` & `sumt-3.2.5/sumt.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,18 +167,24 @@
                               help="majority rule consensus tree [default]")
 
     sumtypecommands.add_argument("--all", action="store_true",
                               help="majority rule consensus tree with all compatible bipartitions added")
 
     sumtypecommands.add_argument("--mbc", action="store_true",
                               help="Maximum Bipartition Credibility (MBC) tree. "
-                              + "MBC is similar to MCC (Maximum Clade Credibility) tree "
+                              + "The MBC is similar to the MCC (Maximum Clade Credibility) tree "
                               + "but counting bipartitions instead of clades, i.e. ignoring rooting. "
-                              + "Additionally, branch lengths are estimated from branch lengths of bipartitions "
-                              + "and not from node depths (i.e., again ignoring rooting)")
+                              + "Specifically, the MBC tree is "
+                              + "determined by inspecting tree samples and selecting the tree that has the "
+                              + "highest sum of log of bipartition frequencies. Hence, the MBC tree is an actual "
+                              + "observed tree from the pool of tree samples, differing from the consensus tree "
+                              + "which typically does not match any individual sample. "
+                              + "Furthermore, branch lengths are estimated from branch lengths of bipartitions "
+                              + "and not from node depths (i.e., again ignoring rooting).")
+
 
     ####################################################################################
 
     bayesgroup = parser.add_argument_group("Bayesian phylogeny options")
 
     bayesgroup.add_argument("-b", type=float, dest="burninfrac", metavar="NUM", default=0.25,
                       help="burnin: fraction of trees to discard [0 - 1; default: %(default)s]")
```

