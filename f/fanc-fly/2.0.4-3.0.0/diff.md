# Comparing `tmp/fanc-fly-2.0.4.tar.gz` & `tmp/fanc-fly-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fanc-fly-2.0.4.tar", last modified: Thu Feb 23 09:58:02 2023, max compression
+gzip compressed data, was "dist/fanc-fly-3.0.0.tar", last modified: Mon Jul 31 20:28:48 2023, max compression
```

## Comparing `fanc-fly-2.0.4.tar` & `fanc-fly-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/
--rw-rw-r--   0 jasper     (501) staff       (20)       25 2022-12-10 21:47:19.000000 fanc-fly-2.0.4/MANIFEST.in
--rw-rw-r--   0 jasper     (501) staff       (20)     5300 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/PKG-INFO
--rw-rw-r--   0 jasper     (501) staff       (20)     4180 2023-02-11 20:39:11.000000 fanc-fly-2.0.4/README.md
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc/
--rw-rw-r--   0 jasper     (501) staff       (20)      325 2023-02-11 13:16:57.000000 fanc-fly-2.0.4/fanc/__init__.py
--rw-rw-r--   0 jasper     (501) staff       (20)     2110 2023-01-24 17:02:26.000000 fanc-fly-2.0.4/fanc/auth.py
--rw-rw-r--   0 jasper     (501) staff       (20)     4197 2023-01-28 13:24:19.000000 fanc-fly-2.0.4/fanc/catmaid.py
--rw-rw-r--   0 jasper     (501) staff       (20)     4396 2022-12-10 21:47:20.000000 fanc-fly-2.0.4/fanc/connectivity.py
--rw-rw-r--   0 jasper     (501) staff       (20)    12728 2023-02-19 21:55:28.000000 fanc-fly-2.0.4/fanc/lookup.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3027 2023-02-23 09:44:50.000000 fanc-fly-2.0.4/fanc/ngl_info.py
--rw-rw-r--   0 jasper     (501) staff       (20)     7798 2023-02-11 13:27:34.000000 fanc-fly-2.0.4/fanc/publish.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3360 2023-02-11 13:16:59.000000 fanc-fly-2.0.4/fanc/render_neurons.py
--rw-rw-r--   0 jasper     (501) staff       (20)     6859 2023-02-11 13:16:57.000000 fanc-fly-2.0.4/fanc/skeletonize.py
--rw-rw-r--   0 jasper     (501) staff       (20)    14493 2023-02-23 09:54:48.000000 fanc-fly-2.0.4/fanc/statebuilder.py
--rw-rw-r--   0 jasper     (501) staff       (20)     1554 2022-12-10 21:47:20.000000 fanc-fly-2.0.4/fanc/statemanager.py
--rw-rw-r--   0 jasper     (501) staff       (20)     9728 2023-02-11 13:16:57.000000 fanc-fly-2.0.4/fanc/synaptic_links.py
--rw-rw-r--   0 jasper     (501) staff       (20)     3287 2023-01-30 21:05:39.000000 fanc-fly-2.0.4/fanc/template_spaces.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc/transforms/
--rw-rw-r--   0 jasper     (501) staff       (20)       83 2022-12-21 21:40:32.000000 fanc-fly-2.0.4/fanc/transforms/__init__.py
--rw-rw-r--   0 jasper     (501) staff       (20)    10074 2022-12-10 21:47:20.000000 fanc-fly-2.0.4/fanc/transforms/realignment.py
--rw-rw-r--   0 jasper     (501) staff       (20)    15072 2023-01-30 21:00:53.000000 fanc-fly-2.0.4/fanc/transforms/template_alignment.py
--rw-rw-r--   0 jasper     (501) staff       (20)    13263 2023-02-11 13:16:57.000000 fanc-fly-2.0.4/fanc/upload.py
--rw-rw-r--   0 jasper     (501) staff       (20)    12500 2023-02-11 20:19:51.000000 fanc-fly-2.0.4/fanc/visualize.py
-drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc_fly.egg-info/
--rw-rw-r--   0 jasper     (501) staff       (20)     5300 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc_fly.egg-info/PKG-INFO
--rw-rw-r--   0 jasper     (501) staff       (20)      583 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc_fly.egg-info/SOURCES.txt
--rw-rw-r--   0 jasper     (501) staff       (20)        1 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc_fly.egg-info/dependency_links.txt
--rw-rw-r--   0 jasper     (501) staff       (20)      211 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc_fly.egg-info/requires.txt
--rw-rw-r--   0 jasper     (501) staff       (20)        5 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/fanc_fly.egg-info/top_level.txt
--rw-rw-r--   0 jasper     (501) staff       (20)      211 2023-02-11 13:16:57.000000 fanc-fly-2.0.4/requirements.txt
--rw-rw-r--   0 jasper     (501) staff       (20)       38 2023-02-23 09:58:02.000000 fanc-fly-2.0.4/setup.cfg
--rw-rw-r--   0 jasper     (501) staff       (20)      905 2023-02-23 09:57:19.000000 fanc-fly-2.0.4/setup.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/
+-rw-rw-r--   0 jasper     (501) staff       (20)    35149 2022-12-10 21:47:19.000000 fanc-fly-3.0.0/LICENSE
+-rw-rw-r--   0 jasper     (501) staff       (20)       75 2023-07-30 17:19:39.000000 fanc-fly-3.0.0/MANIFEST.in
+-rw-rw-r--   0 jasper     (501) staff       (20)     7147 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)     5827 2023-07-30 18:01:17.000000 fanc-fly-3.0.0/README.md
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc/
+-rw-rw-r--   0 jasper     (501) staff       (20)      342 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/__init__.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10190 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/annotations.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     2110 2023-01-24 17:02:26.000000 fanc-fly-3.0.0/fanc/auth.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     4197 2023-01-28 13:24:19.000000 fanc-fly-3.0.0/fanc/catmaid.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     4410 2023-07-22 19:29:57.000000 fanc-fly-3.0.0/fanc/connectivity.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    40101 2023-07-30 19:26:42.000000 fanc-fly-3.0.0/fanc/lookup.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3027 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/ngl_info.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10702 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/fanc/publish.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3258 2023-05-20 17:30:54.000000 fanc-fly-3.0.0/fanc/render_neurons.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     7912 2023-07-31 20:23:30.000000 fanc-fly-3.0.0/fanc/skeletonize.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    17737 2023-07-30 18:56:59.000000 fanc-fly-3.0.0/fanc/statebuilder.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     1554 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/statemanager.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     9728 2023-02-11 13:16:57.000000 fanc-fly-3.0.0/fanc/synaptic_links.py
+-rw-rw-r--   0 jasper     (501) staff       (20)     3287 2023-01-30 21:05:39.000000 fanc-fly-3.0.0/fanc/template_spaces.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc/transforms/
+-rw-rw-r--   0 jasper     (501) staff       (20)       83 2022-12-21 21:40:32.000000 fanc-fly-3.0.0/fanc/transforms/__init__.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    10074 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/realignment.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    15072 2023-01-30 21:00:53.000000 fanc-fly-3.0.0/fanc/transforms/template_alignment.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/
+-rw-rw-r--   0 jasper     (501) staff       (20)  5544904 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedFANC.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)  3338492 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.Bspline.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)     1166 2022-12-10 21:47:20.000000 fanc-fly-3.0.0/fanc/transforms/transform_parameters/TransformParameters.FixedTemplate.affine.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)    26078 2023-07-30 18:57:12.000000 fanc-fly-3.0.0/fanc/upload.py
+-rw-rw-r--   0 jasper     (501) staff       (20)    12528 2023-07-22 19:31:44.000000 fanc-fly-3.0.0/fanc/visualize.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/
+-rw-rw-r--   0 jasper     (501) staff       (20)     7147 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/PKG-INFO
+-rw-rw-r--   0 jasper     (501) staff       (20)      868 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/SOURCES.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        1 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/dependency_links.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/requires.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)        5 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/fanc_fly.egg-info/top_level.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)      219 2023-07-08 11:24:01.000000 fanc-fly-3.0.0/requirements.txt
+-rw-rw-r--   0 jasper     (501) staff       (20)       38 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/setup.cfg
+-rw-rw-r--   0 jasper     (501) staff       (20)      975 2023-07-31 20:26:19.000000 fanc-fly-3.0.0/setup.py
+drwxrwxr-x   0 jasper     (501) staff       (20)        0 2023-07-31 20:28:48.000000 fanc-fly-3.0.0/tests/
+-rwxrwxr-x   0 jasper     (501) staff       (20)     2595 2023-07-31 20:23:30.000000 fanc-fly-3.0.0/tests/test_lookup.py
```

### Comparing `fanc-fly-2.0.4/PKG-INFO` & `fanc-fly-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,99 @@
-Metadata-Version: 2.1
-Name: fanc-fly
-Version: 2.0.4
-Summary: Tools for the Female Adult Nerve Cord Drosophila EM dataset
-Home-page: https://github.com/htem/FANC_auto_recon
-Author: Jasper Phelps
-Author-email: jasper.s.phelps@gmail.com
-License: UNKNOWN
-Description: # FANC_auto_recon
-        
-        FANC (pronounced "fancy") is the Female Adult Nerve Cord, a GridTape-TEM dataset of an adult _Drosophila melanogaster_'s ventral nerve cord. The dataset was first published in [Phelps, Hildebrand, Graham et al. 2021 _Cell_](https://www.lee.hms.harvard.edu/phelps-hildebrand-graham-et-al-2021), after which we applied automated methods for reconstructing neurons, synapses, and nuclei to accelerate reconstruction of the ventral nerve cord connectome. This repository contains a python package for interacting with the connectome (see the folder [`fanc`](fanc)) as well as other supporting files. 
-        
-        Have any questions? Please [open an issue](https://github.com/htem/FANC_auto_recon/issues/new) or contact [Jasper Phelps (jasper.s.phelps@gmail.com)](https://github.com/jasper-tms).
-        
-        ## Installing and configuring the `fanc` python package
-        
-        ### Before you start
-        
-        As is always the case in python, consider making a virtual environment (using your preference of virtualenv/virtualenvwrapper or conda) before installing.
-        
-        ### Installation option 1: pip install from PyPI
-        
-            pip install fanc-fly
-        
-        ### Installation option 2: pip install directly from GitHub
-        The code on GitHub will sometimes be slightly more up to date than the version on PyPI
-        
-            pip install git+https://github.com/htem/FANC_auto_recon.git
-        
-        ### Installation option 3: Clone then install
-        This is the best option if you want to make changes yourself to the code
-        
-            cd ~/repos  # or wherever you keep your repos
-            git clone https://github.com/htem/FANC_auto_recon.git
-            cd FANC_auto_recon
-            pip install -e .
-        
-        ### Provide credentials
-        
-        Access to the latest reconstruction of FANC is restricted to authorized users. If you are a member of the FANC community (see [Collaborative community](../../wiki#collaborative-community) on this repo's wiki) and have been granted access, you can generate an API key by visiting [https://global.daf-apis.com/auth/api/v1/create_token](https://global.daf-apis.com/auth/api/v1/create_token) and logging in with your FANC-authorized google account. Copy the key that is displayed, then run the following commands in python to save your key to the appropriate file:
-        ```python
-        import fanc
-        fanc.save_cave_credentials("THE API KEY YOU COPIED")
-        ```
-        
-        Alternatively, you can manually do what the command above accomplishes, which is to create a text file at `~/.cloudvolume/secrets/cave-secret.json` with these contents:
-        
-            {
-              "token": "THE API KEY YOU COPIED",
-              "fanc_production_mar2021": "THE API KEY YOU COPIED"
-            }
-        
-        You can verify that your API key has been saved successfully by running:
-        ```python
-        import fanc
-        client = fanc.get_caveclient()
-        ```
-        
-        ### Optional installation steps for additional functionality
-        
-        #### Install Elastix to transform neurons into alignment with the VNC template
-        The mesh manipulation and coordinate transform code requires `pytransformix`, which is itself a Python wrapper for Elastix. Therefore, Elastix must be installed and its lib and bin paths must be appended to the `LD_LIBRARY_PATH` and `PATH` environment variables. See [`pytransformix` documentation](https://github.com/jasper-tms/pytransformix#installation) for specific instructions.
-        
-        #### Provide CATMAID credentials to pull data from CATMAID
-        You can get your CATMAID API key by logging into https://radagast.hms.harvard.edu/catmaidvnc then hovering over "You are [Your Name]" in the top-right corner, then clicking "Get API token".
-        
-        Save your CATMAID API key by running:
-        ```python
-        import fanc
-        fanc.catmaid.save_catmaid_credentials("YOUR CATMAID API KEY")
-        ```
-        
-        You can verify that your API key has been saved successfully by running:
-        ```python
-        import fanc
-        fanc.catmaid.connect()
-        ```
-        
-        ## Documentation
-        - First go through [`fanc_python_package_examples.ipynb`](https://github.com/htem/FANC_auto_recon/blob/main/example_notebooks/fanc_python_package_examples.ipynb)
-        - Then check out other notebooks in [`example_notebooks/`](https://github.com/htem/FANC_auto_recon/tree/main/example_notebooks)
-        - Finally you can [browse the code](https://github.com/htem/FANC_auto_recon/tree/main/fanc), check out modules that have names that interest you, and read the docstrings.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# FANC_auto_recon
+
+FANC (pronounced "fancy") is the Female Adult Nerve Cord, a GridTape-TEM dataset of an adult _Drosophila melanogaster_'s ventral nerve cord. The dataset was first published in [Phelps, Hildebrand, Graham et al. 2021 _Cell_](https://www.lee.hms.harvard.edu/phelps-hildebrand-graham-et-al-2021), after which we applied automated methods for reconstructing neurons, synapses, and nuclei to accelerate reconstruction of the ventral nerve cord connectome, as described in [Azevedo, Lesser, Mark, Phelps et al. 2022 _bioRxiv_](https://www.biorxiv.org/content/10.1101/2022.12.15.520299).
+
+This repository contains:
+- A python package for interacting with the connectome data (see the folder [`fanc/`](fanc), and installation instructions below)
+- Other files and information related to the automated reconstructions (e.g. [`nuclei_prediction/`](nuclei_prediction), [`synapse_prediction/`](synapse_prediction))
+- Information for the collaborative proofreading community (see the [wiki](https://github.com/htem/FANC_auto_recon/wiki)). 
+
+Have any questions? Please [open an issue](https://github.com/htem/FANC_auto_recon/issues/new) or contact [Jasper Phelps (jasper.s.phelps@gmail.com)](https://github.com/jasper-tms).
+
+## Installing and configuring the `fanc` python package
+
+### Before you start
+
+As is always the case in python, consider making a virtual environment (using your preference of virtualenv/virtualenvwrapper or conda) before installing.
+
+### Installation option 1: pip install from PyPI
+
+    pip install fanc-fly
+
+### Installation option 2: pip install directly from GitHub
+The code on GitHub will sometimes be slightly more up to date than the version on PyPI
+
+    pip install git+https://github.com/htem/FANC_auto_recon.git
+
+### Installation option 3: Clone then install
+This is the best option if you want to make changes yourself to the code
+
+    cd ~/repos  # or wherever you keep your repos
+    git clone https://github.com/htem/FANC_auto_recon.git
+    cd FANC_auto_recon
+    pip install -e .
+
+### Troubleshooting
+Depending on your Python 3 version and your operating system, you may need to battle some bugs in order to get the `pip install` commands above to succeed.
+
+If you get something that looks like
+
+    .. ERROR:: Could not find a local HDF5 installation.
+       You may need to explicitly state where your local HDF5 headers and
+       library can be found by setting the ``HDF5_DIR`` environment
+       variable or by using the ``--hdf5`` command-line option.
+
+and you're on a Mac, install `brew` (https://brew.sh) if you haven't yet, then use `brew` to install HDF5 with `brew install hdf5`, then put `HDF5_DIR=/opt/homebrew/opt/hdf5` in front of your `pip install` command (e.g. `HDF5_DIR=/opt/homebrew/opt/hdf5 pip install fanc-fly`).
+
+If you get an error that contains
+
+    Error compiling Cython file:
+    ...
+    Cython.Compiler.Errors.CompileError: tables/utilsextension.pyx
+
+try to `pip install` the latest version of `tables` from GitHub by running `HDF5_DIR=/opt/homebrew/opt/hdf5 pip install git+https://github.com/PyTables/PyTables`, or alternatively, use conda to install it (`conda install tables`). After you get this package installed successfully, try installing `fanc-fly` again.
+
+### Provide credentials
+
+Access to the latest reconstruction of FANC is restricted to authorized users. If you are a member of the FANC community (see [Collaborative community](../../wiki#collaborative-community) on this repo's wiki) and have been granted access, you can generate an API key by visiting [https://global.daf-apis.com/auth/api/v1/create_token](https://global.daf-apis.com/auth/api/v1/create_token) and logging in with your FANC-authorized google account. Copy the key that is displayed, then run the following commands in python to save your key to the appropriate file:
+```python
+import fanc
+fanc.save_cave_credentials("THE API KEY YOU COPIED")
+```
+
+Alternatively, you can manually do what the command above accomplishes, which is to create a text file at `~/.cloudvolume/secrets/cave-secret.json` with these contents:
+
+    {
+      "token": "THE API KEY YOU COPIED",
+      "fanc_production_mar2021": "THE API KEY YOU COPIED"
+    }
+
+You can verify that your API key has been saved successfully by running:
+```python
+import fanc
+client = fanc.get_caveclient()
+```
+
+### Optional installation steps for additional functionality
+
+#### Install Elastix to transform neurons into alignment with the VNC template
+The mesh manipulation and coordinate transform code requires `pytransformix`, which is itself a Python wrapper for Elastix. Therefore, Elastix must be installed and its lib and bin paths must be appended to the `LD_LIBRARY_PATH` and `PATH` environment variables. See [`pytransformix` documentation](https://github.com/jasper-tms/pytransformix#installation) for specific instructions.
+
+#### Provide CATMAID credentials to pull data from CATMAID
+You can get your CATMAID API key by logging into https://radagast.hms.harvard.edu/catmaidvnc then hovering over "You are [Your Name]" in the top-right corner, then clicking "Get API token".
+
+Save your CATMAID API key by running:
+```python
+import fanc
+fanc.catmaid.save_catmaid_credentials("YOUR CATMAID API KEY")
+```
+
+You can verify that your API key has been saved successfully by running:
+```python
+import fanc
+fanc.catmaid.connect()
+```
+
+## Documentation
+- First go through [`fanc_python_package_examples.ipynb`](https://github.com/htem/FANC_auto_recon/blob/main/example_notebooks/fanc_python_package_examples.ipynb)
+- Then check out other notebooks in [`example_notebooks/`](https://github.com/htem/FANC_auto_recon/tree/main/example_notebooks)
+- Finally you can [browse the code](https://github.com/htem/FANC_auto_recon/tree/main/fanc), check out modules that have names that interest you, and read the docstrings.
```

### Comparing `fanc-fly-2.0.4/fanc/auth.py` & `fanc-fly-3.0.0/fanc/auth.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/catmaid.py` & `fanc-fly-3.0.0/fanc/catmaid.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/connectivity.py` & `fanc-fly-3.0.0/fanc/connectivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     threshold:        int, synapse threshold to use. default is 3
     drop_duplicates:  bool, whether to drop links between the same supervoxel pair 
     client:           caveclient.CAVEclient or None
     
     returns:
     a pd.DataFrame of synapse information from CAVE, 
     '''
-    if isinstance(seg_ids, int):
+    if isinstance(seg_ids, (int, np.integer)):
         seg_ids = [seg_ids]
 
     if direction == 'inputs':
         to_find = 'post'
         to_threshold = 'pre'
         
     elif direction == 'outputs':
```

### Comparing `fanc-fly-2.0.4/fanc/ngl_info.py` & `fanc-fly-3.0.0/fanc/ngl_info.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/publish.py` & `fanc-fly-3.0.0/fanc/publish.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,116 @@
 #!/usr/bin/env python3
 
 import os
+from xml.etree import ElementTree
 
+import numpy as np
+import requests
 import cloudvolume
 
 from . import auth, transforms
 
 PUBLISHED_MESHES_CLOUDPATH = ('gs://lee-lab_female-adult-nerve-cord/'
-                              'VNC_templates/{}/FANC_neurons')
-VALID_TEMPLATE_SPACES = ('JRC2018_VNC_FEMALE', 'JRC2018_VNC_UNISEX',
-                         'JRC2018_VNC_MALE')
+                              'meshes/{}/FANC_neurons')
+VALID_TEMPLATE_SPACES = ('FANC', 'JRC2018_VNC_FEMALE',
+                         'JRC2018_VNC_UNISEX', 'JRC2018_VNC_MALE')
+
+
+def list_public_segment_ids(template_space='JRC2018_VNC_FEMALE',
+                            gcloud_path=PUBLISHED_MESHES_CLOUDPATH):
+    """
+    List the segment IDs of all neurons that have been published to the
+    specified template space.
+    """
+    if template_space not in VALID_TEMPLATE_SPACES:
+        raise ValueError('{} not in {}'.format(template_space,
+                                               VALID_TEMPLATE_SPACES))
+    gcloud_path = gcloud_path.format(template_space)
+    # Implementation aided by GPT-4
+    url = f'https://storage.googleapis.com/{gcloud_path.split("/")[2]}'
+    params = {'prefix': '/'.join(gcloud_path.split('/')[3:])}
+
+    segids = []
+    while True:
+        response = requests.get(url, params=params)
+        tree = ElementTree.fromstring(response.text)
+
+        # namespaces cause trouble, so find them and remove them
+        namespaces = {'ns': 'http://doc.s3.amazonaws.com/2006-03-01'}
+
+        for elem in tree.findall('ns:Contents/ns:Key', namespaces):
+            filename = elem.text.split('/')[-1]
+            if filename.endswith(':0'):
+                segids.append(np.int64(filename[:-2]))
+
+        # Each query can only get 500 neurons, so we need to check whether
+        # there are more results to fetch
+        marker_elem = tree.find('ns:NextMarker', namespaces)
+        if marker_elem is None:
+            break
+        # If there are, add the marker to the params and allow the while loop
+        # to continue, making a request for the next batch
+        params['marker'] = marker_elem.text
+
+    return segids
 
 
 def publish_mesh_to_gcloud(segids,
                            template_space='JRC2018_VNC_FEMALE',
                            gcloud_path=PUBLISHED_MESHES_CLOUDPATH):
     """
     Download the mesh for a neuron, warp it into alignment with the specified
-    VNC template, and upload it to a public google cloud storage bucket.
+    VNC template (optional), and upload it to a public google cloud storage bucket.
     Neurons uploaded to the public project will have the same ID as the source
     neuron they came from in FANC.
 
     Currently only admins like Jasper and Wei have the necessary permissions
     for the upload to succeed. Please ask one of them to run this function for
     you when you have a list of neurons you're ready to make public.
 
-    The complete list of public neurons can be seen at:
-    https://console.cloud.google.com/storage/browser/lee-lab_female-adult-nerve-cord/VNC_templates/JRC2018_VNC_FEMALE/FANC_neurons/meshes
+    See a complete list of IDs of public neurons via one of the following
+    links, depending on which template space you want to see neurons in:
+    https://console.cloud.google.com/storage/browser/lee-lab_female-adult-nerve-cord/meshes/FANC/FANC_neurons/meshes
+    https://console.cloud.google.com/storage/browser/lee-lab_female-adult-nerve-cord/meshes/JRC2018_VNC_FEMALE/FANC_neurons/meshes
+    Not implemented yet: https://console.cloud.google.com/storage/browser/lee-lab_female-adult-nerve-cord/meshes/JRC2018_VNC_UNISEX/FANC_neurons/meshes
+    Not implemented yet: https://console.cloud.google.com/storage/browser/lee-lab_female-adult-nerve-cord/meshes/JRC2018_VNC_MALE/FANC_neurons/meshes
+
+    These neurons can be viewed by entering their ID(s) into one of the following neuroglancer links:
+    FANC: https://neuromancer-seung-import.appspot.com/?json_url=https://global.daf-apis.com/nglstate/api/v1/5104409098846208
+    JRC2018_VNC_FEMALE: https://neuromancer-seung-import.appspot.com/?json_url=https://global.daf-apis.com/nglstate/api/v1/6230309005688832
+    JRC2018_VNC_UNISEX: Not implemented yet
+    JRC2018_VNC_MALE: Not implemented yet
 
-    Public neurons can be viewed by entering their ID into this neuroglancer state:
-    https://neuromancer-seung-import.appspot.com/?json_url=https://global.daf-apis.com/nglstate/api/v1/5850904959909888
     """
     try:
         iter(segids)
     except:
         segids = [segids]
 
     if template_space not in VALID_TEMPLATE_SPACES:
         raise ValueError('{} not in {}'.format(template_space,
                                                VALID_TEMPLATE_SPACES))
+
+    already_published_ids = list_public_segment_ids(template_space=template_space,
+                                                    gcloud_path=gcloud_path)
+    already_published_ids = set(already_published_ids)
+
     
     fancneurons_cloudvolume = cloudvolume.CloudVolume(gcloud_path.format(template_space))
 
     mm = auth.get_meshmanager()
     for segid in segids:
+        if segid in already_published_ids:
+            print(f'Segment {segid} already published in {template_space}-space, skipping.')
+            continue
+        print(f'Publishing segment {segid} to {template_space}-space.')
         mesh = mm.mesh(seg_id=segid)
-        transforms.template_alignment.align_mesh(mesh, target_space=template_space)
-        mesh.vertices *= 1000  # TODO delete this after adding nm/um to align_mesh
+        if template_space != 'FANC':
+            transforms.template_alignment.align_mesh(mesh, target_space=template_space)
+            mesh.vertices *= 1000  # TODO delete this after adding nm/um to align_mesh
         mesh = cloudvolume.mesh.Mesh(mesh.vertices, mesh.faces, segid=segid)
         fancneurons_cloudvolume.mesh.put(mesh)
 
 
 def publish_skeleton_to_catmaid(segids,
                                 catmaid_instance=None):
     """
```

### Comparing `fanc-fly-2.0.4/fanc/render_neurons.py` & `fanc-fly-3.0.0/fanc/render_neurons.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import tqdm
 import navis
 import flybrains
 import npimage
 import npimage.graphics
 
 from . import auth
-from .skeletonize import get_pcg_skeleton
 from .template_spaces import template_info, get_nrrd_metadata
 from .transforms import template_alignment
 
 
 def render_neuron_into_template_space(seg_id: int,
                                       target_space: str,
                                       skeletonize=False,
@@ -51,17 +50,15 @@
     target_info = template_info[target_space]
 
     # Setup
     client = auth.get_caveclient()
     meshmanager = auth.get_meshmanager()
 
     if skeletonize:
-        skel = get_pcg_skeleton(seg_id)
-        #TODO align skeleton
-        #render skeleton
+        raise NotImplementedError
 
     print('Downloading mesh')
     my_mesh = meshmanager.mesh(
         seg_id=seg_id,
         remove_duplicate_vertices=True,
         merge_large_components=False  # False is faster but probably worse quality
     )
```

### Comparing `fanc-fly-2.0.4/fanc/skeletonize.py` & `fanc-fly-3.0.0/fanc/skeletonize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 #!/usr/bin/env python3
+"""
+Generate skeletons from FANC segmentation objects (meshes).
+
+See examples of running these skeletonization functions at:
+https://github.com/htem/FANC_auto_recon/blob/main/example_notebooks/skeletonization.ipynb
+"""
 
 import numpy as np
 import pandas as pd
 from scipy.spatial import distance
 
 from meshparty import trimesh_io, meshwork, mesh_filters
 import navis
@@ -16,15 +22,15 @@
     Create a skeleton from an object in the FANC segmentation.
 
     This function just calls pcg_skel.pcg_skeleton, so its main purpose
     is just to inform you that pcg_skel is the recommended way to
     generate a skeleton from a FANC neuron.
 
     Examples
-    ---
+    --------
     >>> skel = fanc.skeletonize.get_pcg_skeleton(648518346481082458)
     >>> fanc.statebuilder.render_scene(annotations=skel.vertices, annotation_units='nm')
 
     This example pulls a skeleton of the "homepage" FANC neuron, then renders
     a neuroglancer scene with the skeleton nodes displayed as point annotations.
     """
     if 'client' not in kwargs:
@@ -47,17 +53,41 @@
 
 diameter_smoothing_defaults = {'smooth_method': 'smooth',
                                'smooth_bandwidth': 1000}
 
 
 def skeletonize_neuron(seg_id,
                        soma_pt,
-                       cloudvolume,
                        output='meshwork',
+                       cloudvolume=auth.get_cloudvolume(),
                        voxel_resolution=skeletonization_defaults['voxel_resolution']):
+    """
+    Skeletonize a neuron from a FANC segmentation object (mesh).
+
+    This function is more flexible than get_pcg_skeleton (there are a
+    ton of parameters that you could tweak if you're really motivated to
+    get a skeleton that's optimized for your purposes) and produces
+    higher-resolution skeletons, but it takes much longer to run. For
+    most purposes, get_pcg_skeleton is recommended.
+
+    Arguments
+    ---------
+    seg_id: int
+      The segment ID to skeletonize
+
+    soma_pt: 3-element iterable (xyz)
+      The coordinates of the soma, in voxels
+
+    output: 'meshwork' or 'navis'
+      A string specifying the type of object to return.
+
+    cv: cloudvolume.CloudVolume
+      The cloudvolume to use for fetching meshes. Defaults to the FANC
+      segmentation cloudvolume.
+    """
     mesh = cloudvolume.mesh.get(seg_id, use_byte_offsets=True)[seg_id]
 
     mp_mesh = trimesh_io.Mesh(mesh.vertices, mesh.faces)
 
     mp_mesh.merge_large_components(size_threshold=skeletonization_defaults['merge_size_threshold'],
                                    max_dist=skeletonization_defaults['merge_max_dist'],
                                    dist_step=skeletonization_defaults['merge_distance_step'])
@@ -76,22 +106,23 @@
         neuron = diameter_smoothing(neuron)
         neuron.nodes.loc[neuron.soma, 'radius'] = skeletonization_defaults['soma_radius']
 
         return neuron
 
 
 def mp_to_navis(meshparty_skel, node_labels=None, xyz_scaling=1):
-    '''
+    """
     Convert a meshparty skeleton into a dataframe for navis/catmaid import.
-    Args
+
+    Arguments
     ----
-    skel:        meshparty skeleton
+    skel: meshparty skeleton
     node_labels: list , list of node labels, default is None and will generate new ones.
     xyz_scaling: int, scale factor for coordinates
-    '''
+    """
     ds = meshparty_skel.distance_to_root
     order_old = np.argsort(ds)
     new_ids = np.arange(len(ds))
     order_map = dict(zip(order_old, new_ids))
 
     if node_labels is None:
         node_labels = new_ids
```

### Comparing `fanc-fly-2.0.4/fanc/statebuilder.py` & `fanc-fly-3.0.0/fanc/statebuilder.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,30 +17,67 @@
 from cloudvolume.frontends.precomputed import CloudVolumePrecomputed
 from nglui.statebuilder import *
 
 from . import auth, catmaid, lookup
 from .transforms import realignment
 
 
-def skel2scene(skid, project=13, segment_threshold=10, node_threshold=None, return_as='url', dataset='production'):
-    catmaid.connect(project_id=project)
+def skel2scene(skid, hide_primary_neuron_points=True,
+               segment_threshold=10, node_threshold=None,
+               return_as='url', dataset='production', catmaid_project=13):
+    """
+    Create a neuroglancer scene containing a skeleton from CATMAID, and the
+    segments from the automated reconstruction that overlap with each skeleton
+    point. Very useful for quickly proofreading any neuron that has already
+    been traced in CATMAID.
+
+    Arguments
+    ---------
+    skid: int
+      The CATMAID skeleton ID of the neuron of interest
+
+    hide_primary_neuron_points: bool, default True
+      If False, all skeleton points will be shown.
+      If True, the skeleton points within the segment of your neuron of
+      interest will be hidden so that you only see the skeleton points that
+      aren't yet attached to your neuron's segment.
+
+    segment_threshold: int, default 10
+      See `fragment_dataframes` docstring
+
+    node_threshold: int, default None
+      See `fragment_dataframes` docstring
+
+    return_as: str, default 'url'
+      See `render_scene` docstring
+
+    dataset: str, default 'production'
+      Which version of the FANC segmentation to use. The default, 'production',
+      is the main community dataset and it's unlikely you'll want to change this.
+
+    project: int, default 13
+      The CATMAID project ID. The default, 13, is the main community project
+      and it's unlikely you'll need to change this.
+    """
+    catmaid.connect(project_id=catmaid_project)
     try:
         n = pymaid.get_neurons(skid)
     except:
-        return 'No matching skeleton ID in project {}'.format(project)
+        return 'No matching skeleton ID in project {}'.format(catmaid_project)
 
     n.downsample(inplace=True)
 
     target_volume = auth.get_cloudvolume(dataset=dataset)
     seg_ids, points = skel2seg(n, target_volume, transform=True)
 
     neuron_df, skeleton_df = fragment_dataframes(seg_ids,
                                                  points,
                                                  segment_threshold=segment_threshold,
-                                                 node_threshold=node_threshold)
+                                                 node_threshold=node_threshold,
+                                                 hide_primary_neuron_points=hide_primary_neuron_points)
     annotations = [{'name': 'skeleton coords',
                     'type': 'points',
                     'data': skeleton_df}]
     return render_scene(neurons=neuron_df, annotations=annotations, return_as=return_as)
 
 
 def skel2seg(neuron,
@@ -49,30 +86,40 @@
     nodes = neuron.nodes[['x', 'y', 'z']].values / np.array([4.3, 4.3, 45])
 
     if transform is True:
         points = realignment.fanc3_to_4(nodes)
     else:
         points = nodes
 
-    return lookup.segids_from_pts(points, cv=target_volume), points
+    return lookup.segid_from_pt(points, cv=target_volume), points
 
 
-def fragment_dataframes(seg_ids, coords, segment_threshold=20, node_threshold=None):
+def fragment_dataframes(seg_ids, coords,
+                        segment_threshold=20,
+                        node_threshold=None,
+                        hide_primary_neuron_points=False):
     ''' Generate dataframes for skeleton nodes, and subsequent neuron fragments
         seg_ids: list,array      List of rootIDs associated with the skeleton
         coords:  nx3 array       skeleton coords in voxel space
         segment_threshold: int   if not None, the number of segments to include in the dataframe. Will include the most overlapping segment IDs
-        node_threshold: int      if not None, the number of nodes required for a segment ID to be included'''
+        node_threshold: int      if not None, the number of nodes required for a segment ID to be included
+        hide_primary_neuron_points: bool  if True, will not include the primary neuron in the skeleton dataframe
+    '''
 
     ids, counts = np.unique(seg_ids, return_counts=True)
     value_counts = np.array(list(zip(ids, counts)), dtype=int)
     value_counts = value_counts[value_counts[:, 0] != 0, :]
 
     primary_neuron = value_counts[value_counts[:, 1] == max(value_counts[:, 1]), 0]
     fragments = value_counts[value_counts[:, 0] != primary_neuron, :]
+    # This is jasper's implementation of the few lines above, might switch to this
+    #unique_segids, segid_counts = np.unique(seg_ids, return_counts=True)
+    #most_common_segid = unique_segids[segid_counts == segid_counts.max()][0]
+    if hide_primary_neuron_points:
+        coords = coords[seg_ids != primary_neuron]
 
     if segment_threshold and not node_threshold:
         ids_to_use = fragments[np.argsort(-fragments[:, 1])[0:segment_threshold], 0]
     elif node_threshold and not segment_threshold:
         ids_to_use = fragments[fragments[:, 1] > node_threshold][:, 0]
     elif node_threshold and segment_threshold:
         print('Warning: cannot use segment and node threshold concurrently,defaulting to segment threshold')
@@ -96,48 +143,51 @@
     return neuron_df, skeleton_df
 
 
 def render_scene(neurons=None,
                  annotations=None,
                  annotation_units='voxels',
                  outlines_layer=True,
-                 nuclei_layer=True,
+                 nuclei_layer=False,
                  synapses_layer=False,
                  return_as='url',
                  **kwargs):
     """
     Render a neuroglancer scene with an arbitrary number of annotation layers
 
+    See some examples at https://github.com/htem/FANC_auto_recon/blob/main/example_notebooks/fanc_python_package_examples.ipynb
+
     ---Arguments---
     neurons:
         Some specification of which neurons you want to be displayed in the
         scene. This argument is flexible and can be provided in a few ways:
         - A int specifying a single segment ID
         - A list or pd.Series containing segment IDs
         - A pd.DataFrame with a column named pt_root_id containing
           segment IDs, and optionally with a column named color
         - A np.array with shape (N, 3) containing the xyz coordinates of
           N points, each of which indicates the location of a neuron you
           want to display. Coordinates should be in units of voxels
         - A string specifying the name of a CAVE table from which to
           pull neurons
 
-    annotations: Nx3 numpy array OR dict OR list of dicts
+    annotations: Nx3 numpy array OR DataFrame OR dict OR list of dicts
         Data (often point coordinates) you want displayed in an annotation layer.
         If Nx3 numpy array, each row must specify a point coordinate (xyz order).
+        If DataFrame, must have column 'pt_position', and optionally 'radius'.
         If dict, format must be
           {'name': str,
            'type': 'points' OR 'spheres',
            'data': numpy array OR DataFrame}
-        where data is formatted appropriately for the specified type.
+        where 'data' is formatted appropriately for the specified 'type'.
         Currently supported types and their corresponding data:
         - 'points': data must be an Nx3 numpy array or a DataFrame with a
                     column named 'pt_position'
         - 'spheres': data must be a DataFrame with columns 'pt_position'
-                     and 'radius'
+                     and 'radius_nm'. Specify radius in nm.
         If list of dicts, each dict must have the format above, and each one
         will be displayed as its own annotation layer.
 
     annotation_units: 'voxel' (Default) or 'nm'
         Whether annotation data is provided in units of voxels or nanometers.
         If in nanometers, data will be divided by `fanc.ngl_info.voxel_size` to
         convert to voxels.
@@ -193,40 +243,44 @@
         raise ValueError(f"annotation_units must be 'nm' or 'voxel' but was {annotation_units}")
 
     # Build a DataFrame containing rootIDs starting from whatever type is given
     if neurons is None:
         # None -> np.array
         # Default to showing the 'homepage' FANC neuron
         neurons = np.array([[48848, 114737, 2690]])
-    elif isinstance(neurons, int):
+    elif isinstance(neurons, (int, np.integer)):
         # int -> list
         neurons = [neurons]
     elif isinstance(neurons, str):
         # str -> DataFrame
         neurons = client.materialize.query_table(neurons, materialization_version=materialization_version)
+
     if isinstance(neurons, pd.Series):
-        # pd.Series -> pd.DataFrame or list
+        # pd.Series -> np.ndarray (if points) or pd.DataFrame (if root IDs)
         try:
-            # If Series contains point coordinates instead of rootIDs, lookup rootIDs
+            # If Series contains iterables, they must be point coordinates
             iter(neurons[0])
-            neurons = lookup.segids_from_pts(neurons.values)
+            neurons = np.vstack(neurons)
+            # Then let the section below turn them into root IDs
         except:
-            neurons = pd.DataFrame(neurons)
+            # Otherwise the series must contain root IDs
+            neurons = neurons.to_frame(name='pt_root_id')
     if isinstance(neurons, np.ndarray):
         # np.array -> list
         if np.any(neurons < 10000000000000000):
             # If array contains point coordinates instead of rootIDs, lookup rootIDs
-            neurons = lookup.segids_from_pts(neurons)
+            neurons = lookup.segid_from_pt(neurons)
         neurons = list(neurons)
     if isinstance(neurons, list):
         # list -> pd.DataFrame
         neurons = pd.DataFrame({'pt_root_id': neurons})
 
     if not isinstance(neurons, pd.DataFrame):
-        raise TypeError('Could not determine how to handle neurons argument')
+        raise TypeError('Could not determine how to handle neurons argument,'
+                        ' which is now a {}'.format(type(neurons)))
 
     # Add a color column
     if kwargs.get('color', False):
         cmap = cm.get_cmap('Set1', len(neurons))
         neurons['color'] = [colors.rgb2hex(cmap(i)) for i in range(cmap.N)]
     color_column = None
     if 'color' in neurons.columns:
@@ -263,51 +317,70 @@
                                                                resolution=ngl_info.voxel_size,
                                                                view_kws=ngl_info.view_options)
 
     # Additional layer(s)
     additional_states = []
     additional_data = []
     if annotations is not None:
+        if annotation_units in ['nm', 'nanometer', 'nanometers']:
+            annotation_layer_resolution = (1, 1, 1)
+        else:
+            annotation_layer_resolution = None
+
         if isinstance(annotations, np.ndarray):
-            annotations = {
-                'name': 'points',
-                'type': 'points',
-                'data': pd.DataFrame({'pt_position': [pt for pt in annotations]})
-            }
+            annotations = pd.DataFrame({'pt_position': [pt for pt in annotations]})
+        if isinstance(annotations, pd.Series):
+            annotations = annotations.to_frame(name='pt_position')
+        if isinstance(annotations, pd.DataFrame):
+            if 'radius' in annotations.columns:
+                annotations = {
+                    'name': 'spheres',
+                    'type': 'spheres',
+                    'data': annotations
+                }
+            else:
+                annotations = {
+                    'name': 'points',
+                    'type': 'points',
+                    'data': annotations
+                }
         if isinstance(annotations, dict):
             annotations = [annotations]
 
         for i in annotations:
+            data = None
             if isinstance(i['data'], np.ndarray):
-                i['data'] = pd.DataFrame({'pt_position': [pt for pt in i['data']]})
+                data = pd.DataFrame({'pt_position': [pt for pt in i['data']]})
+            elif isinstance(i['data'], pd.Series):
+                data = i['data'].to_frame(name='pt_position')
+            elif isinstance(i['data'], pd.DataFrame):
+                data = i['data']
+            else:
+                raise TypeError('Could not convert annotation data to DataFrame')
 
-            if 'pt_root_id' in i['data'].columns:
+            if 'pt_root_id' in data.columns:
                 segid_column = 'pt_root_id'
             else:
                 segid_column = None
 
-            if annotation_units in ['nm', 'nanometer', 'nanometers']:
-                i['data'].pt_position = [row for row in
-                                         np.vstack(i['data'].pt_position) / ngl_info.voxel_size]
-
             if i['type'] == 'points':
                 anno_mapper = PointMapper(point_column='pt_position',
                                           linked_segmentation_column=segid_column)
             elif i['type'] == 'spheres':
                 anno_mapper = SphereMapper(center_column='pt_position',
-                                           radius_column='radius',
+                                           radius_column='radius_nm',
                                            linked_segmentation_column=segid_column)
             else:
                 raise NotImplementedError(f"Unrecognized annotation type: '{i['type']}'")
 
-            anno_layer = AnnotationLayerConfig(name=i['name'], mapping_rules=anno_mapper)
+            anno_layer = AnnotationLayerConfig(name=i['name'], mapping_rules=anno_mapper, data_resolution=annotation_layer_resolution)
             additional_states.append(
                 StateBuilderDefaultSettings([anno_layer])
             )
-            additional_data.append(i['data'])
+            additional_data.append(data)
     if nuclei_layer:
         nuclei_config = SegmentationLayerConfig(name=ngl_info.nuclei['name'],
                                                 source=ngl_info.nuclei['path'],
                                                 selected_ids_column='nucleus_id')
         if 'nuclei' in kwargs:
             try:
                 iter(kwargs['nuclei'])
```

### Comparing `fanc-fly-2.0.4/fanc/statemanager.py` & `fanc-fly-3.0.0/fanc/statemanager.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/synaptic_links.py` & `fanc-fly-3.0.0/fanc/synaptic_links.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/template_spaces.py` & `fanc-fly-3.0.0/fanc/template_spaces.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/transforms/realignment.py` & `fanc-fly-3.0.0/fanc/transforms/realignment.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/transforms/template_alignment.py` & `fanc-fly-3.0.0/fanc/transforms/template_alignment.py`

 * *Files identical despite different names*

### Comparing `fanc-fly-2.0.4/fanc/visualize.py` & `fanc-fly-3.0.0/fanc/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,25 +84,25 @@
     vtk.vtkRenderer
         renderer when code was finished
     png
         output png image 
         (generate two images with/without scale bar if you specify to plot it)
     """
 
-    if isinstance(segment_ids, int):
+    if isinstance(segment_ids, (int, np.integer)):
         segment_ids = [segment_ids]
 
     colormap = cm.get_cmap(cmap, len(segment_ids))
 
     if 'client' in kwargs:
         client = kwargs['client']
     else:
         client = auth.get_caveclient()
 
-    if isinstance(camera, int):
+    if isinstance(camera, (int, np.integer)):
         state = client.state.get_state_json(camera)
         camera = trimesh_vtk.camera_from_ngl_state(state, zoom_factor=zoom_factor)
 
     meshmanager = auth.get_meshmanager()
 
     neuron_actors = []
     annotation_actors = []
```

### Comparing `fanc-fly-2.0.4/fanc_fly.egg-info/PKG-INFO` & `fanc-fly-3.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: fanc-fly
-Version: 2.0.4
+Version: 3.0.0
 Summary: Tools for the Female Adult Nerve Cord Drosophila EM dataset
 Home-page: https://github.com/htem/FANC_auto_recon
 Author: Jasper Phelps
 Author-email: jasper.s.phelps@gmail.com
 License: UNKNOWN
 Description: # FANC_auto_recon
         
-        FANC (pronounced "fancy") is the Female Adult Nerve Cord, a GridTape-TEM dataset of an adult _Drosophila melanogaster_'s ventral nerve cord. The dataset was first published in [Phelps, Hildebrand, Graham et al. 2021 _Cell_](https://www.lee.hms.harvard.edu/phelps-hildebrand-graham-et-al-2021), after which we applied automated methods for reconstructing neurons, synapses, and nuclei to accelerate reconstruction of the ventral nerve cord connectome. This repository contains a python package for interacting with the connectome (see the folder [`fanc`](fanc)) as well as other supporting files. 
+        FANC (pronounced "fancy") is the Female Adult Nerve Cord, a GridTape-TEM dataset of an adult _Drosophila melanogaster_'s ventral nerve cord. The dataset was first published in [Phelps, Hildebrand, Graham et al. 2021 _Cell_](https://www.lee.hms.harvard.edu/phelps-hildebrand-graham-et-al-2021), after which we applied automated methods for reconstructing neurons, synapses, and nuclei to accelerate reconstruction of the ventral nerve cord connectome, as described in [Azevedo, Lesser, Mark, Phelps et al. 2022 _bioRxiv_](https://www.biorxiv.org/content/10.1101/2022.12.15.520299).
+        
+        This repository contains:
+        - A python package for interacting with the connectome data (see the folder [`fanc/`](fanc), and installation instructions below)
+        - Other files and information related to the automated reconstructions (e.g. [`nuclei_prediction/`](nuclei_prediction), [`synapse_prediction/`](synapse_prediction))
+        - Information for the collaborative proofreading community (see the [wiki](https://github.com/htem/FANC_auto_recon/wiki)). 
         
         Have any questions? Please [open an issue](https://github.com/htem/FANC_auto_recon/issues/new) or contact [Jasper Phelps (jasper.s.phelps@gmail.com)](https://github.com/jasper-tms).
         
         ## Installing and configuring the `fanc` python package
         
         ### Before you start
         
@@ -31,14 +36,34 @@
         This is the best option if you want to make changes yourself to the code
         
             cd ~/repos  # or wherever you keep your repos
             git clone https://github.com/htem/FANC_auto_recon.git
             cd FANC_auto_recon
             pip install -e .
         
+        ### Troubleshooting
+        Depending on your Python 3 version and your operating system, you may need to battle some bugs in order to get the `pip install` commands above to succeed.
+        
+        If you get something that looks like
+        
+            .. ERROR:: Could not find a local HDF5 installation.
+               You may need to explicitly state where your local HDF5 headers and
+               library can be found by setting the ``HDF5_DIR`` environment
+               variable or by using the ``--hdf5`` command-line option.
+        
+        and you're on a Mac, install `brew` (https://brew.sh) if you haven't yet, then use `brew` to install HDF5 with `brew install hdf5`, then put `HDF5_DIR=/opt/homebrew/opt/hdf5` in front of your `pip install` command (e.g. `HDF5_DIR=/opt/homebrew/opt/hdf5 pip install fanc-fly`).
+        
+        If you get an error that contains
+        
+            Error compiling Cython file:
+            ...
+            Cython.Compiler.Errors.CompileError: tables/utilsextension.pyx
+        
+        try to `pip install` the latest version of `tables` from GitHub by running `HDF5_DIR=/opt/homebrew/opt/hdf5 pip install git+https://github.com/PyTables/PyTables`, or alternatively, use conda to install it (`conda install tables`). After you get this package installed successfully, try installing `fanc-fly` again.
+        
         ### Provide credentials
         
         Access to the latest reconstruction of FANC is restricted to authorized users. If you are a member of the FANC community (see [Collaborative community](../../wiki#collaborative-community) on this repo's wiki) and have been granted access, you can generate an API key by visiting [https://global.daf-apis.com/auth/api/v1/create_token](https://global.daf-apis.com/auth/api/v1/create_token) and logging in with your FANC-authorized google account. Copy the key that is displayed, then run the following commands in python to save your key to the appropriate file:
         ```python
         import fanc
         fanc.save_cave_credentials("THE API KEY YOU COPIED")
         ```
```

### Comparing `fanc-fly-2.0.4/setup.py` & `fanc-fly-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
     requirements = [l for l in requirements if not l.startswith('#')]
 
 setuptools.setup(
     name='fanc-fly',
-    version='2.0.4',
+    version='3.0.0',
     author='Jasper Phelps',
     author_email='jasper.s.phelps@gmail.com',
     description='Tools for the Female Adult Nerve Cord Drosophila EM dataset',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/htem/FANC_auto_recon',
     packages=setuptools.find_packages(),
+    package_data={'fanc.transforms': ['transform_parameters/*.txt']},
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires=requirements
```

