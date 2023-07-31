# Comparing `tmp/seismic2dreem-0.0.1.tar.gz` & `tmp/seismic2dreem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic2dreem-0.0.1.tar", last modified: Fri Jul 28 23:28:55 2023, max compression
+gzip compressed data, was "seismic2dreem-0.0.2.tar", last modified: Mon Jul 31 17:04:57 2023, max compression
```

## Comparing `seismic2dreem-0.0.1.tar` & `seismic2dreem-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 23:28:55.742660 seismic2dreem-0.0.1/
--rw-r--r--   0 ymdt       (501) staff       (20)     1068 2023-07-28 19:47:55.000000 seismic2dreem-0.0.1/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-07-28 23:28:55.742510 seismic2dreem-0.0.1/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      908 2023-07-28 22:49:57.000000 seismic2dreem-0.0.1/README.md
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 23:28:55.741498 seismic2dreem-0.0.1/seismic2dreem/
--rw-r--r--   0 ymdt       (501) staff       (20)       21 2023-07-28 19:52:38.000000 seismic2dreem-0.0.1/seismic2dreem/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      666 2023-07-28 22:44:00.000000 seismic2dreem-0.0.1/seismic2dreem/cli.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1846 2023-07-28 21:28:39.000000 seismic2dreem-0.0.1/seismic2dreem/dump.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2799 2023-07-28 23:20:18.000000 seismic2dreem-0.0.1/seismic2dreem/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2151 2023-07-28 21:22:43.000000 seismic2dreem-0.0.1/seismic2dreem/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1421 2023-07-28 23:16:58.000000 seismic2dreem-0.0.1/seismic2dreem/translation.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 23:28:55.742307 seismic2dreem-0.0.1/seismic2dreem.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-07-28 23:28:55.000000 seismic2dreem-0.0.1/seismic2dreem.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      392 2023-07-28 23:28:55.000000 seismic2dreem-0.0.1/seismic2dreem.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-28 23:28:55.000000 seismic2dreem-0.0.1/seismic2dreem.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       56 2023-07-28 23:28:55.000000 seismic2dreem-0.0.1/seismic2dreem.egg-info/entry_points.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       19 2023-07-28 23:28:55.000000 seismic2dreem-0.0.1/seismic2dreem.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       14 2023-07-28 23:28:55.000000 seismic2dreem-0.0.1/seismic2dreem.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-28 23:28:55.742701 seismic2dreem-0.0.1/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-28 23:28:49.000000 seismic2dreem-0.0.1/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-31 17:04:57.131309 seismic2dreem-0.0.2/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1068 2023-07-28 19:47:55.000000 seismic2dreem-0.0.2/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-07-31 17:04:57.131171 seismic2dreem-0.0.2/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      997 2023-07-31 16:16:06.000000 seismic2dreem-0.0.2/README.md
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-31 17:04:57.129756 seismic2dreem-0.0.2/seismic2dreem/
+-rw-r--r--   0 ymdt       (501) staff       (20)       21 2023-07-28 19:52:38.000000 seismic2dreem-0.0.2/seismic2dreem/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      671 2023-07-31 16:13:08.000000 seismic2dreem-0.0.2/seismic2dreem/cli.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1998 2023-07-31 15:55:26.000000 seismic2dreem-0.0.2/seismic2dreem/dump.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2615 2023-07-31 16:14:29.000000 seismic2dreem-0.0.2/seismic2dreem/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2151 2023-07-28 21:22:43.000000 seismic2dreem-0.0.2/seismic2dreem/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1421 2023-07-28 23:16:58.000000 seismic2dreem-0.0.2/seismic2dreem/translation.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-31 17:04:57.130954 seismic2dreem-0.0.2/seismic2dreem.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      392 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       56 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/entry_points.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       19 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       14 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-31 17:04:57.131348 seismic2dreem-0.0.2/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-31 17:04:47.000000 seismic2dreem-0.0.2/setup.py
```

### Comparing `seismic2dreem-0.0.1/LICENSE` & `seismic2dreem-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic2dreem-0.0.1/seismic2dreem/cli.py` & `seismic2dreem-0.0.2/seismic2dreem/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from .main import run
 import click
 
 @click.command()
 @click.argument('seismic_dir', required=True, nargs=-1, type=click.Path(exists=True))
 @click.option('--output', '-o', help='Output directory for the DREEM-formatted files', default='.', type=click.Path(exists=True))
-@click.option('--beautify/--no-beautify', default=True, help='Beautify JSON output')
-@click.option('--verbose/--no-verbose', default=True, help='Print warnings')
-def cli(seismic_dir, output, beautify, verbose):
+@click.option('--ow', help='Overwrite existing output files')
+@click.option('--beautify/--no-beautify', help='Beautify JSON output')
+@click.option('--verbose/--no-verbose', help='Print warnings')
+def cli(seismic_dir, **kwargs):
     """seismic2dreem converts SEISMIC data to DREEM format.
 
     SEISMIC_DIR is the name of the SEISMIC input directory.
     
     """
-    run(seismic_dir, output, beautify, verbose)
+    
+    run(seismic_dir, **kwargs)
```

### Comparing `seismic2dreem-0.0.1/seismic2dreem/dump.py` & `seismic2dreem-0.0.2/seismic2dreem/dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,26 +39,32 @@
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         return super(NpEncoder, self).default(obj)
 
 
-def dump_json(data, path):
+def dump_json(data, path, beautify=True):
+    """Beautifies and 
+    
+    """
     import json
     assert isdir(dirname(path)), f"output directory does not exist: {dirname(path)}"
     
     # Write the output
     out = cast_dict(data)
     out = sort_dict(out)
     
     # Make lists in one line
     out = json.dumps(out, cls=NpEncoder, indent=2)
 
-    out = out.replace(']','[').split('[')
-    out = [o.replace('\n        ','') if i%2 else o for i, o in enumerate(out)]
-    out = out[0] + ''.join([('[',']')[i%2] + o for i, o in enumerate(out[1:])])
-    
+    if beautify:
+        out = list(out)
+        out = ''.join(['[' if i == ']' else i for i in out])
+        out = out.split('[')
+        out = [o.replace('\n        ','') if i%2 else o for i, o in enumerate(out)]
+        out = out[0] + ''.join([('[',']')[i%2] + o for i, o in enumerate(out[1:])])
+        
     # Write the output
     with open(os.path.join(path), 'w') as f:
         f.write(out)
```

### Comparing `seismic2dreem-0.0.1/seismic2dreem/main.py` & `seismic2dreem-0.0.2/seismic2dreem/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from os.path import join, exists
 import json
 from .dump import dump_json
 from .path import SeismicPath
 from .translation import seismic_csv_to_dreem_json
 
 
-def run(seismic_folder_path:str, dreem_output_dir:str, beautify_json:bool=True, verbose:bool=True):
+def run(seismic_dir:str, output:str, ow=False, beautify:bool=True, verbose:bool=True):
     """A function to convert a seismic folder to a dreem json output.
     
     Arguments:
-        seismic_folder_path {str} -- The path to the seismic folder
-        dreem_output_dir {str} -- The path to the output directory
-        beautify_json {bool} -- Whether to beautify the json output (default: True). Deactivate for faster processing and less possible errors.
+        seismic_dir {str} -- The path to the seismic folder
+        output {str} -- The path to the output directory
+        ow {bool} -- Whether to overwrite an existing file
+        beautify {bool} -- Whether to beautify the json output (default: True). Deactivate for faster processing and less possible errors.
         verbose {bool} -- Whether to print warnings (default: True)
-        
+
     Returns:
         None
     """
     
-    if type(seismic_folder_path) == str:
-        seismic_folder_path = [seismic_folder_path]
+    if type(seismic_dir) == str:
+        seismic_dir = [seismic_dir]
             
-    for this_seismic_folder_path in seismic_folder_path:
-        seismic_path = SeismicPath(this_seismic_folder_path)
+    for p in seismic_dir:
+        seismic_path = SeismicPath(p)
             
         for sample in seismic_path.list_samples():
+            
+            path = join(output, sample + ".json")
+            if exists(path) and not ow and verbose:
+                print(f"WARNING: {path} already exists")
+                continue
+            
             out = {'sample': sample}
             for construct in seismic_path.list_constructs(sample):
                 out[construct] = {}
                 for section in seismic_path.list_sections(sample, construct):
                     out[construct][section] = {}
                     try:
                         out[construct][section] = seismic_csv_to_dreem_json(seismic_path.get_csv_path(sample, construct, section))
@@ -45,20 +52,10 @@
             # clean up empty constructs
             for construct in seismic_path.list_constructs(sample):
                 if len(out[construct]) == 1:
                     if len(out[construct][list(out[construct].keys())[0]]) == 0:
                         del out[construct]
                         
             # Save to file
-            path = join(dreem_output_dir, sample + ".json")
-            
-            # warning if file already exists
-            if exists(path):
-                print(f"WARNING: {path} already exists")
-            
-            if beautify_json:
-                dump_json(out, path)
-            else:
-                with open(path, 'w') as f:
-                    json.dump(out, f)
+            dump_json(out, path, beautify=beautify)
             if verbose:
                 print(f"saved {sample}.json to {seismic_path.get_sample_path(sample)}")
```

### Comparing `seismic2dreem-0.0.1/seismic2dreem/path.py` & `seismic2dreem-0.0.2/seismic2dreem/path.py`

 * *Files identical despite different names*

### Comparing `seismic2dreem-0.0.1/seismic2dreem/translation.py` & `seismic2dreem-0.0.2/seismic2dreem/translation.py`

 * *Files identical despite different names*

### Comparing `seismic2dreem-0.0.1/setup.py` & `seismic2dreem-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="seismic2dreem",
-    version='0.0.1',
+    version='0.0.2',
     description="Converts seismic data to dreem format",
     author="Yves Martin des Taillades for the Rouskin Lab",
     author_email="yves@martin.yt",
     url="https://github.com/rouskinlab/seismic2dreem",
     packages=find_packages(),
     install_requires=['pandas','numpy','click'],
     python_requires=">=3.9",
```

