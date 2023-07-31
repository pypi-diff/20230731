# Comparing `tmp/kdpeak-0.1.1.tar.gz` & `tmp/kdpeak-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdpeak-0.1.1.tar", last modified: Mon Jul 31 17:27:12 2023, max compression
+gzip compressed data, was "kdpeak-0.2.0.tar", last modified: Mon Jul 31 18:42:45 2023, max compression
```

## Comparing `kdpeak-0.1.1.tar` & `kdpeak-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-07-31 17:27:12.807110 kdpeak-0.1.1/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    35148 2022-09-23 00:29:04.000000 kdpeak-0.1.1/LICENSE
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3253 2023-07-31 17:27:12.805925 kdpeak-0.1.1/PKG-INFO
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2616 2023-07-31 17:07:21.000000 kdpeak-0.1.1/README.md
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-07-31 17:27:12.778631 kdpeak-0.1.1/kdpeak/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      112 2023-07-29 02:26:33.000000 kdpeak-0.1.1/kdpeak/__init__.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3930 2023-07-29 02:50:15.000000 kdpeak-0.1.1/kdpeak/core.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12117 2023-07-31 17:26:03.000000 kdpeak-0.1.1/kdpeak/util.py
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-07-31 17:27:12.801889 kdpeak-0.1.1/kdpeak.egg-info/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3253 2023-07-31 17:27:12.000000 kdpeak-0.1.1/kdpeak.egg-info/PKG-INFO
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      257 2023-07-31 17:27:12.000000 kdpeak-0.1.1/kdpeak.egg-info/SOURCES.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2023-07-31 17:27:12.000000 kdpeak-0.1.1/kdpeak.egg-info/dependency_links.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       44 2023-07-31 17:27:12.000000 kdpeak-0.1.1/kdpeak.egg-info/entry_points.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       41 2023-07-31 17:27:12.000000 kdpeak-0.1.1/kdpeak.egg-info/requires.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        7 2023-07-31 17:27:12.000000 kdpeak-0.1.1/kdpeak.egg-info/top_level.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2023-07-31 17:27:12.808067 kdpeak-0.1.1/setup.cfg
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1126 2023-07-31 17:26:43.000000 kdpeak-0.1.1/setup.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-07-31 18:42:45.774363 kdpeak-0.2.0/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    35148 2022-09-23 00:29:04.000000 kdpeak-0.2.0/LICENSE
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3705 2023-07-31 18:42:45.773051 kdpeak-0.2.0/PKG-INFO
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3068 2023-07-31 18:40:53.000000 kdpeak-0.2.0/README.md
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-07-31 18:42:45.746457 kdpeak-0.2.0/kdpeak/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      112 2023-07-29 02:26:33.000000 kdpeak-0.2.0/kdpeak/__init__.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     4795 2023-07-31 18:38:44.000000 kdpeak-0.2.0/kdpeak/core.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    12039 2023-07-31 18:32:40.000000 kdpeak-0.2.0/kdpeak/util.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-07-31 18:42:45.769086 kdpeak-0.2.0/kdpeak.egg-info/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3705 2023-07-31 18:42:45.000000 kdpeak-0.2.0/kdpeak.egg-info/PKG-INFO
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      257 2023-07-31 18:42:45.000000 kdpeak-0.2.0/kdpeak.egg-info/SOURCES.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2023-07-31 18:42:45.000000 kdpeak-0.2.0/kdpeak.egg-info/dependency_links.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       44 2023-07-31 18:42:45.000000 kdpeak-0.2.0/kdpeak.egg-info/entry_points.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       41 2023-07-31 18:42:45.000000 kdpeak-0.2.0/kdpeak.egg-info/requires.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        7 2023-07-31 18:42:45.000000 kdpeak-0.2.0/kdpeak.egg-info/top_level.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2023-07-31 18:42:45.775580 kdpeak-0.2.0/setup.cfg
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1126 2023-07-31 18:38:17.000000 kdpeak-0.2.0/setup.py
```

### Comparing `kdpeak-0.1.1/LICENSE` & `kdpeak-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kdpeak-0.1.1/PKG-INFO` & `kdpeak-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdpeak
-Version: 0.1.1
+Version: 0.2.0
 Summary: A tool to identify genomic peaks based on kernel density estimation.
 Home-page: https://github.com/settylab/kdpeak
 Author: Dominik Otto
 Author-email: dotto@fredhutch.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -55,15 +55,22 @@
 **Positional Argument:**
 
 - `reads.bed` - Path to the bed file containing the genomic reads.
 
 **Options:**
 
 - `-h, --help` - Show this help message and exit.
-- `--out OUTPUT_FILE` - Path to the output file to save the results. Default is ./peaks.bed.
+- `--out output_file.bed` - Path to the output file where the results will be saved.
+  Peaks are saved in bed format with the columns:
+  start, end, peak name, AUC (area under the cut density curve
+  where cut-density is in cuts per 100 base pairs). Defaults to peaks.bed.
+- `--summits-out summits_file.bed` - Path to the output file where the peak summits will be saved.
+  The file will have columns for start, end (start+1),
+  peak name, and summit height (in cuts per 100 base pairs).
+  If nothing is specified the summits will not be saved.
 - `-l LEVEL, --log LEVEL` - Set the logging level. Options include: DEBUG, INFO, WARNING, ERROR, CRITICAL. Default is INFO.
 - `--logfile LOGFILE` - Path to the file to write a detailed log.
 - `--blacklisted-seqs chrN [chrN ...]` - List of sequences (e.g., chromosomes) to exclude from peak calling. Input as space-separated values.
 - `--kde-bw FLOAT` - Bandwidth (standard deviation, sigma in base pairs) for the KDE. Increase for larger features to reduce noise. Default is 200.
 - `--min-peak-size INT` - Minimal size (in base pairs) for a peak to be considered valid. Default is 100.
 - `--fraction-in-peaks FLOAT, --frip FLOAT` - Expected fraction of total reads to be located in peaks. Default is 0.3.
 - `--span INT` - Resolution of the analysis in base pairs, determining the granularity of the KDE and peak calling. Default is 10.
```

### Comparing `kdpeak-0.1.1/README.md` & `kdpeak-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 **Positional Argument:**
 
 - `reads.bed` - Path to the bed file containing the genomic reads.
 
 **Options:**
 
 - `-h, --help` - Show this help message and exit.
-- `--out OUTPUT_FILE` - Path to the output file to save the results. Default is ./peaks.bed.
+- `--out output_file.bed` - Path to the output file where the results will be saved.
+  Peaks are saved in bed format with the columns:
+  start, end, peak name, AUC (area under the cut density curve
+  where cut-density is in cuts per 100 base pairs). Defaults to peaks.bed.
+- `--summits-out summits_file.bed` - Path to the output file where the peak summits will be saved.
+  The file will have columns for start, end (start+1),
+  peak name, and summit height (in cuts per 100 base pairs).
+  If nothing is specified the summits will not be saved.
 - `-l LEVEL, --log LEVEL` - Set the logging level. Options include: DEBUG, INFO, WARNING, ERROR, CRITICAL. Default is INFO.
 - `--logfile LOGFILE` - Path to the file to write a detailed log.
 - `--blacklisted-seqs chrN [chrN ...]` - List of sequences (e.g., chromosomes) to exclude from peak calling. Input as space-separated values.
 - `--kde-bw FLOAT` - Bandwidth (standard deviation, sigma in base pairs) for the KDE. Increase for larger features to reduce noise. Default is 200.
 - `--min-peak-size INT` - Minimal size (in base pairs) for a peak to be considered valid. Default is 100.
 - `--fraction-in-peaks FLOAT, --frip FLOAT` - Expected fraction of total reads to be located in peaks. Default is 0.3.
 - `--span INT` - Resolution of the analysis in base pairs, determining the granularity of the KDE and peak calling. Default is 10.
```

### Comparing `kdpeak-0.1.1/kdpeak/core.py` & `kdpeak-0.2.0/kdpeak/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,18 +39,31 @@
         metavar="reads.bed",
         type=str,
         help="Path to the bed file containing the genomic reads.",
     )
 
     parser.add_argument(
         "--out",
-        metavar="output_file",
+        metavar="output_file.bed",
         type=str,
         default="./peaks.bed",
-        help="Path to the output file where the results will be saved. Defaults to ./peaks.bed.",
+        help="""Path to the output file where the results will be saved. \
+            Peaks are saved in bed format with the columns: \
+            start, end, peak name, AUC (area under the cut density curve \
+            where cut-density is in cuts per 100 base pairs). Defaults to peaks.bed.""",
+    )
+
+    parser.add_argument(
+        "--summits-out",
+        metavar="summits_file.bed",
+        type=str,
+        help="""Path to the output file where the peak summits will be saved.\
+        The file will have columns for start, end (start+1), \
+        peak name, and summit height (in cuts per 100 base pairs). \
+        If nothing is specified the summits will not be saved.""",
     )
 
     parser.add_argument(
         "-l",
         "--log",
         dest="logLevel",
         choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
@@ -140,12 +153,18 @@
     )
 
     bed = include_auc(name_peaks(peaks))
 
     out_file = args.out
     logger.info("Writing results to %s...", out_file)
     write_bed(bed[["seqname", "start", "end", "name", "auc"]], out_file)
+    
+    if out_file := args.summits_out:
+        logger.info("Writing summits to %s...", out_file)
+        bed["start"] = bed["summit"]
+        bed["end"] = bed["summit"]+1
+        write_bed(bed[["seqname", "start", "end", "name", "summit_height"]], out_file)
+        
     logger.info("Finished successfully.")
 
-
 if __name__ == "__main__":
     main()
```

### Comparing `kdpeak-0.1.1/kdpeak/util.py` & `kdpeak-0.2.0/kdpeak/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
         low_res_cuts = np.round(cuts / step)
 
         grid = full_kde_grid(low_res_cuts)
         cut_idx = (low_res_cuts - grid.min()).astype(int)
 
         _, density = get_kde(low_res_cuts, kde_bw=kde_bw, grid=grid)
-        density *= len(events)
+        density *= len(events) * 100
 
         comb_df = pd.DataFrame(
             {
                 "seqname": seqname,
                 "interval": seqname,
                 "location": grid * step,
                 "density": density,
@@ -280,53 +280,47 @@
     msg = f"{fraction_selected:.2%} of genome covered by peaks."
     logger.info(msg)
 
     return comb_data
 
 
 def track_to_interval(job):
-    """
-    Converts track data to interval representation.
-
-    Parameters
-    ----------
-    job : tuple
-        A tuple containing the combined data, step size, and sequence name.
-
-    Returns
-    -------
-    peaks : pd.DataFrame
-        DataFrame with peak intervals.
-    """
     loc_comb_data, step_size, seqname = job
 
     idx = np.insert(loc_comb_data["peak"].values.astype(int), 0, 0)
     indicator = np.diff(idx)
     loc_comb_data["peak_number"] = np.cumsum(indicator == 1)
     loc_comb_data["peak_name"] = (
         loc_comb_data["interval"]
         + "_"
         + loc_comb_data["peak_number"].astype(str)
         + "_"
         + loc_comb_data["peak"].astype(str)
     )
 
-    peak_location_df = loc_comb_data[loc_comb_data["peak"].values].set_index("location")
-    locations = peak_location_df.groupby("peak_name")["density"].idxmax()
+    peak_indices = loc_comb_data["peak"].values
+    peak_location_df = loc_comb_data.loc[peak_indices].set_index("location")
+
+    summit_locations = peak_location_df.groupby("peak_name")["density"].idxmax()
+    summit_heights = peak_location_df.loc[summit_locations, "density"]
+
     peak_groups = peak_location_df.reset_index().groupby("peak_name")
+
     start = peak_groups["location"].min().values - (step_size / 2)
     end = peak_groups["location"].max().values + (step_size / 2)
     means = peak_groups["density"].mean()
+
     peaks = pd.DataFrame(
         {
             "seqname": seqname,
             "start": start.astype(int),
             "end": end.astype(int),
             "mean": means,
-            "summit": locations,
+            "summit": summit_locations.values.astype(int),
+            "summit_height": summit_heights.values,
         }
     ).sort_values("start")
     return peaks
 
 
 def tracks_to_intervals(comb_data, step_size):
     """
```

### Comparing `kdpeak-0.1.1/kdpeak.egg-info/PKG-INFO` & `kdpeak-0.2.0/kdpeak.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdpeak
-Version: 0.1.1
+Version: 0.2.0
 Summary: A tool to identify genomic peaks based on kernel density estimation.
 Home-page: https://github.com/settylab/kdpeak
 Author: Dominik Otto
 Author-email: dotto@fredhutch.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -55,15 +55,22 @@
 **Positional Argument:**
 
 - `reads.bed` - Path to the bed file containing the genomic reads.
 
 **Options:**
 
 - `-h, --help` - Show this help message and exit.
-- `--out OUTPUT_FILE` - Path to the output file to save the results. Default is ./peaks.bed.
+- `--out output_file.bed` - Path to the output file where the results will be saved.
+  Peaks are saved in bed format with the columns:
+  start, end, peak name, AUC (area under the cut density curve
+  where cut-density is in cuts per 100 base pairs). Defaults to peaks.bed.
+- `--summits-out summits_file.bed` - Path to the output file where the peak summits will be saved.
+  The file will have columns for start, end (start+1),
+  peak name, and summit height (in cuts per 100 base pairs).
+  If nothing is specified the summits will not be saved.
 - `-l LEVEL, --log LEVEL` - Set the logging level. Options include: DEBUG, INFO, WARNING, ERROR, CRITICAL. Default is INFO.
 - `--logfile LOGFILE` - Path to the file to write a detailed log.
 - `--blacklisted-seqs chrN [chrN ...]` - List of sequences (e.g., chromosomes) to exclude from peak calling. Input as space-separated values.
 - `--kde-bw FLOAT` - Bandwidth (standard deviation, sigma in base pairs) for the KDE. Increase for larger features to reduce noise. Default is 200.
 - `--min-peak-size INT` - Minimal size (in base pairs) for a peak to be considered valid. Default is 100.
 - `--fraction-in-peaks FLOAT, --frip FLOAT` - Expected fraction of total reads to be located in peaks. Default is 0.3.
 - `--span INT` - Resolution of the analysis in base pairs, determining the granularity of the KDE and peak calling. Default is 10.
```

### Comparing `kdpeak-0.1.1/setup.py` & `kdpeak-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 
 setup(
     name="kdpeak",
-    version="0.1.1",
+    version="0.2.0",
     author="Dominik Otto",
     author_email="dotto@fredhutch.org",
     description="A tool to identify genomic peaks based on kernel density estimation.",
     long_description=(this_directory / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/settylab/kdpeak",
     packages=find_packages(),
```

