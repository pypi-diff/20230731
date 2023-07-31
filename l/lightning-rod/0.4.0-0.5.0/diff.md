# Comparing `tmp/lightning_rod-0.4.0.tar.gz` & `tmp/lightning_rod-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_rod-0.4.0.tar", max compression
+gzip compressed data, was "lightning_rod-0.5.0.tar", max compression
```

## Comparing `lightning_rod-0.4.0.tar` & `lightning_rod-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1061 2023-07-29 19:32:30.812566 lightning_rod-0.4.0/LICENSE
--rw-r--r--   0        0        0     1389 2023-07-29 19:32:30.812566 lightning_rod-0.4.0/README.md
--rw-r--r--   0        0        0      307 2023-07-29 19:33:45.129567 lightning_rod-0.4.0/lightning_rod/__init__.py
--rw-r--r--   0        0        0      667 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/advancement.bolt
--rw-r--r--   0        0        0      603 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/api.bolt
--rw-r--r--   0        0        0     4562 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/bossbar.bolt
--rw-r--r--   0        0        0       38 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/cancel_momentum.bolt
--rw-r--r--   0        0        0      314 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/clear.bolt
--rw-r--r--   0        0        0       85 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/comment.bolt
--rw-r--r--   0        0        0      184 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/config.bolt
--rw-r--r--   0        0        0     2579 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/damage.bolt
--rw-r--r--   0        0        0     1593 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/effect.bolt
--rw-r--r--   0        0        0      569 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/gamemode.bolt
--rw-r--r--   0        0        0      157 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/give.bolt
--rw-r--r--   0        0        0       25 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/kill.bolt
--rw-r--r--   0        0        0     3615 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/math.bolt
--rw-r--r--   0        0        0       35 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/raw_cmd.bolt
--rw-r--r--   0        0        0       86 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/tag.bolt
--rw-r--r--   0        0        0     1029 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/time.bolt
--rw-r--r--   0        0        0      300 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/utils.bolt
--rw-r--r--   0        0        0     2175 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/modules/xp.bolt
--rw-r--r--   0        0        0        0 2023-07-29 19:32:30.816566 lightning_rod-0.4.0/lightning_rod/py.typed
--rw-r--r--   0        0        0     1242 2023-07-29 19:33:45.145568 lightning_rod-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 lightning_rod-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-31 20:47:46.252010 lightning_rod-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1389 2023-07-31 20:47:46.252010 lightning_rod-0.5.0/README.md
+-rw-r--r--   0        0        0      307 2023-07-31 20:48:54.808010 lightning_rod-0.5.0/lightning_rod/__init__.py
+-rw-r--r--   0        0        0      667 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/advancement.bolt
+-rw-r--r--   0        0        0      664 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/api.bolt
+-rw-r--r--   0        0        0     4562 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/bossbar.bolt
+-rw-r--r--   0        0        0       38 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/cancel_momentum.bolt
+-rw-r--r--   0        0        0      314 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/clear.bolt
+-rw-r--r--   0        0        0       85 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/comment.bolt
+-rw-r--r--   0        0        0      184 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/config.bolt
+-rw-r--r--   0        0        0     2579 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/damage.bolt
+-rw-r--r--   0        0        0     1593 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/effect.bolt
+-rw-r--r--   0        0        0      569 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/gamemode.bolt
+-rw-r--r--   0        0        0      157 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/give.bolt
+-rw-r--r--   0        0        0       25 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/kill.bolt
+-rw-r--r--   0        0        0     4604 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/math.bolt
+-rw-r--r--   0        0        0     3596 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/offset_rotation.bolt
+-rw-r--r--   0        0        0       35 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/raw_cmd.bolt
+-rw-r--r--   0        0        0       86 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/tag.bolt
+-rw-r--r--   0        0        0     1029 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/time.bolt
+-rw-r--r--   0        0        0      300 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/utils.bolt
+-rw-r--r--   0        0        0     2175 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/modules/xp.bolt
+-rw-r--r--   0        0        0        0 2023-07-31 20:47:46.256010 lightning_rod-0.5.0/lightning_rod/py.typed
+-rw-r--r--   0        0        0     1242 2023-07-31 20:48:54.840012 lightning_rod-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 lightning_rod-0.5.0/PKG-INFO
```

### Comparing `lightning_rod-0.4.0/LICENSE` & `lightning_rod-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/README.md` & `lightning_rod-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/advancement.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/advancement.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/api.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/api.bolt`

 * *Files 19% similar despite different names*

```diff
@@ -4,12 +4,13 @@
 from ./tag import tag, untag
 from ./kill import kill
 from ./cancel_momentum import cancel_momentum
 from ./effect import effect, raw_effect
 from ./give import give
 from ./clear import clear
 from ./gamemode import get_gamemode, set_gamemode
-from ./math import random, sqrt, pow, sin, cos
+from ./math import random, sqrt, power, sin, cos
 from ./time import get_gametime, get_time, get_day, set_time
 from ./xp import get_xp, get_level, set_xp, set_level, set_xp_percent
 from ./comment import add_comment
 from ./damage import damage
+from ./offset_rotation import offset_rotation_facing_caret
```

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/bossbar.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/bossbar.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/damage.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/damage.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/effect.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/effect.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/gamemode.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/gamemode.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/time.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/time.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/lightning_rod/modules/xp.bolt` & `lightning_rod-0.5.0/lightning_rod/modules/xp.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.4.0/pyproject.toml` & `lightning_rod-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning_rod"
-version = "0.4.0"
+version = "0.5.0"
 description = "Function library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/lightning-rod"
 readme = "README.md"
```

### Comparing `lightning_rod-0.4.0/PKG-INFO` & `lightning_rod-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-rod
-Version: 0.4.0
+Version: 0.5.0
 Summary: Function library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/lightning-rod
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

