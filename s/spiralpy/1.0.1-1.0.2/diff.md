# Comparing `tmp/spiralpy-1.0.1.tar.gz` & `tmp/spiralpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiralpy-1.0.1.tar", last modified: Sat Jul 29 03:53:26 2023, max compression
+gzip compressed data, was "spiralpy-1.0.2.tar", last modified: Mon Jul 31 17:47:06 2023, max compression
```

## Comparing `spiralpy-1.0.1.tar` & `spiralpy-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:26.010266 spiralpy-1.0.1/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5694 2023-07-25 18:30:42.000000 spiralpy-1.0.1/Contributing.md
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1541 2023-07-20 19:02:18.000000 spiralpy-1.0.1/LICENSE
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)       88 2023-07-25 17:49:05.000000 spiralpy-1.0.1/MANIFEST.in
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-29 03:53:26.010263 spiralpy-1.0.1/PKG-INFO
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6803 2023-07-28 23:28:09.000000 spiralpy-1.0.1/README.md
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:25.974268 spiralpy-1.0.1/examples/
--rwxr-xr-x   0 pbroderick (16220) pbroderick (28128)    10941 2023-07-25 20:31:37.000000 spiralpy-1.0.1/examples/foo.sh
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      659 2023-07-27 19:11:23.000000 spiralpy-1.0.1/examples/print-metadata.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4409 2023-07-28 22:16:43.000000 spiralpy-1.0.1/examples/run-batchdft.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1935 2023-07-28 22:17:23.000000 spiralpy-1.0.1/examples/run-batchmddft.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1542 2023-07-28 22:18:10.000000 spiralpy-1.0.1/examples/run-dft.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      542 2023-07-28 22:19:07.000000 spiralpy-1.0.1/examples/run-hockney130.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      534 2023-07-28 22:19:26.000000 spiralpy-1.0.1/examples/run-hockney8.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2158 2023-07-28 22:19:50.000000 spiralpy-1.0.1/examples/run-mddft.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2592 2023-07-28 22:20:09.000000 spiralpy-1.0.1/examples/run-mdprdft.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1610 2023-07-28 19:30:46.000000 spiralpy-1.0.1/examples/run-mdrconv.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1448 2023-07-28 22:20:37.000000 spiralpy-1.0.1/examples/run-mdrfsconv.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1650 2023-07-28 03:30:38.000000 spiralpy-1.0.1/examples/run-stepphase.py
--rwxr-xr-x   0 pbroderick (16220) pbroderick (28128)     6483 2023-07-28 22:12:20.000000 spiralpy-1.0.1/examples/test-many.sh
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)       38 2023-07-29 03:53:26.011263 spiralpy-1.0.1/setup.cfg
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1952 2023-07-29 03:53:15.000000 spiralpy-1.0.1/setup.py
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:26.000266 spiralpy-1.0.1/spiralpy/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3859 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/CMakeLists.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4692 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/__init__.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5382 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/batchmddftsolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2400 2023-07-27 18:29:55.000000 spiralpy-1.0.1/spiralpy/constants.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6092 2023-07-27 18:00:26.000000 spiralpy-1.0.1/spiralpy/dftsolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6537 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/hockneysolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4687 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/mddftsolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6537 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/mdprdftsolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6229 2023-07-28 19:29:46.000000 spiralpy-1.0.1/spiralpy/mdrconvsolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6597 2023-07-28 04:13:51.000000 spiralpy-1.0.1/spiralpy/mdrfsconvsolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3139 2023-07-27 18:57:42.000000 spiralpy-1.0.1/spiralpy/metadata.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2955 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/spiral.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)    14114 2023-07-28 03:44:11.000000 spiralpy-1.0.1/spiralpy/spsolver.py
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5079 2023-07-28 04:18:23.000000 spiralpy-1.0.1/spiralpy/stepphasesolver.py
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:26.008262 spiralpy-1.0.1/spiralpy.egg-info/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/PKG-INFO
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      886 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/SOURCES.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)        1 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/dependency_links.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)        9 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/top_level.txt
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:47:06.604944 spiralpy-1.0.2/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1864 2023-07-29 14:15:26.000000 spiralpy-1.0.2/.gitignore
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5695 2023-07-31 17:44:19.000000 spiralpy-1.0.2/Contributing.md
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1541 2023-07-29 14:15:26.000000 spiralpy-1.0.2/LICENSE
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)       56 2023-07-29 14:15:26.000000 spiralpy-1.0.2/MANIFEST.in
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-31 17:47:06.604941 spiralpy-1.0.2/PKG-INFO
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6803 2023-07-29 14:15:26.000000 spiralpy-1.0.2/README.md
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:47:06.569942 spiralpy-1.0.2/examples/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      659 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/print-metadata.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4409 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-batchdft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1935 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-batchmddft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1542 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-dft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      542 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-hockney130.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      534 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-hockney8.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2158 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-mddft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2592 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-mdprdft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1610 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-mdrconv.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1448 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-mdrfsconv.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1650 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/run-stepphase.py
+-rwxr-xr-x   0 pbroderick (16220) pbroderick (28128)     6483 2023-07-29 14:15:26.000000 spiralpy-1.0.2/examples/test-many.sh
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)       38 2023-07-31 17:47:06.605941 spiralpy-1.0.2/setup.cfg
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2059 2023-07-31 17:00:16.000000 spiralpy-1.0.2/setup.py
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:47:06.595940 spiralpy-1.0.2/spiralpy/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3859 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/CMakeLists.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4692 2023-07-31 17:01:24.000000 spiralpy-1.0.2/spiralpy/__init__.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5382 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/batchmddftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2400 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/constants.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6092 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/dftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6537 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/hockneysolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4687 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/mddftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6537 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/mdprdftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6229 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/mdrconvsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6597 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/mdrfsconvsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3139 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/metadata.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2955 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/spiral.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)    14114 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/spsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5079 2023-07-29 14:15:26.000000 spiralpy-1.0.2/spiralpy/stepphasesolver.py
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:47:06.602944 spiralpy-1.0.2/spiralpy.egg-info/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-31 17:47:06.000000 spiralpy-1.0.2/spiralpy.egg-info/PKG-INFO
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      855 2023-07-31 17:47:06.000000 spiralpy-1.0.2/spiralpy.egg-info/SOURCES.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)        1 2023-07-31 17:47:06.000000 spiralpy-1.0.2/spiralpy.egg-info/dependency_links.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)        9 2023-07-31 17:47:06.000000 spiralpy-1.0.2/spiralpy.egg-info/top_level.txt
```

### Comparing `spiralpy-1.0.1/Contributing.md` & `spiralpy-1.0.2/Contributing.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       > origin   https://github.com:/<your_username>/python-package-spiralpy.git (push)
       > upstream	https://github.com/spiral-software/python-package-spiralpy.git (fetch)
       > upstream	https://github.com/spiral-software/python-package-spiralpy.git (push)
 ```
 
 Now, you can keep your fork synced with the upstream repository, using **git**:
 ```
-git fetch upstream                    ## pulls any updates from upstream to local branch called upstream/master
+git fetch upstream                    ## pulls any updates from upstream to local branch called upstream/main
 git branch <your_branch>              ## create a unique branch for your changes
 git checkout <your_branch>            ## switch to the your branch 
 git merge upstream/main               ## merges any changes from the upstream to the local
 ```
 
 ### Develop / Make Changes
 
@@ -81,15 +81,15 @@
 To create the pull request, do the following:
 
 1.  Navigate to the repository on GitHub (i.e., your fork of the original).
 2.  In the **Branch** menu choose the branch that contains your committed changes.
 3.  Above the list of files, click **Pull request**.
 4.  The pull request shows dropdowns for branch selection: The **base repository** should be the
 master repository from which your clone was made.  The **base** branch dropdown selects the branch
-to which you want your changes added (normally **main**).  The **head repository** is your clone
+to which you want your changes added (normally **develop**).  The **head repository** is your clone
 of the original.  In the **compare** branch dropdown select the branch to which you committed your
 changes (i.e., *\<your_branch\>*).
 5.  Enter a title and brief description for your pull request.
 6.  To create a pull request that is ready for review, click the **Create Pull Request** button.
 
 After submitting the pull request it is available for review by the SpiralPy team.  In the course
 of the review comments or issues may be raised that require resolution before the changes can be
```

### Comparing `spiralpy-1.0.1/LICENSE` & `spiralpy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/PKG-INFO` & `spiralpy-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python front end to specify high-level numerical computations
 Home-page: https://github.com/spiral-software/python-package-spiralpy
 Author: SpiralGen Inc.
 Author-email: Patrick.Broderick@spiralgen.com
 License: BSD-2-Clause
 Project-URL: Source Code, https://github.com/spiral-software/python-package-spiralpy
 Platform: UNKNOWN
```

### Comparing `spiralpy-1.0.1/README.md` & `spiralpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/print-metadata.py` & `spiralpy-1.0.2/examples/print-metadata.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-batchdft.py` & `spiralpy-1.0.2/examples/run-batchdft.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-batchmddft.py` & `spiralpy-1.0.2/examples/run-batchmddft.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-dft.py` & `spiralpy-1.0.2/examples/run-dft.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-hockney130.py` & `spiralpy-1.0.2/examples/run-hockney130.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-hockney8.py` & `spiralpy-1.0.2/examples/run-hockney8.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-mddft.py` & `spiralpy-1.0.2/examples/run-mddft.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-mdprdft.py` & `spiralpy-1.0.2/examples/run-mdprdft.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-mdrconv.py` & `spiralpy-1.0.2/examples/run-mdrconv.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-mdrfsconv.py` & `spiralpy-1.0.2/examples/run-mdrfsconv.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/run-stepphase.py` & `spiralpy-1.0.2/examples/run-stepphase.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/examples/test-many.sh` & `spiralpy-1.0.2/examples/test-many.sh`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/setup.py` & `spiralpy-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,20 +20,24 @@
     for line in read(rel_path).splitlines():
         if line.startswith('__version__'):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
-def find_example_files():
+def find_data_files():
     examples_dir = 'examples'
     example_files = glob.glob(os.path.join(examples_dir, '*.py'))
     example_files = example_files + glob.glob(os.path.join(examples_dir, 'test-many.sh'))
-    example_files = example_files + glob.glob(os.path.join(examples_dir, '../README.md'))
-    return [('share/spiralpy/examples', example_files)]
+
+    misc_dir = '.'
+    misc_files = glob.glob(os.path.join(misc_dir, 'Contributing.md'))
+    misc_files = misc_files + glob.glob(os.path.join(misc_dir, 'README.md'))
+
+    return [('share/spiralpy/examples', example_files)] + [('share/spiralpy', misc_files)]
 
 setup(
     name="spiralpy",
     version=get_version("spiralpy/__init__.py"),
     license="BSD-2-Clause",
     description="A Python front end to specify high-level numerical computations",
     long_description="Python front end for the SPIRAL project's Spiralpy system, which compiles high-level specifications of numerical computations into hardware-specific optimized code.  It supports a variety of CPU's as well as Nvidia and AMD GPU's on systems running Linux, Windows, or MacOS.",
@@ -42,9 +46,9 @@
         "Source Code": "https://github.com/spiral-software/python-package-spiralpy",
     },
     author="SpiralGen Inc.",
     author_email="Patrick.Broderick@spiralgen.com",
     python_requires=">=3.7",
     packages=find_packages(),
     include_package_data=True,
-    data_files=find_example_files(),
+    data_files=find_data_files(),
 )
```

### Comparing `spiralpy-1.0.1/spiralpy/CMakeLists.txt` & `spiralpy-1.0.2/spiralpy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/__init__.py` & `spiralpy-1.0.2/spiralpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import numpy as _numpy
 
 try:
     import cupy as _cupy
 except ModuleNotFoundError:
     _cupy = None
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 # # internal names
 
 # SP_LIBSDIR  = '.libs'
 
 # # environment varibles
```

### Comparing `spiralpy-1.0.1/spiralpy/batchmddftsolver.py` & `spiralpy-1.0.2/spiralpy/batchmddftsolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/constants.py` & `spiralpy-1.0.2/spiralpy/constants.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/dftsolver.py` & `spiralpy-1.0.2/spiralpy/dftsolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/hockneysolver.py` & `spiralpy-1.0.2/spiralpy/hockneysolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/mddftsolver.py` & `spiralpy-1.0.2/spiralpy/mddftsolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/mdprdftsolver.py` & `spiralpy-1.0.2/spiralpy/mdprdftsolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/mdrconvsolver.py` & `spiralpy-1.0.2/spiralpy/mdrconvsolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/mdrfsconvsolver.py` & `spiralpy-1.0.2/spiralpy/mdrfsconvsolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/metadata.py` & `spiralpy-1.0.2/spiralpy/metadata.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/spiral.py` & `spiralpy-1.0.2/spiralpy/spiral.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/spsolver.py` & `spiralpy-1.0.2/spiralpy/spsolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy/stepphasesolver.py` & `spiralpy-1.0.2/spiralpy/stepphasesolver.py`

 * *Files identical despite different names*

### Comparing `spiralpy-1.0.1/spiralpy.egg-info/PKG-INFO` & `spiralpy-1.0.2/spiralpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python front end to specify high-level numerical computations
 Home-page: https://github.com/spiral-software/python-package-spiralpy
 Author: SpiralGen Inc.
 Author-email: Patrick.Broderick@spiralgen.com
 License: BSD-2-Clause
 Project-URL: Source Code, https://github.com/spiral-software/python-package-spiralpy
 Platform: UNKNOWN
```

### Comparing `spiralpy-1.0.1/spiralpy.egg-info/SOURCES.txt` & `spiralpy-1.0.2/spiralpy.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+.gitignore
 Contributing.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+./Contributing.md
 ./README.md
-../spiralpy/README.md
-examples/foo.sh
 examples/print-metadata.py
 examples/run-batchdft.py
 examples/run-batchmddft.py
 examples/run-dft.py
 examples/run-hockney130.py
 examples/run-hockney8.py
 examples/run-mddft.py
 examples/run-mdprdft.py
 examples/run-mdrconv.py
 examples/run-mdrfsconv.py
 examples/run-stepphase.py
 examples/test-many.sh
-examples/../README.md
 spiralpy/CMakeLists.txt
 spiralpy/__init__.py
 spiralpy/batchmddftsolver.py
 spiralpy/constants.py
 spiralpy/dftsolver.py
 spiralpy/hockneysolver.py
 spiralpy/mddftsolver.py
```

