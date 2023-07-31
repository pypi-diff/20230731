# Comparing `tmp/pyPPG-1.0.2.tar.gz` & `tmp/pyPPG-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPPG-1.0.2.tar", last modified: Thu Jul 27 15:38:56 2023, max compression
+gzip compressed data, was "pyPPG-1.0.3.tar", last modified: Mon Jul 31 07:41:09 2023, max compression
```

## Comparing `pyPPG-1.0.2.tar` & `pyPPG-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:56.005346 pyPPG-1.0.2/
--rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      619 2023-07-27 15:38:56.005346 pyPPG-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3415 2023-07-27 14:35:58.000000 pyPPG-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:55.989700 pyPPG-1.0.2/pyPPG/
--rw-rw-rw-   0        0        0     3194 2023-07-26 11:45:26.000000 pyPPG-1.0.2/pyPPG/Biomarkers.py
--rw-rw-rw-   0        0        0     9372 2023-07-27 08:33:09.000000 pyPPG-1.0.2/pyPPG/DataHandling.py
--rw-rw-rw-   0        0        0     2145 2023-07-27 09:19:15.000000 pyPPG-1.0.2/pyPPG/EXAMPLE.py
--rw-rw-rw-   0        0        0    49759 2023-07-27 08:52:59.000000 pyPPG-1.0.2/pyPPG/FiducialPoints.py
--rw-rw-rw-   0        0        0     1845 2023-07-27 08:06:54.000000 pyPPG-1.0.2/pyPPG/Preprocessing.py
--rw-rw-rw-   0        0        0     1906 2023-07-26 12:38:04.000000 pyPPG-1.0.2/pyPPG/Statistics.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.2/pyPPG/__init__.py
--rw-rw-rw-   0        0        0     4945 2023-07-23 15:56:13.000000 pyPPG-1.0.2/pyPPG/ppgSQI.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:56.005346 pyPPG-1.0.2/pyPPG/ppg_bm/
--rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.2/pyPPG/ppg_bm/__init__.py
--rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_biomarkers.py
--rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_derivs_ratios.py
--rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_derivs.py
--rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_sig.py
--rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_sig_ratios.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:38:56.005346 pyPPG-1.0.2/pyPPG.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 15:38:55.000000 pyPPG-1.0.2/pyPPG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 15:38:56.005346 pyPPG-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-07-27 15:38:28.000000 pyPPG-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.200176 pyPPG-1.0.3/
+-rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      619 2023-07-31 07:41:09.200176 pyPPG-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3415 2023-07-27 14:35:58.000000 pyPPG-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.172618 pyPPG-1.0.3/pyPPG/
+-rw-rw-rw-   0        0        0     3194 2023-07-26 11:45:26.000000 pyPPG-1.0.3/pyPPG/Biomarkers.py
+-rw-rw-rw-   0        0        0    19510 2023-07-31 07:08:30.000000 pyPPG-1.0.3/pyPPG/DataHandling.py
+-rw-rw-rw-   0        0        0     2204 2023-07-30 08:11:19.000000 pyPPG-1.0.3/pyPPG/EXAMPLE.py
+-rw-rw-rw-   0        0        0    49745 2023-07-30 11:49:30.000000 pyPPG-1.0.3/pyPPG/FiducialPoints.py
+-rw-rw-rw-   0        0        0     1845 2023-07-27 08:06:54.000000 pyPPG-1.0.3/pyPPG/Preprocessing.py
+-rw-rw-rw-   0        0        0     1906 2023-07-26 12:38:04.000000 pyPPG-1.0.3/pyPPG/Statistics.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.3/pyPPG/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.193787 pyPPG-1.0.3/pyPPG/pack_ppg/
+-rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.3/pyPPG/pack_ppg/_ErrorHandler.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.3/pyPPG/pack_ppg/__init__.py
+-rw-rw-rw-   0        0        0     4945 2023-07-23 15:56:13.000000 pyPPG-1.0.3/pyPPG/ppgSQI.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.198837 pyPPG-1.0.3/pyPPG/ppg_bm/
+-rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.3/pyPPG/ppg_bm/__init__.py
+-rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_biomarkers.py
+-rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_derivs_ratios.py
+-rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_derivs.py
+-rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_sig.py
+-rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_sig_ratios.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.192159 pyPPG-1.0.3/pyPPG.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 07:41:09.200176 pyPPG-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      962 2023-07-31 07:39:37.000000 pyPPG-1.0.3/setup.py
```

### Comparing `pyPPG-1.0.2/LICENSE.txt` & `pyPPG-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/PKG-INFO` & `pyPPG-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.2
+Version: 1.0.3
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `pyPPG-1.0.2/README.md` & `pyPPG-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/Biomarkers.py` & `pyPPG-1.0.3/pyPPG/Biomarkers.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/EXAMPLE.py` & `pyPPG-1.0.3/pyPPG/EXAMPLE.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from Statistics import*
 
 import matplotlib.pyplot as plt
 import numpy as np
 from dotmap import DotMap
 import time
 
+import sys
+
 ###########################################################################
 ################################## EXAMPLE ################################
 ###########################################################################
 def example_code(filtering=True,correct=True,savefig=True):
     '''
     This is an example code for PPG analysis. The main parts:
         1) Loading a raw PPG signal: various file formats such as .mat, .csv, .txt, or .edf.
@@ -27,14 +29,16 @@
         6) Save data: save the extracted Fiducial points, Biomarkers, and Statistics into .csv file
 
     :param filtering: a bool for filtering
     :param savefig: a bool for fiducial points saving
     :param correct: a bool for fiducials points corretion
     '''
 
+    python_executable_path = sys.executable
+
     ## Loading a raw PPG signal
     s=load_data(filtering)
 
     ## Get Fiducial points
     fp = Fp.FiducialPoints(s)
     fiducials=fp.getFiducialPoints(correct)
 
@@ -54,8 +58,8 @@
     print('Program finished')
 
 
 
 ###########################################################################
 ############################## RUN EXAMPLE CODE ###########################
 ###########################################################################
-# example_code()
+example_code()
```

### Comparing `pyPPG-1.0.2/pyPPG/FiducialPoints.py` & `pyPPG-1.0.3/pyPPG/FiducialPoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 
     ###########################################################################
     ############################ PPG beat detector ############################
     ###########################################################################
     def abdp_beat_detector(self, peak_detector: str):
         '''ABDP_BEAT_DETECTOR detects beats in a photoplethysmogram (PPG) signal
-        using the improved 'Automatic Beat Detection' beat detector of Aboy M et al.
+        using the improved 'Automatic Beat Detection' of Aboy M et al.
 
         :param peak_detector: type of peak detector
         :type peak_detector: str
 
         :return:
             - peaks, 1-d array: indices of detected systolic peaks
             - onsets, 1-d array: indices of detected pulse onsets
```

### Comparing `pyPPG-1.0.2/pyPPG/Preprocessing.py` & `pyPPG-1.0.3/pyPPG/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/Statistics.py` & `pyPPG-1.0.3/pyPPG/Statistics.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/ppgSQI.py` & `pyPPG-1.0.3/pyPPG/ppgSQI.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/ppg_bm/get_biomarkers.py` & `pyPPG-1.0.3/pyPPG/ppg_bm/get_biomarkers.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_derivs_ratios.py` & `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_derivs_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_derivs.py` & `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_derivs.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_ppg_sig.py` & `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_sig.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG/ppg_bm/get_bm_sig_ratios.py` & `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_sig_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.2/pyPPG.egg-info/PKG-INFO` & `pyPPG-1.0.3/pyPPG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.2
+Version: 1.0.3
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `pyPPG-1.0.2/pyPPG.egg-info/SOURCES.txt` & `pyPPG-1.0.3/pyPPG.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,13 +12,15 @@
 pyPPG/__init__.py
 pyPPG/ppgSQI.py
 pyPPG.egg-info/PKG-INFO
 pyPPG.egg-info/SOURCES.txt
 pyPPG.egg-info/dependency_links.txt
 pyPPG.egg-info/requires.txt
 pyPPG.egg-info/top_level.txt
+pyPPG/pack_ppg/_ErrorHandler.py
+pyPPG/pack_ppg/__init__.py
 pyPPG/ppg_bm/__init__.py
 pyPPG/ppg_bm/get_biomarkers.py
 pyPPG/ppg_bm/get_bm_derivs_ratios.py
 pyPPG/ppg_bm/get_bm_ppg_derivs.py
 pyPPG/ppg_bm/get_bm_ppg_sig.py
 pyPPG/ppg_bm/get_bm_sig_ratios.py
```

### Comparing `pyPPG-1.0.2/setup.py` & `pyPPG-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyPPG',
-    version='1.0.2',
+    version='1.0.3',
     description='pyPPG: a python toolbox for PPG morphological analysis.',
     author='Marton A. Goda, PhD',
     author_email="marton.goda@campus.technion.ac.il",
     long_description=0,
     long_description_content_type="text/markdown",
     url="https://github.com/godamartonaron/GODA_pyPPG",
     project_urls={"Bug Tracker": "https://github.com/pypa/sampleproject/issues",},
-    packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
     ],
-    package_data={'GODA_pyPPG':['docs/*']},
+    packages={"pyPPG", "pyPPG/ppg_bm", "pyPPG/pack_ppg"},
+    package_data={
+        "pyPPG": ["*"],
+        "pyPPG/ppg_bm": ["*"],
+        "pyPPG/pack_ppg": ["*"],
+    },
+
     install_requires=["numpy", "mne"],
     python_requires=">=3.10",
     include_package_data=True,
-
 )
```

