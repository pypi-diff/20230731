# Comparing `tmp/discord-ext-voice_recv-0.1.9a106.tar.gz` & `tmp/discord-ext-voice_recv-0.2.0a108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-voice_recv-0.1.9a106.tar", last modified: Sun Jul 30 22:59:11 2023, max compression
+gzip compressed data, was "discord-ext-voice_recv-0.2.0a108.tar", last modified: Mon Jul 31 02:39:18 2023, max compression
```

## Comparing `discord-ext-voice_recv-0.1.9a106.tar` & `discord-ext-voice_recv-0.2.0a108.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.212984 discord-ext-voice_recv-0.1.9a106/
--rw-rw-rw-   0        0        0     1091 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.9a106/LICENSE
--rw-rw-rw-   0        0        0    10039 2023-07-30 22:59:11.212984 discord-ext-voice_recv-0.1.9a106/PKG-INFO
--rw-rw-rw-   0        0        0     8952 2023-07-29 00:55:14.000000 discord-ext-voice_recv-0.1.9a106/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.137028 discord-ext-voice_recv-0.1.9a106/discord/
-drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.138027 discord-ext-voice_recv-0.1.9a106/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.176005 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/
--rw-rw-rw-   0        0        0      362 2023-07-30 20:09:15.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/__init__.py
--rw-rw-rw-   0        0        0     5487 2023-07-29 19:04:30.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/buffer.py
--rw-rw-rw-   0        0        0     3278 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/gateway.py
--rw-rw-rw-   0        0        0    35905 2023-07-30 22:54:36.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/opus.py
--rw-rw-rw-   0        0        0     8387 2023-07-30 19:38:50.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/reader.py
--rw-rw-rw-   0        0        0    12432 2023-07-30 16:48:39.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/rtp.py
--rw-rw-rw-   0        0        0     5426 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/silence.py
--rw-rw-rw-   0        0        0    12365 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/sinks.py
--rw-rw-rw-   0        0        0      911 2023-06-17 04:25:42.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/types.py
--rw-rw-rw-   0        0        0     2237 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/utils.py
--rw-rw-rw-   0        0        0     2623 2023-06-17 05:04:12.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/video.py
--rw-rw-rw-   0        0        0     5740 2023-07-30 19:39:09.000000 discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-07-30 22:59:11.209988 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/
--rw-rw-rw-   0        0        0    10039 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-07-30 22:59:11.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-05 23:03:01.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 22:59:10.000000 discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 22:59:11.213989 discord-ext-voice_recv-0.1.9a106/setup.cfg
--rw-rw-rw-   0        0        0     1917 2023-07-23 07:43:28.000000 discord-ext-voice_recv-0.1.9a106/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:39:18.491102 discord-ext-voice_recv-0.2.0a108/
+-rw-rw-rw-   0        0        0     1091 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.2.0a108/LICENSE
+-rw-rw-rw-   0        0        0    10574 2023-07-31 02:39:18.491102 discord-ext-voice_recv-0.2.0a108/PKG-INFO
+-rw-rw-rw-   0        0        0     9476 2023-07-31 02:29:00.000000 discord-ext-voice_recv-0.2.0a108/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:39:18.434119 discord-ext-voice_recv-0.2.0a108/discord/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:39:18.434119 discord-ext-voice_recv-0.2.0a108/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:39:18.461104 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/
+-rw-rw-rw-   0        0        0      362 2023-07-31 02:32:57.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/__init__.py
+-rw-rw-rw-   0        0        0     5487 2023-07-29 19:04:30.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/buffer.py
+-rw-rw-rw-   0        0        0     3459 2023-07-31 01:52:03.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/gateway.py
+-rw-rw-rw-   0        0        0    35905 2023-07-30 22:54:36.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/opus.py
+-rw-rw-rw-   0        0        0     8458 2023-07-31 00:50:41.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/reader.py
+-rw-rw-rw-   0        0        0    12432 2023-07-30 16:48:39.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/rtp.py
+-rw-rw-rw-   0        0        0     5426 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/silence.py
+-rw-rw-rw-   0        0        0    12365 2023-07-30 22:38:02.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/sinks.py
+-rw-rw-rw-   0        0        0      911 2023-06-17 04:25:42.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/types.py
+-rw-rw-rw-   0        0        0     2237 2023-04-09 21:50:44.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/utils.py
+-rw-rw-rw-   0        0        0     2623 2023-06-17 05:04:12.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/video.py
+-rw-rw-rw-   0        0        0     6244 2023-07-31 01:13:17.000000 discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:39:18.489103 discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/
+-rw-rw-rw-   0        0        0    10574 2023-07-31 02:39:18.000000 discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-31 02:39:18.000000 discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:39:18.000000 discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-05 23:03:01.000000 discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-07-31 02:39:18.000000 discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 02:39:18.000000 discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:39:18.492084 discord-ext-voice_recv-0.2.0a108/setup.cfg
+-rw-rw-rw-   0        0        0     1917 2023-07-23 07:43:28.000000 discord-ext-voice_recv-0.2.0a108/setup.py
```

### Comparing `discord-ext-voice_recv-0.1.9a106/LICENSE` & `discord-ext-voice_recv-0.2.0a108/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/PKG-INFO` & `discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: discord-ext-voice_recv
-Version: 0.1.9a106
+Name: discord-ext-voice-recv
+Version: 0.2.0a108
 Summary: Experimental voice receive extension for discord.py
 Home-page: https://github.com/imayhaveborkedit/discord-ext-voice-recv
 Author: Imayhaveborkedit
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,17 @@
 ## Feature overview
 ### Custom VoiceProtocol client
 No monkey patching or bizarre hacks required.  Simply use the library feature to use `VoiceRecvClient` as the voice client class.  See [Usage](#usage).
 
 ### Six new events
 This extension adds the unimplemented voice websocket events and one virtual event.  See [New Events](#new-events).
 
+### Speaking state
+It is now possible to determine if a member is speaking or not, using `VoiceRecvClient.get_speaking()`.  An event for changes is on the todo list as a maybe.
+
 ### Simple and familiar API
 The overall API is designed to mirror the discord.py voice send API, with `AudioSink` being the counterpart to the existing `AudioSource`.  See [Sinks](#sinks).
 
 ### Convenient included utilities
 Batteries included in the form of useful built in `AudioSinks`.  Some to match their `AudioSource` counterpart, some I merely considered useful.  See... uh... TODO.
 
 ### More or less typed
@@ -91,14 +94,19 @@
 Stops receiving audio.
 
 ```python
 def stop_playing() -> None
 ```
 Stops playing audio.  This function is identical to `discord.VoiceClient.stop()`.
 
+```python
+def get_speaking(member: discord.Member | discord.User) -> bool | None
+```
+Gets the speaking state (voice activity, the green circle) of a member.  User is typed in for convenience.  Returns None if the member was not found.
+
 ## Sinks
 The api of this extension is designed to mirror the discord.py voice send api.  Sending audio uses the `AudioSource` class, while receiving audio uses the `AudioSink` class.  A sink is designed to be the inverse of a source.  Essentially, a source is a callback called by discord.py to produce a chunk of audio data.  Conversely, a sink is a callback called by the library to handle a chunk of audio.  Sinks can be composed in the same fashion as sources, creating an audio processing pipeline.  Sources and sinks can even combined into one object to handle both tasks, such as creating a feedback loop.
 
 Special care should be taken not to write excessively computationally expensive code, as python is not particularly well suited to realtime audio processing.
 
 Due to voice receive being somewhat more complex than voice sending, sinks have additional functionality compared to sources.  However, the core sink functions should look relatively familiar.
 
@@ -138,19 +146,22 @@
         self.do_something_like_handle_disconnect(ssrc)
 ```
 
 Note that these functions must be sync functions, as they are dispatched from a thread.  Trying to use a coroutine will result in an error.  This restriction only applies to sink listeners, and normal async event listeners will function as per usual.  The event listener dispatch thread is different from the one used to dispatch the `write()` callback so potential threadsafety issues should be considered.  A decorator argument to run the event callback in the other thread may be added later.
 
 ## New events
 ```python
-async def on_voice_member_speak(member: discord.Member, ssrc: int)
+async def on_voice_member_speaking_state(member: discord.Member, ssrc: int, state: SpeakingState | int)
 ```
-Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
+First and foremost, this event does **NOT** refer to the speaking indicator in discord (the green circle).  For voice activity, see `...TODO...`.
+This event is fired when the speaking state of a member changes.  This happens when:
+- A member first speaks (transmits audio) in a voice, but only once
+- A member activates or deactivates priority speaker mode
 
-This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
+This event is fired once initially to reveal the ssrc of a member, an identifier to map packets to their originating member.  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.
 
 ```python
 async def on_voice_member_disconnect(member: discord.Member, ssrc: int | None)
 ```
 Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
 
 ```python
```

### Comparing `discord-ext-voice_recv-0.1.9a106/README.md` & `discord-ext-voice_recv-0.2.0a108/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 ## Feature overview
 ### Custom VoiceProtocol client
 No monkey patching or bizarre hacks required.  Simply use the library feature to use `VoiceRecvClient` as the voice client class.  See [Usage](#usage).
 
 ### Six new events
 This extension adds the unimplemented voice websocket events and one virtual event.  See [New Events](#new-events).
 
+### Speaking state
+It is now possible to determine if a member is speaking or not, using `VoiceRecvClient.get_speaking()`.  An event for changes is on the todo list as a maybe.
+
 ### Simple and familiar API
 The overall API is designed to mirror the discord.py voice send API, with `AudioSink` being the counterpart to the existing `AudioSource`.  See [Sinks](#sinks).
 
 ### Convenient included utilities
 Batteries included in the form of useful built in `AudioSinks`.  Some to match their `AudioSource` counterpart, some I merely considered useful.  See... uh... TODO.
 
 ### More or less typed
@@ -68,14 +71,19 @@
 Stops receiving audio.
 
 ```python
 def stop_playing() -> None
 ```
 Stops playing audio.  This function is identical to `discord.VoiceClient.stop()`.
 
+```python
+def get_speaking(member: discord.Member | discord.User) -> bool | None
+```
+Gets the speaking state (voice activity, the green circle) of a member.  User is typed in for convenience.  Returns None if the member was not found.
+
 ## Sinks
 The api of this extension is designed to mirror the discord.py voice send api.  Sending audio uses the `AudioSource` class, while receiving audio uses the `AudioSink` class.  A sink is designed to be the inverse of a source.  Essentially, a source is a callback called by discord.py to produce a chunk of audio data.  Conversely, a sink is a callback called by the library to handle a chunk of audio.  Sinks can be composed in the same fashion as sources, creating an audio processing pipeline.  Sources and sinks can even combined into one object to handle both tasks, such as creating a feedback loop.
 
 Special care should be taken not to write excessively computationally expensive code, as python is not particularly well suited to realtime audio processing.
 
 Due to voice receive being somewhat more complex than voice sending, sinks have additional functionality compared to sources.  However, the core sink functions should look relatively familiar.
 
@@ -115,19 +123,22 @@
         self.do_something_like_handle_disconnect(ssrc)
 ```
 
 Note that these functions must be sync functions, as they are dispatched from a thread.  Trying to use a coroutine will result in an error.  This restriction only applies to sink listeners, and normal async event listeners will function as per usual.  The event listener dispatch thread is different from the one used to dispatch the `write()` callback so potential threadsafety issues should be considered.  A decorator argument to run the event callback in the other thread may be added later.
 
 ## New events
 ```python
-async def on_voice_member_speak(member: discord.Member, ssrc: int)
+async def on_voice_member_speaking_state(member: discord.Member, ssrc: int, state: SpeakingState | int)
 ```
-Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
+First and foremost, this event does **NOT** refer to the speaking indicator in discord (the green circle).  For voice activity, see `...TODO...`.
+This event is fired when the speaking state of a member changes.  This happens when:
+- A member first speaks (transmits audio) in a voice, but only once
+- A member activates or deactivates priority speaker mode
 
-This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
+This event is fired once initially to reveal the ssrc of a member, an identifier to map packets to their originating member.  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.
 
 ```python
 async def on_voice_member_disconnect(member: discord.Member, ssrc: int | None)
 ```
 Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
 
 ```python
```

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/buffer.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/buffer.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/gateway.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import logging
 
-from typing import TYPE_CHECKING
+from discord.enums import SpeakingState
 
 from .video import VoiceVideoStreams
 
+from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from discord.gateway import DiscordVoiceWebSocket
     from .voice_client import VoiceRecvClient
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
@@ -61,20 +62,21 @@
         # log.info("Doing voice hacks")
         # await _do_hacks(self)
 
         if vc._reader:
             vc._reader.update_secret_box()
 
     elif op == self.SPEAKING:
-        # SPEAKING is not actually speaking anymore but it still has the ssrc
+        # this event refers to the speaking MODE, e.g. priority speaker
         uid = int(data['user_id'])
         ssrc = data['ssrc']
+        state = SpeakingState.try_value(data['speaking']) # type: ignore
         vc._add_ssrc(uid, ssrc)
         member = vc.guild.get_member(uid)
-        vc.dispatch("voice_member_speak", member, ssrc)
+        vc.dispatch("voice_member_speaking_state", member, ssrc, state)
 
     # aka VIDEO
     elif op == self.CLIENT_CONNECT:
         uid = int(data['user_id'])
         vc._add_ssrc(uid, data['audio_ssrc'])
         member = vc.guild.get_member(uid)
         streams = VoiceVideoStreams(data=data, vc=vc) # type: ignore
@@ -87,14 +89,15 @@
         if vc._reader is not None and ssrc is not None:
             log.debug("Destroying decoder for %s, ssrc=%s", uid, ssrc)
             vc._reader.router.destroy_decoder(ssrc)
 
         vc._remove_ssrc(user_id=uid)
         member = vc.guild.get_member(uid)
         vc.dispatch("voice_member_disconnect", member, ssrc)
+        vc._speaking_cache.pop(ssrc, None) # type: ignore
 
     elif op == FLAGS:
         uid = int(data['user_id'])
         member = vc.guild.get_member(uid)
         vc.dispatch("voice_member_flags", member, data['flags'])
 
     elif op == PLATFORM:
```

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/opus.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/opus.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/reader.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,15 @@
                 if not packet:
                     continue
 
             # I could combine these in a function in the router but this is faster
             if rtcp:
                 self.router.feed_rtcp(packet) # type: ignore
             else:
+                self.client._speaking_cache[packet.ssrc] = time.time()
                 self.router.feed_rtp(packet) # type: ignore
 
     def is_listening(self):
         return not self._end.is_set()
 
     def stop(self):
         self._end.set()
```

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/rtp.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/rtp.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/silence.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/silence.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/sinks.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/sinks.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/types.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/types.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/utils.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/utils.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/video.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/video.py`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/discord/ext/voice_recv/voice_client.py` & `discord-ext-voice_recv-0.2.0a108/discord/ext/voice_recv/voice_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
+import time
 import asyncio
 import logging
 import threading
 
 import discord
 from discord.gateway import DiscordVoiceWebSocket
 from discord.utils import MISSING
@@ -33,15 +34,16 @@
     def __init__(self, client, channel):
         super().__init__(client, channel)
 
         self._connecting = threading.Condition()
         self._reader: Optional[AudioReader] = None
         self._ssrc_to_id: Dict[int, int] = {}
         self._id_to_ssrc: Dict[int, int] = {}
-        self._event_listeners: dict[str, list] = {}
+        self._event_listeners: Dict[str, list] = {}
+        self._speaking_cache: Dict[int, float] = {}
 
     async def connect_websocket(self):
         ws = await DiscordVoiceWebSocket.from_client(self, hook=hook)
         self._connected.clear()
         while ws.secret_key is None:
             await ws.poll_event()
         self._connected.set()
@@ -174,7 +176,20 @@
         if not isinstance(sink, AudioSink):
             raise TypeError('expected AudioSink not {0.__class__.__name__}.'.format(sink))
 
         if self._reader is None:
             raise ValueError('Not receiving anything.')
 
         self._reader.set_sink(sink)
+
+    def get_speaking(self, member: discord.Member | discord.User) -> Optional[bool]:
+        """Returns if a member is speaking (approximately), or None if not found."""
+
+        ssrc = self._get_ssrc_from_id(member.id)
+        if ssrc is None:
+            return
+
+        last_packet_time = self._speaking_cache.get(ssrc, None)
+        if last_packet_time is None:
+            return
+
+        return time.time() - last_packet_time < 0.02
```

### Comparing `discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/PKG-INFO` & `discord-ext-voice_recv-0.2.0a108/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: discord-ext-voice-recv
-Version: 0.1.9a106
+Name: discord-ext-voice_recv
+Version: 0.2.0a108
 Summary: Experimental voice receive extension for discord.py
 Home-page: https://github.com/imayhaveborkedit/discord-ext-voice-recv
 Author: Imayhaveborkedit
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,17 @@
 ## Feature overview
 ### Custom VoiceProtocol client
 No monkey patching or bizarre hacks required.  Simply use the library feature to use `VoiceRecvClient` as the voice client class.  See [Usage](#usage).
 
 ### Six new events
 This extension adds the unimplemented voice websocket events and one virtual event.  See [New Events](#new-events).
 
+### Speaking state
+It is now possible to determine if a member is speaking or not, using `VoiceRecvClient.get_speaking()`.  An event for changes is on the todo list as a maybe.
+
 ### Simple and familiar API
 The overall API is designed to mirror the discord.py voice send API, with `AudioSink` being the counterpart to the existing `AudioSource`.  See [Sinks](#sinks).
 
 ### Convenient included utilities
 Batteries included in the form of useful built in `AudioSinks`.  Some to match their `AudioSource` counterpart, some I merely considered useful.  See... uh... TODO.
 
 ### More or less typed
@@ -91,14 +94,19 @@
 Stops receiving audio.
 
 ```python
 def stop_playing() -> None
 ```
 Stops playing audio.  This function is identical to `discord.VoiceClient.stop()`.
 
+```python
+def get_speaking(member: discord.Member | discord.User) -> bool | None
+```
+Gets the speaking state (voice activity, the green circle) of a member.  User is typed in for convenience.  Returns None if the member was not found.
+
 ## Sinks
 The api of this extension is designed to mirror the discord.py voice send api.  Sending audio uses the `AudioSource` class, while receiving audio uses the `AudioSink` class.  A sink is designed to be the inverse of a source.  Essentially, a source is a callback called by discord.py to produce a chunk of audio data.  Conversely, a sink is a callback called by the library to handle a chunk of audio.  Sinks can be composed in the same fashion as sources, creating an audio processing pipeline.  Sources and sinks can even combined into one object to handle both tasks, such as creating a feedback loop.
 
 Special care should be taken not to write excessively computationally expensive code, as python is not particularly well suited to realtime audio processing.
 
 Due to voice receive being somewhat more complex than voice sending, sinks have additional functionality compared to sources.  However, the core sink functions should look relatively familiar.
 
@@ -138,19 +146,22 @@
         self.do_something_like_handle_disconnect(ssrc)
 ```
 
 Note that these functions must be sync functions, as they are dispatched from a thread.  Trying to use a coroutine will result in an error.  This restriction only applies to sink listeners, and normal async event listeners will function as per usual.  The event listener dispatch thread is different from the one used to dispatch the `write()` callback so potential threadsafety issues should be considered.  A decorator argument to run the event callback in the other thread may be added later.
 
 ## New events
 ```python
-async def on_voice_member_speak(member: discord.Member, ssrc: int)
+async def on_voice_member_speaking_state(member: discord.Member, ssrc: int, state: SpeakingState | int)
 ```
-Called when a member first speaks (transmits audio) in a voice channel.  This event is only called once per their voice session (ssrc assignment).  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.  The main purpose of this event is to reveal the ssrc of a member, to map packets to their originating member.
+First and foremost, this event does **NOT** refer to the speaking indicator in discord (the green circle).  For voice activity, see `...TODO...`.
+This event is fired when the speaking state of a member changes.  This happens when:
+- A member first speaks (transmits audio) in a voice, but only once
+- A member activates or deactivates priority speaker mode
 
-This is **NOT** a speaking indicator event.  The speaking indicator is determined by packet activity.  This functionality will be added in the future.
+This event is fired once initially to reveal the ssrc of a member, an identifier to map packets to their originating member.  Any packets received from this member before this event fires can (probably) be safely ignored since they are likely just silence packets.
 
 ```python
 async def on_voice_member_disconnect(member: discord.Member, ssrc: int | None)
 ```
 Called when a member disconnects from a voice channel. The `ssrc` parameter is the unique id a member has to identify which packets belong to them.  This is useful when using custom sinks, particularly those that handle packets from multiple members.
 
 ```python
```

### Comparing `discord-ext-voice_recv-0.1.9a106/discord_ext_voice_recv.egg-info/SOURCES.txt` & `discord-ext-voice_recv-0.2.0a108/discord_ext_voice_recv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-ext-voice_recv-0.1.9a106/setup.py` & `discord-ext-voice_recv-0.2.0a108/setup.py`

 * *Files identical despite different names*

