# Comparing `tmp/pyvidplayer2-0.9.1.tar.gz` & `tmp/pyvidplayer2-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvidplayer2-0.9.1.tar", last modified: Sun Jul 30 14:52:15 2023, max compression
+gzip compressed data, was "pyvidplayer2-0.9.2.tar", last modified: Mon Jul 31 02:31:22 2023, max compression
```

## Comparing `pyvidplayer2-0.9.1.tar` & `pyvidplayer2-0.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:52:15.285997 pyvidplayer2-0.9.1/
--rw-rw-rw-   0        0        0     1085 2023-07-19 21:30:21.000000 pyvidplayer2-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     2493 2023-07-30 14:52:15.285997 pyvidplayer2-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2160 2023-07-30 14:05:34.000000 pyvidplayer2-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 14:52:15.269986 pyvidplayer2-0.9.1/pyvidplayer2/
--rw-rw-rw-   0        0        0      694 2023-07-30 13:39:04.000000 pyvidplayer2-0.9.1/pyvidplayer2/__init__.py
--rw-rw-rw-   0        0        0     2442 2023-07-30 13:40:30.000000 pyvidplayer2-0.9.1/pyvidplayer2/audio_handler.py
--rw-rw-rw-   0        0        0     1339 2023-07-30 13:44:08.000000 pyvidplayer2-0.9.1/pyvidplayer2/post_processing.py
--rw-rw-rw-   0        0        0     2232 2023-07-29 04:31:47.000000 pyvidplayer2-0.9.1/pyvidplayer2/subtitles.py
--rw-rw-rw-   0        0        0     7473 2023-07-30 14:34:13.000000 pyvidplayer2-0.9.1/pyvidplayer2/video.py
--rw-rw-rw-   0        0        0     9560 2023-07-30 14:48:47.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_player.py
--rw-rw-rw-   0        0        0     1336 2023-07-30 14:33:49.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_pygame.py
--rw-rw-rw-   0        0        0     1531 2023-07-26 18:35:59.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_pyglet.py
--rw-rw-rw-   0        0        0     1662 2023-07-30 14:49:19.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_pyqt.py
--rw-rw-rw-   0        0        0     1500 2023-07-30 02:15:43.000000 pyvidplayer2-0.9.1/pyvidplayer2/video_tkinter.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:52:15.284996 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/
--rw-rw-rw-   0        0        0     2493 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-30 14:52:15.000000 pyvidplayer2-0.9.1/pyvidplayer2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 14:52:15.285997 pyvidplayer2-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-07-30 14:06:44.000000 pyvidplayer2-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:31:22.415891 pyvidplayer2-0.9.2/
+-rw-rw-rw-   0        0        0     1085 2023-07-19 21:30:21.000000 pyvidplayer2-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0     2493 2023-07-31 02:31:22.414891 pyvidplayer2-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2160 2023-07-30 14:05:34.000000 pyvidplayer2-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:31:22.404818 pyvidplayer2-0.9.2/pyvidplayer2/
+-rw-rw-rw-   0        0        0      694 2023-07-30 13:39:04.000000 pyvidplayer2-0.9.2/pyvidplayer2/__init__.py
+-rw-rw-rw-   0        0        0     2678 2023-07-31 02:21:17.000000 pyvidplayer2-0.9.2/pyvidplayer2/audio_handler.py
+-rw-rw-rw-   0        0        0     1339 2023-07-30 13:44:08.000000 pyvidplayer2-0.9.2/pyvidplayer2/post_processing.py
+-rw-rw-rw-   0        0        0     2232 2023-07-29 04:31:47.000000 pyvidplayer2-0.9.2/pyvidplayer2/subtitles.py
+-rw-rw-rw-   0        0        0     7477 2023-07-31 02:20:08.000000 pyvidplayer2-0.9.2/pyvidplayer2/video.py
+-rw-rw-rw-   0        0        0     9558 2023-07-31 02:29:04.000000 pyvidplayer2-0.9.2/pyvidplayer2/video_player.py
+-rw-rw-rw-   0        0        0     1336 2023-07-30 14:33:49.000000 pyvidplayer2-0.9.2/pyvidplayer2/video_pygame.py
+-rw-rw-rw-   0        0        0     1531 2023-07-26 18:35:59.000000 pyvidplayer2-0.9.2/pyvidplayer2/video_pyglet.py
+-rw-rw-rw-   0        0        0     1662 2023-07-30 14:49:19.000000 pyvidplayer2-0.9.2/pyvidplayer2/video_pyqt.py
+-rw-rw-rw-   0        0        0     1500 2023-07-30 02:15:43.000000 pyvidplayer2-0.9.2/pyvidplayer2/video_tkinter.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:31:22.413891 pyvidplayer2-0.9.2/pyvidplayer2.egg-info/
+-rw-rw-rw-   0        0        0     2493 2023-07-31 02:31:22.000000 pyvidplayer2-0.9.2/pyvidplayer2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-07-31 02:31:22.000000 pyvidplayer2-0.9.2/pyvidplayer2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:31:22.000000 pyvidplayer2-0.9.2/pyvidplayer2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-07-31 02:31:22.000000 pyvidplayer2-0.9.2/pyvidplayer2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 02:31:22.000000 pyvidplayer2-0.9.2/pyvidplayer2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:31:22.415891 pyvidplayer2-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-07-31 02:31:11.000000 pyvidplayer2-0.9.2/setup.py
```

### Comparing `pyvidplayer2-0.9.1/LICENSE` & `pyvidplayer2-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/PKG-INFO` & `pyvidplayer2-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.1
+Version: 0.9.2
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
```

### Comparing `pyvidplayer2-0.9.1/README.md` & `pyvidplayer2-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/__init__.py` & `pyvidplayer2-0.9.2/pyvidplayer2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/audio_handler.py` & `pyvidplayer2-0.9.2/pyvidplayer2/audio_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pyaudio
 import wave
 import math 
+import time
 import numpy
 from threading import Thread
 from io import BytesIO
 
 
 _p = pyaudio.PyAudio()
 
@@ -14,14 +15,16 @@
         self.stream = None
         self.wave = None
 
         self.thread = None
         self.stop_thread = False
 
         self.position = 0
+
+        self.loaded = False
         self.paused = False
         self.active = False
 
         self.volume = 1.0
 
     def get_busy(self):
         return self.active
@@ -34,24 +37,30 @@
 
         self.stream = _p.open(
         format=_p.get_format_from_width(self.wave.getsampwidth()),
         channels=self.wave.getnchannels(),
         rate=self.wave.getframerate(),
         output=True)
 
+        self.loaded = True
+
     def unload(self):
         self.stop()
 
-        self.stream.stop_stream()
-        self.stream.close()
-        self.wave.close()
+        if self.loaded:
 
-        self.wave = None 
-        self.stream = None
-        self.thread = None
+            self.stream.stop_stream()
+            self.stream.close()
+            self.wave.close()
+
+            self.wave = None 
+            self.stream = None
+            self.thread = None
+
+            self.loaded = False
 
     def play(self):
         self.stop_thread = False 
         self.position = 0
         self.active = True
 
         self.wave.rewind()
@@ -61,15 +70,17 @@
 
     def _threaded_play(self):
         chunk = 2048
         data = self.wave.readframes(chunk)
 
         while data != b'' and not self.stop_thread:
 
-            if not self.paused:
+            if self.paused:
+                time.sleep(0.01)
+            else:
                 audio = numpy.frombuffer(data, dtype=numpy.int16)
 
                 if self.volume == 0.0:
                     audio = numpy.zeros_like(audio)
                 else:
                     db = 20 * math.log10(self.volume)
                     audio = (audio * 10**(db/20)).astype(numpy.int16)
@@ -87,16 +98,17 @@
     def get_volume(self):
         return self.volume
 
     def get_pos(self):
         return self.position
 
     def stop(self):
-        if self.get_busy():
+        if self.active:
             self.stop_thread = True
             self.thread.join()
+            self.position = 0
 
     def pause(self):
         self.paused = True 
 
     def unpause(self):
         self.paused = False
```

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/post_processing.py` & `pyvidplayer2-0.9.2/pyvidplayer2/post_processing.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/subtitles.py` & `pyvidplayer2-0.9.2/pyvidplayer2/subtitles.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/video.py` & `pyvidplayer2-0.9.2/pyvidplayer2/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,24 +188,24 @@
 
     def get_pos(self) -> float:
         return min(self.duration, self._starting_time + max(0, self._chunks_played - 1) * self.chunk_size + self._audio.get_pos())
 
     def seek(self, time: float, relative=True) -> None:
         # seeking accurate to 1 tenth of a second
 
-        self._starting_time = self.get_pos() + time if relative else time
+        self._starting_time = (self.get_pos() + time) if relative else time
         self._starting_time = round(min(max(0, self._starting_time), self.duration), 1)
 
         for t in self._threads:
             t.join()
         self._chunks = []
         self._threads = []
         self._chunks_claimed = 0
         self._chunks_played = 0
-        self._audio.stop()
+        self._audio.unload()
 
         self._vid.set(cv2.CAP_PROP_POS_FRAMES, self._starting_time * self.frame_rate)
         if self.subs is not None:
             self.subs._seek(self._starting_time)
 
     def draw(self, surf, pos: Tuple[int, int], force_draw=True) -> bool:
         if self._update() or force_draw:
```

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/video_player.py` & `pyvidplayer2-0.9.2/pyvidplayer2/video_player.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,14 @@
                     click = True
 
             self._show_ui = self.frame_rect.collidepoint(mouse) if show_ui is None else show_ui
 
             if self._show_ui:
                 self._progress_bar.w = self._progress_back.w * (self.video.get_pos() / self.video.duration)
                 self._smooth_bar += (self._progress_bar.w - self._smooth_bar) / (dt * 0.25)
-
                 self._show_seek = self._progress_back.collidepoint(mouse)
 
                 if self._show_seek:
                     t = (self._progress_back.w - (self._progress_back.right - mouse[0])) * (self.video.duration / self._progress_back.w)
 
                     self._seek_pos = self._progress_back.w * (round(t, 1) / self.video.duration) + self._progress_back.x
                     self._seek_time = t
```

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/video_pygame.py` & `pyvidplayer2-0.9.2/pyvidplayer2/video_pygame.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/video_pyglet.py` & `pyvidplayer2-0.9.2/pyvidplayer2/video_pyglet.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/video_pyqt.py` & `pyvidplayer2-0.9.2/pyvidplayer2/video_pyqt.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2/video_tkinter.py` & `pyvidplayer2-0.9.2/pyvidplayer2/video_tkinter.py`

 * *Files identical despite different names*

### Comparing `pyvidplayer2-0.9.1/pyvidplayer2.egg-info/PKG-INFO` & `pyvidplayer2-0.9.2/pyvidplayer2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvidplayer2
-Version: 0.9.1
+Version: 0.9.2
 Summary: Video playback in Python
 Home-page: https://github.com/ree1261/pyvidplayer2
 Author: Anray Liu
 Author-email: anrayliu@gmail.com
 License: MIT
 Keywords: pygame,video,playback
 Platform: windows
```

### Comparing `pyvidplayer2-0.9.1/setup.py` & `pyvidplayer2-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", 'r') as f:
     long_desc = f.read()
 
 
 setup(
     name="pyvidplayer2",
-    version="0.9.1",
+    version="0.9.2",
     description="Video playback in Python",
     long_description=long_desc,
     long_description_content_type = "text/markdown",
     author="Anray Liu",
     author_email="anrayliu@gmail.com",
     license="MIT",
     packages=["pyvidplayer2"],
```

