# Comparing `tmp/fortnitepy-3.6.8.tar.gz` & `tmp/fortnitepy-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortnitepy-3.6.8.tar", last modified: Sun Dec 18 00:06:41 2022, max compression
+gzip compressed data, was "fortnitepy-3.6.9.tar", last modified: Mon Jul 31 14:12:03 2023, max compression
```

## Comparing `fortnitepy-3.6.8.tar` & `fortnitepy-3.6.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 terbau    (1000) terbau    (1000)        0 2022-12-18 00:06:41.290682 fortnitepy-3.6.8/
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     1068 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/LICENSE
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     4282 2022-12-18 00:06:41.290682 fortnitepy-3.6.8/PKG-INFO
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     3221 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/README.md
-drwxrwxr-x   0 terbau    (1000) terbau    (1000)        0 2022-12-18 00:06:41.290682 fortnitepy-3.6.8/fortnitepy/
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     2293 2022-12-18 00:00:54.000000 fortnitepy-3.6.8/fortnitepy/__init__.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    40932 2022-12-18 00:00:29.000000 fortnitepy-3.6.8/fortnitepy/auth.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)   117774 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/client.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     7723 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/enums.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     7760 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/errors.py
-drwxrwxr-x   0 terbau    (1000) terbau    (1000)        0 2022-12-18 00:06:41.286682 fortnitepy-3.6.8/fortnitepy/ext/
-drwxrwxr-x   0 terbau    (1000) terbau    (1000)        0 2022-12-18 00:06:41.290682 fortnitepy-3.6.8/fortnitepy/ext/commands/
--rw-rw-r--   0 terbau    (1000) terbau    (1000)      195 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/__init__.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     1130 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/_types.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    32192 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/bot.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    15374 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/cog.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    11690 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/context.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     6113 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/converter.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     8382 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/cooldown.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    60255 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/core.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    14407 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/errors.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    50693 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/help.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     1214 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/typedefs.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     6204 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/ext/commands/view.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    18535 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/friend.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    61318 2022-12-18 00:00:29.000000 fortnitepy-3.6.8/fortnitepy/http.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     3674 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/kairos.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     3852 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/message.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     2670 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/news.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)   149622 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/party.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     3748 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/playlist.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    13918 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/presence.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    10143 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/stats.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    10533 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/store.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     1361 2022-12-17 23:23:48.000000 fortnitepy-3.6.8/fortnitepy/typedefs.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    22715 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/user.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     2556 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/utils.py
--rw-rw-r--   0 terbau    (1000) terbau    (1000)    58476 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/fortnitepy/xmpp.py
-drwxrwxr-x   0 terbau    (1000) terbau    (1000)        0 2022-12-18 00:06:41.290682 fortnitepy-3.6.8/fortnitepy.egg-info/
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     4282 2022-12-18 00:06:41.000000 fortnitepy-3.6.8/fortnitepy.egg-info/PKG-INFO
--rw-rw-r--   0 terbau    (1000) terbau    (1000)      994 2022-12-18 00:06:41.000000 fortnitepy-3.6.8/fortnitepy.egg-info/SOURCES.txt
--rw-rw-r--   0 terbau    (1000) terbau    (1000)        1 2022-12-18 00:06:41.000000 fortnitepy-3.6.8/fortnitepy.egg-info/dependency_links.txt
--rw-rw-r--   0 terbau    (1000) terbau    (1000)      101 2022-12-18 00:06:41.000000 fortnitepy-3.6.8/fortnitepy.egg-info/requires.txt
--rw-rw-r--   0 terbau    (1000) terbau    (1000)       11 2022-12-18 00:06:41.000000 fortnitepy-3.6.8/fortnitepy.egg-info/top_level.txt
--rw-rw-r--   0 terbau    (1000) terbau    (1000)       38 2022-12-18 00:06:41.290682 fortnitepy-3.6.8/setup.cfg
--rw-rw-r--   0 terbau    (1000) terbau    (1000)     1831 2022-12-18 00:00:15.000000 fortnitepy-3.6.8/setup.py
+drwxr-xr-x   0 brage.baugerod   (501) staff       (20)        0 2023-07-31 14:12:03.503559 fortnitepy-3.6.9/
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     1068 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/LICENSE
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     4282 2023-07-31 14:12:03.503284 fortnitepy-3.6.9/PKG-INFO
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     3221 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/README.md
+drwxr-xr-x   0 brage.baugerod   (501) staff       (20)        0 2023-07-31 14:12:03.479599 fortnitepy-3.6.9/fortnitepy/
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     2293 2023-07-31 14:06:18.000000 fortnitepy-3.6.9/fortnitepy/__init__.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    40932 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/auth.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)   117774 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/client.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     7746 2023-07-31 14:08:45.000000 fortnitepy-3.6.9/fortnitepy/enums.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     7760 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/errors.py
+drwxr-xr-x   0 brage.baugerod   (501) staff       (20)        0 2023-07-31 14:12:03.460684 fortnitepy-3.6.9/fortnitepy/ext/
+drwxr-xr-x   0 brage.baugerod   (501) staff       (20)        0 2023-07-31 14:12:03.502350 fortnitepy-3.6.9/fortnitepy/ext/commands/
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)      195 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/__init__.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     1130 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/_types.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    32192 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/bot.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    15374 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/cog.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    11690 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/context.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     6113 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/converter.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     8382 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/cooldown.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    60255 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/core.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    14407 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/errors.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    50693 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/help.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     1214 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/typedefs.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     6204 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/ext/commands/view.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    18535 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/friend.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    61318 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/http.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     3674 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/kairos.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     3852 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/message.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     2670 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/news.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)   149858 2023-07-31 14:08:45.000000 fortnitepy-3.6.9/fortnitepy/party.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     3748 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/playlist.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    13918 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/presence.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    10143 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/stats.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    10533 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/store.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     1361 2023-07-31 13:31:49.000000 fortnitepy-3.6.9/fortnitepy/typedefs.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    22715 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/user.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     2556 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/utils.py
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)    58476 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/fortnitepy/xmpp.py
+drwxr-xr-x   0 brage.baugerod   (501) staff       (20)        0 2023-07-31 14:12:03.490925 fortnitepy-3.6.9/fortnitepy.egg-info/
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     4282 2023-07-31 14:12:03.000000 fortnitepy-3.6.9/fortnitepy.egg-info/PKG-INFO
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)      994 2023-07-31 14:12:03.000000 fortnitepy-3.6.9/fortnitepy.egg-info/SOURCES.txt
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)        1 2023-07-31 14:12:03.000000 fortnitepy-3.6.9/fortnitepy.egg-info/dependency_links.txt
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)      101 2023-07-31 14:12:03.000000 fortnitepy-3.6.9/fortnitepy.egg-info/requires.txt
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)       11 2023-07-31 14:12:03.000000 fortnitepy-3.6.9/fortnitepy.egg-info/top_level.txt
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)       38 2023-07-31 14:12:03.503639 fortnitepy-3.6.9/setup.cfg
+-rw-r--r--   0 brage.baugerod   (501) staff       (20)     1831 2023-07-31 13:42:02.000000 fortnitepy-3.6.9/setup.py
```

### Comparing `fortnitepy-3.6.8/LICENSE` & `fortnitepy-3.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/PKG-INFO` & `fortnitepy-3.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortnitepy
-Version: 3.6.8
+Version: 3.6.9
 Summary: Library for interacting with fortnite services
 Home-page: https://github.com/Terbau/fortnitepy
 Author: Terbau
 License: MIT
 Project-URL: Documentation, https://fortnitepy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Terbau/fortnitepy/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortnitepy-3.6.8/README.md` & `fortnitepy-3.6.9/README.md`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/__init__.py` & `fortnitepy-3.6.9/fortnitepy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = '3.6.8'
+__version__ = '3.6.9'
 
 from .client import Client, run_multiple, start_multiple, close_multiple
 from .auth import (Auth, EmailAndPasswordAuth, ExchangeCodeAuth,
                    AuthorizationCodeAuth, DeviceAuth, RefreshTokenAuth,
                    AdvancedAuth)
 from .friend import Friend, IncomingPendingFriend, OutgoingPendingFriend
 from .message import FriendMessage, PartyMessage
```

### Comparing `fortnitepy-3.6.8/fortnitepy/auth.py` & `fortnitepy-3.6.9/fortnitepy/auth.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/client.py` & `fortnitepy-3.6.9/fortnitepy/client.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/enums.py` & `fortnitepy-3.6.9/fortnitepy/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     GAMEPAD          = 'gamepad'
     TOUCH            = 'touch'
 
 
 class Region(Enum):
     NAEAST     = 'NAE'
     NAWEST     = 'NAW'
+    NACENTRAL  = 'NAC'
     EUROPE     = 'EU'
     BRAZIL     = 'BR'
     OCEANIA    = 'OCE'
     ASIA       = 'ASIA'
     MIDDLEEAST = 'ME'
```

### Comparing `fortnitepy-3.6.8/fortnitepy/errors.py` & `fortnitepy-3.6.9/fortnitepy/errors.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/_types.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/bot.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/cog.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/context.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/converter.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/cooldown.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/cooldown.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/core.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/errors.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/help.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/typedefs.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/typedefs.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/ext/commands/view.py` & `fortnitepy-3.6.9/fortnitepy/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/friend.py` & `fortnitepy-3.6.9/fortnitepy/friend.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/http.py` & `fortnitepy-3.6.9/fortnitepy/http.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/kairos.py` & `fortnitepy-3.6.9/fortnitepy/kairos.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/message.py` & `fortnitepy-3.6.9/fortnitepy/message.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/news.py` & `fortnitepy-3.6.9/fortnitepy/news.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/party.py` & `fortnitepy-3.6.9/fortnitepy/party.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         .. code-block:: python3
 
             from fortnitepy import ClientParty
             from functools import partial
 
             [
                 partial(ClientParty.set_custom_key, 'myawesomekey'),
-                partial(ClientParty.set_playlist, 'Playlist_PlaygroundV2', region=fortnitepy.Region.EUROPE)
+                partial(ClientParty.set_playlist, 'Playlist_PlaygroundV2')
             ]
 
     Attributes
     ----------
     team_change_allowed: :class:`bool`
         Whether or not players are able to manually swap party team
         with another player. This setting only works if the client is the
@@ -591,15 +591,15 @@
             }),
             'Default:MatchmakingLevel_U': '0',
             'Default:ZoneInstanceId_s': '',
             'Default:HomeBaseVersion_U': '1',
             'Default:FrontendEmote_j': json.dumps({
                 'FrontendEmote': {
                     'emoteItemDef': 'None',
-                    'emoteItemDefEncryptionKey': '',
+                    'emoteEKey': '',
                     'emoteSection': -1,
                 },
             }),
             'Default:NumAthenaPlayersLeft_U': '0',
             'Default:UtcTimeStartedMatchAthena_s': '0001-01-01T00:00:00.000Z',
             'Default:LobbyState_j': json.dumps({
                 'LobbyState': {
@@ -915,15 +915,15 @@
                   emote_ekey: Optional[str] = None,
                   section: Optional[int] = None) -> Dict[str, Any]:
         data = (self.get_prop('Default:FrontendEmote_j'))['FrontendEmote']
 
         if emote is not None:
             data['emoteItemDef'] = self.maybesub(emote)
         if emote_ekey is not None:
-            data['emoteItemDefEncryptionKey'] = emote_ekey
+            data['emoteEKey'] = emote_ekey
         if section is not None:
             data['emoteSection'] = section
 
         final = {'FrontendEmote': data}
         key = 'Default:FrontendEmote_j'
         return {key: self.set_prop(key, final)}
 
@@ -1092,17 +1092,17 @@
             'Default:MatchmakingInfoString_s': '',
             'Default:CustomMatchKey_s': '',
             'Default:PlaylistData_j': json.dumps({
                 'PlaylistData': {
                     'playlistName': 'Playlist_DefaultDuo',
                     'tournamentId': '',
                     'eventWindowId': '',
-                    'regionId': 'EU',
                 },
             }),
+            'Default:RegionId_s': 'EU',
             'Default:AthenaSquadFill_b': 'true',
             'Default:AllowJoinInProgress_b': 'false',
             'Default:LFGTime_s': '0001-01-01T00:00:00.000Z',
             'Default:PartyIsJoinedInProgress_b': 'false',
             'Default:GameSessionKey_s': '',
             'Default:RawSquadAssignments_j': json.dumps({
                 'RawSquadAssignments': []
@@ -1134,22 +1134,25 @@
     @property
     def playlist_info(self) -> Tuple[str]:
         base = self.get_prop('Default:PlaylistData_j')
         info = base['PlaylistData']
 
         return (info['playlistName'],
                 info['tournamentId'],
-                info['eventWindowId'],
-                info['regionId'])
+                info['eventWindowId'])
 
     @property
     def squad_fill(self) -> bool:
         return self.get_prop('Default:AthenaSquadFill_b')
 
     @property
+    def region(self) -> Region:
+        return Region(self.get_prop('Default:RegionId_s'))
+
+    @property
     def privacy(self) -> Optional[PartyPrivacy]:
         raw = self.get_prop('Default:PrivacySettings_j')
         curr_priv = raw['PrivacySettings']
 
         for privacy in PartyPrivacy:
             if curr_priv['partyType'] != privacy.value['partyType']:
                 continue
@@ -1175,31 +1178,32 @@
     def set_squad_assignments(self, data: List[dict]) -> Dict[str, Any]:
         final = {'RawSquadAssignments': data}
         key = 'Default:RawSquadAssignments_j'
         return {key: self.set_prop(key, final)}
 
     def set_playlist(self, playlist: Optional[str] = None, *,
                      tournament: Optional[str] = None,
-                     event_window: Optional[str] = None,
-                     region: Optional[Region] = None) -> Dict[str, Any]:
+                     event_window: Optional[str] = None) -> Dict[str, Any]:
         data = (self.get_prop('Default:PlaylistData_j'))['PlaylistData']
 
         if playlist is not None:
             data['playlistName'] = playlist
         if tournament is not None:
             data['tournamentId'] = tournament
         if event_window is not None:
             data['eventWindowId'] = event_window
-        if region is not None:
-            data['regionId'] = region
 
         final = {'PlaylistData': data}
         key = 'Default:PlaylistData_j'
         return {key: self.set_prop(key, final)}
 
+    def set_region(self, region: Region) -> Dict[str, Any]:
+        key = 'Default:RegionId_s'
+        return {key: self.set_prop(key, region.value)}
+
     def set_custom_key(self, key: str) -> Dict[str, Any]:
         _key = 'Default:CustomMatchKey_s'
         return {_key: self.set_prop(_key, key)}
 
     def set_fill(self, val: str) -> Dict[str, Any]:
         key = 'Default:AthenaSquadFill_b'
         return {key: self.set_prop(key, (str(val)).lower())}
@@ -2540,16 +2544,16 @@
 
         Raises
         ------
         HTTPException
             An error occured while requesting.
         """
         if asset != '' and '.' not in asset:
-            asset = ("AthenaDanceItemDefinition'/Game/Athena/Items/"
-                     "Cosmetics/Dances/{0}.{0}'".format(asset))
+            asset = ("/BRCosmetics/Athena/Items/"
+                     "Cosmetics/Dances/{0}.{0}".format(asset))
 
         prop = self.meta.set_emote(
             emote=asset,
             emote_ekey=key,
             section=section
         )
 
@@ -2594,16 +2598,16 @@
 
         Raises
         ------
         HTTPException
             An error occured while requesting.
         """
         if asset != '' and '.' not in asset:
-            asset = ("AthenaDanceItemDefinition'/Game/Athena/Items/"
-                     "Cosmetics/Dances/Emoji/{0}.{0}'".format(asset))
+            asset = ("/BRCosmetics/Athena/Items/"
+                     "Cosmetics/Dances/Emoji/{0}.{0}".format(asset))
 
         prop = self.meta.set_emote(
             emote=asset,
             emote_ekey=key,
             section=section
         )
 
@@ -3025,43 +3029,46 @@
         """:class:`PartyMember`: The leader of the party."""
         for member in self._members.values():
             if member.leader:
                 return member
 
     @property
     def playlist_info(self) -> Tuple[str]:
-        """:class:`tuple`: A tuple containing the name, tournament, event
-        window and region of the currently set playlist.
+        """:class:`tuple`: A tuple containing the name, tournament and
+        event window of the currently set playlist.
 
         Example output: ::
 
             # output for default duos
             (
                 'Playlist_DefaultDuo',
                 '',
                 '',
-                'EU'
             )
 
             # output for arena trios
             (
                 'Playlist_ShowdownAlt_Trios',
                 'epicgames_Arena_S10_Trios',
                 'Arena_S10_Division1_Trios',
-                'EU'
             )
         """
         return self.meta.playlist_info
 
     @property
     def squad_fill(self) -> bool:
         """:class:`bool`: ``True`` if squad fill is enabled else ``False``."""
         return self.meta.squad_fill
 
     @property
+    def region(self) -> Region:
+        """Optional[:class:`Region`]: The region of the party."""
+        return self.meta.region
+
+    @property
     def privacy(self) -> PartyPrivacy:
         """:class:`PartyPrivacy`: The currently set privacy of this party."""
         return self.meta.privacy
 
     @property
     def squad_assignments(self) -> Dict[PartyMember, SquadAssignment]:
         """Dict[:class:`PartyMember`, :class:`SquadAssignment`]: The squad assignments
@@ -3598,24 +3605,23 @@
                             *coros: List[Union[Awaitable, functools.partial]]
                             ) -> None:
         """|coro|
 
         Edits multiple meta parts at once and keeps the changes for when new
         parties are created.
 
-        This example sets the custom key to ``myawesomekey`` and the playlist to Creative
-        in the Europe region.: ::
+        This example sets the custom key to ``myawesomekey`` and the playlist to Creative.: ::
 
             from functools import partial
 
             async def edit_and_keep_party():
                 party = client.party
                 await party.edit_and_keep(
                     partial(party.set_custom_key, 'myawesomekey'),
-                    partial(party.set_playlist, 'Playlist_PlaygroundV2', region=fortnitepy.Region.EUROPE)
+                    partial(party.set_playlist, 'Playlist_PlaygroundV2')
                 )
 
         Parameters
         ----------
         *coros: :class:`functools.partial`
             A list of coroutines that should be included in the edit. Unlike
             :meth:`ClientParty.edit()`, this method only takes
@@ -3910,65 +3916,79 @@
                 updated=updated,
                 deleted=deleted,
                 config=config,
             )
 
     async def set_playlist(self, playlist: Optional[str] = None,
                            tournament: Optional[str] = None,
-                           event_window: Optional[str] = None,
-                           region: Optional[Region] = None) -> None:
+                           event_window: Optional[str] = None) -> None:
         """|coro|
 
         Sets the current playlist of the party.
 
-        Sets the playlist to Duos EU: ::
+        Sets the playlist to Duos: ::
 
             await party.set_playlist(
-                playlist='Playlist_DefaultDuo',
-                region=fortnitepy.Region.EUROPE
+                playlist='Playlist_DefaultDuo'
             )
 
-        Sets the playlist to Arena Trios EU (Replace ``Trios`` with ``Solo``
+        Sets the playlist to Arena Trios (Replace ``Trios`` with ``Solo``
         for arena solo): ::
 
             await party.set_playlist(
                 playlist='Playlist_ShowdownAlt_Trios',
                 tournament='epicgames_Arena_S13_Trios',
-                event_window='Arena_S13_Division1_Trios',
-                region=fortnitepy.Region.EUROPE
+                event_window='Arena_S13_Division1_Trios'
             )
 
         Parameters
         ----------
         playlist: Optional[:class:`str`]
             The name of the playlist.
-            Defaults to :attr:`Region.EUROPE`
         tournament: Optional[:class:`str`]
             The tournament id.
         event_window: Optional[:class:`str`]
             The event window id.
-        region: Optional[:class:`Region`]
-            The region to use.
-            *Defaults to :attr:`Region.EUROPE`*
 
         Raises
         ------
         Forbidden
             The client is not the leader of the party.
         """
         if self.me is not None and not self.me.leader:
             raise Forbidden('You have to be leader for this action to work.')
 
-        if region is not None:
-            region = region.value
-
         prop = self.meta.set_playlist(
             playlist=playlist,
             tournament=tournament,
-            event_window=event_window,
+            event_window=event_window
+        )
+        if not self.edit_lock.locked():
+            return await self.patch(updated=prop)
+
+    async def set_region(self, region: Region) -> None:
+        """|coro|
+
+        Sets the region of the party.
+
+        Parameters
+        ----------
+        region: :class:`Region`
+            The region to set.
+
+        Raises
+        ------
+        Forbidden
+            The client is not the leader of the party.
+        """
+
+        if self.me is not None and not self.me.leader:
+            raise Forbidden('You have to be leader for this action to work.')
+
+        prop = self.meta.set_region(
             region=region
         )
         if not self.edit_lock.locked():
             return await self.patch(updated=prop)
 
     async def set_custom_key(self, key: str) -> None:
         """|coro|
```

### Comparing `fortnitepy-3.6.8/fortnitepy/playlist.py` & `fortnitepy-3.6.9/fortnitepy/playlist.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/presence.py` & `fortnitepy-3.6.9/fortnitepy/presence.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/stats.py` & `fortnitepy-3.6.9/fortnitepy/stats.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/store.py` & `fortnitepy-3.6.9/fortnitepy/store.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/typedefs.py` & `fortnitepy-3.6.9/fortnitepy/typedefs.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/user.py` & `fortnitepy-3.6.9/fortnitepy/user.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/utils.py` & `fortnitepy-3.6.9/fortnitepy/utils.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy/xmpp.py` & `fortnitepy-3.6.9/fortnitepy/xmpp.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/fortnitepy.egg-info/PKG-INFO` & `fortnitepy-3.6.9/fortnitepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortnitepy
-Version: 3.6.8
+Version: 3.6.9
 Summary: Library for interacting with fortnite services
 Home-page: https://github.com/Terbau/fortnitepy
 Author: Terbau
 License: MIT
 Project-URL: Documentation, https://fortnitepy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Terbau/fortnitepy/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortnitepy-3.6.8/fortnitepy.egg-info/SOURCES.txt` & `fortnitepy-3.6.9/fortnitepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortnitepy-3.6.8/setup.py` & `fortnitepy-3.6.9/setup.py`

 * *Files identical despite different names*

