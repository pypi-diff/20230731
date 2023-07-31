# Comparing `tmp/neural-admixture-1.2.3b0.tar.gz` & `tmp/neural-admixture-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-admixture-1.2.3b0.tar", last modified: Mon May 15 21:03:13 2023, max compression
+gzip compressed data, was "neural-admixture-1.3.0.tar", last modified: Mon Jul 31 19:18:42 2023, max compression
```

## Comparing `neural-admixture-1.2.3b0.tar` & `neural-admixture-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.140070 neural-admixture-1.2.3b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.132069 neural-admixture-1.2.3b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.132069 neural-admixture-1.2.3b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-15 21:03:13.140070 neural-admixture-1.2.3b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14757 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.132069 neural-admixture-1.2.3b0/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.132069 neural-admixture-1.2.3b0/demo/data/
--rw-r--r--   0 runner    (1001) docker     (123)   228180 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/data/demo_data.bed
--rw-r--r--   0 runner    (1001) docker     (123)   244365 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/data/demo_data.bim
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/data/demo_data.fam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.136069 neural-admixture-1.2.3b0/demo/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)  1478925 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/outputs/demo_run.7.P.expected
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/outputs/demo_run.7.Q.expected
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/run_demo.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/demo/run_diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.136069 neural-admixture-1.2.3b0/neural_admixture/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 21:03:13.000000 neural-admixture-1.2.3b0/neural_admixture/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.136069 neural-admixture-1.2.3b0/neural_admixture/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.136069 neural-admixture-1.2.3b0/neural_admixture/model/__test__/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/model/__test__/test_initializations.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/model/__test__/test_switchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/model/initializations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/model/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/model/neural_admixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/model/switchers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.140070 neural-admixture-1.2.3b0/neural_admixture/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/src/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/src/snp_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/src/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/neural_admixture/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:03:13.136069 neural-admixture-1.2.3b0/neural_admixture.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-15 21:03:13.000000 neural-admixture-1.2.3b0/neural_admixture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 21:03:13.000000 neural-admixture-1.2.3b0/neural_admixture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:03:13.000000 neural-admixture-1.2.3b0/neural_admixture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 21:03:13.000000 neural-admixture-1.2.3b0/neural_admixture.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 21:03:13.000000 neural-admixture-1.2.3b0/neural_admixture.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 21:03:13.000000 neural-admixture-1.2.3b0/neural_admixture.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-15 21:03:13.140070 neural-admixture-1.2.3b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-15 21:03:05.000000 neural-admixture-1.2.3b0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.356615 neural-admixture-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.360615 neural-admixture-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.360615 neural-admixture-1.3.0/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.360615 neural-admixture-1.3.0/demo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   228180 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/data/demo_data.bed
+-rw-r--r--   0 runner    (1001) docker     (123)   244365 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/data/demo_data.bim
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/data/demo_data.fam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/demo/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1478925 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/outputs/demo_run.7.P.expected
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/outputs/demo_run.7.Q.expected
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/run_demo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/demo/run_diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/neural_admixture/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 19:18:42.000000 neural-admixture-1.3.0/neural_admixture/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/neural_admixture/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/neural_admixture/model/__test__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/model/__test__/test_initializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/model/__test__/test_switchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/model/initializations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/model/neural_admixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/model/switchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/neural_admixture/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/src/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/src/snp_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/src/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/neural_admixture/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:18:42.364615 neural-admixture-1.3.0/neural_admixture.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-07-31 19:18:42.000000 neural-admixture-1.3.0/neural_admixture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 19:18:42.000000 neural-admixture-1.3.0/neural_admixture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:18:42.000000 neural-admixture-1.3.0/neural_admixture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-31 19:18:42.000000 neural-admixture-1.3.0/neural_admixture.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-31 19:18:42.000000 neural-admixture-1.3.0/neural_admixture.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 19:18:42.000000 neural-admixture-1.3.0/neural_admixture.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-31 19:18:42.368615 neural-admixture-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-31 19:18:32.000000 neural-admixture-1.3.0/tox.ini
```

### Comparing `neural-admixture-1.2.3b0/.github/workflows/release.yml` & `neural-admixture-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/.gitignore` & `neural-admixture-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/PKG-INFO` & `neural-admixture-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-admixture
-Version: 1.2.3b0
+Version: 1.3.0
 Summary: Rapid population clustering with autoencoders
 Home-page: https://github.com/AI-sandbox/neural-admixture
 Author: Albert Dominguez Mantes
 Author-email: albert.dominguezmantes@epfl.ch
 License: CC BY-NC 4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 ![PyPI - Status](https://img.shields.io/pypi/status/neural-admixture)
 [![tests](https://github.com/AI-sandbox/neural-admixture/workflows/tests/badge.svg)](https://github.com/AI-sandbox/neural-admixture/actions)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/neural-admixture)
 [![DOI](https://zenodo.org/badge/331290967.svg)](https://zenodo.org/badge/latestdoi/331290967)
 
 # Neural ADMIXTURE
 
-Neural ADMIXTURE is an unsupervised global ancestry inference technique based on ADMIXTURE. By using neural networks, Neural ADMIXTURE offers high quality ancestry assignments with a running time which is much faster than ADMIXTURE's. For more information, we recommend reading [the corresponding article](https://www.biorxiv.org/content/10.1101/2021.06.27.450081).
+Neural ADMIXTURE is an unsupervised global ancestry inference technique based on ADMIXTURE. By using neural networks, Neural ADMIXTURE offers high quality ancestry assignments with a running time which is much faster than ADMIXTURE's. For more information, we recommend reading [our corresponding article](https://www.nature.com/articles/s43588-023-00482-7).
 
 The software can be invoked via CLI and has a similar interface to ADMIXTURE (_e.g._ the output format is completely interchangeable). While the software runs in both CPU and GPU, we recommend using GPUs if available to take advantage of the neural network-based implementation.
 
 ![nadm_mna](https://github.com/AI-sandbox/neural-admixture/assets/31998088/048d04e2-8d62-4c14-870f-218e208dacb4)
 
 ## System requirements
 
@@ -42,75 +42,75 @@
 ### Software requirements
 
 The package has been tested on both Linux (CentOS 7.9.2009, Ubuntu 18.04.5 LTS) and MacOS (BigSur 11.2.3, Intel and Monterey 12.3.1, M1). If using GPUs, make sure CUDA drivers are properly installed.
 
 We recommend creating a fresh Python 3.9 environment using `virtualenv` (or `conda`), and then install the package `neural-admixture` there. As an example, for `virtualenv`, one should launch the following commands:
 
 ```console
-> virtualenv --python=python3.9 ~/venv/nadmenv
-> source ~/venv/nadmenv/bin/activate
-(nadmenv) > pip install neural-admixture
+$ virtualenv --python=python3.9 ~/venv/nadmenv
+$ source ~/venv/nadmenv/bin/activate
+(nadmenv) $ pip install neural-admixture
 ```
 
 ## Installation Guide
 
 The package can be easily installed in at most a few minutes using `pip` (make sure to add the `--upgrade` flag if updating the version):
 
 ```console
-(nadmenv) > pip install neural-admixture
+(nadmenv) $ pip install neural-admixture
 ```
 
 ## Usage 
 ### Running Neural ADMIXTURE
 
 To train a model from scratch, simply invoke the following commands from the root directory of the project. For more info about all the arguments, please run `neural-admixture train --help`. If training a single-head version of the network suffices, please use the flag `--k` instead of `--min_k` and `--max_k`. Note that VCF, BED, PGEN and HDF5 files are supported as of now. 
 
 For unsupervised Neural ADMIXTURE (single-head):
 
 ```console
-> neural-admixture train --k K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
+$ neural-admixture train --k K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
 ````
 
 For unsupervised Neural ADMIXTURE (multi-head):
 
 ```console
-> neural-admixture train --min_k MIN_K --max_k MAX_K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
+$ neural-admixture train --min_k MIN_K --max_k MAX_K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
 ```
 
 For supervised Neural ADMIXTURE:
 
 ```console
-> neural-admixture train --k K --supervised --populations_path POPS_PATH --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH # only single-head support at the moment
+$ neural-admixture train --k K --supervised --populations_path POPS_PATH --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH # only single-head support at the moment
 ```
 
 As an example, the following ADMIXTURE call
 
 ```console
-> ./admixture snps_data.bed 8 -s 42
+$ ./admixture snps_data.bed 8 -s 42
 ```
 
 would be mimicked in Neural ADMIXTURE by running
 
 ```console
-> neural-admixture train --k 8 --data_path snps_data.bed --save_dir SAVE_PATH --init_file INIT_FILE --name snps_data --seed 42
+$ neural-admixture train --k 8 --data_path snps_data.bed --save_dir SAVE_PATH --init_file INIT_FILE --name snps_data --seed 42
 ```
 
 with some parameters such as the decoder initialization or the save directories not having a direct equivalent.
 
 Several files will be output to the `SAVE_PATH` directory (the `name` parameter will be used to create the whole filenames):
 - If the unsupervised version is run, a `Pickle` binary file containing the PCA object (using the `init_name` parameter), as well as an image file containing a PCA plot.
 - A `.P` file, similar to ADMIXTURE.
 - A `.Q` file, similar to ADMIXTURE.
 - A `.pt` file, containing the weights of the trained network.
 - A `.json` file, with the configuration of the network.
 
 The last two files are required to run posterior inference using the network, so be aware of not deleting them accidentally! Logs are printed to the `stdout` channel by default. If you want to save them to a file, you can use the command `tee` along with a pipe:
 
 ```console
-> neural-admixture train --k 8 ... | tee run.log
+$ neural-admixture train --k 8 ... | tee run.log
 ```
 
 ### Initialization method
 
 As described in the article, Neural ADMIXTURE's decoder(s) can be initialized using several methods, which will be indicated by the required `initialization` argument. The best-performing initialization method depends, mainly, on the structure of the data. The main options are:
 
 - `pckmeans`: initialize using PCK-Means (Algorithm 1 in the paper). Performs best if data contains a large number of single-ancestry individuals.
@@ -121,15 +121,15 @@
 ### Inference mode (projective analysis)
 
 ADMIXTURE allows reusing computations in the _projective analysis_ mode, in which the `P` (`F`, frequencies) matrix is fixed to an already known result and only the assignments are computed. Due to the nature of our algorithm, assignments can be computed for unseen data by simply feeding the data through the encoder. This mode can be run by typing `infer` instead of `train` right after the `neural-admixture` call.
 
 For example, assuming we have a trained Neural ADMIXTURE (named `nadm_test`) in the path `./outputs`, one could run inference on unseen data (`./data/unseen_data.vcf`) via the following command:
 
 ```console
-> neural-admixture infer --name nadm_test --save_dir ./outputs --out_name unseen_nadm_test --data_path ./data/unseen_data.vcf
+$ neural-admixture infer --name nadm_test --save_dir ./outputs --out_name unseen_nadm_test --data_path ./data/unseen_data.vcf
 ```
 
 For this command to work, files `./outputs/nadm_test.pt` and `./outputs/nadm_test_config.json`, which are training outputs, must exist. In this case, only a `.Q` will be created, which will contain the assignments for this data (the parameter of the flag `out_name` will be used to generate the output file name). This file will be written in the `--save_dir` directory (in this case, `./outputs`).
 
 ### Pretrained Neural ADMIXTURE
 
 As also mentioned in the paper, Neural ADMIXTURE can be used to learn a function (through the encoder) given the results of the frequency matrix `P`/`F` of another algorithm so out-of-training data inference can be performed using the structure learnt by the other algorithm. The following arguments should be used to run Neural ADMIXTURE in this mode:
@@ -163,35 +163,35 @@
 
 ## Using Plink2 binary files (.pgen)
 
 If the data format you will be working on is _Plink2 Binary Files (.pgen, .psam, .pvar)_ then you also need to install the package `pgenlib`. This package is not available in PyPi, but is included in the [plink repository](https://github.com/chrchang/plink-ng/tree/master/2.0/Python). Installation instructions can be found in the [corresponding `README.md` file](https://github.com/chrchang/plink-ng/blob/master/2.0/Python/ReadMe.md). While you will need to clone the whole repository, you can remove it after installing the package, unless you plan to work with it.
 
 ## Experiments replication
 
-The datasets _All-Chms_, _Chm-22_ and _Chm-22-Sim_ used in the Experiments section of the article can be found in [figshare](https://doi.org/10.6084/m9.figshare.19387538.v1). For descriptions of the datasets, please refer to the corresponding section in the paper. The exact hyperparameters used in the experiments to allow replication can be found in Appendix B of the article.
+The datasets _All-Chms_, _Chm-22_ and _Chm-22-Sim_ used in the Experiments section of the article can be found in [figshare](https://doi.org/10.6084/m9.figshare.19387538.v1). For descriptions of the datasets, please refer to the corresponding section in the paper. The exact hyperparameters used in the experiments to allow replication can be found in the Supplementary Table 3 of the article.
 
 ## Demo
 
 To run the software with a small demo dataset, check the instructions in [the corresponding folder of the repository](https://github.com/AI-sandbox/neural-admixture/tree/main/demo).
 
 ## License
 
 **NOTICE**: This software is available for use free of charge for academic research use only. Academic users may fork this repository and modify and improve to suit their research needs, but also inherit these terms and must include a licensing notice to that effect. Commercial users, for profit companies or consultants, and non-profit institutions not qualifying as "academic research" should contact the authors for a separate license. This applies to this repository directly and any other repository that includes source, executables, or git commands that pull/clone this repository as part of its function. Such repositories, whether ours or others, must include this notice.
 
 ## Cite
 
-When using this software, please cite the following paper (currently pre-print):
+When using this software, please cite the following paper:
 
 ```{tex}
-@article {Mantes2021.06.27.450081,
-	author = {Mantes, Albert Dominguez and Montserrat, Daniel Mas and Bustamante, Carlos D. and Gir{\'o}-i-Nieto, Xavier and Ioannidis, Alexander G.},
-	title = {Neural ADMIXTURE: rapid population clustering with autoencoders},
-	elocation-id = {2021.06.27.450081},
-	year = {2022},
-	doi = {10.1101/2021.06.27.450081},
-	publisher = {Cold Spring Harbor Laboratory},
-	abstract = {Characterizing the genetic substructure of large cohorts has become increasingly important as genetic association and prediction studies are extended to massive, increasingly diverse, biobanks. ADMIXTURE and STRUCTURE are widely used unsupervised clustering algorithms for characterizing such ancestral genetic structure. These methods decompose individual genomes into fractional cluster assignments with each cluster representing a vector of DNA marker frequencies. The assignments, and clusters, provide an interpretable representation for geneticists to describe population substructure at the sample level. However, with the rapidly increasing size of population biobanks and the growing numbers of variants genotyped (or sequenced) per sample, such traditional methods become computationally intractable. Furthermore, multiple runs with different hyperparameters are required to properly depict the population clustering using these traditional methods, increasing the computational burden. This can lead to days of compute. In this work we present Neural ADMIXTURE, a neural network autoencoder that follows the same modeling assumptions as ADMIXTURE, providing similar (or better) clustering, while reducing the compute time by orders of magnitude. Indeed, the equivalent of one month of continuous compute can be reduced to hours. In addition, Neural ADMIXTURE can include multiple outputs, providing the equivalent results as running the original ADMIXTURE algorithm many times with different numbers of clusters. Our models can also be stored, allowing later cluster assignment to be performed with a linear computational time. The software implementation of Neural ADMIXTURE can be found at https://github.com/ai-sandbox/neural-admixture.},
-	URL = {https://www.biorxiv.org/content/early/2022/01/14/2021.06.27.450081},
-	eprint = {https://www.biorxiv.org/content/early/2022/01/14/2021.06.27.450081.full.pdf},
-	journal = {bioRxiv}
-}
+@article{dominguezmantes23,
+	abstract = {Characterizing the genetic structure of large cohorts has become increasingly important as genetic studies extend to massive, increasingly diverse biobanks. Popular methods decompose individual genomes into fractional cluster assignments with each cluster representing a vector of DNA variant frequencies. However, with rapidly increasing biobank sizes, these methods have become computationally intractable. Here we present Neural ADMIXTURE, a neural network autoencoder that follows the same modeling assumptions as the current standard algorithm, ADMIXTURE, while reducing the compute time by orders of magnitude surpassing even the fastest alternatives. One month of continuous compute using ADMIXTURE can be reduced to just hours with Neural ADMIXTURE. A multi-head approach allows Neural ADMIXTURE to offer even further acceleration by computing multiple cluster numbers in a single run. Furthermore, the models can be stored, allowing cluster assignment to be performed on new data in linear time without needing to share the training samples.},
+	author = {Dominguez Mantes, Albert and Mas Montserrat, Daniel and Bustamante, Carlos D. and Gir{\'o}-i-Nieto, Xavier and Ioannidis, Alexander G.},
+	doi = {10.1038/s43588-023-00482-7},
+	id = {Dominguez Mantes2023},
+	isbn = {2662-8457},
+	journal = {Nature Computational Science},
+	title = {Neural ADMIXTURE for rapid genomic clustering},
+	url = {https://doi.org/10.1038/s43588-023-00482-7},
+	year = {2023},
+	bdsk-url-1 = {https://doi.org/10.1038/s43588-023-00482-7}}
+
 ```
```

### Comparing `neural-admixture-1.2.3b0/README.md` & `neural-admixture-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![PyPI - Status](https://img.shields.io/pypi/status/neural-admixture)
 [![tests](https://github.com/AI-sandbox/neural-admixture/workflows/tests/badge.svg)](https://github.com/AI-sandbox/neural-admixture/actions)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/neural-admixture)
 [![DOI](https://zenodo.org/badge/331290967.svg)](https://zenodo.org/badge/latestdoi/331290967)
 
 # Neural ADMIXTURE
 
-Neural ADMIXTURE is an unsupervised global ancestry inference technique based on ADMIXTURE. By using neural networks, Neural ADMIXTURE offers high quality ancestry assignments with a running time which is much faster than ADMIXTURE's. For more information, we recommend reading [the corresponding article](https://www.biorxiv.org/content/10.1101/2021.06.27.450081).
+Neural ADMIXTURE is an unsupervised global ancestry inference technique based on ADMIXTURE. By using neural networks, Neural ADMIXTURE offers high quality ancestry assignments with a running time which is much faster than ADMIXTURE's. For more information, we recommend reading [our corresponding article](https://www.nature.com/articles/s43588-023-00482-7).
 
 The software can be invoked via CLI and has a similar interface to ADMIXTURE (_e.g._ the output format is completely interchangeable). While the software runs in both CPU and GPU, we recommend using GPUs if available to take advantage of the neural network-based implementation.
 
 ![nadm_mna](https://github.com/AI-sandbox/neural-admixture/assets/31998088/048d04e2-8d62-4c14-870f-218e208dacb4)
 
 ## System requirements
 
@@ -22,75 +22,75 @@
 ### Software requirements
 
 The package has been tested on both Linux (CentOS 7.9.2009, Ubuntu 18.04.5 LTS) and MacOS (BigSur 11.2.3, Intel and Monterey 12.3.1, M1). If using GPUs, make sure CUDA drivers are properly installed.
 
 We recommend creating a fresh Python 3.9 environment using `virtualenv` (or `conda`), and then install the package `neural-admixture` there. As an example, for `virtualenv`, one should launch the following commands:
 
 ```console
-> virtualenv --python=python3.9 ~/venv/nadmenv
-> source ~/venv/nadmenv/bin/activate
-(nadmenv) > pip install neural-admixture
+$ virtualenv --python=python3.9 ~/venv/nadmenv
+$ source ~/venv/nadmenv/bin/activate
+(nadmenv) $ pip install neural-admixture
 ```
 
 ## Installation Guide
 
 The package can be easily installed in at most a few minutes using `pip` (make sure to add the `--upgrade` flag if updating the version):
 
 ```console
-(nadmenv) > pip install neural-admixture
+(nadmenv) $ pip install neural-admixture
 ```
 
 ## Usage 
 ### Running Neural ADMIXTURE
 
 To train a model from scratch, simply invoke the following commands from the root directory of the project. For more info about all the arguments, please run `neural-admixture train --help`. If training a single-head version of the network suffices, please use the flag `--k` instead of `--min_k` and `--max_k`. Note that VCF, BED, PGEN and HDF5 files are supported as of now. 
 
 For unsupervised Neural ADMIXTURE (single-head):
 
 ```console
-> neural-admixture train --k K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
+$ neural-admixture train --k K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
 ````
 
 For unsupervised Neural ADMIXTURE (multi-head):
 
 ```console
-> neural-admixture train --min_k MIN_K --max_k MAX_K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
+$ neural-admixture train --min_k MIN_K --max_k MAX_K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
 ```
 
 For supervised Neural ADMIXTURE:
 
 ```console
-> neural-admixture train --k K --supervised --populations_path POPS_PATH --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH # only single-head support at the moment
+$ neural-admixture train --k K --supervised --populations_path POPS_PATH --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH # only single-head support at the moment
 ```
 
 As an example, the following ADMIXTURE call
 
 ```console
-> ./admixture snps_data.bed 8 -s 42
+$ ./admixture snps_data.bed 8 -s 42
 ```
 
 would be mimicked in Neural ADMIXTURE by running
 
 ```console
-> neural-admixture train --k 8 --data_path snps_data.bed --save_dir SAVE_PATH --init_file INIT_FILE --name snps_data --seed 42
+$ neural-admixture train --k 8 --data_path snps_data.bed --save_dir SAVE_PATH --init_file INIT_FILE --name snps_data --seed 42
 ```
 
 with some parameters such as the decoder initialization or the save directories not having a direct equivalent.
 
 Several files will be output to the `SAVE_PATH` directory (the `name` parameter will be used to create the whole filenames):
 - If the unsupervised version is run, a `Pickle` binary file containing the PCA object (using the `init_name` parameter), as well as an image file containing a PCA plot.
 - A `.P` file, similar to ADMIXTURE.
 - A `.Q` file, similar to ADMIXTURE.
 - A `.pt` file, containing the weights of the trained network.
 - A `.json` file, with the configuration of the network.
 
 The last two files are required to run posterior inference using the network, so be aware of not deleting them accidentally! Logs are printed to the `stdout` channel by default. If you want to save them to a file, you can use the command `tee` along with a pipe:
 
 ```console
-> neural-admixture train --k 8 ... | tee run.log
+$ neural-admixture train --k 8 ... | tee run.log
 ```
 
 ### Initialization method
 
 As described in the article, Neural ADMIXTURE's decoder(s) can be initialized using several methods, which will be indicated by the required `initialization` argument. The best-performing initialization method depends, mainly, on the structure of the data. The main options are:
 
 - `pckmeans`: initialize using PCK-Means (Algorithm 1 in the paper). Performs best if data contains a large number of single-ancestry individuals.
@@ -101,15 +101,15 @@
 ### Inference mode (projective analysis)
 
 ADMIXTURE allows reusing computations in the _projective analysis_ mode, in which the `P` (`F`, frequencies) matrix is fixed to an already known result and only the assignments are computed. Due to the nature of our algorithm, assignments can be computed for unseen data by simply feeding the data through the encoder. This mode can be run by typing `infer` instead of `train` right after the `neural-admixture` call.
 
 For example, assuming we have a trained Neural ADMIXTURE (named `nadm_test`) in the path `./outputs`, one could run inference on unseen data (`./data/unseen_data.vcf`) via the following command:
 
 ```console
-> neural-admixture infer --name nadm_test --save_dir ./outputs --out_name unseen_nadm_test --data_path ./data/unseen_data.vcf
+$ neural-admixture infer --name nadm_test --save_dir ./outputs --out_name unseen_nadm_test --data_path ./data/unseen_data.vcf
 ```
 
 For this command to work, files `./outputs/nadm_test.pt` and `./outputs/nadm_test_config.json`, which are training outputs, must exist. In this case, only a `.Q` will be created, which will contain the assignments for this data (the parameter of the flag `out_name` will be used to generate the output file name). This file will be written in the `--save_dir` directory (in this case, `./outputs`).
 
 ### Pretrained Neural ADMIXTURE
 
 As also mentioned in the paper, Neural ADMIXTURE can be used to learn a function (through the encoder) given the results of the frequency matrix `P`/`F` of another algorithm so out-of-training data inference can be performed using the structure learnt by the other algorithm. The following arguments should be used to run Neural ADMIXTURE in this mode:
@@ -143,35 +143,35 @@
 
 ## Using Plink2 binary files (.pgen)
 
 If the data format you will be working on is _Plink2 Binary Files (.pgen, .psam, .pvar)_ then you also need to install the package `pgenlib`. This package is not available in PyPi, but is included in the [plink repository](https://github.com/chrchang/plink-ng/tree/master/2.0/Python). Installation instructions can be found in the [corresponding `README.md` file](https://github.com/chrchang/plink-ng/blob/master/2.0/Python/ReadMe.md). While you will need to clone the whole repository, you can remove it after installing the package, unless you plan to work with it.
 
 ## Experiments replication
 
-The datasets _All-Chms_, _Chm-22_ and _Chm-22-Sim_ used in the Experiments section of the article can be found in [figshare](https://doi.org/10.6084/m9.figshare.19387538.v1). For descriptions of the datasets, please refer to the corresponding section in the paper. The exact hyperparameters used in the experiments to allow replication can be found in Appendix B of the article.
+The datasets _All-Chms_, _Chm-22_ and _Chm-22-Sim_ used in the Experiments section of the article can be found in [figshare](https://doi.org/10.6084/m9.figshare.19387538.v1). For descriptions of the datasets, please refer to the corresponding section in the paper. The exact hyperparameters used in the experiments to allow replication can be found in the Supplementary Table 3 of the article.
 
 ## Demo
 
 To run the software with a small demo dataset, check the instructions in [the corresponding folder of the repository](https://github.com/AI-sandbox/neural-admixture/tree/main/demo).
 
 ## License
 
 **NOTICE**: This software is available for use free of charge for academic research use only. Academic users may fork this repository and modify and improve to suit their research needs, but also inherit these terms and must include a licensing notice to that effect. Commercial users, for profit companies or consultants, and non-profit institutions not qualifying as "academic research" should contact the authors for a separate license. This applies to this repository directly and any other repository that includes source, executables, or git commands that pull/clone this repository as part of its function. Such repositories, whether ours or others, must include this notice.
 
 ## Cite
 
-When using this software, please cite the following paper (currently pre-print):
+When using this software, please cite the following paper:
 
 ```{tex}
-@article {Mantes2021.06.27.450081,
-	author = {Mantes, Albert Dominguez and Montserrat, Daniel Mas and Bustamante, Carlos D. and Gir{\'o}-i-Nieto, Xavier and Ioannidis, Alexander G.},
-	title = {Neural ADMIXTURE: rapid population clustering with autoencoders},
-	elocation-id = {2021.06.27.450081},
-	year = {2022},
-	doi = {10.1101/2021.06.27.450081},
-	publisher = {Cold Spring Harbor Laboratory},
-	abstract = {Characterizing the genetic substructure of large cohorts has become increasingly important as genetic association and prediction studies are extended to massive, increasingly diverse, biobanks. ADMIXTURE and STRUCTURE are widely used unsupervised clustering algorithms for characterizing such ancestral genetic structure. These methods decompose individual genomes into fractional cluster assignments with each cluster representing a vector of DNA marker frequencies. The assignments, and clusters, provide an interpretable representation for geneticists to describe population substructure at the sample level. However, with the rapidly increasing size of population biobanks and the growing numbers of variants genotyped (or sequenced) per sample, such traditional methods become computationally intractable. Furthermore, multiple runs with different hyperparameters are required to properly depict the population clustering using these traditional methods, increasing the computational burden. This can lead to days of compute. In this work we present Neural ADMIXTURE, a neural network autoencoder that follows the same modeling assumptions as ADMIXTURE, providing similar (or better) clustering, while reducing the compute time by orders of magnitude. Indeed, the equivalent of one month of continuous compute can be reduced to hours. In addition, Neural ADMIXTURE can include multiple outputs, providing the equivalent results as running the original ADMIXTURE algorithm many times with different numbers of clusters. Our models can also be stored, allowing later cluster assignment to be performed with a linear computational time. The software implementation of Neural ADMIXTURE can be found at https://github.com/ai-sandbox/neural-admixture.},
-	URL = {https://www.biorxiv.org/content/early/2022/01/14/2021.06.27.450081},
-	eprint = {https://www.biorxiv.org/content/early/2022/01/14/2021.06.27.450081.full.pdf},
-	journal = {bioRxiv}
-}
+@article{dominguezmantes23,
+	abstract = {Characterizing the genetic structure of large cohorts has become increasingly important as genetic studies extend to massive, increasingly diverse biobanks. Popular methods decompose individual genomes into fractional cluster assignments with each cluster representing a vector of DNA variant frequencies. However, with rapidly increasing biobank sizes, these methods have become computationally intractable. Here we present Neural ADMIXTURE, a neural network autoencoder that follows the same modeling assumptions as the current standard algorithm, ADMIXTURE, while reducing the compute time by orders of magnitude surpassing even the fastest alternatives. One month of continuous compute using ADMIXTURE can be reduced to just hours with Neural ADMIXTURE. A multi-head approach allows Neural ADMIXTURE to offer even further acceleration by computing multiple cluster numbers in a single run. Furthermore, the models can be stored, allowing cluster assignment to be performed on new data in linear time without needing to share the training samples.},
+	author = {Dominguez Mantes, Albert and Mas Montserrat, Daniel and Bustamante, Carlos D. and Gir{\'o}-i-Nieto, Xavier and Ioannidis, Alexander G.},
+	doi = {10.1038/s43588-023-00482-7},
+	id = {Dominguez Mantes2023},
+	isbn = {2662-8457},
+	journal = {Nature Computational Science},
+	title = {Neural ADMIXTURE for rapid genomic clustering},
+	url = {https://doi.org/10.1038/s43588-023-00482-7},
+	year = {2023},
+	bdsk-url-1 = {https://doi.org/10.1038/s43588-023-00482-7}}
+
 ```
```

### Comparing `neural-admixture-1.2.3b0/demo/README.md` & `neural-admixture-1.3.0/demo/README.md`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/demo/data/demo_data.bed` & `neural-admixture-1.3.0/demo/data/demo_data.bed`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/demo/data/demo_data.bim` & `neural-admixture-1.3.0/demo/data/demo_data.bim`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/demo/data/demo_data.fam` & `neural-admixture-1.3.0/demo/data/demo_data.fam`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/demo/outputs/demo_run.7.P.expected` & `neural-admixture-1.3.0/demo/outputs/demo_run.7.P.expected`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/demo/outputs/demo_run.7.Q.expected` & `neural-admixture-1.3.0/demo/outputs/demo_run.7.Q.expected`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/demo/run_diagnostics.py` & `neural-admixture-1.3.0/demo/run_diagnostics.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/neural_admixture/model/__test__/test_initializations.py` & `neural-admixture-1.3.0/neural_admixture/model/__test__/test_initializations.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,41 +12,42 @@
     caplog.set_level(logging.CRITICAL)
     X = da.random.binomial(n=2, p=.1, size=(n,d))/2
     path = None
     run_name = "pckmeans_test"
     n_components = 4
     seed = 42
     batch_size = 200
-    P_init = PCKMeansInitialization().get_decoder_init(X, K, path, run_name, n_components, seed, batch_size)
+    P_init, Q_inits = PCKMeansInitialization().get_decoder_init(X, K, path, run_name, n_components, seed, batch_size)
     assert P_init.shape[0] == sum(K) and P_init.shape[1] == d
-
+    assert len(Q_inits) == len(K)
+    assert all([Q_init.shape[0] == n and Q_init.shape[1] == k for Q_init, k in zip(Q_inits, K)])
 
 @pytest.mark.parametrize(["n", "d", "K"], [[42, 1000, [2,3,4]], [500, 100, [3,4,5]], [30,100,[6,7,8]]])
 def test_pcarchetypal(n, d, K, caplog):
     caplog.set_level(logging.CRITICAL)
     X = da.random.binomial(n=2, p=.1, size=(n,d))/2
     path = None
     run_name = "test_pcarchetypal"
     n_components = 4
     seed = 42
     batch_size = 200
-    P_init = PCArchetypal().get_decoder_init(X, K, path, run_name, n_components, seed, batch_size)
+    P_init, _ = PCArchetypal().get_decoder_init(X, K, path, run_name, n_components, seed, batch_size)
     assert P_init.shape[0] == sum(K) and P_init.shape[1] == d
 
 @pytest.mark.parametrize(["n", "d", "K"], [[42, 1000, [2]], [500, 100, [5]], [30,100,[10]]])
 def test_supervised(n, d, K, caplog):
     caplog.set_level(logging.CRITICAL)
     X = da.random.binomial(n=2, p=.1, size=(n,d))/2
     ancs = random.sample(string.ascii_lowercase, K[0]) + ["-"]
     y = ancs+random.choices(ancs, k=n-len(ancs))
-    P_init = SupervisedInitialization().get_decoder_init(X, y, K)
+    P_init, _ = SupervisedInitialization().get_decoder_init(X, y, K)
     assert P_init.shape[0] == K[0] and P_init.shape[1] == d
 
 def test_supervised_fail(caplog):
     caplog.set_level(logging.CRITICAL)
     n, d = 100, 10
     K = [5,6,7]
     X = da.random.binomial(n=2, p=.1, size=(n,d))/2
     ancs = random.sample(string.ascii_lowercase, 5) + ["-"]
     y = random.choices(ancs, k=n)
     with pytest.raises(NotImplementedError):
-        _ = SupervisedInitialization().get_decoder_init(X, y, K)
+        _, _ = SupervisedInitialization().get_decoder_init(X, y, K)
```

### Comparing `neural-admixture-1.2.3b0/neural_admixture/model/__test__/test_switchers.py` & `neural-admixture-1.3.0/neural_admixture/model/__test__/test_switchers.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/neural_admixture/model/initializations.py` & `neural-admixture-1.3.0/neural_admixture/model/initializations.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 with open(path, 'rb') as fb:
                     pca_obj = pickle.load(fb)
                 log.info('PCA loaded.')
                 if pca_obj.n_components_ != n_components:
                     raise FileNotFoundError
             else:
                 raise FileNotFoundError
-        except FileNotFoundError as fnfe:
+        except FileNotFoundError as _:
             log.info(f"{n_components}D PCA object not found. Performing IncrementalPCA...")
             pca_obj = DaskIncrementalPCA(n_components=n_components, random_state=42, batch_size=batch_size)
             pca_obj.fit(X)
             if path is not None:
                 with open(path, 'wb') as fb:
                     pickle.dump(pca_obj, fb)
         except Exception as e:
@@ -76,29 +76,33 @@
         assert pca_obj.n_features_ == X.shape[1], 'Computed PCA and training data do not have same number of SNPs' 
         log.info('Projecting data...')
         X_pca = pca_obj.transform(X).compute()
         log.info('Running KMeans on projected data...')
         if isinstance(K, Iterable):
             k_means_objs = [KMeans(n_clusters=i, random_state=42, n_init=10, max_iter=10).fit(X_pca) for i in K]
             centers = np.concatenate([obj.cluster_centers_ for obj in k_means_objs])
+            dists = [obj.transform(X_pca) for obj in k_means_objs]
+            Q_inits = [torch.as_tensor(-d, dtype=torch.float32).softmax(dim=1) for d in dists]
             P_init = torch.as_tensor(pca_obj.inverse_transform(centers).compute(), dtype=torch.float32).view(sum(K), -1)
         else:
             k_means_obj = KMeans(n_clusters=K, random_state=42, n_init=10, max_iter=10).fit(X_pca)
+            dists = k_means_obj.transform(X_pca)
             P_init = torch.as_tensor(pca_obj.inverse_transform(k_means_obj.cluster_centers_).compute(), dtype=torch.float32).view(K, -1)
+            Q_inits = [torch.as_tensor(-dists, dtype=torch.float32).softmax(dim=1)]
         te = time.time()
         log.info('Weights initialized in {} seconds.'.format(te-t0))
         log.info('Rendering PCA plot...')
         try:
             if path is not None:
                 plot_save_path = Path(path).parent/f"{run_name}_training_pca.png"
                 pca_plot(X_pca, plot_save_path)
         except Exception as e:
             log.warn(f'Could not render PCA plot: {e}')
             log.info('Resuming...')
-        return P_init
+        return P_init, Q_inits
 
 class PCArchetypal(object):
     """PCArchetypal initialization
     """
     @classmethod
     def get_decoder_init(cls, X: da.core.Array, K: Union[Iterable, int], path: str, run_name: str, n_components: int, seed: int, batch_size: int):
         """Get decoder initialization weights using PCArchetypal
@@ -150,15 +154,15 @@
         try:
             if path is not None:
                 plot_save_path = Path(path).parent/f"{run_name}_training_pca.png"
                 pca_plot(X_proj, plot_save_path)
         except Exception as e:
             log.warn(f'Could not render PCA plot: {e}')
             log.info('Resuming...')
-        return P_init
+        return P_init, None
 
 
 class SupervisedInitialization(object):
     """Supervised initialization
     """
     @classmethod
     def get_decoder_init(cls, X, y, K):
@@ -176,23 +180,23 @@
         y_num = to_idx_mapper(y[:])
         mask = y_num > -1
         masked_y_num = y_num[mask]
         X_masked = X[mask,:]
         P_init = torch.as_tensor(np.vstack([X_masked[masked_y_num==idx,:].mean(axis=0).compute() for idx in range(k)]), dtype=torch.float32)
         te = time.time()
         log.info('Weights initialized in {} seconds.'.format(te-t0))
-        return P_init
+        return P_init, None
 
 
 class PretrainedInitialization(object):
     """Pretrained initialization
     """
     @classmethod
     def get_decoder_init(cls, X, K, path):
         log.info('Fetching pretrained weights...')
         if len(K) > 1:
             raise NotImplementedError("Pretrained mode is only supported for single-head runs.")
         # Loads standard ADMIXTURE output format
         P_init = torch.as_tensor(1-np.genfromtxt(path, delimiter=' ').T, dtype=torch.float32)
         assert P_init.shape[0] == K[0], 'Input P is not coherent with the value of K'
         log.info('Weights fetched.')
-        return P_init
+        return P_init, None
```

### Comparing `neural-admixture-1.2.3b0/neural_admixture/model/modules.py` & `neural-admixture-1.3.0/neural_admixture/model/modules.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,33 +32,43 @@
         return outputs
 
 
 class NeuralDecoder(nn.Module):
     def __init__(self, ks, output_size, bias=False, inits=None, freeze=False):
         super().__init__()
         self.ks = ks
-        self.freeze = freeze
+        self.force_freeze = freeze
         if inits is None:
             self.decoders = nn.ModuleList(
                 [nn.Linear(k, output_size, bias=bias) for k in self.ks]
             )
-            if self.freeze:
+            if freeze:
                 log.warn('Not going to freeze weights as no initialization was provided.')   
         else:
             layers = [None]*len(self.ks)
             for i in range(len(ks)):
                 ini = end if i != 0 else 0
                 end = ini+self.ks[i]
                 layers[i] = nn.Linear(self.ks[i], output_size, bias=bias)
-                layers[i].weight = torch.nn.Parameter(inits[ini:end].clone().detach().requires_grad_(not self.freeze).T)
+                layers[i].weight = torch.nn.Parameter(inits[ini:end].clone().detach().T)
             self.decoders = nn.ModuleList(layers)
-            if self.freeze:
+            if self.force_freeze:
                 log.info('Decoder weights will be frozen.')
+                self.freeze()
         assert len(self.decoders) == len(self.ks)
 
     def _get_decoder_for_k(self, k):
         return self.decoders[k-min(self.ks)]
 
     def forward(self, hid_states):
         outputs = [torch.clamp(self._get_decoder_for_k(self.ks[i])(hid_states[i]), 0, 1) for i in range(len(self.ks))]
         return outputs
-
+    
+    def freeze(self) -> None:
+        for param in self.parameters():
+            param.requires_grad = False
+        return
+    
+    def unfreeze(self) -> None:
+        for param in self.parameters():
+            param.requires_grad = True
+        return
```

### Comparing `neural-admixture-1.2.3b0/neural_admixture/model/switchers.py` & `neural-admixture-1.3.0/neural_admixture/model/switchers.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/neural_admixture/src/inference.py` & `neural-admixture-1.3.0/neural_admixture/src/inference.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/neural_admixture/src/snp_reader.py` & `neural-admixture-1.3.0/neural_admixture/src/snp_reader.py`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/neural_admixture/src/train.py` & `neural-admixture-1.3.0/neural_admixture/src/train.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import argparse
+import dask
 import dask.array as da
 import logging
+import pandas as pd
 import sys
 import torch
 import torch.nn as nn
 import wandb
 from codetiming import Timer
+from pathlib import Path
+from sklearn.model_selection import KFold
+from typing import Dict, List, Tuple, Union
+
 from ..model.neural_admixture import NeuralAdmixture
 from ..model.switchers import Switchers
-from pathlib import Path
 from . import utils
-from typing import List, Tuple, Union
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 log = logging.getLogger(__name__)
 
 def fit_model(trX: da.core.Array, args: argparse.Namespace, valX: Union[None, da.core.Array]=None,
-              trY: Union[None, List[str]]=None, valY: Union[None, List[str]]=None) -> Tuple[NeuralAdmixture, torch.device]:
+              trY: Union[None, List[str]]=None, valY: Union[None, List[str]]=None,
+              dry_run: bool=False) -> Tuple[NeuralAdmixture, torch.device, List[Dict[int, float]]]:
     """Wrapper function to start training
 
     Args:
         trX (da.core.Array): Dask array containing training data.
         args (argparse.Namespace): parsed argument from CLI.
         valX (Union[None, da.core.Array], optional): Dask array containing validation data. Defaults to None.
         trY (Union[None, List[str]], optional): list containing training labels. Defaults to None.
-        valY (_type_, optional): list containing validation labels. Defaults to Union[None, List[str]]=None.
+        valY (Union[None, List[str]], optional): list containing validation labels. Defaults to Union[None, List[str]]=None.
+        dry_run (bool, optional): whether to run a dry run (no output is written to disk). Defaults to False.
 
     Returns:
-        Tuple[NeuralAdmixture, torch.device]: instantiated model object along with device.
+        Tuple[NeuralAdmixture, torch.device, List[Dict[int, float]]]: instantiated model object along with device and validation error.
     """
     switchers = Switchers.get_switchers()
     num_max_epochs = args.max_epochs
     batch_size = args.batch_size
     learning_rate = args.learning_rate
     save_dir = args.save_dir
     optimizer_str = args.optimizer
@@ -42,41 +48,52 @@
     freeze_decoder = bool(args.freeze_decoder)
     init_file = args.init_file
     supervised = bool(args.supervised)
     supervised_loss_weight = float(args.supervised_loss_weight)
     decoder_init = args.initialization if not supervised else 'supervised'
     n_components = int(args.pca_components)
     tol = float(args.tol)
+    warmup_epochs = int(args.warmup_epochs)
     name = args.name
     if args.k is not None:
         Ks = [int(args.k)]
     elif args.min_k is not None and args.max_k is not None:
         Ks = [i for i in range(args.min_k, args.max_k+1)]
     else:
         log.error('Either --k (single-head) or --min_k and --max_k (multi-head) must be provided.')
         sys.exit(1)
     assert not (supervised and len(Ks) != 1), 'Supervised version is currently only available on a single head'
     seed = args.seed
     log_to_wandb = bool(args.wandb_log)
     run_name = name
-    Path(save_dir).mkdir(parents=True, exist_ok=True)
+    if not dry_run:
+        Path(save_dir).mkdir(parents=True, exist_ok=True)
     log.info(f'Job args: {args}')
-    log.info('Will use GPU.' if torch.cuda.is_available() else 'No GPUs available.')
-    device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
-    if log_to_wandb:
+    log.info('Will use GPU.' if torch.cuda.is_available() else 'Will use Apple Metal acceleration.' if torch.backends.mps.is_available() else 'No GPUs available.')
+    device = torch.device('cuda:0' if torch.cuda.is_available() else 'mps' if torch.backends.mps.is_available() else 'cpu')
+    if log_to_wandb and not dry_run:
         utils.initialize_wandb(run_name, trX, valX, args, save_dir)
     save_path = f'{save_dir}/{run_name}.pt'
     torch.manual_seed(seed)
     # Initialization
     log.info('Initializing...')
     if init_file is None and decoder_init != "pretrained":
-        log.warning(f'Initialization filename not provided. Going to store it to {Path(save_dir)/run_name}.pkl')
+        if not dry_run:
+            log.warning(f'Initialization filename not provided. Going to store it to {Path(save_dir)/run_name}.pkl')
         init_file = f'{run_name}.pkl'
-    init_path = f'{Path(save_dir)/init_file}' if decoder_init != "pretrained" else init_file
-    P_init = switchers['initializations'][decoder_init](trX, trY, Ks, seed, init_path, run_name, n_components, batch_size)
+    init_path = f'{Path(save_dir)/init_file}' if decoder_init != "pretrained" else init_file if not dry_run else None
+    P_init, Q_inits = switchers['initializations'][decoder_init](
+        trX,
+        trY,
+        Ks,
+        seed,
+        init_path,
+        run_name,
+        n_components,
+        batch_size)
     activation = switchers['activations'][activation_str](0)
     log.info(f'Variants: {trX.shape[1]}')
     model = NeuralAdmixture(Ks, trX.shape[1], P_init=P_init,
                                 lambda_l2=l2_penalty,
                                 encoder_activation=activation,
                                 hidden_size=hidden_size,
                                 freeze_decoder=freeze_decoder,
@@ -95,33 +112,61 @@
     # Fitting
     log.info('Fitting...')
     t = Timer()
     t.start()
     actual_num_epochs = model.launch_training(trX, optimizer, loss_f, num_max_epochs, device, valX=valX,
                        batch_size=batch_size, save_every=save_every,
                        save_path=save_path, trY=trY, valY=valY,
-                       seed=seed, log_to_wandb=log_to_wandb, tol=tol)
+                       seed=seed, log_to_wandb=log_to_wandb, tol=tol,
+                       warmup_epochs=warmup_epochs, Q_inits=Q_inits)
+    deviances = utils.compute_deviances(model, valX, batch_size, device) if valX is not None else -1
     elapsed_time = t.stop()
-    if log_to_wandb:
-        wandb.run.summary['total_elapsed_time'] = elapsed_time
-        wandb.run.summary['avg_epoch_time'] = elapsed_time/actual_num_epochs
-    torch.save(model.state_dict(), save_path)
-    model.save_config(run_name, save_dir)
+    if not dry_run:
+        if log_to_wandb:
+            wandb.run.summary['total_elapsed_time'] = elapsed_time
+            wandb.run.summary['avg_epoch_time'] = elapsed_time/actual_num_epochs
+        torch.save(model.state_dict(), save_path)
+        model.save_config(run_name, save_dir)
     log.info('Optimization process finished.')
-    return model, device
+    return model, device, deviances
 
 def main(argv: List[str]):
     """Training entry point
     """
     args = utils.parse_train_args(argv)
     tr_file, val_file = args.data_path, args.validation_data_path
+    assert not (val_file and args.cv is not None), 'Cross-validation not available when validation data path is provided.'
     tr_pops_f, val_pops_f = args.populations_path, args.validation_populations_path
     trX, trY, valX, valY = utils.read_data(tr_file, val_file, tr_pops_f, val_pops_f)
-    model, device = fit_model(trX, args, valX, trY, valY)
+    """
+    if args.cv is not None:
+        log.info(f'Performing {args.cv}-fold cross-validation...')
+        cv_obj = KFold(n_splits=args.cv, random_state=args.seed, shuffle=True)
+        cv_errs = []
+        # TODO: TQDM or improve logging for cross-validation
+        for tr_idx, val_idx in cv_obj.split(trX):
+            with dask.config.set(**{'array.slicing.split_large_chunks': True}):
+                trX_curr, valX_curr = trX[tr_idx], trX[val_idx]
+            trY_curr = [trY[idx] for idx in tr_idx] if trY is not None else None
+            valY_curr = [trY[idx] for idx in val_idx] if trY is not None else None
+            model, device, deviance_curr = fit_model(trX_curr, args, valX_curr, trY_curr, valY_curr, dry_run=True)
+            cv_errs += [deviance_curr]
+
+        # TODO: wrap this in a function
+        cv_errs = pd.DataFrame.from_records(cv_errs)
+        cv_errs_reduced = pd.DataFrame(cv_errs.mean())
+        cv_errs_reduced["K"] = cv_errs_reduced.index.copy()
+        cv_errs_reduced.rename(columns={0: "cv_error_mean"}, inplace=True)
+        cv_errs_reduced["cv_error_std"] = cv_errs.std()
+        cv_errs_reduced = cv_errs_reduced.sort_values("K")
+    """
+    model, device, _ = fit_model(trX, args, valX, trY, valY)
     log.info('Computing divergences...')
     model.display_divergences()
+#     if args.cv:
+#         for _, row in cv_errs_reduced.iterrows():
+#             log.info(f"CV error (K={int(row['K'])}): {row['cv_error_mean']:.5f} ± {row['cv_error_std']:.3f}")
     log.info('Writing outputs...')
     utils.write_outputs(model, trX, valX, args.batch_size, device, args.name, args.save_dir)
     log.info('Exiting...')
     logging.shutdown()
     return 0
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neural-admixture-1.2.3b0/neural_admixture/src/utils.py` & `neural-admixture-1.3.0/neural_admixture/src/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 import os
 import sys
 import torch
 import wandb
 
 import dask.array as da
 from pathlib import Path
-from typing import List, Tuple, Union
+from typing import Dict, List, Tuple, Union
 
 from .snp_reader import SNPReader
 from ..model.neural_admixture import NeuralAdmixture
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 log = logging.getLogger(__name__)
 
 def parse_train_args(argv: List[str]):
     """Training arguments parser
     """
     parser = configargparse.ArgumentParser(prog='neural-admixture train',
                                            description='Rapid population clustering with autoencoders - training mode',
                                            config_file_parser_class=configargparse.YAMLConfigFileParser)
-    parser.add_argument('--learning_rate', required=False, default=0.0001, type=float, help='Learning rate')
+    parser.add_argument('--learning_rate', required=False, default=1e-5, type=float, help='Learning rate')
     parser.add_argument('--max_epochs', required=False, type=int, default=50, help='Maximum number of epochs')
-    parser.add_argument('--initialization', required=False, type=str, default = 'pcarchetypal',
+    parser.add_argument('--initialization', required=False, type=str, default = 'pckmeans',
                         choices=['pretrained', 'pckmeans', 'supervised', 'pcarchetypal'],
                         help='Decoder initialization (overriden if supervised)')
     parser.add_argument('--optimizer', required=False, default='adam', type=str, choices=['adam', 'sgd'], help='Optimizer')
     parser.add_argument('--save_every', required=False, default=10, type=int, help='Save checkpoint every this number of epochs')
     parser.add_argument('--l2_penalty', required=False, default=0.0005, type=float, help='L2 penalty on encoder weights')
     parser.add_argument('--activation', required=False, default='gelu', type=str, choices=['relu', 'tanh', 'gelu'], help='Activation function for encoder layers')
     parser.add_argument('--seed', required=False, type=int, default=42, help='Seed')
@@ -50,14 +50,16 @@
     parser.add_argument('--pca_components', required=False, type=int, default=2, help='Number of components to use for the PCKMeans initialization')
     parser.add_argument('--tol', required=False, type=float, default=1e-6, help='Convergence criterion: will stop when difference in objective function between two iterations is smaller than this')
     parser.add_argument('--save_dir', required=True, type=str, help='Save model in this directory')
     parser.add_argument('--data_path', required=True, type=str, help='Path containing the main data')
     parser.add_argument('--name', required=True, type=str, help='Experiment/model name')
     parser.add_argument('--batch_size', required=False, default=400, type=int, help='Batch size')
     parser.add_argument('--supervised_loss_weight', required=False, default=0.05, type=float, help='Weight given to the supervised loss')
+    parser.add_argument('--warmup_epochs', required=False, default=10, type=int, help='Number of warmup epochs to bring Q to a good initialization. Set to 0 to skip warmup.')
+    # parser.add_argument('--cv', required=False, default=None, type=int, help='Number of folds for cross-validation')
     return parser.parse_args(argv)
 
 def parse_infer_args(argv: List[str]):
     """Inference arguments parser
     """
     parser = argparse.ArgumentParser(prog='neural-admixture infer',
                                      description='Rapid population clustering with autoencoders - inference mode')
@@ -105,15 +107,15 @@
     Args:
         tr_file (str): denotes the path of the main data file
         val_file (str, optional): denotes the path of the validation data file. Defaults to None.
         tr_pops_f (str, optional): denotes the path containing the main populations file. Defaults to None.
         val_pops_f (str, optional): denotes the path containing the validation populations file. Defaults to None.
 
     Returns:
-        _type_: _description_
+        Tuple[da.core.Array, Union[None, da.core.Array], Union[None, List[str]], Union[None, List[str]]]: data objects
     """
     ''' 
     tr_file: string denoting the path of the main data file. The format of this file must be either HDF5 or VCF.
     val_file: optional. String denoting the path of the validation data file. The format of this file must be either HDF5 or VCF.
     tr_pops_f: optional. String denoting the path containing the main populations file. It must be a plain txt file where each row is a number specifying the population of the corresponding sample, as in ADMIXTURE.
     val_pops_f: optional. String denoting the path containing the validation populations file. It must be a plain txt file where each row is a number specifying the population of the corresponding sample, as in ADMIXTURE.
     '''
@@ -159,27 +161,50 @@
     Args:
         model (NeuralAdmixture): trained model object.
         data (da.core.Array): Dask array containing data to get results from.
         bsize (int): batch size.
         device (torch.device): torch device.
 
     Returns:
-        _type_: _description_
+        List[np.ndarray]: list of Q matrices
     """
     model.to(torch.device(device))
     outs = [torch.tensor([]) for _ in range(len(model.ks))]
     model.eval()
     with torch.inference_mode():
-        for X, _ in model.batch_generator(data, bsize, shuffle=False):
+        for X, _, _ in model.batch_generator(data, bsize, shuffle=False):
             X = X.to(device)
             out = model(X, True)
             for j in range(len(model.ks)):
                 outs[j] = torch.cat((outs[j], out[j].detach().cpu()), axis=0)
     return [out.cpu().numpy() for out in outs]
 
+def get_model_reconstructions(model: NeuralAdmixture, data: da.core.Array, bsize: int, device: torch.device) -> List[np.ndarray]:
+    """Helper function to run inference on data
+
+    Args:
+        model (NeuralAdmixture): trained model object.
+        data (da.core.Array): Dask array containing data to get results from.
+        bsize (int): batch size.
+        device (torch.device): torch device.
+
+    Returns:
+        List[np.ndarray]: list of reconstructions (matrix product of Q and P) for different Ks
+    """
+    model.to(torch.device(device))
+    outs = [torch.tensor([]) for _ in range(len(model.ks))]
+    model.eval()
+    with torch.inference_mode():
+        for X, _, _ in model.batch_generator(data, bsize, shuffle=False):
+            X = X.to(device)
+            out, _ = model(X)
+            for j in range(len(model.ks)):
+                outs[j] = torch.cat((outs[j], out[j].detach().cpu()), axis=0)
+    return [out.cpu().numpy() for out in outs]
+
 def write_outputs(model: NeuralAdmixture, trX: da.core.Array, valX: Union[da.core.Array, None],
                   bsize: int, device: torch.device, run_name: str, out_path: str, only_Q: bool=False) -> int:
     """Helper function to write Q and P matrices to disk
 
     Args:
         model (NeuralAdmixture): trained model object.
         trX (da.core.Array): Dask array containing training data.
@@ -204,7 +229,30 @@
         np.savetxt(out_path/f"{run_name}.{k}.Q", tr_preds[i], delimiter=' ')
     if valX is not None:
         val_preds = get_model_predictions(model, valX, bsize, device)
         for i, k in enumerate(model.ks):
             np.savetxt(out_path/f"{run_name}_validation.{k}.Q", val_preds[i], delimiter=' ')
     return 0
 
+def compute_deviances(model: NeuralAdmixture, data: da.core.Array, bsize: int, device: torch.device) -> Dict[int, float]:
+    """_summary_
+
+    Args:
+        model (NeuralAdmixture): _description_
+        trX (np.ndarray): _description_
+        bsize (int): _description_
+        device (torch.device): _description_
+
+    Returns:
+        Dict[int, float]: _description_
+    """
+    eps = 1e-7
+    reconstructions = get_model_reconstructions(model, data, bsize, device)
+    data_tmp = 2*data # Multiply by 2 to get to same reconstruction range to ADMIXTURE
+    data_tmp = da.clip(data_tmp, eps, 2-eps) # To avoid log(0)
+    deviances = {}
+    for rec, K in zip(reconstructions, model.ks):
+        rec *= 2 # Multiply by 2 to get to same reconstruction range to ADMIXTURE
+        rec = da.clip(rec, eps, 2-eps) # To avoid division by zero
+        deviance = (data_tmp * da.log(data_tmp/rec) + (2-data_tmp) * da.log((2-data_tmp)/(2-rec)))**2
+        deviances[K] = da.mean(deviance).compute()
+    return deviances
```

### Comparing `neural-admixture-1.2.3b0/neural_admixture.egg-info/PKG-INFO` & `neural-admixture-1.3.0/neural_admixture.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-admixture
-Version: 1.2.3b0
+Version: 1.3.0
 Summary: Rapid population clustering with autoencoders
 Home-page: https://github.com/AI-sandbox/neural-admixture
 Author: Albert Dominguez Mantes
 Author-email: albert.dominguezmantes@epfl.ch
 License: CC BY-NC 4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 ![PyPI - Status](https://img.shields.io/pypi/status/neural-admixture)
 [![tests](https://github.com/AI-sandbox/neural-admixture/workflows/tests/badge.svg)](https://github.com/AI-sandbox/neural-admixture/actions)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/neural-admixture)
 [![DOI](https://zenodo.org/badge/331290967.svg)](https://zenodo.org/badge/latestdoi/331290967)
 
 # Neural ADMIXTURE
 
-Neural ADMIXTURE is an unsupervised global ancestry inference technique based on ADMIXTURE. By using neural networks, Neural ADMIXTURE offers high quality ancestry assignments with a running time which is much faster than ADMIXTURE's. For more information, we recommend reading [the corresponding article](https://www.biorxiv.org/content/10.1101/2021.06.27.450081).
+Neural ADMIXTURE is an unsupervised global ancestry inference technique based on ADMIXTURE. By using neural networks, Neural ADMIXTURE offers high quality ancestry assignments with a running time which is much faster than ADMIXTURE's. For more information, we recommend reading [our corresponding article](https://www.nature.com/articles/s43588-023-00482-7).
 
 The software can be invoked via CLI and has a similar interface to ADMIXTURE (_e.g._ the output format is completely interchangeable). While the software runs in both CPU and GPU, we recommend using GPUs if available to take advantage of the neural network-based implementation.
 
 ![nadm_mna](https://github.com/AI-sandbox/neural-admixture/assets/31998088/048d04e2-8d62-4c14-870f-218e208dacb4)
 
 ## System requirements
 
@@ -42,75 +42,75 @@
 ### Software requirements
 
 The package has been tested on both Linux (CentOS 7.9.2009, Ubuntu 18.04.5 LTS) and MacOS (BigSur 11.2.3, Intel and Monterey 12.3.1, M1). If using GPUs, make sure CUDA drivers are properly installed.
 
 We recommend creating a fresh Python 3.9 environment using `virtualenv` (or `conda`), and then install the package `neural-admixture` there. As an example, for `virtualenv`, one should launch the following commands:
 
 ```console
-> virtualenv --python=python3.9 ~/venv/nadmenv
-> source ~/venv/nadmenv/bin/activate
-(nadmenv) > pip install neural-admixture
+$ virtualenv --python=python3.9 ~/venv/nadmenv
+$ source ~/venv/nadmenv/bin/activate
+(nadmenv) $ pip install neural-admixture
 ```
 
 ## Installation Guide
 
 The package can be easily installed in at most a few minutes using `pip` (make sure to add the `--upgrade` flag if updating the version):
 
 ```console
-(nadmenv) > pip install neural-admixture
+(nadmenv) $ pip install neural-admixture
 ```
 
 ## Usage 
 ### Running Neural ADMIXTURE
 
 To train a model from scratch, simply invoke the following commands from the root directory of the project. For more info about all the arguments, please run `neural-admixture train --help`. If training a single-head version of the network suffices, please use the flag `--k` instead of `--min_k` and `--max_k`. Note that VCF, BED, PGEN and HDF5 files are supported as of now. 
 
 For unsupervised Neural ADMIXTURE (single-head):
 
 ```console
-> neural-admixture train --k K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
+$ neural-admixture train --k K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
 ````
 
 For unsupervised Neural ADMIXTURE (multi-head):
 
 ```console
-> neural-admixture train --min_k MIN_K --max_k MAX_K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
+$ neural-admixture train --min_k MIN_K --max_k MAX_K --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH --init_file INIT_FILE
 ```
 
 For supervised Neural ADMIXTURE:
 
 ```console
-> neural-admixture train --k K --supervised --populations_path POPS_PATH --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH # only single-head support at the moment
+$ neural-admixture train --k K --supervised --populations_path POPS_PATH --name RUN_NAME --data_path DATA_PATH --save_dir SAVE_PATH # only single-head support at the moment
 ```
 
 As an example, the following ADMIXTURE call
 
 ```console
-> ./admixture snps_data.bed 8 -s 42
+$ ./admixture snps_data.bed 8 -s 42
 ```
 
 would be mimicked in Neural ADMIXTURE by running
 
 ```console
-> neural-admixture train --k 8 --data_path snps_data.bed --save_dir SAVE_PATH --init_file INIT_FILE --name snps_data --seed 42
+$ neural-admixture train --k 8 --data_path snps_data.bed --save_dir SAVE_PATH --init_file INIT_FILE --name snps_data --seed 42
 ```
 
 with some parameters such as the decoder initialization or the save directories not having a direct equivalent.
 
 Several files will be output to the `SAVE_PATH` directory (the `name` parameter will be used to create the whole filenames):
 - If the unsupervised version is run, a `Pickle` binary file containing the PCA object (using the `init_name` parameter), as well as an image file containing a PCA plot.
 - A `.P` file, similar to ADMIXTURE.
 - A `.Q` file, similar to ADMIXTURE.
 - A `.pt` file, containing the weights of the trained network.
 - A `.json` file, with the configuration of the network.
 
 The last two files are required to run posterior inference using the network, so be aware of not deleting them accidentally! Logs are printed to the `stdout` channel by default. If you want to save them to a file, you can use the command `tee` along with a pipe:
 
 ```console
-> neural-admixture train --k 8 ... | tee run.log
+$ neural-admixture train --k 8 ... | tee run.log
 ```
 
 ### Initialization method
 
 As described in the article, Neural ADMIXTURE's decoder(s) can be initialized using several methods, which will be indicated by the required `initialization` argument. The best-performing initialization method depends, mainly, on the structure of the data. The main options are:
 
 - `pckmeans`: initialize using PCK-Means (Algorithm 1 in the paper). Performs best if data contains a large number of single-ancestry individuals.
@@ -121,15 +121,15 @@
 ### Inference mode (projective analysis)
 
 ADMIXTURE allows reusing computations in the _projective analysis_ mode, in which the `P` (`F`, frequencies) matrix is fixed to an already known result and only the assignments are computed. Due to the nature of our algorithm, assignments can be computed for unseen data by simply feeding the data through the encoder. This mode can be run by typing `infer` instead of `train` right after the `neural-admixture` call.
 
 For example, assuming we have a trained Neural ADMIXTURE (named `nadm_test`) in the path `./outputs`, one could run inference on unseen data (`./data/unseen_data.vcf`) via the following command:
 
 ```console
-> neural-admixture infer --name nadm_test --save_dir ./outputs --out_name unseen_nadm_test --data_path ./data/unseen_data.vcf
+$ neural-admixture infer --name nadm_test --save_dir ./outputs --out_name unseen_nadm_test --data_path ./data/unseen_data.vcf
 ```
 
 For this command to work, files `./outputs/nadm_test.pt` and `./outputs/nadm_test_config.json`, which are training outputs, must exist. In this case, only a `.Q` will be created, which will contain the assignments for this data (the parameter of the flag `out_name` will be used to generate the output file name). This file will be written in the `--save_dir` directory (in this case, `./outputs`).
 
 ### Pretrained Neural ADMIXTURE
 
 As also mentioned in the paper, Neural ADMIXTURE can be used to learn a function (through the encoder) given the results of the frequency matrix `P`/`F` of another algorithm so out-of-training data inference can be performed using the structure learnt by the other algorithm. The following arguments should be used to run Neural ADMIXTURE in this mode:
@@ -163,35 +163,35 @@
 
 ## Using Plink2 binary files (.pgen)
 
 If the data format you will be working on is _Plink2 Binary Files (.pgen, .psam, .pvar)_ then you also need to install the package `pgenlib`. This package is not available in PyPi, but is included in the [plink repository](https://github.com/chrchang/plink-ng/tree/master/2.0/Python). Installation instructions can be found in the [corresponding `README.md` file](https://github.com/chrchang/plink-ng/blob/master/2.0/Python/ReadMe.md). While you will need to clone the whole repository, you can remove it after installing the package, unless you plan to work with it.
 
 ## Experiments replication
 
-The datasets _All-Chms_, _Chm-22_ and _Chm-22-Sim_ used in the Experiments section of the article can be found in [figshare](https://doi.org/10.6084/m9.figshare.19387538.v1). For descriptions of the datasets, please refer to the corresponding section in the paper. The exact hyperparameters used in the experiments to allow replication can be found in Appendix B of the article.
+The datasets _All-Chms_, _Chm-22_ and _Chm-22-Sim_ used in the Experiments section of the article can be found in [figshare](https://doi.org/10.6084/m9.figshare.19387538.v1). For descriptions of the datasets, please refer to the corresponding section in the paper. The exact hyperparameters used in the experiments to allow replication can be found in the Supplementary Table 3 of the article.
 
 ## Demo
 
 To run the software with a small demo dataset, check the instructions in [the corresponding folder of the repository](https://github.com/AI-sandbox/neural-admixture/tree/main/demo).
 
 ## License
 
 **NOTICE**: This software is available for use free of charge for academic research use only. Academic users may fork this repository and modify and improve to suit their research needs, but also inherit these terms and must include a licensing notice to that effect. Commercial users, for profit companies or consultants, and non-profit institutions not qualifying as "academic research" should contact the authors for a separate license. This applies to this repository directly and any other repository that includes source, executables, or git commands that pull/clone this repository as part of its function. Such repositories, whether ours or others, must include this notice.
 
 ## Cite
 
-When using this software, please cite the following paper (currently pre-print):
+When using this software, please cite the following paper:
 
 ```{tex}
-@article {Mantes2021.06.27.450081,
-	author = {Mantes, Albert Dominguez and Montserrat, Daniel Mas and Bustamante, Carlos D. and Gir{\'o}-i-Nieto, Xavier and Ioannidis, Alexander G.},
-	title = {Neural ADMIXTURE: rapid population clustering with autoencoders},
-	elocation-id = {2021.06.27.450081},
-	year = {2022},
-	doi = {10.1101/2021.06.27.450081},
-	publisher = {Cold Spring Harbor Laboratory},
-	abstract = {Characterizing the genetic substructure of large cohorts has become increasingly important as genetic association and prediction studies are extended to massive, increasingly diverse, biobanks. ADMIXTURE and STRUCTURE are widely used unsupervised clustering algorithms for characterizing such ancestral genetic structure. These methods decompose individual genomes into fractional cluster assignments with each cluster representing a vector of DNA marker frequencies. The assignments, and clusters, provide an interpretable representation for geneticists to describe population substructure at the sample level. However, with the rapidly increasing size of population biobanks and the growing numbers of variants genotyped (or sequenced) per sample, such traditional methods become computationally intractable. Furthermore, multiple runs with different hyperparameters are required to properly depict the population clustering using these traditional methods, increasing the computational burden. This can lead to days of compute. In this work we present Neural ADMIXTURE, a neural network autoencoder that follows the same modeling assumptions as ADMIXTURE, providing similar (or better) clustering, while reducing the compute time by orders of magnitude. Indeed, the equivalent of one month of continuous compute can be reduced to hours. In addition, Neural ADMIXTURE can include multiple outputs, providing the equivalent results as running the original ADMIXTURE algorithm many times with different numbers of clusters. Our models can also be stored, allowing later cluster assignment to be performed with a linear computational time. The software implementation of Neural ADMIXTURE can be found at https://github.com/ai-sandbox/neural-admixture.},
-	URL = {https://www.biorxiv.org/content/early/2022/01/14/2021.06.27.450081},
-	eprint = {https://www.biorxiv.org/content/early/2022/01/14/2021.06.27.450081.full.pdf},
-	journal = {bioRxiv}
-}
+@article{dominguezmantes23,
+	abstract = {Characterizing the genetic structure of large cohorts has become increasingly important as genetic studies extend to massive, increasingly diverse biobanks. Popular methods decompose individual genomes into fractional cluster assignments with each cluster representing a vector of DNA variant frequencies. However, with rapidly increasing biobank sizes, these methods have become computationally intractable. Here we present Neural ADMIXTURE, a neural network autoencoder that follows the same modeling assumptions as the current standard algorithm, ADMIXTURE, while reducing the compute time by orders of magnitude surpassing even the fastest alternatives. One month of continuous compute using ADMIXTURE can be reduced to just hours with Neural ADMIXTURE. A multi-head approach allows Neural ADMIXTURE to offer even further acceleration by computing multiple cluster numbers in a single run. Furthermore, the models can be stored, allowing cluster assignment to be performed on new data in linear time without needing to share the training samples.},
+	author = {Dominguez Mantes, Albert and Mas Montserrat, Daniel and Bustamante, Carlos D. and Gir{\'o}-i-Nieto, Xavier and Ioannidis, Alexander G.},
+	doi = {10.1038/s43588-023-00482-7},
+	id = {Dominguez Mantes2023},
+	isbn = {2662-8457},
+	journal = {Nature Computational Science},
+	title = {Neural ADMIXTURE for rapid genomic clustering},
+	url = {https://doi.org/10.1038/s43588-023-00482-7},
+	year = {2023},
+	bdsk-url-1 = {https://doi.org/10.1038/s43588-023-00482-7}}
+
 ```
```

### Comparing `neural-admixture-1.2.3b0/neural_admixture.egg-info/SOURCES.txt` & `neural-admixture-1.3.0/neural_admixture.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-admixture-1.2.3b0/setup.cfg` & `neural-admixture-1.3.0/setup.cfg`

 * *Files identical despite different names*

