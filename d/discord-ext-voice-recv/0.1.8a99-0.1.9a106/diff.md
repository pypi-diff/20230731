# Comparing `tmp/discord-ext-voice_recv-0.1.8a99.tar.gz` & `tmp/discord-ext-voice_recv-0.1.9a106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-voice_recv-0.1.8a99.tar", last modified: Sat Jul 29 00:59:47 2023, max compression
+gzip compressed data, was "discord-ext-voice_recv-0.1.9a106.tar", last modified: Sun Jul 30 22:59:11 2023, max compression
```

## Comparing `discord-ext-voice_recv-0.1.8a99.tar` & `discord-ext-voice_recv-0.1.9a106.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.897738 discord-ext-voice_recv-0.1.8a99/
--rw-rw-rw-   0        0        0     1091 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.8a99/LICENSE
--rw-rw-rw-   0        0        0    10038 2023-07-29 00:59:47.896739 discord-ext-voice_recv-0.1.8a99/PKG-INFO
--rw-rw-rw-   0        0        0     8952 2023-07-29 00:55:14.000000 discord-ext-voice_recv-0.1.8a99/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.795797 discord-ext-voice_recv-0.1.8a99/discord/
-drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.796796 discord-ext-voice_recv-0.1.8a99/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.858761 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/
--rw-rw-rw-   0        0        0      362 2023-07-29 00:57:11.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/__init__.py
--rw-rw-rw-   0        0        0     5487 2023-06-19 01:13:13.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/buffer.py
--rw-rw-rw-   0        0        0     3278 2023-07-23 07:28:37.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/gateway.py
--rw-rw-rw-   0        0        0    35866 2023-07-28 22:56:15.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/opus.py
--rw-rw-rw-   0        0        0     8387 2023-06-22 02:45:57.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/reader.py
--rw-rw-rw-   0        0        0    12486 2023-06-19 07:12:45.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/rtp.py
--rw-rw-rw-   0        0        0     1617 2023-07-23 07:28:37.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/silence.py
--rw-rw-rw-   0        0        0    12401 2023-07-29 00:55:44.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/sinks.py
--rw-rw-rw-   0        0        0      911 2023-06-17 04:25:42.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/types.py
--rw-rw-rw-   0        0        0     2237 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/utils.py
--rw-rw-rw-   0        0        0     2623 2023-06-17 05:04:12.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/video.py
--rw-rw-rw-   0        0        0     5707 2023-07-28 22:01:55.000000 discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:59:47.894740 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/
--rw-rw-rw-   0        0        0    10038 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-05 23:03:01.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 00:59:47.000000 discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 00:59:47.897738 discord-ext-voice_recv-0.1.8a99/setup.cfg
--rw-rw-rw-   0        0        0     1917 2023-07-23 07:43:28.000000 discord-ext-voice_recv-0.1.8a99/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.212984 discord-ext-voice_recv-0.1.9a106/
+-rw-rw-rw-   0        0        0     1091 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.9a106/LICENSE
+-rw-rw-rw-   0        0        0    10039 2023-07-30 22:59:11.212984 discord-ext-voice_recv-0.1.9a106/PKG-INFO
+-rw-rw-rw-   0        0        0     8952 2023-07-29 00:55:14.000000 discord-ext-voice_recv-0.1.9a106/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.137028 discord-ext-voice_recv-0.1.9a106/discord/
+drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.138027 discord-ext-voice_recv-0.1.9a106/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.176005 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/
+-rw-rw-rw-   0        0        0      362 2023-07-30 20:09:15.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-07-29 19:04:30.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/buffer.py
+-rw-rw-rw-   0        0        0     3278 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/gateway.py
+-rw-rw-rw-   0        0        0    35905 2023-07-30 22:54:36.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/opus.py
+-rw-rw-rw-   0        0        0     8387 2023-07-30 19:38:50.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/reader.py
+-rw-rw-rw-   0        0        0    12432 2023-07-30 16:48:39.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/rtp.py
+-rw-rw-rw-   0        0        0     5426 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/silence.py
+-rw-rw-rw-   0        0        0    12365 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/sinks.py
+-rw-rw-rw-   0        0        0      911 2023-06-17 04:25:42.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/types.py
+-rw-rw-rw-   0        0        0     2237 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/utils.py
+-rw-rw-rw-   0        0        0     2623 2023-06-17 05:04:12.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/video.py
+-rw-rw-rw-   0        0        0     5740 2023-07-30 19:39:09.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.209988 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/
+-rw-rw-rw-   0        0        0    10039 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-30 22:59:11.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-05 23:03:01.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 22:59:11.213989 discord-ext-voice_recv-0.1.9a106/setup.cfg
+-rw-rw-rw-   0        0        0     1917 2023-07-23 07:43:28.000000 discord-ext-voice_recv-0.1.9a106/setup.py
```

### Comparing `discord-ext-voice_recv-0.1.8a99/LICENSE` & `discord-ext-voice_recv-0.1.9a106/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/PKG-INFO` & `discord-ext-voice_recv-0.1.9a106/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-voice_recv
-Version: 0.1.8a99
+Version: 0.1.9a106
 Summary: Experimental voice receive extension for discord.py
 Home-page: https://github.com/imayhaveborkedit/discord-ext-voice-recv
 Author: Imayhaveborkedit
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `discord-ext-voice_recv-0.1.8a99/README.md` & `discord-ext-voice_recv-0.1.9a106/README.md`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/buffer.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/buffer.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/gateway.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/gateway.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/opus.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/opus.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     "VoiceData"
 ]
 
 
 class VoiceData:
     """docstring for VoiceData"""
 
+    __slots__ = ('packet', 'source', 'pcm')
+
     def __init__(self,
         packet: Packet,
         source: Optional[User],
         *,
         pcm: Optional[bytes]=None
     ):
         self.packet = packet
@@ -106,21 +108,21 @@
     def register_events(self):
         with self._lock:
             self._register_listeners(self.sink)
             for child in self.sink.walk_children():
                 self._register_listeners(child)
 
     def _register_listeners(self, sink: AudioSink):
-        log.warning("registering events for %s", self.sink)
-        log.warning("listeners: %s", self.sink.__sink_listeners__)
+        log.debug("registering events for %s", sink)
+        log.debug("listeners: %s", sink.__sink_listeners__)
 
         for name, method_name in sink.__sink_listeners__:
             func = getattr(sink, method_name)
 
-            log.warning("Registering %s for %s", name, method_name)
+            log.debug("Registering event: %r, func: %r", name, method_name)
             if name in self._event_listeners:
                 self._event_listeners[name].append(func)
             else:
                 self._event_listeners[name] = [func]
 
     def unregister_events(self):
         with self._lock:
```

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/reader.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/reader.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/rtp.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/rtp.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,28 +78,14 @@
             return False
         return self.timestamp == other.timestamp
 
     def is_silence(self) -> bool:
         data = getattr(self, 'decrypted_data', None)
         return data == OPUS_SILENCE
 
-class SilencePacket(_PacketCmpMixin):
-    __slots__ = ('ssrc', 'timestamp')
-    decrypted_data: Literal[OpusSilence] = OPUS_SILENCE
-    extension_data: dict = {}
-
-    def __init__(self, ssrc: int, timestamp: int):
-        self.ssrc = ssrc
-        self.timestamp = timestamp
-
-    def __repr__(self):
-        return '<SilencePacket ssrc={0.ssrc}, timestamp={0.timestamp}>'.format(self)
-
-    def is_silence(self) -> bool:
-        return True
 
 class FakePacket(_PacketCmpMixin):
     __slots__ = ('ssrc', 'sequence', 'timestamp')
     decrypted_data: bytes = b''
     extension_data: dict = {}
 
     def __init__(self, ssrc: int, sequence: int, timestamp: int):
@@ -109,15 +95,31 @@
 
     def __repr__(self):
         return '<FakePacket ssrc={0.ssrc}, sequence={0.sequence}, timestamp={0.timestamp}>'.format(self)
 
     def __bool__(self) -> Literal[False]:
         return False
 
-# Consider adding silence attribute to differentiate (to skip isinstance)
+
+class SilencePacket(FakePacket):
+    __slots__ = ('ssrc', 'timestamp')
+    decrypted_data: Literal[OpusSilence] = OPUS_SILENCE
+    extension_data: dict = {}
+    sequence: int = -1
+
+    def __init__(self, ssrc: int, timestamp: int):
+        self.ssrc = ssrc
+        self.timestamp = timestamp
+
+    def __repr__(self):
+        return '<SilencePacket ssrc={0.ssrc}, timestamp={0.timestamp}>'.format(self)
+
+    def is_silence(self) -> bool:
+        return True
+
 
 class RTPPacket(_PacketCmpMixin):
     __slots__ = ('version', 'padding', 'extended', 'cc', 'marker', 'payload',
                  'sequence', 'timestamp', 'ssrc', 'csrcs', 'header', 'data',
                  'decrypted_data', 'extension', 'extension_data')
 
     _hstruct = struct.Struct('>xxHII')
```

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/sinks.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/sinks.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     'MultiAudioSink',
     'BasicSink',
     'WaveSink',
     'PCMVolumeTransformer',
     'ConditionalFilter',
     'TimedFilter',
     'UserFilter',
+    'SilenceGeneratorSink',
 ]
 
 # TODO: use this in more places
 class VoiceRecvException(discord.DiscordException):
     """Generic exception for voice recv related errors"""
 
     def __init__(self, message: str):
@@ -117,18 +118,14 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def write(self, user: Optional[User], data: VoiceData):
         """Callback for when the sink receives data"""
         raise NotImplementedError
 
-    def write_rtcp(self, packet: RTCPPacket):
-        """Optional callback for when the sink receives an rtcp packet"""
-        pass
-
     @abc.abstractmethod
     def cleanup(self):
         raise NotImplementedError
 
     def walk_children(self) -> Generator[AudioSink, None, None]:
         for child in self.children:
             yield child
@@ -234,16 +231,17 @@
 
     def wants_opus(self) -> bool:
         return not self.decode
 
     def write(self, user: Optional[User], data: VoiceData):
         self.cb(user, data)
 
-    def write_rtcp(self, data: RTCPPacket):
-        self.cb_rtcp(data) if self.cb_rtcp else None
+    @AudioSink.listener()
+    def on_rtcp_packet(self, packet: RTCPPacket, guild: discord.Guild):
+        self.cb_rtcp(packet) if self.cb_rtcp else None
 
     def cleanup(self):
         pass
 
 
 class WaveSink(AudioSink):
     """Endpoint AudioSink that generates a wav file.
@@ -304,17 +302,14 @@
     def volume(self, value: float): # TODO: type range
         self._volume = max(value, 0.0)
 
     def write(self, user: Optional[User], data: VoiceData):
         data.pcm = audioop.mul(data.pcm, 2, min(self._volume, 2.0))
         self.destination.write(user, data)
 
-    def write_rtcp(self, packet: RTCPPacket):
-        self.destination.write_rtcp(packet)
-
     def cleanup(self):
         pass
 
 
 class ConditionalFilter(AudioSink):
     """AudioSink for filtering packets based on an arbitrary predicate function."""
 
@@ -327,17 +322,14 @@
     def wants_opus(self) -> bool:
         return self.destination.wants_opus()
 
     def write(self, user: Optional[User], data: VoiceData):
         if self.predicate(user, data):
             self.destination.write(user, data)
 
-    def write_rtcp(self, packet: RTCPPacket):
-        self.destination.write_rtcp(packet)
-
     def cleanup(self):
         del self.predicate
 
 
 class UserFilter(ConditionalFilter):
     """A convenience class for a User based ConditionalFilter."""
 
@@ -346,14 +338,16 @@
         self.user = user
 
     def _predicate(self, user: Optional[User], data: VoiceData) -> bool:
         return user == self.user
 
 
 class TimedFilter(ConditionalFilter):
+    """A convenience class for a timed ConditionalFilter."""
+
     def __init__(self,
         destination: AudioSink,
         duration: int | float,
         *,
         start_on_init: bool=False
     ):
         super().__init__(destination, self.predicate)
@@ -376,34 +370,37 @@
     def get_time(self) -> int | float:
         """Function to generate a timestamp.  Defaults to `time.perf_counter()`.
         Can be overridden.
         """
         return time.perf_counter()
 
 
-class SilencePaddingSink(AudioSink):
-    """docstring for SilencePaddingSink"""
+class SilenceGeneratorSink(AudioSink):
+    """Generates intermittent silence packets during transmission downtime."""
 
     def __init__(self, destination: AudioSink):
         super().__init__(destination)
 
         self.destination = destination
-        # self.silencegen = SilenceGenerator()
+        self.silencegen = SilenceGenerator(self.destination.write)
+        self.silencegen.start()
 
     def wants_opus(self) -> bool:
         return self.destination.wants_opus()
 
     def write(self, user: Optional[User], data: VoiceData):
-        return super().write(user, data)
+        self.silencegen.push(user, data.packet)
+        self.destination.write(user, data)
 
-    def write_rtcp(self, packet: RTCPPacket):
-        self.destination.write_rtcp(packet)
+    @AudioSink.listener()
+    def on_voice_member_disconnect(self, member: discord.Member, ssrc: int | None):
+        self.silencegen.drop(ssrc=ssrc, user=member)
 
     def cleanup(self):
-        pass
+        self.silencegen.stop()
 
 
 class DejitterSink(AudioSink):
     """docstring for DejitterSink"""
 
     def __init__(self, destination: AudioSink):
         super().__init__(destination)
@@ -412,12 +409,9 @@
 
     def wants_opus(self) -> bool:
         return self.destination.wants_opus()
 
     def write(self, user: Optional[User], data: VoiceData):
         ...
 
-    def write_rtcp(self, packet: RTCPPacket):
-        self.destination.write_rtcp(packet)
-
     def cleanup(self):
         ...
```

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/types.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/types.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/utils.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/utils.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/video.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/video.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/discord/ext/voice_recv/voice_client.py` & `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/voice_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         """Indicates if we're currently receiving audio."""
         return self._reader is not None and self._reader.is_listening()
 
     def stop_listening(self):
         """Stops receiving audio."""
         if self._reader:
             self._reader.stop()
+            self._reader.join(5)
             self._reader = None
 
     def stop_playing(self):
         """Stops playing audio."""
         if self._player:
             self._player.stop()
             self._player = None
```

### Comparing `discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/PKG-INFO` & `discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-voice-recv
-Version: 0.1.8a99
+Version: 0.1.9a106
 Summary: Experimental voice receive extension for discord.py
 Home-page: https://github.com/imayhaveborkedit/discord-ext-voice-recv
 Author: Imayhaveborkedit
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `discord-ext-voice_recv-0.1.8a99/discord_ext_voice_recv.egg-info/SOURCES.txt` & `discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.8a99/setup.py` & `discord-ext-voice_recv-0.1.9a106/setup.py`

 * *Files identical despite different names*

