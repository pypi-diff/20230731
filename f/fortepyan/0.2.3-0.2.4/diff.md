# Comparing `tmp/fortepyan-0.2.3.tar.gz` & `tmp/fortepyan-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortepyan-0.2.3.tar", last modified: Mon Jul 24 19:16:36 2023, max compression
+gzip compressed data, was "fortepyan-0.2.4.tar", last modified: Mon Jul 31 19:13:18 2023, max compression
```

## Comparing `fortepyan-0.2.3.tar` & `fortepyan-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 19:16:36.280838 fortepyan-0.2.3/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.3/README.md
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-07-24 19:16:23.000000 fortepyan-0.2.3/fortepyan/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.276838 fortepyan-0.2.3/fortepyan/analytics/
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/analytics/clustering/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7845 2023-07-17 15:32:45.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/process.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.3/fortepyan/analytics/clustering/views.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/audio/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1145 2023-02-11 18:30:36.000000 fortepyan-0.2.3/fortepyan/audio/render.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.3/fortepyan/audio/soundfont.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.3/fortepyan/config.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.3/fortepyan/main.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/midi/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.3/fortepyan/midi/structures.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.3/fortepyan/midi/tools.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/view/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      358 2023-07-24 18:12:33.000000 fortepyan-0.2.3/fortepyan/view/__init__.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/view/animation/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.3/fortepyan/view/animation/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     3124 2023-07-24 06:40:43.000000 fortepyan-0.2.3/fortepyan/view/animation/dualroll.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.3/fortepyan/view/animation/evolution.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-07-24 18:09:37.000000 fortepyan-0.2.3/fortepyan/view/animation/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5091 2023-07-05 16:46:38.000000 fortepyan-0.2.3/fortepyan/view/animation/pianoroll.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan/view/pianoroll/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      126 2023-07-24 06:16:22.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/__init__.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2389 2023-07-24 19:16:08.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/dual.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5064 2023-07-24 05:44:31.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/main.py
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     6102 2023-07-24 05:43:12.000000 fortepyan-0.2.3/fortepyan/view/pianoroll/structures.py
-drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-24 19:16:36.280838 fortepyan-0.2.3/fortepyan.egg-info/
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/PKG-INFO
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      878 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/SOURCES.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/dependency_links.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      172 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/requires.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-07-24 19:16:36.000000 fortepyan-0.2.3/fortepyan.egg-info/top_level.txt
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1474 2023-07-24 19:16:23.000000 fortepyan-0.2.3/pyproject.toml
--rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-07-24 19:16:36.280838 fortepyan-0.2.3/setup.cfg
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.563669 fortepyan-0.2.4/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-31 19:13:18.563669 fortepyan-0.2.4/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      964 2023-06-11 10:38:07.000000 fortepyan-0.2.4/README.md
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.559669 fortepyan-0.2.4/fortepyan/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      361 2023-07-31 19:13:00.000000 fortepyan-0.2.4/fortepyan/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.559669 fortepyan-0.2.4/fortepyan/analytics/
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.559669 fortepyan-0.2.4/fortepyan/analytics/clustering/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 11:22:34.000000 fortepyan-0.2.4/fortepyan/analytics/clustering/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     7845 2023-07-17 15:32:45.000000 fortepyan-0.2.4/fortepyan/analytics/clustering/process.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1519 2023-06-11 11:36:25.000000 fortepyan-0.2.4/fortepyan/analytics/clustering/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      768 2023-06-11 11:36:24.000000 fortepyan-0.2.4/fortepyan/analytics/clustering/views.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.559669 fortepyan-0.2.4/fortepyan/audio/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1146 2023-07-30 12:38:56.000000 fortepyan-0.2.4/fortepyan/audio/render.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      514 2023-02-28 06:46:10.000000 fortepyan-0.2.4/fortepyan/audio/soundfont.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      249 2023-02-26 12:33:07.000000 fortepyan-0.2.4/fortepyan/config.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1962 2023-01-29 11:21:01.000000 fortepyan-0.2.4/fortepyan/main.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.563669 fortepyan-0.2.4/fortepyan/midi/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     8284 2023-06-11 10:56:41.000000 fortepyan-0.2.4/fortepyan/midi/structures.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2189 2023-04-23 12:50:22.000000 fortepyan-0.2.4/fortepyan/midi/tools.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.563669 fortepyan-0.2.4/fortepyan/view/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      358 2023-07-24 18:12:33.000000 fortepyan-0.2.4/fortepyan/view/__init__.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.563669 fortepyan-0.2.4/fortepyan/view/animation/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        0 2023-06-11 08:05:25.000000 fortepyan-0.2.4/fortepyan/view/animation/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     3124 2023-07-31 19:12:36.000000 fortepyan-0.2.4/fortepyan/view/animation/dualroll.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)    15618 2023-06-11 08:41:59.000000 fortepyan-0.2.4/fortepyan/view/animation/evolution.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1644 2023-07-31 19:11:49.000000 fortepyan-0.2.4/fortepyan/view/animation/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5091 2023-07-05 16:46:38.000000 fortepyan-0.2.4/fortepyan/view/animation/pianoroll.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.563669 fortepyan-0.2.4/fortepyan/view/pianoroll/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      126 2023-07-24 06:16:22.000000 fortepyan-0.2.4/fortepyan/view/pianoroll/__init__.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     2389 2023-07-24 19:16:08.000000 fortepyan-0.2.4/fortepyan/view/pianoroll/dual.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     5064 2023-07-24 05:44:31.000000 fortepyan-0.2.4/fortepyan/view/pianoroll/main.py
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     6102 2023-07-24 05:43:12.000000 fortepyan-0.2.4/fortepyan/view/pianoroll/structures.py
+drwxrwxr-x   0 hagrid    (1000) hagrid    (1000)        0 2023-07-31 19:13:18.559669 fortepyan-0.2.4/fortepyan.egg-info/
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1416 2023-07-31 19:13:18.000000 fortepyan-0.2.4/fortepyan.egg-info/PKG-INFO
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      878 2023-07-31 19:13:18.000000 fortepyan-0.2.4/fortepyan.egg-info/SOURCES.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)        1 2023-07-31 19:13:18.000000 fortepyan-0.2.4/fortepyan.egg-info/dependency_links.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)      172 2023-07-31 19:13:18.000000 fortepyan-0.2.4/fortepyan.egg-info/requires.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       10 2023-07-31 19:13:18.000000 fortepyan-0.2.4/fortepyan.egg-info/top_level.txt
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)     1474 2023-07-31 19:13:00.000000 fortepyan-0.2.4/pyproject.toml
+-rw-rw-r--   0 hagrid    (1000) hagrid    (1000)       38 2023-07-31 19:13:18.563669 fortepyan-0.2.4/setup.cfg
```

### Comparing `fortepyan-0.2.3/PKG-INFO` & `fortepyan-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.3
+Version: 0.2.4
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.3/README.md` & `fortepyan-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/analytics/clustering/process.py` & `fortepyan-0.2.4/fortepyan/analytics/clustering/process.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/analytics/clustering/structures.py` & `fortepyan-0.2.4/fortepyan/analytics/clustering/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/analytics/clustering/views.py` & `fortepyan-0.2.4/fortepyan/analytics/clustering/views.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/audio/render.py` & `fortepyan-0.2.4/fortepyan/audio/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,11 +28,12 @@
     # This will be deleted
     tmp_wav_path = tempfile.mkstemp(suffix=".wav")[1]
     midi_to_wav(midi=midi, wavpath=tmp_wav_path)
 
     # Wav to mp3
     if not mp3_path:
         mp3_path = tempfile.mkstemp(suffix=".mp3")[1]
+
     print("Rendering audio to file:", mp3_path)
     AudioSegment.from_wav(tmp_wav_path).export(mp3_path, format="mp3")
 
     return mp3_path
```

### Comparing `fortepyan-0.2.3/fortepyan/audio/soundfont.py` & `fortepyan-0.2.4/fortepyan/audio/soundfont.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/main.py` & `fortepyan-0.2.4/fortepyan/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/midi/structures.py` & `fortepyan-0.2.4/fortepyan/midi/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/midi/tools.py` & `fortepyan-0.2.4/fortepyan/midi/tools.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/view/animation/dualroll.py` & `fortepyan-0.2.4/fortepyan/view/animation/dualroll.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/view/animation/evolution.py` & `fortepyan-0.2.4/fortepyan/view/animation/evolution.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/view/animation/main.py` & `fortepyan-0.2.4/fortepyan/view/animation/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import subprocess
 
 from fortepyan.audio.render import midi_to_mp3
 from fortepyan.midi.structures import MidiPiece
+from fortepyan.view.pianoroll.structures import FigureResolution
 from fortepyan.view.animation import dualroll as dualroll_animation
 from fortepyan.view.animation import pianoroll as pianoroll_animation
 
 
 def make_piano_roll_video(
     piece: MidiPiece,
     movie_path: str,
@@ -27,20 +28,22 @@
 
 def make_dual_roll_video(
     piece: MidiPiece,
     movie_path: str,
     title: str = "animation",
     base_cmap: str = "PuBuGn",
     marked_cmap: str = "Reds",
+    figres: FigureResolution = None,
 ):
     scene = dualroll_animation.DualRollScene(
         piece=piece,
         title=title,
         base_cmap=base_cmap,
         marked_cmap=marked_cmap,
+        figres=figres,
     )
     mp3_path = midi_to_mp3(piece.to_midi())
 
     scene_frames_dir = scene.render_mp()
     command = f"""
         ffmpeg -y -f image2 -framerate 30 -i {str(scene_frames_dir)}/10%4d.png\
         -loglevel quiet -i {mp3_path} -map 0:v:0 -map 1:a:0\
```

### Comparing `fortepyan-0.2.3/fortepyan/view/animation/pianoroll.py` & `fortepyan-0.2.4/fortepyan/view/animation/pianoroll.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/view/pianoroll/dual.py` & `fortepyan-0.2.4/fortepyan/view/pianoroll/dual.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/view/pianoroll/main.py` & `fortepyan-0.2.4/fortepyan/view/pianoroll/main.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan/view/pianoroll/structures.py` & `fortepyan-0.2.4/fortepyan/view/pianoroll/structures.py`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/fortepyan.egg-info/PKG-INFO` & `fortepyan-0.2.4/fortepyan.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortepyan
-Version: 0.2.3
+Version: 0.2.4
 Summary: Process MIDI piano with (almost) no pain
 Author-email: Piano For AI <roszcz+fortepyan@gmail.com>
 Project-URL: Homepage, https://github.com/Nospoko/fortepyan
 Keywords: midi,music,piano
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fortepyan-0.2.3/fortepyan.egg-info/SOURCES.txt` & `fortepyan-0.2.4/fortepyan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortepyan-0.2.3/pyproject.toml` & `fortepyan-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fortepyan"
-version = "0.2.3"
+version = "0.2.4"
 description = "Process MIDI piano with (almost) no pain"
 readme = "README.md"
 authors = [{ name = "Piano For AI", email = "roszcz+fortepyan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -43,15 +43,15 @@
     "fortepyan.audio",
     "fortepyan.view.animation",
     "fortepyan.view.pianoroll",
     "fortepyan.analytics.clustering",
 ]
 
 [tool.bumpver]
-current_version = "0.2.3"
+current_version = "0.2.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

