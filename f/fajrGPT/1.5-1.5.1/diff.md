# Comparing `tmp/fajrGPT-1.5.tar.gz` & `tmp/fajrGPT-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.5.tar", last modified: Mon Jul 31 02:20:01 2023, max compression
+gzip compressed data, was "fajrGPT-1.5.1.tar", last modified: Mon Jul 31 02:37:49 2023, max compression
```

## Comparing `fajrGPT-1.5.tar` & `fajrGPT-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:20:01.658887 fajrGPT-1.5/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-31 02:20:01.658708 fajrGPT-1.5/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:20:01.656663 fajrGPT-1.5/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    20575 2023-07-31 02:14:44.000000 fajrGPT-1.5/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:20:01.658509 fajrGPT-1.5/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       62 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-31 02:20:01.658926 fajrGPT-1.5/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1146 2023-07-31 02:19:24.000000 fajrGPT-1.5/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:37:49.671103 fajrGPT-1.5.1/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5.1/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-31 02:37:49.670929 fajrGPT-1.5.1/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5.1/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:37:49.669451 fajrGPT-1.5.1/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5.1/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5.1/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    20600 2023-07-31 02:24:50.000000 fajrGPT-1.5.1/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:37:49.670729 fajrGPT-1.5.1/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-31 02:37:49.000000 fajrGPT-1.5.1/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-31 02:37:49.000000 fajrGPT-1.5.1/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-31 02:37:49.000000 fajrGPT-1.5.1/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-31 02:37:49.000000 fajrGPT-1.5.1/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       62 2023-07-31 02:37:49.000000 fajrGPT-1.5.1/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-31 02:37:49.000000 fajrGPT-1.5.1/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-31 02:37:49.671146 fajrGPT-1.5.1/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1148 2023-07-31 02:34:59.000000 fajrGPT-1.5.1/setup.py
```

### Comparing `fajrGPT-1.5/LICENSE` & `fajrGPT-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5/PKG-INFO` & `fajrGPT-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5
+Version: 1.5.1
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5/README.md` & `fajrGPT-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5/fajrGPT/quran_metadata.py` & `fajrGPT-1.5.1/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.5/fajrGPT/wake.py` & `fajrGPT-1.5.1/fajrGPT/wake.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     # Check surah option
     if surah:
         # make the output file name the same as the surah
         output = 'quran-' + '{:03d}'.format(int(surah))
         if not english:
             flag = download_surah(surah, output)
         else:
+            output += '-english'
             flag = download_surah_with_english(surah, output)
     else:
         # Download video
         flag = download_video(url, output)
 
     # test audio
     test_audio(f'{output}.mp3',output,flag)
@@ -94,15 +95,15 @@
         file_path = download_file_and_sleep(url,0.5)
 
         # combine the audio files
         combined_audio = AudioSegment.empty()
         combined_audio += AudioSegment.from_mp3(file_path)
 
         # save the combined audio file
-        combined_audio.export(f'{output}-english.mp3', format="mp3")
+        combined_audio.export(f'{output}.mp3', format="mp3")
 
         # return False
         return False
 
 def download_surah(surah, output):
     # check if the output file already exists
     if os.path.exists(f'{output}.mp3'):
```

### Comparing `fajrGPT-1.5/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.5.1/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.5
+Version: 1.5.1
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.5/setup.py` & `fajrGPT-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.5",
+    version="1.5.1",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

