# Comparing `tmp/varvamp-0.9.tar.gz` & `tmp/varvamp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.9.tar", last modified: Mon Jul 24 13:43:17 2023, max compression
+gzip compressed data, was "varvamp-0.9.1.tar", last modified: Mon Jul 31 14:23:15 2023, max compression
```

## Comparing `varvamp-0.9.tar` & `varvamp-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.838111 varvamp-0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-24 13:43:17.838111 varvamp-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-24 13:42:54.000000 varvamp-0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:43:17.838111 varvamp-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 13:42:54.000000 varvamp-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.834111 varvamp-0.9/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.838111 varvamp-0.9/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/blast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-07-24 13:42:54.000000 varvamp-0.9/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:43:17.834111 varvamp-0.9/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 13:43:17.000000 varvamp-0.9/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.420872 varvamp-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-31 14:23:15.420872 varvamp-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-31 14:22:55.000000 varvamp-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:23:15.420872 varvamp-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-31 14:22:55.000000 varvamp-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.412872 varvamp-0.9.1/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.420872 varvamp-0.9.1/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/blast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.416872 varvamp-0.9.1/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.9/PKG-INFO` & `varvamp-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.9
+Version: 0.9.1
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-0.9/README.md` & `varvamp-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/setup.py` & `varvamp-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/command.py` & `varvamp-0.9.1/varvamp/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 main workflow
 """
 
 # BUILT-INS
 import sys
 import os
-import time
+import datetime
 import argparse
 
 # varVAMP
 from varvamp.scripts import alignment
 from varvamp.scripts import config
 from varvamp.scripts import consensus
 from varvamp.scripts import regions
@@ -460,15 +460,15 @@
     main varvamp workflow
     """
 
     # start varVAMP
     args = get_args(sysargs)
     if not args.verbose:
         sys.stdout = open(os.devnull, 'w')
-    start_time = time.process_time()
+    start_time = datetime.datetime.now()
     results_dir, data_dir, log_file = logging.create_dir_structure(args.input[1])
     # check if blast is installed
     if args.mode == "tiled" or args.mode == "sanger":
         if args.database is not None:
             blast.check_BLAST_installation(log_file)
 
     # mode unspecific part of the workflow
@@ -546,7 +546,8 @@
             probe_regions=probe_regions,
             amplicon_scheme=final_schemes
         )
         reporting.per_base_mismatch_plot(results_dir, final_schemes, args.threshold, mode="QPCR")
 
     # varVAMP finished
     logging.varvamp_progress(log_file, progress=1, start_time=start_time)
+    logging.goodbye_message()
```

### Comparing `varvamp-0.9/varvamp/scripts/alignment.py` & `varvamp-0.9.1/varvamp/scripts/alignment.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/scripts/blast.py` & `varvamp-0.9.1/varvamp/scripts/blast.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,20 +72,21 @@
                "ref",
                "query_len",
                "aln_len",
                "mismatch",
                "gaps",
                "ref_start",
                "ref_end",
+               "strand"
                ]
 
     blast_df = pd.read_table(blast_out, names=columns)
     blast_df = blast_df[
-        blast_df["query_len"] - blast_df["aln_len"] + blast_df["mismatch"] + blast_df["gaps"] <= round(
-            blast_df["query_len"] * config.BLAST_MAX_DIFF)
+        blast_df["query_len"] - blast_df["aln_len"] + blast_df["mismatch"] + blast_df["gaps"] <=
+        blast_df["query_len"]-(round(blast_df["query_len"] * config.BLAST_MAX_DIFF))
         ]
     # removes tabular output
     os.remove(blast_out)
 
     return(blast_df)
 
 
@@ -97,44 +98,52 @@
     off_target_amp = []
 
     for amp in amplicons:
         fw_primer = amplicons[amp][2]
         rw_primer = amplicons[amp][3]
         # subset df for primers
         df_amp_primers = blast_df[blast_df["query"].isin([fw_primer, rw_primer])]
-        # sort by reference and ref start (so one can easily iterate over rows)
+        # sort by reference and ref start
         df_amp_primers_sorted = df_amp_primers.sort_values(["ref", "ref_start"])
         # iterate over ref for each primer pair
         for ref in set(df_amp_primers_sorted["ref"]):
             df_ref_subset = df_amp_primers_sorted[df_amp_primers_sorted["ref"] == ref]
-            # reindex to remember the correct index
+            # reindex to remember the correct index later on
             df_ref_subset.reset_index(inplace=True, drop=True)
             # ini the primer search
             indices = []  # remember the index of the subset df
             start = -float("inf")
             off_target = False
-            for i, row in df_ref_subset.iterrows():
+            for row in df_ref_subset.itertuples():
                 # for the current row check if start of the current batch is close enough
-                if row[7] - start <= config.BLAST_SIZE_MULTI * max_length:
-                    indices.append(i)
+                if row[8] - start <= config.BLAST_SIZE_MULTI * max_length:
+                    indices.append(row[0])
                 else:
                     # reset start to the next element in the index list if list has more than
                     # one element
                     if len(indices) > 1:
                         indices.pop(0)
                         start = df_ref_subset.iloc[indices[0]]["ref_start"]
                     # else reset to the current row and empty index list
                     else:
-                        start = row[6]
+                        start = row[7]
                         indices = []
-                # do we need to check the current index list?
-                if len(indices) <= 1:
+                # check if in the df subset is more than one primer
+                if len(set(df_ref_subset.iloc[indices]["query"])) <= 1:
                     continue
-                # check if in the df subset is more than one query
-                if len(set(df_ref_subset.iloc[indices]["query"])) > 1:
+                # subset of df with potential off-targets
+                possible_off_targets = df_ref_subset.iloc[indices]
+                # check if fw and rw primers bind in different directions
+                direction_fw = set(possible_off_targets[possible_off_targets["query"] == fw_primer]["strand"])
+                direction_rw = set(possible_off_targets[possible_off_targets["query"] == rw_primer]["strand"])
+                # do we have one primer in subset that binds both directions or are the
+                # direction sets different? --> 2 different primers bind on the same chrom,
+                # are close enough and are in opposite direction ->[seq]<-
+                # >this classifies as an off-target<
+                if len(direction_fw) > 1 or len(direction_rw) > 1 or direction_fw != direction_rw:
                     off_target = True
                     break
             if off_target:
                 amplicons[amp][5] = amplicons[amp][5] + config.BLAST_PENALTY
                 off_target_amp.append(amp)
                 break
```

### Comparing `varvamp-0.9/varvamp/scripts/config.py` & `varvamp-0.9.1/varvamp/scripts/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,22 @@
 PRIMER_3_PENALTY = (32, 16, 8, 4, 2)  # penalties for 3' mismatches
 PRIMER_PERMUTATION_PENALTY = 0.1  # penalty for the number of permutations
 
 # BLAST parameters (ref: PrimerBLAST (YE, Jian, et al. Primer-BLAST: a tool to design
 # target-specific primers for polymerase chain reaction. BMC bioinformatics, 2012, 13.
 # Jg., S. 1-11.)
 BLAST_SETTINGS = {  # blast settings for query search
-    "outfmt": "6 qseqid sseqid qlen length mismatch gapopen sstart send",  # do NOT change
+    "outfmt": "6 qseqid sseqid qlen length mismatch gapopen sstart send sstrand",  # do NOT change
     "evalue": 5000,
     "reward": 1,
     "penalty": -1,
     "gapopen": 2,
     "gapextend": 1
 }
-BLAST_MAX_DIFF = 0.8  # allowed % differences between primer and BLAST hit
+BLAST_MAX_DIFF = 0.7  # allowed % differences between primer and BLAST hit
 BLAST_SIZE_MULTI = 2  # multiplier for the max_amp size of off targets (in relation to max amp size)
 BLAST_PENALTY = 50  # amplicon score increase -> considered only if no other possibilities
 
 # nucleotide definitions, do NOT change
 NUCS = set("atcg")
 AMBIG_NUCS = {
     "r": ["a", "g"],
```

### Comparing `varvamp-0.9/varvamp/scripts/consensus.py` & `varvamp-0.9.1/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/scripts/logging.py` & `varvamp-0.9.1/varvamp/scripts/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 varVAMP logging and raising errors
 """
 
 # BUILT-INS
 import sys
 import os
 import shutil
-import time
 import datetime
+import random
 
 # varVAMP
 from varvamp.scripts import config
 from varvamp import __version__
 
 
 def create_dir_structure(dir):
@@ -46,16 +46,16 @@
             "\nStarting \033[31m\033[1mvarVAMP ◥(ºwº)◤\033[0m primer design\n",
             flush=True
         )
         with open(log_file, 'w') as f:
             print(f"VARVAMP log \n\nMODE = {mode}\n", file=f)
     else:
         if progress == 1:
-            stop_time = str(round(time.process_time() - start_time, 2))
-            progress_text = f"all done \n\n\rvarVAMP {__version__} finished in {stop_time} sec!\n{datetime.datetime.now()}"
+            stop_time = datetime.datetime.now() - start_time
+            progress_text = f"all done \n\n\rvarVAMP {__version__} finished in {stop_time.total_seconds()} sec!\n{datetime.datetime.now()}"
             job = "Finalizing output."
         print(
             "\rJob:\t\t " + job + "\nProgress: \t [{0}] {1}%".format("█"*block + "-"*(barLength-block), progress*100) + "\t" + progress_text,
             flush=True
         )
         with open(log_file, 'a') as f:
             print(
@@ -409,15 +409,15 @@
     # confirm proper BLAST settings in dictionary
     if not isinstance(config.BLAST_SETTINGS, dict):
         raise_error(
             "BLAST settings have to be in a dictionary format!",
             log_file,
             exit=True
         )
-    if config.BLAST_SETTINGS["outfmt"] != "6 qseqid sseqid qlen length mismatch gapopen sstart send":
+    if config.BLAST_SETTINGS["outfmt"] != "6 qseqid sseqid qlen length mismatch gapopen sstart send sstrand":
         raise_error(
             "output format (outfmt) of BLAST settings is not correct",
             log_file,
             exit=True
         )
 
     # check all dict values
@@ -492,7 +492,32 @@
             if args.database is not None:
                 for var in all_vars[2]:
                     print(f"{var} = {var_dic[var]}", file=f)
         if args.mode == "qpcr":
             for var in all_vars[1]:
                 print(f"{var} = {var_dic[var]}", file=f)
         print("\nPROGRESS", file=f)
+
+def goodbye_message():
+    """
+    This is what happens when I am bored...
+    """
+
+    messages = [
+        "Thank you. Come again.",
+        ">Placeholder for your advertisement<",
+        "Make primers great again!",
+        "And now lets pray to the PCR gods.",
+        "**bibobibobop** task finished",
+        "Thank you for traveling with varVAMP.",
+        "This message will self-destruct in 0 seconds.... PUFF!",
+        "What? Already finished? Errr I mean, thanks for using varVAMP!",
+        "One primer design to rule them all.",
+        "42",
+        "Hope to see you again!",
+        "Wohooooo everything worked somehow!",
+        "Reminder: Get yourself a cup of coffee!",
+        "Barba non facit philosophum.",
+        "Task failed successfully.",
+        "Never gonna give you up, never gonna let you down.",
+    ]
+    print(f"\n{random.choice(messages)}")
```

### Comparing `varvamp-0.9/varvamp/scripts/param_estimation.py` & `varvamp-0.9.1/varvamp/scripts/param_estimation.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/scripts/primers.py` & `varvamp-0.9.1/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/scripts/qpcr.py` & `varvamp-0.9.1/varvamp/scripts/qpcr.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/scripts/regions.py` & `varvamp-0.9.1/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/scripts/reporting.py` & `varvamp-0.9.1/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp/scripts/scheme.py` & `varvamp-0.9.1/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9/varvamp.egg-info/PKG-INFO` & `varvamp-0.9.1/varvamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.9
+Version: 0.9.1
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
```

### Comparing `varvamp-0.9/varvamp.egg-info/SOURCES.txt` & `varvamp-0.9.1/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

