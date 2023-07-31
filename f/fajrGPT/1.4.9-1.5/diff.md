# Comparing `tmp/fajrGPT-1.4.9.tar.gz` & `tmp/fajrGPT-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.4.9.tar", last modified: Sat Jul 29 13:33:59 2023, max compression
+gzip compressed data, was "fajrGPT-1.5.tar", last modified: Mon Jul 31 02:20:01 2023, max compression
```

## Comparing `fajrGPT-1.4.9.tar` & `fajrGPT-1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-29 13:33:59.644154 fajrGPT-1.4.9/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.9/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-29 13:33:59.643975 fajrGPT-1.4.9/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.9/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-29 13:33:59.642021 fajrGPT-1.4.9/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.9/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.9/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    19713 2023-07-29 13:12:25.000000 fajrGPT-1.4.9/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-29 13:33:59.643757 fajrGPT-1.4.9/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       62 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-29 13:33:59.000000 fajrGPT-1.4.9/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-29 13:33:59.644197 fajrGPT-1.4.9/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1148 2023-07-29 13:27:37.000000 fajrGPT-1.4.9/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:20:01.658887 fajrGPT-1.5/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.5/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-31 02:20:01.658708 fajrGPT-1.5/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.5/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:20:01.656663 fajrGPT-1.5/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.5/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     4095 2023-07-31 02:16:34.000000 fajrGPT-1.5/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    20575 2023-07-31 02:14:44.000000 fajrGPT-1.5/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-31 02:20:01.658509 fajrGPT-1.5/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2944 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       62 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-31 02:20:01.000000 fajrGPT-1.5/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-31 02:20:01.658926 fajrGPT-1.5/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1146 2023-07-31 02:19:24.000000 fajrGPT-1.5/setup.py
```

### Comparing `fajrGPT-1.4.9/LICENSE` & `fajrGPT-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.9/PKG-INFO` & `fajrGPT-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.9
+Version: 1.5
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.9/README.md` & `fajrGPT-1.5/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.9/fajrGPT/wake.py` & `fajrGPT-1.5/fajrGPT/wake.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys; sys.path.append('./')
 import click
 import youtube_dl
 import pygame
 from pydub import AudioSegment
 from threading import Thread
-from fajrGPT.quran_metadata import quran_chapter_to_verse
+from fajrGPT.quran_metadata import quran_chapter_to_verse, surah_number_to_name_tag
 import time
 import subprocess
 import requests
 import openai
 import random
 import tempfile
 import mutagen.mp3 as mp3
@@ -22,22 +22,25 @@
 @click.command()
 @click.option('--url', required=True, help='YouTube URL containing desired audio data.')
 @click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
 @click.option('--output', required=True, help='Name of the output file.')
 @click.option('--names-flag', required=False, help='Whether or not to include a randomly selected name of Allah in the preamble.', default=True)
 @click.option('--transition-time', required=False, help='Time in seconds for the transition between the output audio and the Quran verses.', default=600)
 @click.option('--surah', required=False, help='Specific Surah from the Quran. Should be given as integer.')
-# TODO: add option for including english translation of each surah if the user selects the surah option. Perhaps use a natural language generation model to generate the translation from the english translation of the Quran verses.
+@click.option('--english', required=False, help='Whether or not to play audio with the english translation of the Quran verses. Note this option only applies if the --surah option is not None.', default=False)
 
-def main(url, time, output, names_flag, transition_time=600, surah=None):
+def main(url, time, output, names_flag, transition_time=600, surah=None, english=False):
     # Check surah option
     if surah:
         # make the output file name the same as the surah
         output = 'quran-' + '{:03d}'.format(int(surah))
-        flag = download_surah(surah, output)
+        if not english:
+            flag = download_surah(surah, output)
+        else:
+            flag = download_surah_with_english(surah, output)
     else:
         # Download video
         flag = download_video(url, output)
 
     # test audio
     test_audio(f'{output}.mp3',output,flag)
 
@@ -74,14 +77,36 @@
 
     # stop the audio once the user has completed reading the verses
     stop_audio()
 
     # return back to the main thread
     play_audio_thread.join()
 
+def download_surah_with_english(surah, output):
+    # check if the output file already exists
+    if os.path.exists(f'{output}.mp3'):
+        # if the output file exists, then return True
+        return True
+    else:        
+        # get the url directly from thechosenone.info
+        url = quran_surah_with_english_to_mp3_url(surah)
+
+        # download the verse audio and sleep for 0.5 seconds between each download
+        file_path = download_file_and_sleep(url,0.5)
+
+        # combine the audio files
+        combined_audio = AudioSegment.empty()
+        combined_audio += AudioSegment.from_mp3(file_path)
+
+        # save the combined audio file
+        combined_audio.export(f'{output}-english.mp3', format="mp3")
+
+        # return False
+        return False
+
 def download_surah(surah, output):
     # check if the output file already exists
     if os.path.exists(f'{output}.mp3'):
         # if the output file exists, then return True
         return True
     else:
         # obtain the number of verses in the surah
@@ -107,21 +132,14 @@
 
     return True    
 
 def play_quran_verses_audio(verses,transition_time=0.5):
     # convert verses to urls
     urls = [quran_verse_to_mp3_url(verse) for verse in verses]
 
-    # TODO: find mp3 url for the english translation of each verse and append it to the urls list depending on an option the user selects
-    # if include_english_translation:
-    ## if insert_translation_after_verse:
-    ### urls.append(english_translation_url)
-    ## elif insert_translation_within_verse:
-    ### urls.insert(1,english_translation_url)
-
     # download the verse audio
     file_paths = [download_file_and_sleep(url,0.5) for url in urls]
 
     # concatenate the audio files into one
     combined_audio_file_name = combine_audio_from_files(file_paths)
 
     # delete the temporary files
@@ -142,14 +160,24 @@
 
     # export the combined audio to the temporary file
     combined_audio.export(temp_file.name, format='mp3')
 
     # return the path to the temporary file
     return temp_file.name
 
+def quran_surah_with_english_to_mp3_url(surah):
+    # convert surah to int and get the tag from the quran_chapter_to_tag dictionary
+    surah = int(surah)
+    tag = surah_number_to_name_tag[surah]
+
+    # get the url of the mp3 file
+    url = f'https://thechosenone.info/wp-content/uploads/2014/09/{tag}.mp3'
+
+    return url
+
 def quran_verse_to_mp3_url(verse):
     # get the chapter and verse number
     chapter, verse_number = verse.split(':')
 
     # convert the numbers to the correct string format
     chapter = chapter.zfill(3)
     verse_number = verse_number.zfill(3)
```

### Comparing `fajrGPT-1.4.9/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.5/fajrGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.9
+Version: 1.5
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.9/setup.py` & `fajrGPT-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.4.9",
+    version="1.5",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

