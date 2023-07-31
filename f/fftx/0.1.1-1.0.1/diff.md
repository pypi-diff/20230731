# Comparing `tmp/fftx-0.1.1.tar.gz` & `tmp/fftx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fftx-0.1.1.tar", last modified: Tue Jul 25 19:25:29 2023, max compression
+gzip compressed data, was "fftx-1.0.1.tar", last modified: Mon Jul 31 17:46:45 2023, max compression
```

## Comparing `fftx-0.1.1.tar` & `fftx-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,28 @@
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-25 19:25:29.494493 fftx-0.1.1/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5613 2023-07-25 18:51:51.000000 fftx-0.1.1/Contributing.md
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2512 2022-04-19 17:35:14.000000 fftx-0.1.1/LICENSE
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)       52 2023-07-25 19:07:22.000000 fftx-0.1.1/MANIFEST.in
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1036 2023-07-25 19:25:29.493498 fftx-0.1.1/PKG-INFO
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3252 2023-07-25 19:06:11.000000 fftx-0.1.1/README.md
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-25 19:25:29.485490 fftx-0.1.1/fftx/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      619 2023-07-25 19:19:37.000000 fftx-0.1.1/fftx/__init__.py
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-25 19:25:29.491496 fftx-0.1.1/fftx.egg-info/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1036 2023-07-25 19:25:29.000000 fftx-0.1.1/fftx.egg-info/PKG-INFO
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      183 2023-07-25 19:25:29.000000 fftx-0.1.1/fftx.egg-info/SOURCES.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)        1 2023-07-25 19:25:29.000000 fftx-0.1.1/fftx.egg-info/dependency_links.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)        5 2023-07-25 19:25:29.000000 fftx-0.1.1/fftx.egg-info/top_level.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)       38 2023-07-25 19:25:29.494500 fftx-0.1.1/setup.cfg
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1874 2023-07-25 19:17:41.000000 fftx-0.1.1/setup.py
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:46:45.469108 fftx-1.0.1/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      430 2022-04-19 17:35:14.000000 fftx-1.0.1/.gitignore
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5622 2023-07-31 17:42:01.000000 fftx-1.0.1/Contributing.md
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2512 2023-07-29 16:32:57.000000 fftx-1.0.1/LICENSE
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)       24 2023-07-29 17:14:30.000000 fftx-1.0.1/MANIFEST.in
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      805 2023-07-31 17:46:45.469103 fftx-1.0.1/PKG-INFO
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4669 2023-07-29 16:53:18.000000 fftx-1.0.1/README.md
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:46:45.452105 fftx-1.0.1/examples/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1458 2023-07-29 16:25:23.000000 fftx-1.0.1/examples/run-fft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1742 2023-07-29 16:25:23.000000 fftx-1.0.1/examples/run-fftn.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1596 2023-07-31 14:01:08.000000 fftx-1.0.1/examples/run-mdrconv.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1428 2023-07-29 16:25:23.000000 fftx-1.0.1/examples/run-mdrfsconv.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2044 2023-07-29 16:25:23.000000 fftx-1.0.1/examples/run-rfftn.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1527 2023-07-29 16:25:23.000000 fftx-1.0.1/examples/run-stepphase.py
+-rwxr-xr-x   0 pbroderick (16220) pbroderick (28128)     1584 2023-07-31 14:38:13.000000 fftx-1.0.1/examples/test-many.sh
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2547 2023-07-29 16:25:23.000000 fftx-1.0.1/examples/time-fftn.py
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:46:45.458102 fftx-1.0.1/fftx/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      615 2023-07-29 16:25:23.000000 fftx-1.0.1/fftx/__init__.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2725 2023-07-31 14:10:35.000000 fftx-1.0.1/fftx/convo.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4742 2023-07-29 16:25:23.000000 fftx-1.0.1/fftx/fft.py
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-31 17:46:45.467100 fftx-1.0.1/fftx.egg-info/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      805 2023-07-31 17:46:45.000000 fftx-1.0.1/fftx.egg-info/PKG-INFO
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      460 2023-07-31 17:46:45.000000 fftx-1.0.1/fftx.egg-info/SOURCES.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)        1 2023-07-31 17:46:45.000000 fftx-1.0.1/fftx.egg-info/dependency_links.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)        9 2023-07-31 17:46:45.000000 fftx-1.0.1/fftx.egg-info/requires.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)        5 2023-07-31 17:46:45.000000 fftx-1.0.1/fftx.egg-info/top_level.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)       38 2023-07-31 17:46:45.470103 fftx-1.0.1/setup.cfg
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2173 2023-07-31 17:16:08.000000 fftx-1.0.1/setup.py
```

### Comparing `fftx-0.1.1/Contributing.md` & `fftx-1.0.1/Contributing.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 
 ### Fork the Repository
 
 1.  On GitHub navigate to the [**repository**](https://github.com/spiral-software/python-package-fftx.git).
 2.  In the top-right corner of the page click the **Fork** button.  This will create a private repository for your use, called: <br>*github.com/\<your_username\>/python-package-fftx.git*, where **\<your_username\>** is your GitHub username.
 3.  Clone the new repository to your machine so you can develop, e.g., use **git** as follows: <br>*git clone github.com/\<your_username\>/python-package-fftx.git*
 4.  It is good practice to regularly sync your fork with the upstream repository.  Using the command line:
-```
+```shell
    cd <folder_you_created_when_cloning_above>
    git remote -v		## this will show:
       > origin   https://github.com:/<your_username>/python-package-fftx.git (fetch)
       > origin   https://github.com:/<your_username>/python-package-fftx.git (push)
       
    git remote add upstream https://github.com/spiral-software/python-package-fftx.git	## Sync with upstream
    git remote -v		## verify added
       > origin   https://github.com:/<your_username>/python-package-fftx.git (fetch)
       > origin   https://github.com:/<your_username>/python-package-fftx.git (push)
       > upstream	https://github.com/spiral-software/python-package-fftx.git (fetch)
       > upstream	https://github.com/spiral-software/python-package-fftx.git (push)
 ```
 
 Now, you can keep your fork synced with the upstream repository, using **git**:
-```
-git fetch upstream                    ## pulls any updates from upstream to local branch called upstream/master
+```shell
+git fetch upstream                    ## pulls any updates from upstream to local branch called upstream/main
 git branch <your_branch>              ## create a unique branch for your changes
 git checkout <your_branch>            ## switch to the your branch 
 git merge upstream/main               ## merges any changes from the upstream to the local
 ```
 
 ### Develop / Make Changes
 
@@ -55,12 +55,12 @@
 The important thing to note here is one completed **feature** per pull request.  The changes one proposes in a PR should correspond to one feature/bug fix/extension/etc.  One can create PRs with changes relevant to different ideas, however reviewing such PRs becomes tedious and error prone.  If possible, please follow the one-PR-one-package/feature rule.
 
 To create the pull request, do the following:
 
 1.  Navigate to the repository on GitHub (i.e., your fork of the original).
 2.  In the **Branch** menu choose the branch that contains your committed changes.
 3.  Above the list of files, click **Pull request**.
-4.  The pull request shows dropdowns for branch selection: The **base repository** should be the master repository from which your clone was made.  The **base** branch dropdown selects the branch to which you want your changes added (normally **master**).  The **head repository** is your clone of the original.  In the **compare** branch dropdown select the branch to which you committed your changes (i.e., *\<your_branch\>*).
+4.  The pull request shows dropdowns for branch selection: The **base repository** should be the master repository from which your clone was made.  The **base** branch dropdown selects the branch to which you want your changes added (normally **develop**).  The **head repository** is your clone of the original.  In the **compare** branch dropdown select the branch to which you committed your changes (i.e., *\<your_branch\>*).
 5.  Enter a title and brief description for your pull request.
 6.  To create a pull request that is ready for review, click the **Create Pull Request** button.
 
 After submitting the pull request it is available for review by the FFTX team.  In the course of the review comments or issues may be raised that require resolution before the changes can be committed to the main branch.  GitHub will notify the submitter of any such comments.
```

### Comparing `fftx-0.1.1/LICENSE` & `fftx-1.0.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FFTX Copyright (c) 2021 The Regents of the University of California, through Lawrence Berkeley National Laboratory 
+FFTX Copyright (c) 2023 The Regents of the University of California, through Lawrence Berkeley National Laboratory 
 (subject to receipt of any required approvals from the U.S. Dept. of Energy), Carnegie Mellon University and 
 SpiralGen, Inc.  All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following 
 conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `fftx-0.1.1/PKG-INFO` & `fftx-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fftx
-Version: 0.1.1
-Summary: A Python front end to access the high performance capabilities of the FFTX Project
+Version: 1.0.1
+Summary: A Python front end to access the FFTX Project
 Home-page: https://github.com/spiral-software/python-package-fftx
 Author: SpiralGen Inc.
 Author-email: Patrick.Broderick@spiralgen.com
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/spiral-software/python-package-fftx
 Platform: UNKNOWN
 Requires-Python: >=3.7
 License-File: LICENSE
 
-This Python package provides NumPy/CuPy-compatible access to the high performance multi-platform code generation capabilities of the FFTX Project.  The package provides a single API for several FFTs, along with some convolution-like transforms, that run on either CPUs or GPUs (NVIDIA and AMD) and supports single and double precision and both C (row-major) and Fortran (column-major) arrays.  The API uses the dimensions, datatype, ordering, and location of an array to determine which variant of a transform to invoke, simplifying application code intended for multiple target environments.
+This Python package provides NumPy/CuPy-compatible access to the high performance multi-platform code generation capabilities of the FFTX Project (https://github.com/spiral-software/fftx).  Both FFTX and this Python package originated under the Exascale Computing Project, with a focus on perforance-portable FFTs and FFT-using methods for the rapidly evolving high performance computing landscape.
```

### Comparing `fftx-0.1.1/README.md` & `fftx-1.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Python Package for FFTX
 =======================
 
 This Python package provides NumPy/CuPy-compatible access to the high performance multi-platform 
-code generation capabilities of the [FFTX Project](https://github.com/spiral-software/fftx), 
-which is currently under development as part of the Department of Energy's 
-[Exascale Computing Project](https://www.exascaleproject.org/).
+code generation capabilities of the [FFTX Project](https://github.com/spiral-software/fftx).  Both
+FFTX and this Python package originated as part of the Department of Energy's [Exascale Computing
+Project](https://www.exascaleproject.org/). 
 
 The package provides a single API for several FFTs, along with some convolution-like transforms,
 that run on either CPUs or GPUs (NVIDIA and AMD) and supports single and double precision and both
 C (row-major) and Fortran (column-major) arrays.  The API uses the dimensions, datatype, ordering,
 and location of an array to determine which variant of a transform to invoke, simplifying
 application code intended for multiple target environments.
 
@@ -24,60 +24,85 @@
 
    Direct replacements for several NumPy/CuPy fft functions.
    
 - **convo**
 
    Convolution and convolultion-like functions.
 
-See the docstrings in the code or use Python's `help()` function to view a module's internal
-documentation.  For example:
+See the docstrings in the code or use Python's `help()` function to view a module's internal documentation.  For example:
 
 ```python console
 >>> import fftx
 >>> help(fftx.fft)
 ```
 
-## Installing and Configuring FFTX Python Package
+## Installation
 
 The easiest method to install **fftx** is to use Python's package manager **pip**, e.g.,
 ```shell
 pip install fftx
 ```
 
-If you want to develop, contribute to, or possibly modify **fftx** it may be better to clone or
-fork the **fftx** repository, see
+When you install **fftx** the modules are installed in your ```site-packages``` location.  You
+can determine this location (and your base location) by running this python command:
+```shell
+python -m site --user-site --user-base
+##   Sample output -- On Unix/Linux/MacOS
+##   ~/.local:~/.local/lib/python3.9/site-packages
+##   Windows
+##   C:\Users\<user>\AppData\Roaming\Python;C:\Users\<user>\AppData\Roaming\Python\Python38\site-packages
+```
+
+Base location is always output first, the two locations are separated by a ':' (Unix/Linux/MacOS)
+or a ';' (Windows).
+
+The examples and other miscellaneous files will be installed at ```share/fftx``` under your
+base location.
+
+If you want to develop, contribute to, or possibly modify **fftx** it may be better to clone
+or fork the **fftx** repository, see
 [**Contributing**](https://github.com/spiral-software/python-package-fftx/blob/main/Contributing.md).
 Clone **python-package-fftx** to a location on your computer renaming it to **fftx**.  For
 example:
 ```shell
 cd ~/work/python-packages
 git clone https://github.com/spiral-software/python-package-fftx fftx
 ```
 
 If you clone or fork the **fftx** repository (vs installing the package) you need to add the
 directory that contains it to the environment variable **PYTHONPATH**.  (In the above example that
-would be ```~/work/python-packages/fftx```.)  This allows Python to locate the **fftx** module.
+would be ```~/work/python-packages/fftx```).  This allows Python to locate the **fftx**
+module.
+
+NOTE:  The **fftx** Python package depends on the
+[SpiralPy](https://github.com/spiral-software/python-package-spiralpy) package.  If you install
+using **pip** that module will be automatically installed also.  However, if you install maually,
+you will need to download and install **SpiralPy** also.  Follow the instructions in **SpiralPy**'s 
+[README](https://github.com/spiral-software/python-package-spiralpy#readme) to install and 
+configure **SpiralPy** and its dependencies. Once you have **SpiralPy** working properly 
+clone **python-package-fftx** into the same root directory as **SpiralPy** and rename it **fftx**.
 
 ## Examples
 
 For a quick start, look through the example scripts in the **examples** subdirectory.  Run an
 example script without arguments to see its help message.  For example:
 
 ```shell
 python run-fftn.py
 usage: run-fftn sz [ F|I [ d|s [ GPU|CPU ]]]
-  sz is N or N1,N2,N3
+  sz is N or N1,N2,.. all N >= 2, single N implies 3D cube
   F  = Forward, I = Inverse           (default: Forward)
   d  = double, s = single precision   (default: double precision)
-
+                                    
   (GPU is default target unless none exists or no CuPy)
-
-Three-dimensional complex FFT
+  
+Multi-dimensional complex FFT
 ```
 
 Typically the examples run an FFTX function along with the equivalent NumPy/CuPy function and
 compare the results.  Notice how the FFTX functions support both NumPy and CuPy arrays
-transparently.
+transparently. 
 
 The first time you run a script for a specific set of arguments, you will see a a few extra lines
 of output from about code generation, but on subsequent runs you will not, as the generated
-libraries are cached in the SpiralPy's **.libs** subdirectory.
+libraries are cached as explained in the **SpiralPy**
+[README](https://github.com/spiral-software/python-package-spiralpy#readme).
```

### Comparing `fftx-0.1.1/fftx/__init__.py` & `fftx-1.0.1/fftx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 fft
     Compatible subset of NumPy and CuPy fft subpackages
 
 convo
     Convolutions and convolution-like methods
 """
 
-# from . import fft
-# from . import convo
+from . import fft
+from . import convo
 
-__version__ = '0.1.1'
+__version__ = '1.0.1'
```

### Comparing `fftx-0.1.1/fftx.egg-info/PKG-INFO` & `fftx-1.0.1/fftx.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: fftx
-Version: 0.1.1
-Summary: A Python front end to access the high performance capabilities of the FFTX Project
+Version: 1.0.1
+Summary: A Python front end to access the FFTX Project
 Home-page: https://github.com/spiral-software/python-package-fftx
 Author: SpiralGen Inc.
 Author-email: Patrick.Broderick@spiralgen.com
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/spiral-software/python-package-fftx
 Platform: UNKNOWN
 Requires-Python: >=3.7
 License-File: LICENSE
 
-This Python package provides NumPy/CuPy-compatible access to the high performance multi-platform code generation capabilities of the FFTX Project.  The package provides a single API for several FFTs, along with some convolution-like transforms, that run on either CPUs or GPUs (NVIDIA and AMD) and supports single and double precision and both C (row-major) and Fortran (column-major) arrays.  The API uses the dimensions, datatype, ordering, and location of an array to determine which variant of a transform to invoke, simplifying application code intended for multiple target environments.
+This Python package provides NumPy/CuPy-compatible access to the high performance multi-platform code generation capabilities of the FFTX Project (https://github.com/spiral-software/fftx).  Both FFTX and this Python package originated under the Exascale Computing Project, with a focus on perforance-portable FFTs and FFT-using methods for the rapidly evolving high performance computing landscape.
```

### Comparing `fftx-0.1.1/setup.py` & `fftx-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,23 +20,36 @@
     for line in read(rel_path).splitlines():
         if line.startswith('__version__'):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
+def find_data_files():
+    examples_dir = 'examples'
+    example_files = glob.glob(os.path.join(examples_dir, '*.py'))
+    example_files = example_files + glob.glob(os.path.join(examples_dir, 'test-many.sh'))
+
+    misc_dir = '.'
+    misc_files = glob.glob(os.path.join(misc_dir, 'Contributing.md'))
+    misc_files = misc_files + glob.glob(os.path.join(misc_dir, 'README.md'))
+
+    return [('share/fftx/examples', example_files)] + [('share/fftx', misc_files)]
+
 setup(
     name="fftx",
     version=get_version("fftx/__init__.py"),
     license="BSD-3-Clause",
-    description="A Python front end to access the high performance capabilities of the FFTX Project",
-    long_description="This Python package provides NumPy/CuPy-compatible access to the high performance multi-platform code generation capabilities of the FFTX Project.  The package provides a single API for several FFTs, along with some convolution-like transforms, that run on either CPUs or GPUs (NVIDIA and AMD) and supports single and double precision and both C (row-major) and Fortran (column-major) arrays.  The API uses the dimensions, datatype, ordering, and location of an array to determine which variant of a transform to invoke, simplifying application code intended for multiple target environments.",
+    description="A Python front end to access the FFTX Project",
+    long_description="This Python package provides NumPy/CuPy-compatible access to the high performance multi-platform code generation capabilities of the FFTX Project (https://github.com/spiral-software/fftx).  Both FFTX and this Python package originated under the Exascale Computing Project, with a focus on perforance-portable FFTs and FFT-using methods for the rapidly evolving high performance computing landscape.",
     url="https://github.com/spiral-software/python-package-fftx",
     project_urls={
         "Source Code": "https://github.com/spiral-software/python-package-fftx",
     },
     author="SpiralGen Inc.",
     author_email="Patrick.Broderick@spiralgen.com",
     python_requires=">=3.7",
     packages=find_packages(),
     include_package_data=True,
+    data_files=find_data_files(),
+    install_requires=['spiralpy'],
 )
```

