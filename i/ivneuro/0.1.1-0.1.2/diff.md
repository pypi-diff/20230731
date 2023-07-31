# Comparing `tmp/ivneuro-0.1.1.tar.gz` & `tmp/ivneuro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivneuro-0.1.1.tar", last modified: Mon Jul 31 14:13:10 2023, max compression
+gzip compressed data, was "ivneuro-0.1.2.tar", last modified: Mon Jul 31 14:17:23 2023, max compression
```

## Comparing `ivneuro-0.1.1.tar` & `ivneuro-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:13:10.001462 ivneuro-0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-07-12 14:04:04.000000 ivneuro-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-07-28 10:39:06.000000 ivneuro-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4792 2023-07-31 14:13:10.001462 ivneuro-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4378 2023-07-31 12:20:46.000000 ivneuro-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 14:13:09.954557 ivneuro-0.1.1/ivneuro/
--rw-rw-rw-   0        0        0     1079 2023-07-31 12:58:45.000000 ivneuro-0.1.1/ivneuro/__init__.py
--rw-rw-rw-   0        0        0    13085 2023-07-31 07:04:20.000000 ivneuro-0.1.1/ivneuro/continuous.py
--rw-rw-rw-   0        0        0     5887 2023-07-31 06:55:24.000000 ivneuro-0.1.1/ivneuro/delta_coherence.py
--rw-rw-rw-   0        0        0     3758 2023-07-31 06:55:29.000000 ivneuro-0.1.1/ivneuro/delta_coherence_core.py
--rw-rw-rw-   0        0        0     6077 2023-07-31 06:54:24.000000 ivneuro-0.1.1/ivneuro/delta_power_spectral.py
--rw-rw-rw-   0        0        0     2314 2023-07-06 09:22:48.000000 ivneuro-0.1.1/ivneuro/delta_power_spectral_core.py
--rw-rw-rw-   0        0        0     2279 2023-07-06 13:32:35.000000 ivneuro-0.1.1/ivneuro/events.py
--rw-rw-rw-   0        0        0     1938 2023-07-31 10:00:47.000000 ivneuro-0.1.1/ivneuro/generate_signal.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:13:10.001462 ivneuro-0.1.1/ivneuro/nex/
--rw-rw-rw-   0        0        0     5604 2023-07-31 07:12:02.000000 ivneuro-0.1.1/ivneuro/nex/NexData.py
--rw-rw-rw-   0        0        0      568 2023-07-31 07:21:14.000000 ivneuro-0.1.1/ivneuro/nex/__init__.py
--rw-rw-rw-   0        0        0    51441 2022-11-18 15:23:48.000000 ivneuro-0.1.1/ivneuro/nex/nexfile.py
--rw-rw-rw-   0        0        0    10097 2023-07-10 09:01:59.000000 ivneuro-0.1.1/ivneuro/nex/pull_nex_data.py
--rw-rw-rw-   0        0        0    25686 2023-07-31 06:52:47.000000 ivneuro-0.1.1/ivneuro/spectograms.py
--rw-rw-rw-   0        0        0     3580 2023-07-31 06:53:01.000000 ivneuro-0.1.1/ivneuro/spectograms_core.py
--rw-rw-rw-   0        0        0    12948 2023-07-31 10:39:54.000000 ivneuro-0.1.1/ivneuro/tracking.py
--rw-rw-rw-   0        0        0     2788 2023-07-31 07:08:15.000000 ivneuro-0.1.1/ivneuro/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:13:09.985843 ivneuro-0.1.1/ivneuro.egg-info/
--rw-rw-rw-   0        0        0     4792 2023-07-31 14:13:09.000000 ivneuro-0.1.1/ivneuro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-07-31 14:13:09.000000 ivneuro-0.1.1/ivneuro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:13:09.000000 ivneuro-0.1.1/ivneuro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-31 14:13:09.000000 ivneuro-0.1.1/ivneuro.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 14:13:09.000000 ivneuro-0.1.1/ivneuro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 14:13:10.001462 ivneuro-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      925 2023-07-31 13:58:28.000000 ivneuro-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:17:23.116002 ivneuro-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-07-12 14:04:04.000000 ivneuro-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-07-28 10:39:06.000000 ivneuro-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4792 2023-07-31 14:17:23.116002 ivneuro-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4378 2023-07-31 14:15:59.000000 ivneuro-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 14:17:23.084749 ivneuro-0.1.2/ivneuro/
+-rw-rw-rw-   0        0        0     1079 2023-07-31 12:58:45.000000 ivneuro-0.1.2/ivneuro/__init__.py
+-rw-rw-rw-   0        0        0    13085 2023-07-31 07:04:20.000000 ivneuro-0.1.2/ivneuro/continuous.py
+-rw-rw-rw-   0        0        0     5887 2023-07-31 06:55:24.000000 ivneuro-0.1.2/ivneuro/delta_coherence.py
+-rw-rw-rw-   0        0        0     3758 2023-07-31 06:55:29.000000 ivneuro-0.1.2/ivneuro/delta_coherence_core.py
+-rw-rw-rw-   0        0        0     6077 2023-07-31 06:54:24.000000 ivneuro-0.1.2/ivneuro/delta_power_spectral.py
+-rw-rw-rw-   0        0        0     2314 2023-07-06 09:22:48.000000 ivneuro-0.1.2/ivneuro/delta_power_spectral_core.py
+-rw-rw-rw-   0        0        0     2279 2023-07-06 13:32:35.000000 ivneuro-0.1.2/ivneuro/events.py
+-rw-rw-rw-   0        0        0     1938 2023-07-31 10:00:47.000000 ivneuro-0.1.2/ivneuro/generate_signal.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:17:23.116002 ivneuro-0.1.2/ivneuro/nex/
+-rw-rw-rw-   0        0        0     5604 2023-07-31 07:12:02.000000 ivneuro-0.1.2/ivneuro/nex/NexData.py
+-rw-rw-rw-   0        0        0      568 2023-07-31 07:21:14.000000 ivneuro-0.1.2/ivneuro/nex/__init__.py
+-rw-rw-rw-   0        0        0    51441 2022-11-18 15:23:48.000000 ivneuro-0.1.2/ivneuro/nex/nexfile.py
+-rw-rw-rw-   0        0        0    10097 2023-07-10 09:01:59.000000 ivneuro-0.1.2/ivneuro/nex/pull_nex_data.py
+-rw-rw-rw-   0        0        0    25686 2023-07-31 06:52:47.000000 ivneuro-0.1.2/ivneuro/spectograms.py
+-rw-rw-rw-   0        0        0     3580 2023-07-31 06:53:01.000000 ivneuro-0.1.2/ivneuro/spectograms_core.py
+-rw-rw-rw-   0        0        0    12948 2023-07-31 10:39:54.000000 ivneuro-0.1.2/ivneuro/tracking.py
+-rw-rw-rw-   0        0        0     2788 2023-07-31 07:08:15.000000 ivneuro-0.1.2/ivneuro/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:17:23.100374 ivneuro-0.1.2/ivneuro.egg-info/
+-rw-rw-rw-   0        0        0     4792 2023-07-31 14:17:22.000000 ivneuro-0.1.2/ivneuro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-07-31 14:17:23.000000 ivneuro-0.1.2/ivneuro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:17:22.000000 ivneuro-0.1.2/ivneuro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-31 14:17:22.000000 ivneuro-0.1.2/ivneuro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 14:17:22.000000 ivneuro-0.1.2/ivneuro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:17:23.116002 ivneuro-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      925 2023-07-31 14:16:28.000000 ivneuro-0.1.2/setup.py
```

### Comparing `ivneuro-0.1.1/LICENSE` & `ivneuro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/PKG-INFO` & `ivneuro-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivneuro
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for processing and analyzing neurophysiological signals recorded in-vivo.
 Home-page: https://github.com/casey-e/ivneuro
 Author: Eric Casey
 Author-email: e.toccalino@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/casey-e/ivneuro
 Requires-Python: >=3.11.3
@@ -138,11 +138,11 @@
 >>> pos = ivn.EventPosition(x, y, timestamps, event)
 >>> pos.plot()
 ```
 ![image](https://github.com/casey-e/ivneuro/assets/92745842/e76b65fa-c361-4897-bc85-bfab1cc7620e)
 
 <br>
 
-Licence
+License
 -------
 The codes are released under [MIT License](https://mit-license.org/)
```

### Comparing `ivneuro-0.1.1/README.md` & `ivneuro-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -125,11 +125,11 @@
 >>> pos = ivn.EventPosition(x, y, timestamps, event)
 >>> pos.plot()
 ```
 ![image](https://github.com/casey-e/ivneuro/assets/92745842/e76b65fa-c361-4897-bc85-bfab1cc7620e)
 
 <br>
 
-Licence
+License
 -------
 The codes are released under [MIT License](https://mit-license.org/)
```

### Comparing `ivneuro-0.1.1/ivneuro/__init__.py` & `ivneuro-0.1.2/ivneuro/__init__.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/continuous.py` & `ivneuro-0.1.2/ivneuro/continuous.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/delta_coherence.py` & `ivneuro-0.1.2/ivneuro/delta_coherence.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/delta_coherence_core.py` & `ivneuro-0.1.2/ivneuro/delta_coherence_core.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/delta_power_spectral.py` & `ivneuro-0.1.2/ivneuro/delta_power_spectral.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/delta_power_spectral_core.py` & `ivneuro-0.1.2/ivneuro/delta_power_spectral_core.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/events.py` & `ivneuro-0.1.2/ivneuro/events.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/generate_signal.py` & `ivneuro-0.1.2/ivneuro/generate_signal.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/nex/NexData.py` & `ivneuro-0.1.2/ivneuro/nex/NexData.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/nex/__init__.py` & `ivneuro-0.1.2/ivneuro/nex/__init__.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/nex/nexfile.py` & `ivneuro-0.1.2/ivneuro/nex/nexfile.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/nex/pull_nex_data.py` & `ivneuro-0.1.2/ivneuro/nex/pull_nex_data.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/spectograms.py` & `ivneuro-0.1.2/ivneuro/spectograms.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/spectograms_core.py` & `ivneuro-0.1.2/ivneuro/spectograms_core.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/tracking.py` & `ivneuro-0.1.2/ivneuro/tracking.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro/utils.py` & `ivneuro-0.1.2/ivneuro/utils.py`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/ivneuro.egg-info/PKG-INFO` & `ivneuro-0.1.2/ivneuro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ivneuro
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for processing and analyzing neurophysiological signals recorded in-vivo.
 Home-page: https://github.com/casey-e/ivneuro
 Author: Eric Casey
 Author-email: e.toccalino@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/casey-e/ivneuro
 Requires-Python: >=3.11.3
@@ -138,11 +138,11 @@
 >>> pos = ivn.EventPosition(x, y, timestamps, event)
 >>> pos.plot()
 ```
 ![image](https://github.com/casey-e/ivneuro/assets/92745842/e76b65fa-c361-4897-bc85-bfab1cc7620e)
 
 <br>
 
-Licence
+License
 -------
 The codes are released under [MIT License](https://mit-license.org/)
```

### Comparing `ivneuro-0.1.1/ivneuro.egg-info/SOURCES.txt` & `ivneuro-0.1.2/ivneuro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ivneuro-0.1.1/setup.py` & `ivneuro-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,13 +14,13 @@
     author_email = 'e.toccalino@gmail.com',
     description="Tools for processing and analyzing neurophysiological signals recorded in-vivo.",
     name="ivneuro",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(include=["ivneuro", "ivneuro.*"]),
     license='MIT',
-    version="0.1.1",
+    version="0.1.2",
     install_requires = ['numpy >= 1.24.1','pandas >= 2.0.1', 'matplotlib >= 3.6.2','scipy >= 1.10'],
     python_requires = '>=3.11.3',
     project_urls = {'Homepage':'https://github.com/casey-e/ivneuro'},
     url = 'https://github.com/casey-e/ivneuro',
 )
```

