# Comparing `tmp/Musicreater-1.2.0.tar.gz` & `tmp/Musicreater-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-1.2.0.tar", last modified: Sat Jul  1 13:54:25 2023, max compression
+gzip compressed data, was "Musicreater-1.2.1.tar", last modified: Mon Jul 31 14:48:22 2023, max compression
```

## Comparing `Musicreater-1.2.0.tar` & `Musicreater-1.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.697469 Musicreater-1.2.0/
--rw-rw-rw-   0        0        0    13072 2023-07-01 13:48:04.000000 Musicreater-1.2.0/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.649052 Musicreater-1.2.0/Musicreater/
--rw-rw-rw-   0        0        0      991 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     6525 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/constants.py
--rw-rw-rw-   0        0        0     3142 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0    18362 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/experiment.py
--rw-rw-rw-   0        0        0    10301 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    28535 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/main.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.676538 Musicreater-1.2.0/Musicreater/plugin/
--rw-rw-rw-   0        0        0      581 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/__init__.py
--rw-rw-rw-   0        0        0     2435 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/archive.py
--rw-rw-rw-   0        0        0     5999 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/bdx.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.679528 Musicreater-1.2.0/Musicreater/plugin/bdxfile/
--rw-rw-rw-   0        0        0      569 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/bdxfile/__init__.py
--rw-rw-rw-   0        0        0     6211 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/bdxfile/main.py
--rw-rw-rw-   0        0        0      809 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/common.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.683513 Musicreater-1.2.0/Musicreater/plugin/funcpack/
--rw-rw-rw-   0        0        0      547 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/funcpack/__init__.py
--rw-rw-rw-   0        0        0     4182 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/funcpack/main.py
--rw-rw-rw-   0        0        0     2523 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/main.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.687500 Musicreater-1.2.0/Musicreater/plugin/mcstructfile/
--rw-rw-rw-   0        0        0      557 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructfile/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructfile/main.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.691488 Musicreater-1.2.0/Musicreater/plugin/mcstructpack/
--rw-rw-rw-   0        0        0      550 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructpack/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructpack/main.py
--rw-rw-rw-   0        0        0     7219 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/mcstructure.py
--rw-rw-rw-   0        0        0     3797 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/noteblock.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.694483 Musicreater-1.2.0/Musicreater/plugin/websocket/
--rw-rw-rw-   0        0        0      522 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/websocket/__init__.py
--rw-rw-rw-   0        0        0      771 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/websocket/main.py
--rw-rw-rw-   0        0        0     1168 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/plugin/websocket.py
--rw-rw-rw-   0        0        0    13264 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/previous.py
--rw-rw-rw-   0        0        0     4238 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/subclass.py
--rw-rw-rw-   0        0        0     1125 2023-07-01 13:48:04.000000 Musicreater-1.2.0/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:54:25.659595 Musicreater-1.2.0/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     7718 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1055 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 13:54:25.000000 Musicreater-1.2.0/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7718 2023-07-01 13:54:25.696478 Musicreater-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6842 2023-07-01 13:48:04.000000 Musicreater-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 13:54:25.697469 Musicreater-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-07-01 13:48:04.000000 Musicreater-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:22.014341 Musicreater-1.2.1/
+-rw-rw-rw-   0        0        0    13072 2023-07-01 13:48:04.000000 Musicreater-1.2.1/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:21.927341 Musicreater-1.2.1/Musicreater/
+-rw-rw-rw-   0        0        0     1010 2023-07-31 14:47:39.000000 Musicreater-1.2.1/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     6525 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/constants.py
+-rw-rw-rw-   0        0        0     3142 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0    18362 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/experiment.py
+-rw-rw-rw-   0        0        0    10301 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    28499 2023-07-31 14:47:39.000000 Musicreater-1.2.1/Musicreater/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:21.973341 Musicreater-1.2.1/Musicreater/plugin/
+-rw-rw-rw-   0        0        0      581 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/__init__.py
+-rw-rw-rw-   0        0        0     2435 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/archive.py
+-rw-rw-rw-   0        0        0     5999 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/bdx.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:21.980345 Musicreater-1.2.1/Musicreater/plugin/bdxfile/
+-rw-rw-rw-   0        0        0      569 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/bdxfile/__init__.py
+-rw-rw-rw-   0        0        0     6211 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/bdxfile/main.py
+-rw-rw-rw-   0        0        0      809 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/common.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:21.985341 Musicreater-1.2.1/Musicreater/plugin/funcpack/
+-rw-rw-rw-   0        0        0      547 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/funcpack/__init__.py
+-rw-rw-rw-   0        0        0     4182 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/funcpack/main.py
+-rw-rw-rw-   0        0        0     2523 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:21.995342 Musicreater-1.2.1/Musicreater/plugin/mcstructfile/
+-rw-rw-rw-   0        0        0      557 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/mcstructfile/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/mcstructfile/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:22.002341 Musicreater-1.2.1/Musicreater/plugin/mcstructpack/
+-rw-rw-rw-   0        0        0      550 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/mcstructpack/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/mcstructpack/main.py
+-rw-rw-rw-   0        0        0     7219 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/mcstructure.py
+-rw-rw-rw-   0        0        0     3797 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/noteblock.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:22.010341 Musicreater-1.2.1/Musicreater/plugin/websocket/
+-rw-rw-rw-   0        0        0      522 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/websocket/__init__.py
+-rw-rw-rw-   0        0        0      771 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/websocket/main.py
+-rw-rw-rw-   0        0        0     1168 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/plugin/websocket.py
+-rw-rw-rw-   0        0        0    13264 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/previous.py
+-rw-rw-rw-   0        0        0     4238 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/subclass.py
+-rw-rw-rw-   0        0        0     1125 2023-07-01 13:48:04.000000 Musicreater-1.2.1/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:48:21.947345 Musicreater-1.2.1/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     7616 2023-07-31 14:48:21.000000 Musicreater-1.2.1/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-07-31 14:48:21.000000 Musicreater-1.2.1/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:48:21.000000 Musicreater-1.2.1/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-31 14:48:21.000000 Musicreater-1.2.1/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 14:48:21.000000 Musicreater-1.2.1/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7616 2023-07-31 14:48:22.013344 Musicreater-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6842 2023-07-01 13:48:04.000000 Musicreater-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:48:22.014341 Musicreater-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1500 2023-07-31 14:47:39.000000 Musicreater-1.2.1/setup.py
```

### Comparing `Musicreater-1.2.0/LICENSE.md` & `Musicreater-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/__init__.py` & `Musicreater-1.2.1/Musicreater/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 """
 
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 
-__version__ = "1.2.0"
-__vername__ = "更高效的算法管理"
+__version__ = "1.2.1"
+__vername__ = "扩大对有问题的Midi文件的兼容性"
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"), ("鸣凤鸽子", "MingFengPigeon"))
 __all__ = [
     # 主要类
     "MidiConvert",
     # 附加类
     # "SingleNote",
     "SingleCommand",
```

### Comparing `Musicreater-1.2.0/Musicreater/constants.py` & `Musicreater-1.2.1/Musicreater/constants.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/exceptions.py` & `Musicreater-1.2.1/Musicreater/exceptions.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/experiment.py` & `Musicreater-1.2.1/Musicreater/experiment.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/magicmain.py` & `Musicreater-1.2.1/Musicreater/magicmain.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/main.py` & `Musicreater-1.2.1/Musicreater/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
         midi_music_name = os.path.splitext(os.path.basename(midi_file_path))[0].replace(
             " ", "_"
         )
         """文件名，不含路径且不含后缀"""
 
         try:
-            return cls(mido.MidiFile(midi_file_path), midi_music_name, old_exe_format)
+            return cls(mido.MidiFile(midi_file_path,clip=True), midi_music_name, old_exe_format)
         except (ValueError, TypeError) as E:
             raise MidiDestroyedError(f"文件{midi_file_path}损坏：{E}")
         except FileNotFoundError as E:
             raise FileNotFoundError(f"文件{midi_file_path}不存在：{E}")
 
     @staticmethod
     def inst_to_souldID_withX(
@@ -533,55 +533,53 @@
                 "你是否正在使用的是一个由 copy_important 生成的MidiConvert对象？这是不可复用的。"
             )
 
         # 一个midi中仅有16个通道 我们通过通道来识别而不是音轨
         midi_channels: ChannelType = empty_midi_channels()
         tempo = mido.midifiles.midifiles.DEFAULT_TEMPO
 
-        # a = 0
         # 我们来用通道统计音乐信息
         # 但是是用分轨的思路的
         for track_no, track in enumerate(self.midi.tracks):
-            # print(track_no,track)
             microseconds = 0
             if not track:
                 continue
 
-            # print(track_no,"="*20)
             for msg in track:
-                # print("+++",msg)
                 if msg.time != 0:
                     microseconds += msg.time * tempo / self.midi.ticks_per_beat / 1000
 
                 if msg.is_meta:
                     if msg.type == "set_tempo":
                         tempo = msg.tempo
                 else:
-
-                    if not track_no in midi_channels[msg.channel].keys():
-                        midi_channels[msg.channel][track_no] = []
+                    
+                    try:
+                        if not track_no in midi_channels[msg.channel].keys():
+                            midi_channels[msg.channel][track_no] = []
+                    except AttributeError as E:
+                        print(msg,E)
+                    
                     if msg.type == "program_change":
                         midi_channels[msg.channel][track_no].append(
                             ("PgmC", msg.program, microseconds)
                         )
 
                     elif msg.type == "note_on" and msg.velocity != 0:
                         midi_channels[msg.channel][track_no].append(
                             ("NoteS", msg.note, msg.velocity, microseconds)
                         )
-                        # a+=1
 
                     elif (msg.type == "note_on" and msg.velocity == 0) or (
                         msg.type == "note_off"
                     ):
                         midi_channels[msg.channel][track_no].append(
                             ("NoteE", msg.note, microseconds)
                         )
 
-        # print(a)
 
         """整合后的音乐通道格式
         每个通道包括若干消息元素其中逃不过这三种：
 
         1 切换乐器消息
         ("PgmC", 切换后的乐器ID: int, 距离演奏开始的毫秒)
 
@@ -634,16 +632,14 @@
             # 如果当前通道为空 则跳过
             if not self.channels[i]:
                 continue
 
             # 第十通道是打击乐通道
             SpecialBits = True if i == 9 else False
 
-            # nowChannel = []
-
             for track_no, track in self.channels[i].items():
                 nowTrack = []
 
                 for msg in track:
                     if msg[0] == "PgmC":
                         InstID = msg[1]
```

### Comparing `Musicreater-1.2.0/Musicreater/plugin/__init__.py` & `Musicreater-1.2.1/Musicreater/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/archive.py` & `Musicreater-1.2.1/Musicreater/plugin/archive.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/bdx.py` & `Musicreater-1.2.1/Musicreater/plugin/bdx.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/bdxfile/__init__.py` & `Musicreater-1.2.1/Musicreater/plugin/bdxfile/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/bdxfile/main.py` & `Musicreater-1.2.1/Musicreater/plugin/bdxfile/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/common.py` & `Musicreater-1.2.1/Musicreater/plugin/common.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/funcpack/__init__.py` & `Musicreater-1.2.1/Musicreater/plugin/funcpack/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/funcpack/main.py` & `Musicreater-1.2.1/Musicreater/plugin/funcpack/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/main.py` & `Musicreater-1.2.1/Musicreater/plugin/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/mcstructfile/__init__.py` & `Musicreater-1.2.1/Musicreater/plugin/mcstructfile/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/mcstructfile/main.py` & `Musicreater-1.2.1/Musicreater/plugin/mcstructfile/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/mcstructpack/__init__.py` & `Musicreater-1.2.1/Musicreater/plugin/mcstructpack/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/mcstructpack/main.py` & `Musicreater-1.2.1/Musicreater/plugin/mcstructpack/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/mcstructure.py` & `Musicreater-1.2.1/Musicreater/plugin/mcstructure.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/noteblock.py` & `Musicreater-1.2.1/Musicreater/plugin/noteblock.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/websocket/__init__.py` & `Musicreater-1.2.1/Musicreater/plugin/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/websocket/main.py` & `Musicreater-1.2.1/Musicreater/plugin/websocket/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/plugin/websocket.py` & `Musicreater-1.2.1/Musicreater/plugin/websocket.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/previous.py` & `Musicreater-1.2.1/Musicreater/previous.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/subclass.py` & `Musicreater-1.2.1/Musicreater/subclass.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater/utils.py` & `Musicreater-1.2.1/Musicreater/utils.py`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/Musicreater.egg-info/PKG-INFO` & `Musicreater-1.2.1/Musicreater.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 1.2.0
+Version: 1.2.1
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <h1 align="center">
```

### Comparing `Musicreater-1.2.0/Musicreater.egg-info/SOURCES.txt` & `Musicreater-1.2.1/Musicreater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/PKG-INFO` & `Musicreater-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 1.2.0
+Version: 1.2.1
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <h1 align="center">
```

### Comparing `Musicreater-1.2.0/README.md` & `Musicreater-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Musicreater-1.2.0/setup.py` & `Musicreater-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,16 +25,14 @@
         "Intended Audience :: Developers",
         "Natural Language :: Chinese (Simplified)",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     # 需要安装的依赖
     install_requires=dependences,
 )
```

