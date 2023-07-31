# Comparing `tmp/jamofetch-3.7.3.tar.gz` & `tmp/jamofetch-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamofetch-3.7.3.tar", max compression
+gzip compressed data, was "jamofetch-3.7.5.tar", max compression
```

## Comparing `jamofetch-3.7.3.tar` & `jamofetch-3.7.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4675 2023-07-27 23:09:54.226061 jamofetch-3.7.3/README.md
--rw-r--r--   0        0        0      522 2023-07-30 20:28:25.297045 jamofetch-3.7.3/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-27 23:09:54.227061 jamofetch-3.7.3/src/jamofetch/__init__.py
--rwxr-xr-x   0        0        0    10931 2023-07-30 20:05:03.823308 jamofetch-3.7.3/src/jamofetch/jamofetch.py
--rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.7.3/PKG-INFO
+-rw-r--r--   0        0        0     4666 2023-07-31 16:50:12.396721 jamofetch-3.7.5/README.md
+-rw-r--r--   0        0        0      522 2023-07-31 16:51:27.673295 jamofetch-3.7.5/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-27 23:09:54.227061 jamofetch-3.7.5/src/jamofetch/__init__.py
+-rwxr-xr-x   0        0        0    10922 2023-07-31 16:50:12.397721 jamofetch-3.7.5/src/jamofetch/jamofetch.py
+-rw-r--r--   0        0        0     5195 1970-01-01 00:00:00.000000 jamofetch-3.7.5/PKG-INFO
```

### Comparing `jamofetch-3.7.3/README.md` & `jamofetch-3.7.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 ```
 
 ## Usage
 See script **docs/demo_script.py** in the project for a sample script.
 
 Create a JamoFetcher:
 ```pthon
-from jamofetch.jamofetch import JamoFetcher, JamoLibSeq
+from jamofetch.jamofetch import JamoFetcher, LibSeq
 
 WAIT_INTERVAL = 10  # check if JAMO has provisioned sequence every 10 seconds
 WAIT_MAX = 7200     # max wait for sequence is 7200 seconds or 2 hours
 
 # directory where JAMO will link sequence, will be created if it doesn't exist
 link_dir = '/tmp/sequence-links'
 
 # create a fetcher
 fetcher: JamoFetcher = JamoFetcher(link_dir=link_dir, wait_interval_secs=WAIT_INTERVAL, wait_max_secs=WAIT_MAX)
 ```
 
-Note the following default configuration parameters for JamoLibSeq.
+Note the following default configuration parameters for LibSeq.
 Setting wait_max_secs to -1 causes the JamoFetcher instance to wait indefenitely for
 JAMO sequence.
 ```python
 class JamoFetcher():
     def __init__(self, link_dir='.', wait_interval_secs=10, wait_max_secs=-1):
 ```
 
 Fetch sequence for a library, print path of symlink to sequence file and the real path
 to the file.
 ```python
 LIBRARY = 'NPUNN'
 # Call JAMO to link sequence in the background.  Symlinks to the sequence
 # files are created by JAMO in the directory specified by the
 # link_dir parameter supplied to the JamoFetcher constructor.
-lib_seq: JamoLibSeq = fetcher.fetch_lib_seq(LIBRARY)
+lib_seq: LibSeq = fetcher.fetch_lib_seq(LIBRARY)
 
 printf(f"library name: {lib_seq.get_lib_name()}")
 print(f"sequence symlink: {lib_seq.get_seq_path()}")
 print(f"sequence real path: {lib_seq.get_real_path()}")
 ```
 
 Check if sequence has been provided by JAMO, i.e. the symlink is not broken.  Wait
@@ -60,24 +60,24 @@
 ```
 ## Command Line Tool
 Installing jamofetch with pip exposes a command line interface.
 ```
 (venv) [dnscott@ln004 jamofetch]$ jamofetch  -h
 usage: jamofetch [-h] [-l LIBRARY] [-d DIRECTORY] [-i INTERVAL] [-m MAX] [-w] [--logging LOGGING]
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -l LIBRARY, --library LIBRARY
                         library name(s) for which to retrieve sequence
   -d DIRECTORY, --directory DIRECTORY
                         directory where to link sequence, defaults to current directory. Directory will be created if it doesn't exit.
   -i INTERVAL, --interval INTERVAL
                         wait interval in seconds to check if sequence has been fetched, ignored if wait flag not set
   -m MAX, --max MAX     maximum time to wait for sequence in seconds, ignored if wait flag not set. Specify -1 to wait indefinetely.
-  -w, --wait            wait for jamo to link sequence, output real path of linked sequence
+  -w, --wait            wait for jamo to link sequence, then print "sequence ready"
   --logging LOGGING     logging level (specify DEBUG for verbose logging)
 (venv) [dnscott@ln004 jamofetch]$ jamofetch -d data -l NPUNN -l NOOHG -l HOGH -w --max -1
 fetching sequence:
 NPUNN /global/dna/dm_archive/sdm/pacbio/00/27/47/pbio-2747.27352.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz BACKUP_COMPLETE 6391936239a7711d789a9380
 NOOHG /global/dna/dm_archive/sdm/pacbio/00/26/91/pbio-2691.26653.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz RESTORED 6347dbb35bc59487d7e768d6
 HOGH /global/dna/dm_archive/sdm/illumina/00/63/97/6397.2.44053.GGCTAC.fastq.gz RESTORE_IN_PROGRESS 51d52a82067c014cd6ef4f6f
```

### Comparing `jamofetch-3.7.3/pyproject.toml` & `jamofetch-3.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jamofetch"
-version = "3.7.3"
+version = "3.7.5"
 description = "A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori."
 authors = ["Duncan Scott"]
 license = "None"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `jamofetch-3.7.3/src/jamofetch/jamofetch.py` & `jamofetch-3.7.5/src/jamofetch/jamofetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from argparse import ArgumentParser
 from stat import ST_CTIME
 
 JAMO_CMD_NERSC = 'module load jamo; jamo link library'
 JAMO_CMD_DORI = 'apptainer --silent run docker://doejgi/jamo-dori jamo link -s dori library'
 
 TWO_HOURS = 7200  # seconds
-ONE_MINUTE = 60   # seconds
+ONE_MINUTE = 60  # seconds
 
 
 def _get_cmd(clean_lib_name) -> str:
     if os.getenv('SLURM_PARTITION') == 'dori':
         return f"{JAMO_CMD_DORI} {clean_lib_name}"
     return f"{JAMO_CMD_NERSC} {clean_lib_name}"
 
@@ -249,15 +249,15 @@
         parser.add_argument('-i', '--interval', required=False, type=int, default=10,
                             help="wait interval in seconds to check if sequence has been fetched, " +
                                  "ignored if wait flag not set")
         parser.add_argument('-m', '--max', required=False, type=int, default=TWO_HOURS,
                             help="maximum time to wait for sequence in seconds, " +
                                  "ignored if wait flag not set.  Specify -1 to wait indefinetely.")
         parser.add_argument('-w', '--wait', action='store_true',
-                            help='wait for jamo to link sequence, output real path of linked sequence')
+                            help='wait for jamo to link sequence, then print "sequence ready"')
         parser.add_argument('--logging', required=False, default='WARN',
                             help="logging level (specify DEBUG for verbose logging)")
 
         ARGS = parser.parse_args()
         # logging.basicConfig(format='%(asctime)s %(message)s', datefmt='%m/%d/%Y %I:%M:%S %p', level=log_level)
         logging.basicConfig(format='%(message)s', level=ARGS.logging.upper())
         main(ARGS)
```

### Comparing `jamofetch-3.7.3/PKG-INFO` & `jamofetch-3.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamofetch
-Version: 3.7.3
+Version: 3.7.5
 Summary: A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori.
 License: None
 Author: Duncan Scott
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -25,42 +25,42 @@
 ```
 
 ## Usage
 See script **docs/demo_script.py** in the project for a sample script.
 
 Create a JamoFetcher:
 ```pthon
-from jamofetch.jamofetch import JamoFetcher, JamoLibSeq
+from jamofetch.jamofetch import JamoFetcher, LibSeq
 
 WAIT_INTERVAL = 10  # check if JAMO has provisioned sequence every 10 seconds
 WAIT_MAX = 7200     # max wait for sequence is 7200 seconds or 2 hours
 
 # directory where JAMO will link sequence, will be created if it doesn't exist
 link_dir = '/tmp/sequence-links'
 
 # create a fetcher
 fetcher: JamoFetcher = JamoFetcher(link_dir=link_dir, wait_interval_secs=WAIT_INTERVAL, wait_max_secs=WAIT_MAX)
 ```
 
-Note the following default configuration parameters for JamoLibSeq.
+Note the following default configuration parameters for LibSeq.
 Setting wait_max_secs to -1 causes the JamoFetcher instance to wait indefenitely for
 JAMO sequence.
 ```python
 class JamoFetcher():
     def __init__(self, link_dir='.', wait_interval_secs=10, wait_max_secs=-1):
 ```
 
 Fetch sequence for a library, print path of symlink to sequence file and the real path
 to the file.
 ```python
 LIBRARY = 'NPUNN'
 # Call JAMO to link sequence in the background.  Symlinks to the sequence
 # files are created by JAMO in the directory specified by the
 # link_dir parameter supplied to the JamoFetcher constructor.
-lib_seq: JamoLibSeq = fetcher.fetch_lib_seq(LIBRARY)
+lib_seq: LibSeq = fetcher.fetch_lib_seq(LIBRARY)
 
 printf(f"library name: {lib_seq.get_lib_name()}")
 print(f"sequence symlink: {lib_seq.get_seq_path()}")
 print(f"sequence real path: {lib_seq.get_real_path()}")
 ```
 
 Check if sequence has been provided by JAMO, i.e. the symlink is not broken.  Wait
@@ -75,24 +75,24 @@
 ```
 ## Command Line Tool
 Installing jamofetch with pip exposes a command line interface.
 ```
 (venv) [dnscott@ln004 jamofetch]$ jamofetch  -h
 usage: jamofetch [-h] [-l LIBRARY] [-d DIRECTORY] [-i INTERVAL] [-m MAX] [-w] [--logging LOGGING]
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -l LIBRARY, --library LIBRARY
                         library name(s) for which to retrieve sequence
   -d DIRECTORY, --directory DIRECTORY
                         directory where to link sequence, defaults to current directory. Directory will be created if it doesn't exit.
   -i INTERVAL, --interval INTERVAL
                         wait interval in seconds to check if sequence has been fetched, ignored if wait flag not set
   -m MAX, --max MAX     maximum time to wait for sequence in seconds, ignored if wait flag not set. Specify -1 to wait indefinetely.
-  -w, --wait            wait for jamo to link sequence, output real path of linked sequence
+  -w, --wait            wait for jamo to link sequence, then print "sequence ready"
   --logging LOGGING     logging level (specify DEBUG for verbose logging)
 (venv) [dnscott@ln004 jamofetch]$ jamofetch -d data -l NPUNN -l NOOHG -l HOGH -w --max -1
 fetching sequence:
 NPUNN /global/dna/dm_archive/sdm/pacbio/00/27/47/pbio-2747.27352.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz BACKUP_COMPLETE 6391936239a7711d789a9380
 NOOHG /global/dna/dm_archive/sdm/pacbio/00/26/91/pbio-2691.26653.bc1001_BAK8A_OA--bc1001_BAK8A_OA.ccs.fastq.gz RESTORED 6347dbb35bc59487d7e768d6
 HOGH /global/dna/dm_archive/sdm/illumina/00/63/97/6397.2.44053.GGCTAC.fastq.gz RESTORE_IN_PROGRESS 51d52a82067c014cd6ef4f6f
```

