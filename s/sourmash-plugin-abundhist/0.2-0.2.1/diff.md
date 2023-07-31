# Comparing `tmp/sourmash_plugin_abundhist-0.2.tar.gz` & `tmp/sourmash_plugin_abundhist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_abundhist-0.2.tar", last modified: Mon Jul 31 13:33:18 2023, max compression
+gzip compressed data, was "sourmash_plugin_abundhist-0.2.1.tar", last modified: Mon Jul 31 13:39:22 2023, max compression
```

## Comparing `sourmash_plugin_abundhist-0.2.tar` & `sourmash_plugin_abundhist-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:33:18.476473 sourmash_plugin_abundhist-0.2/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:13:48.000000 sourmash_plugin_abundhist-0.2/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     1396 2023-07-31 13:33:18.476346 sourmash_plugin_abundhist-0.2/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     1185 2023-07-31 13:31:15.000000 sourmash_plugin_abundhist-0.2/README.md
--rw-r--r--   0 t          (502) staff       (20)      415 2023-07-31 13:32:12.000000 sourmash_plugin_abundhist-0.2/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-07-31 13:33:18.476509 sourmash_plugin_abundhist-0.2/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:33:18.474944 sourmash_plugin_abundhist-0.2/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:33:18.475921 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     1396 2023-07-31 13:33:18.000000 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      415 2023-07-31 13:33:18.000000 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-07-31 13:33:18.000000 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       86 2023-07-31 13:33:18.000000 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       45 2023-07-31 13:33:18.000000 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       26 2023-07-31 13:33:18.000000 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     5176 2023-07-31 13:31:15.000000 sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:33:18.476051 sourmash_plugin_abundhist-0.2/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2023-07-30 11:13:48.000000 sourmash_plugin_abundhist-0.2/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.017693 sourmash_plugin_abundhist-0.2.1/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:13:48.000000 sourmash_plugin_abundhist-0.2.1/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     1665 2023-07-31 13:39:22.017538 sourmash_plugin_abundhist-0.2.1/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     1452 2023-07-31 13:38:21.000000 sourmash_plugin_abundhist-0.2.1/README.md
+-rw-r--r--   0 t          (502) staff       (20)      417 2023-07-31 13:38:21.000000 sourmash_plugin_abundhist-0.2.1/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-07-31 13:39:22.017736 sourmash_plugin_abundhist-0.2.1/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.016118 sourmash_plugin_abundhist-0.2.1/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.017067 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     1665 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      415 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)       86 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       45 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       26 2023-07-31 13:39:22.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     5405 2023-07-31 13:38:21.000000 sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:39:22.017200 sourmash_plugin_abundhist-0.2.1/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2023-07-30 11:13:48.000000 sourmash_plugin_abundhist-0.2.1/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_abundhist-0.2/LICENSE` & `sourmash_plugin_abundhist-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_abundhist-0.2/PKG-INFO` & `sourmash_plugin_abundhist-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_abundhist
-Version: 0.2
+Version: 0.2.1
 Summary: sourmash plugin to calculate abundance profiles.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_abundhist
 
@@ -36,15 +36,25 @@
 214  [   3]
 249  [   7]  *
 285  [   0]
 320  [   2]
 356  [   2]
 ```
 
-#### Create a nice histogram figure:
+#### Create a nice histogram figure for an isolate reads data set
+
+```
+sourmash scripts abundhist --max 100 --min 1 --bins 100 example/reads.sig.gz --figure example/ecoli-reads.png --ymax=200
+```
+
+will create:
+
+![histogram](example/ecoli-reads.png)
+
+#### Create a nice histogram figure for a metagenome:
 
 ```
 % sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip --figure hist.png
 ```
 will create this figure:
 
 ![histogram](example/hist.png)
```

### Comparing `sourmash_plugin_abundhist-0.2/README.md` & `sourmash_plugin_abundhist-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -28,15 +28,25 @@
 214  [   3]
 249  [   7]  *
 285  [   0]
 320  [   2]
 356  [   2]
 ```
 
-#### Create a nice histogram figure:
+#### Create a nice histogram figure for an isolate reads data set
+
+```
+sourmash scripts abundhist --max 100 --min 1 --bins 100 example/reads.sig.gz --figure example/ecoli-reads.png --ymax=200
+```
+
+will create:
+
+![histogram](example/ecoli-reads.png)
+
+#### Create a nice histogram figure for a metagenome:
 
 ```
 % sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip --figure hist.png
 ```
 will create this figure:
 
 ![histogram](example/hist.png)
```

### Comparing `sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.egg-info/PKG-INFO` & `sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash-plugin-abundhist
-Version: 0.2
+Version: 0.2.1
 Summary: sourmash plugin to calculate abundance profiles.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_abundhist
 
@@ -36,15 +36,25 @@
 214  [   3]
 249  [   7]  *
 285  [   0]
 320  [   2]
 356  [   2]
 ```
 
-#### Create a nice histogram figure:
+#### Create a nice histogram figure for an isolate reads data set
+
+```
+sourmash scripts abundhist --max 100 --min 1 --bins 100 example/reads.sig.gz --figure example/ecoli-reads.png --ymax=200
+```
+
+will create:
+
+![histogram](example/ecoli-reads.png)
+
+#### Create a nice histogram figure for a metagenome:
 
 ```
 % sourmash scripts abundhist example/SRR606249-abund-100k.sig.zip --figure hist.png
 ```
 will create this figure:
 
 ![histogram](example/hist.png)
```

### Comparing `sourmash_plugin_abundhist-0.2/src/sourmash_plugin_abundhist.py` & `sourmash_plugin_abundhist-0.2.1/src/sourmash_plugin_abundhist.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from sourmash import sourmash_args
 from sourmash.cli.utils import add_ksize_arg, add_moltype_args
 from sourmash.logging import debug_literal, set_quiet, notify
 from sourmash.plugins import CommandLinePlugin
 
 import numpy, collections, csv
 import termplotlib as tpl
-import seaborn, pylab
+import seaborn
+import matplotlib.pyplot as plt
 
 
 ###
 
 #
 # CLI plugin - supports 'sourmash scripts abundhist'
 #
@@ -60,22 +61,24 @@
             help='select signatures whose md5 contains this substring'
         )
         subparser.add_argument(
             '--name', default=None,
             help='select signatures whose name contains this substring'
         )
         subparser.add_argument(
-            '--max', type=int, default=None,
+            '-M', '--max', type=int, default=None,
             help='max value for histogram range (default none)')
         subparser.add_argument(
-            '--min', type=int, default=None,
+            '-m', '--min', type=int, default=None,
             help='min value for histogram range (default none)')
         subparser.add_argument(
             '--bins', type=int, default=10,
             help='number of bins (default 10)')
+        subparser.add_argument('--ymax', type=int,
+                               help='maximum Y value for histogram display')
         add_ksize_arg(subparser, default=31)
         add_moltype_args(subparser)
 
 
     def main(self, args):
         """
         output abundance histogram and/or raw abundances.
@@ -150,8 +153,10 @@
                 for hashval, count in counts_d.items():
                     w.writerow([hashval, count])
 
         # output figure?
         if args.figure:
             seaborn.histplot(all_counts, binrange=(min_range, max_range),
                              bins=n_bins, kde=True)
-            pylab.savefig(args.figure)
+            if args.ymax:
+                plt.ylim(top=args.ymax)
+            plt.savefig(args.figure)
```

