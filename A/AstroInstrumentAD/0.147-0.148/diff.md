# Comparing `tmp/AstroInstrumentAD-0.147.tar.gz` & `tmp/AstroInstrumentAD-0.148.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/Jay.Stephan/Library/CloudStorage/OneDrive-ScienceandTechnologyFacilitiesCouncil/Documents/General/AD/Package/dist/.tmp-g", last modified: Mon Jul 31 14:20:48 2023, max compression
+gzip compressed data, was "/Users/Jay.Stephan/Library/CloudStorage/OneDrive-ScienceandTechnologyFacilitiesCouncil/Documents/General/AD/Package/dist/.tmp-5", last modified: Mon Jul 31 14:23:22 2023, max compression
```

## Comparing `AstroInstrumentAD-0.147.tar` & `AstroInstrumentAD-0.148.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)    21104 2023-07-31 14:20:41.000000 AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_analysis.py
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_functions.py
-drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/SOURCES.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/dependency_links.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/requires.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/top_level.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.147/LICENSE.txt
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)      736 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/PKG-INFO
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 14:17:20.000000 AstroInstrumentAD-0.147/README.md
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-31 14:20:48.000000 AstroInstrumentAD-0.147/setup.cfg
--rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1732 2023-07-31 14:20:42.000000 AstroInstrumentAD-0.147/setup.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/AstroInstrumentAD/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)    21104 2023-07-31 14:20:41.000000 AstroInstrumentAD-0.148/AstroInstrumentAD/dispersion_analysis.py
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     7563 2023-07-28 13:08:17.000000 AstroInstrumentAD-0.148/AstroInstrumentAD/dispersion_functions.py
+drwxr-xr-x   0 Jay.Stephan   (503) staff       (20)        0 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/AstroInstrumentAD.egg-info/
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      806 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/AstroInstrumentAD.egg-info/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      327 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/AstroInstrumentAD.egg-info/SOURCES.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        1 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/AstroInstrumentAD.egg-info/dependency_links.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       31 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/AstroInstrumentAD.egg-info/requires.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       18 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/AstroInstrumentAD.egg-info/top_level.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)        0 2023-06-06 10:17:20.000000 AstroInstrumentAD-0.148/LICENSE.txt
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)      806 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/PKG-INFO
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       39 2023-07-28 14:17:20.000000 AstroInstrumentAD-0.148/README.md
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)       79 2023-07-31 14:23:22.000000 AstroInstrumentAD-0.148/setup.cfg
+-rw-r--r--   0 Jay.Stephan   (503) staff       (20)     1913 2023-07-31 14:23:16.000000 AstroInstrumentAD-0.148/setup.py
```

### Comparing `AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_analysis.py` & `AstroInstrumentAD-0.148/AstroInstrumentAD/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.147/AstroInstrumentAD/dispersion_functions.py` & `AstroInstrumentAD-0.148/AstroInstrumentAD/dispersion_functions.py`

 * *Files identical despite different names*

### Comparing `AstroInstrumentAD-0.147/AstroInstrumentAD.egg-info/PKG-INFO` & `AstroInstrumentAD-0.148/AstroInstrumentAD.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.147
+Version: 0.148
 Summary: A Python package to characterise the impact of atmospheric dispersion on a spectrographs throughput
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-README.md
+# AstroInstrumentAD
+This is a test line
```

### Comparing `AstroInstrumentAD-0.147/PKG-INFO` & `AstroInstrumentAD-0.148/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: AstroInstrumentAD
-Version: 0.147
+Version: 0.148
 Summary: A Python package to characterise the impact of atmospheric dispersion on a spectrographs throughput
 Home-page: https://github.com/JamianStephan/AstroInstrumentAD
 Download-URL: https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip
 Author: Jay Stephan
 Author-email: Jay.Stephan@STFC.ac.uk
 License: MIT
 Keywords: Astronomy,Instrumentation,Atmospheric Dispersion
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-README.md
+# AstroInstrumentAD
+This is a test line
```

### Comparing `AstroInstrumentAD-0.147/setup.py` & `AstroInstrumentAD-0.148/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from distutils.core import setup
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
   name = 'AstroInstrumentAD',         # How you named your package folder (MyLib)
   packages = ['AstroInstrumentAD'],   # Chose the same as "name"
-  version = '0.147',      # Start with a small number and increase it with every change you make
+  version = '0.148',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A Python package to characterise the impact of atmospheric dispersion on a spectrographs throughput',   # Give a short description about your library
   author = 'Jay Stephan',                   # Type in your name
   author_email = 'Jay.Stephan@STFC.ac.uk',      # Type in your E-Mail
   url = 'https://github.com/JamianStephan/AstroInstrumentAD',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/JamianStephan/AstroInstrumentAD/archive/refs/tags/v0.1.zip',    # I explain this later on
-  long_description='README.md',
+  long_description=long_description,
+  long_description_content_type='text/markdown',
   keywords = ['Astronomy', 'Instrumentation', 'Atmospheric Dispersion'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'matplotlib',
           'astropy',
           'scipy',
       ],
```

