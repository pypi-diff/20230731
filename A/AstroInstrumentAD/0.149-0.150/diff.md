# Comparing `tmp/AstroInstrumentAD-0.149.tar.gz` & `tmp/AstroInstrumentAD-0.150.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/Jay.Stephan/Library/CloudStorage/OneDrive-ScienceandTechnologyFacilitiesCouncil/Documents/General/AD/Package/dist/.tmp-h", last modified: Mon Jul 31 15:06:55 2023, max compression
+gzip compressed data, was "AstroInstrumentAD-0.150.tar", last modified: Mon Jul 31 15:23:48 2023, max compression
```

## Comparing `AstroInstrumentAD-0.149.tar` & `AstroInstrumentAD-0.150.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    21595 2023-07-31 15:05:18.000000 AstroInstrumentAD-0.149/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.149/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      907 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.149/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      907 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      140 2023-07-31 15:05:58.000000 AstroInstrumentAD-0.149/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-31 15:06:55.000000 AstroInstrumentAD-0.149/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1913 2023-07-31 15:06:49.000000 AstroInstrumentAD-0.149/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 15:23:48.921592 AstroInstrumentAD-0.150/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 15:23:48.920426 AstroInstrumentAD-0.150/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    21595 2023-07-31 15:05:18.000000 AstroInstrumentAD-0.150/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.150/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 15:23:48.921461 AstroInstrumentAD-0.150/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      982 2023-07-31 15:23:48.000000 AstroInstrumentAD-0.150/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-31 15:23:48.000000 AstroInstrumentAD-0.150/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-31 15:23:48.000000 AstroInstrumentAD-0.150/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-31 15:23:48.000000 AstroInstrumentAD-0.150/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-31 15:23:48.000000 AstroInstrumentAD-0.150/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.150/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      982 2023-07-31 15:23:48.921655 AstroInstrumentAD-0.150/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      215 2023-07-31 15:22:07.000000 AstroInstrumentAD-0.150/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-31 15:23:48.921898 AstroInstrumentAD-0.150/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1913 2023-07-31 15:23:33.000000 AstroInstrumentAD-0.150/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `AstroInstrumentAD-0.149/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.150/AstroInstrumentAD/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.149/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.150/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.149/setup.py` & `AstroInstrumentAD-0.150/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.149',      # Start with a small number and increase it with every change you make
+  version = '0.150',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A Python package to characterise the impact of atmospheric dispersion on a spectrographs throughput',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@STFC.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
   long_description=long_description,
```

