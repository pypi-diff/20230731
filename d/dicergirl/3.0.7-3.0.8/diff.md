# Comparing `tmp/dicergirl-3.0.7.tar.gz` & `tmp/dicergirl-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicergirl-3.0.7.tar", last modified: Mon Jul 31 07:36:24 2023, max compression
+gzip compressed data, was "dicergirl-3.0.8.tar", last modified: Mon Jul 31 09:40:52 2023, max compression
```

## Comparing `dicergirl-3.0.7.tar` & `dicergirl-3.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.269765 dicergirl-3.0.7/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.7/LICENSE
--rw-rw-rw-   0        0        0     9363 2023-07-31 07:36:24.269765 dicergirl-3.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.232723 dicergirl-3.0.7/dicergirl/
--rw-rw-rw-   0        0        0    18920 2023-07-31 05:49:32.000000 dicergirl-3.0.7/dicergirl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl/coc/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:17:05.000000 dicergirl-3.0.7/dicergirl/coc/__init__.py
--rw-rw-rw-   0        0        0     4362 2023-07-31 05:29:50.000000 dicergirl-3.0.7/dicergirl/coc/coccards.py
--rw-rw-rw-   0        0        0     9147 2023-07-30 05:42:11.000000 dicergirl-3.0.7/dicergirl/coc/cocutils.py
--rw-rw-rw-   0        0        0     6020 2023-07-30 16:30:57.000000 dicergirl-3.0.7/dicergirl/coc/investigator.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl/dnd/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:30:32.000000 dicergirl-3.0.7/dicergirl/dnd/__init__.py
--rw-rw-rw-   0        0        0     2988 2023-07-30 16:18:46.000000 dicergirl-3.0.7/dicergirl/dnd/adventurer.py
--rw-rw-rw-   0        0        0     2831 2023-07-30 14:43:40.000000 dicergirl-3.0.7/dicergirl/dnd/dndcards.py
--rw-rw-rw-   0        0        0     4580 2023-07-30 14:39:09.000000 dicergirl-3.0.7/dicergirl/dnd/dndutils.py
--rw-rw-rw-   0        0        0    17306 2023-07-31 07:23:30.000000 dicergirl-3.0.7/dicergirl/main.py
--rw-rw-rw-   0        0        0     3439 2023-07-30 16:39:51.000000 dicergirl-3.0.7/dicergirl/run.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl/scp/
--rw-rw-rw-   0        0        0       19 2023-07-31 06:30:31.000000 dicergirl-3.0.7/dicergirl/scp/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-07-30 16:20:07.000000 dicergirl-3.0.7/dicergirl/scp/agent.py
--rw-rw-rw-   0        0        0     2824 2023-07-31 06:08:08.000000 dicergirl-3.0.7/dicergirl/scp/scpcards.py
--rw-rw-rw-   0        0        0     5191 2023-07-30 05:42:11.000000 dicergirl-3.0.7/dicergirl/scp/scputils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.269238 dicergirl-3.0.7/dicergirl/utils/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.7/dicergirl/utils/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.7/dicergirl/utils/chat.py
--rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.7/dicergirl/utils/decorators.py
--rw-rw-rw-   0        0        0     7129 2023-07-30 06:42:58.000000 dicergirl-3.0.7/dicergirl/utils/dicer.py
--rw-rw-rw-   0        0        0    22450 2023-07-31 07:16:02.000000 dicergirl-3.0.7/dicergirl/utils/handlers.py
--rw-rw-rw-   0        0        0    23207 2023-07-31 07:18:19.000000 dicergirl-3.0.7/dicergirl/utils/messages.py
--rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.7/dicergirl/utils/settings.py
--rw-rw-rw-   0        0        0     5839 2023-07-31 06:36:24.000000 dicergirl-3.0.7/dicergirl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl.egg-info/
--rw-rw-rw-   0        0        0     9363 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 07:36:24.269765 dicergirl-3.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-07-31 07:36:19.000000 dicergirl-3.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.069190 dicergirl-3.0.8/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.8/LICENSE
+-rw-rw-rw-   0        0        0     9363 2023-07-31 09:40:52.069190 dicergirl-3.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.015192 dicergirl-3.0.8/dicergirl/
+-rw-rw-rw-   0        0        0    18920 2023-07-31 05:49:32.000000 dicergirl-3.0.8/dicergirl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.053189 dicergirl-3.0.8/dicergirl/coc/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:17:05.000000 dicergirl-3.0.8/dicergirl/coc/__init__.py
+-rw-rw-rw-   0        0        0     4362 2023-07-31 05:29:50.000000 dicergirl-3.0.8/dicergirl/coc/coccards.py
+-rw-rw-rw-   0        0        0     9165 2023-07-31 08:22:11.000000 dicergirl-3.0.8/dicergirl/coc/cocutils.py
+-rw-rw-rw-   0        0        0     6020 2023-07-30 16:30:57.000000 dicergirl-3.0.8/dicergirl/coc/investigator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.057191 dicergirl-3.0.8/dicergirl/dnd/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:30:32.000000 dicergirl-3.0.8/dicergirl/dnd/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-07-31 09:32:44.000000 dicergirl-3.0.8/dicergirl/dnd/adventurer.py
+-rw-rw-rw-   0        0        0     2831 2023-07-30 14:43:40.000000 dicergirl-3.0.8/dicergirl/dnd/dndcards.py
+-rw-rw-rw-   0        0        0     4024 2023-07-31 09:35:10.000000 dicergirl-3.0.8/dicergirl/dnd/dndutils.py
+-rw-rw-rw-   0        0        0    17465 2023-07-31 09:30:37.000000 dicergirl-3.0.8/dicergirl/main.py
+-rw-rw-rw-   0        0        0     3439 2023-07-30 16:39:51.000000 dicergirl-3.0.8/dicergirl/run.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.060190 dicergirl-3.0.8/dicergirl/scp/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:30:31.000000 dicergirl-3.0.8/dicergirl/scp/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-07-30 16:20:07.000000 dicergirl-3.0.8/dicergirl/scp/agent.py
+-rw-rw-rw-   0        0        0     2824 2023-07-31 06:08:08.000000 dicergirl-3.0.8/dicergirl/scp/scpcards.py
+-rw-rw-rw-   0        0        0     5188 2023-07-31 09:33:55.000000 dicergirl-3.0.8/dicergirl/scp/scputils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.068189 dicergirl-3.0.8/dicergirl/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.8/dicergirl/utils/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.8/dicergirl/utils/chat.py
+-rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.8/dicergirl/utils/decorators.py
+-rw-rw-rw-   0        0        0     8656 2023-07-31 09:37:09.000000 dicergirl-3.0.8/dicergirl/utils/dicer.py
+-rw-rw-rw-   0        0        0    22438 2023-07-31 08:50:24.000000 dicergirl-3.0.8/dicergirl/utils/handlers.py
+-rw-rw-rw-   0        0        0    23207 2023-07-31 07:18:19.000000 dicergirl-3.0.8/dicergirl/utils/messages.py
+-rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.8/dicergirl/utils/settings.py
+-rw-rw-rw-   0        0        0     5839 2023-07-31 09:40:17.000000 dicergirl-3.0.8/dicergirl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:40:52.049232 dicergirl-3.0.8/dicergirl.egg-info/
+-rw-rw-rw-   0        0        0     9363 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 09:40:51.000000 dicergirl-3.0.8/dicergirl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:40:52.070191 dicergirl-3.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-07-31 07:36:19.000000 dicergirl-3.0.8/setup.py
```

### Comparing `dicergirl-3.0.7/LICENSE` & `dicergirl-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/PKG-INFO` & `dicergirl-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.7
+Version: 3.0.8
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.7/README.md` & `dicergirl-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/__init__.py` & `dicergirl-3.0.8/dicergirl/__init__.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/coc/coccards.py` & `dicergirl-3.0.8/dicergirl/coc/coccards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/coc/cocutils.py` & `dicergirl-3.0.8/dicergirl/coc/cocutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     if len(args) == 0:
         return help_message("ra")
     if len(args) > 2:
         return "[Oracle] 错误: 参数过多(2需要 %d给予)." % len(args)
 
     card_data = cards.get(event)
     if not card_data:
-        return "[Oracle] 在执行参数检定前, 请先完成车卡并保存."
+        return "[Oracle] 在执行参数检定前, 请先执行`.coc`车卡并执行`.set`保存."
     inv = Investigator().load(card_data)
     is_base = False
     for _, alias in attrs_dict.items():
         if args[0] in alias:
             v = int(eval("inv.{prop}".format(prop=alias[0])))
             is_base = True
             break
```

### Comparing `dicergirl-3.0.7/dicergirl/coc/investigator.py` & `dicergirl-3.0.8/dicergirl/coc/investigator.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/dnd/adventurer.py` & `dicergirl-3.0.8/dicergirl/scp/agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,80 @@
+import random
 try:
     from ..utils.dicer import Dice
 except ImportError:
     from dicergirl.utils.dicer import Dice
 
-class Adventurer(object):
+class Agent(object):
     def __init__(self) -> None:
-        self.name = "无名冒险者"
+        self.name = "无名特工"
         self.age = 20
         self.sex = "女"
         self.str = 0
+        self.hth = 0
+        self.per = 0
         self.dex = 0
-        self.con = 0
-        self.int = 0
-        self.fel = 0
+        self.fte = 0
         self.chr = 0
+        self.int = 0
+        self.wil = 0
         self.hp_max = 0
         self.hp = 0
+        self.enp = 0
         self.dices = {}
         self.skills = {}
         self.tools = {}
 
     def init(self):
         prop = {
-            "str": 0,
-            "dex": 0,
-            "con": 0,
-            "int": 0,
-            "fel": 0,
-            "chr": 0,
+            "str": 1,
+            "hth": 1,
+            "per": 1,
+            "dex": 1,
+            "fte": 1,
+            "chr": 1,
+            "int": 1,
+            "wil": 1
         }
-        attr = {key : value for key, value in prop.items()}
+        attr = {
+            "str": 1,
+            "hth": 1,
+            "per": 1,
+            "dex": 1,
+            "fte": 1,
+            "chr": 1,
+            "int": 1,
+            "wil": 1
+        }
+        total = 20 - len(prop)
+        for _ in range(total):
+            name = random.choice(list(prop.keys()))
+            prop[name] += 1
 
         for p in prop.keys():
-            outcome = []
-            for _ in range(6):
-                outcome.append(Dice("1d6").roll().calc())
-            d1 = max(outcome)
-            outcome.remove(d1)
-            d2 = max(outcome)
-            outcome.remove(d2)
-            d3 = max(outcome)
-            outcome.remove(d3)
-            if p != "con":
-                result, _ = self.__correct(d1 + d2 + d3)
-            else:
-                result, self.correct = self.__correct(d1 + d2 + d3)
-            prop[p] = result
+            num = prop[p]
+            dice = Dice(f"{num}d8", explode=True)
+            dice.roll()
+            prop[p] = dice.total
+            attr[p] = dice.dices
 
+        self.dices = attr
         self.__dict__.update(prop)
         self.reset_hp()
-
-    def __correct(self, result):
-        correct = (result - 10) // 2
-        return result + correct, correct
+        self.reset_enp()
 
     def reset_hp(self):
-        base = Dice("1d10").roll().calc() + self.correct
+        base = 10
+        for d in self.dices["hth"]:
+            if d == "D8":
+                base += 3
+            elif d == "D10":
+                base += 6
+            elif d == "D12":
+                base += 16
         self.hp_max = base
         self.hp = base
     
     def reset_enp(self):
         base = 1
         for d in self.dices["wil"]:
             if d == "D10":
@@ -74,17 +89,19 @@
         elif age >= 90:
             return "该特工已经被清理, 他(或者她)年龄过大, 显然是一个需要被清理的异常."
         self.age = age
 
     def __repr__(self) -> str:
         data = "姓名: %s\n" % self.name
         data += "性别: %s 年龄: %d\n" % (self.sex, self.age)
-        data += "力量: %d 智力: %d\n" % (self.str, self.int)
-        data += "敏捷: %d 感知: %d\n" % (self.dex, self.fel)
-        data += "体质: %d 魅力: %d\n" % (self.con, self.chr)
+        data += "强度: %d 命运: %d\n" % (self.str, self.fte)
+        data += "感知: %d 魅力: %d\n" % (self.per, self.chr) 
+        data += "灵巧: %d 情报: %d\n" % (self.dex, self.int)
+        data += "健康: %d 意志: %d\n" % (self.hth, self.wil)
+        data += "激励点: %d\n" % (self.enp)
         data += "生命: %d/%d" % (self.hp, self.hp_max)
         return data
 
     def skills_output(self) -> str:
         if not self.skills:
             return "%s 当前无任何技能数据。" % self.name
         r = "%s技能数据: " % self.name
@@ -93,8 +110,8 @@
         return r
 
     def output(self) -> str:
         return self.__repr__()
 
     def load(self, data: dict):
         self.__dict__.update(data)
-        return self
+        return self
```

### Comparing `dicergirl-3.0.7/dicergirl/dnd/dndcards.py` & `dicergirl-3.0.8/dicergirl/dnd/dndcards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/dnd/dndutils.py` & `dicergirl-3.0.8/dicergirl/dnd/dndutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from ..utils.messages import help_messages, help_message
-    from ..utils.dicer import Dice, scp_doc
+    from ..utils.dicer import Dice, dnd_doc
     from .dndcards import dnd_cards, dnd_attrs_dict as attrs_dict
     from .adventurer import Adventurer
 except ImportError:
     from dicergirl.utils.messages import help_messages, help_message
-    from dicergirl.utils.dicer import Dice, scp_doc
+    from dicergirl.utils.dicer import Dice, dnd_doc
     from dicergirl.dnd.dndcards import dnd_cards, dnd_attrs_dict as attrs_dict
     from dicergirl.dnd.adventurer import Adventurer
 
 import random
 
 def st():
     result = random.randint(1, 20)
@@ -32,15 +32,15 @@
 def at(args):
     if args:
         d = Dice().parse(args).roll()
     else:
         d = Dice().parse("1d6").roll()
     return f"[Oracle] 投掷 {d.db}={d.total}\n造成了 {d.total}点 伤害."
 
-def scp_dam(args, message):
+def dnd_dam(args, message):
     card = dnd_cards.get(message)
     if not card:
         return "[Oracle] 未找到缓存数据, 请先使用`.dnd`指令进行车卡生成角色卡并`.set`进行保存."
     max_hp = card["hp_max"]
     if len(args) == 1:
         if not args[0] in ["check", "c"]:
             arg = int(args[0])
@@ -78,55 +78,35 @@
     return r
 
 def dra(args, event):
     if len(args) == 0:
         return help_message("sra")
     if len(args) > 2:
         return "[Oracle] 错误: 参数过多(最多2需要但%d给予)." % len(args)
-    
+
     if len(args) == 2:
-        difficulty = int(args[1])
+        dc = int(args[1])
     else:
-        difficulty = 12
+        dc = 12
 
     card_data = dnd_cards.get(event)
     if not card_data:
-        return "[Oracle] 在执行参数检定前, 请先完成`.dnd`车卡并执行`.set`保存."
+        return "[Oracle] 在执行参数检定前, 请先执行`.dnd`车卡并执行`.set`保存."
     inv = Adventurer().load(card_data)
     is_base = False
-    for attr, alias in attrs_dict.items():
+    for _, alias in attrs_dict.items():
         if args[0] in alias:
-            dices: list = eval("inv.dices['{prop}']".format(prop=alias[0]))
+            v = int(eval("inv.{prop}".format(prop=alias[0]))[1])
             is_base = True
             break
     is_skill = False
     if not is_base:
         for skill in inv.skills:
             if args[0] == skill:
-                v = inv.skills[skill]
+                v = int(inv.skills[skill][1])
+                is_skill = True
                 break
     if not is_base and not is_skill:
         return "[Oracle] 错误: 没有这个数据或技能."
-    
-    all_dices = []
-    if len(dices) > 4:
-        while True:
-            if len(all_dices) == 4:
-                break
-            choice = random.choice(dices)
-            all_dices.append(choice)
-            dices.remove(choice)
-    elif len(dices) <= 4:
-        all_dices = dices
-    
-    results = []
-    great = False
-    for dice in all_dices:
-        dice = Dice("1"+dice.lower()).roll()
-        results.append(dice.total)
-        if dice.great == True:
-            great = True
-    result = max(results)
-    results.remove(result)
-    result += max(results)
-    r = scp_doc(result, difficulty, agent=inv.name, great=great)
-    return r
+
+    outcome = Dice("1d20").roll().calc() + v
+    return dnd_doc(outcome, dc, adventurer=card_data["name"])
```

### Comparing `dicergirl-3.0.7/dicergirl/main.py` & `dicergirl-3.0.8/dicergirl/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from dicergirl.scp.agent import Agent
 from dicergirl.scp.scpcards import scp_cards, scp_cache_cards
 from dicergirl.scp.scputils import sra, scp_dam, at as sat
 
 from dicergirl.dnd.adventurer import Adventurer
 from dicergirl.dnd.dndcards import dnd_cards, dnd_cache_cards
+from dicergirl.dnd.dndutils import dra
 
 from dicergirl.utils.decorators import Commands
 from dicergirl.utils.messages import help_message, version
 from dicergirl.utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers, get_config, modes
 from dicergirl.utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, coc_set_handler, coc_show_handler, coc_del_handler, dnd_set_handler, dnd_show_handler, dnd_del_handler
 from dicergirl.utils.chat import chat
 
@@ -197,20 +198,20 @@
         await message.reply(content=f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
         args = 20
 
     adv = Adventurer()
     adv.age_check(args)
     adv.init()
     
-    if adv.int <= 8:
+    if adv.int[0] <= 8:
         await message.reply(content="[Orcale] 很遗憾, 检定新的冒险者智力不足, 弱智是不允许成为冒险者的, 请重新进行车卡检定.")
         return True
 
     if 15 <= args and args < 90:
-        scp_cache_cards.update(message, adv.__dict__, save=False)
+        dnd_cache_cards.update(message, adv.__dict__, save=False)
         await message.reply(content=str(adv.output()))
     return True
 
 @Commands(name=(".show"))
 async def showhandler(api: BotAPI, message: Message, params=None):
     args = format_msg(message, begin=(".show", ".display"))
     if not args:
@@ -331,14 +332,16 @@
 async def rahandler(api: BotAPI, message: Message, params=None):
     args = format_msg(message, begin=".ra")
     if mode in ["coc", "scp", "dnd"]:
         if mode == "scp":
             await message.reply(content=sra(args, message))
         elif mode == "coc":
             await message.reply(content=ra(args, message))
+        elif mode == "dnd":
+            await message.reply(content=dra(args, message))
     return True
 
 @Commands(name=(".rh"))
 async def rhhandler(api: BotAPI, message: Message, params=None):
     args = format_str(message, begin=".rh")
     await message.reply(content="[Oracle] 暗骰: 命运的齿轮在转动.")
     await api.post_dms(guild_id=message.guild_id, msg_id=message.id, content=rd0(args))
@@ -437,14 +440,15 @@
                 sys.stdout,
                 level = "DEBUG"
             )
             logger.info("DEBUG 模式已启动.")
         init()
         cards.load()
         scp_cards.load()
+        dnd_cards.load()
         logger.success("机器人启动成功, 将进行心跳维持链接.")
 
     async def on_at_message_create(self, message: Message):
         is_command = False
         for handler in self.handlers:
             if await handler(api=self.api, message=message, params=None):
                 isbot = "玩家" if message.author.bot == False else "机器人"
```

### Comparing `dicergirl-3.0.7/dicergirl/run.py` & `dicergirl-3.0.8/dicergirl/run.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/scp/agent.py` & `dicergirl-3.0.8/dicergirl/scp/scpcards.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,79 @@
-import random
+from typing import Dict, List
 try:
-    from ..utils.dicer import Dice
+    from ..utils.utils import logger as _log, _scp_cachepath
+    from ..utils.utils import get_group_id, get_user_id
 except ImportError:
-    from dicergirl.utils.dicer import Dice
+    from dicergirl.utils.utils import logger as _log, _scp_cachepath
+    from dicergirl.utils.utils import get_group_id, get_user_id
 
-class Agent(object):
-    def __init__(self) -> None:
-        self.name = "无名特工"
-        self.age = 20
-        self.sex = "女"
-        self.str = 0
-        self.hth = 0
-        self.per = 0
-        self.dex = 0
-        self.fte = 0
-        self.chr = 0
-        self.int = 0
-        self.wil = 0
-        self.hp_max = 0
-        self.hp = 0
-        self.enp = 0
-        self.dices = {}
-        self.skills = {}
-        self.tools = {}
-
-    def init(self):
-        prop = {
-            "str": 1,
-            "hth": 1,
-            "per": 1,
-            "dex": 1,
-            "fte": 1,
-            "chr": 1,
-            "int": 1,
-            "wil": 1
-        }
-        attr = {
-            "str": 1,
-            "hth": 1,
-            "per": 1,
-            "dex": 1,
-            "fte": 1,
-            "chr": 1,
-            "int": 1,
-            "wil": 1
-        }
-        total = 20 - len(prop)
-        for _ in range(total):
-            name = random.choice(list(prop.keys()))
-            prop[name] += 1
-
-        for p in prop.keys():
-            num = prop[p]
-            dice = Dice(f"{num}d8", explode=True)
-            dice.roll()
-            prop[p] = dice.total
-            attr[p] = dice.dices
-
-        self.dices = attr
-        self.__dict__.update(prop)
-        self.reset_hp()
-        self.reset_enp()
-
-    def reset_hp(self):
-        base = 10
-        for d in self.dices["hth"]:
-            if d == "D8":
-                base += 3
-            elif d == "D10":
-                base += 6
-            elif d == "D12":
-                base += 16
-        self.hp_max = base
-        self.hp = base
-    
-    def reset_enp(self):
-        base = 1
-        for d in self.dices["wil"]:
-            if d == "D10":
-                base += 1
-        self.enp = base
-
-    def age_check(self, age=20):
-        if self.age != 20:
-            return
-        if age < 15:
-            return "[scpdicer] 年龄过小, 无法担任基金会特工."
-        elif age >= 90:
-            return "该特工已经被清理, 他(或者她)年龄过大, 显然是一个需要被清理的异常."
-        self.age = age
-
-    def __repr__(self) -> str:
-        data = "姓名: %s\n" % self.name
-        data += "性别: %s 年龄: %d\n" % (self.sex, self.age)
-        data += "强度: %d 命运: %d\n" % (self.str, self.fte)
-        data += "感知: %d 魅力: %d\n" % (self.per, self.chr) 
-        data += "灵巧: %d 情报: %d\n" % (self.dex, self.int)
-        data += "健康: %d 意志: %d\n" % (self.hth, self.wil)
-        data += "激励点: %d\n" % (self.enp)
-        data += "生命: %d/%d" % (self.hp, self.hp_max)
-        return data
-
-    def skills_output(self) -> str:
-        if not self.skills:
-            return "%s 当前无任何技能数据。" % self.name
-        r = "%s技能数据: " % self.name
-        for k, v in self.skills.items():
-            r += "\n%s: %d" % (k, v)
-        return r
-
-    def output(self) -> str:
-        return self.__repr__()
-
-    def load(self, data: dict):
-        self.__dict__.update(data)
-        return self
+import json
+
+class Cards():
+    def __init__(self):
+        self.data = {}
+
+    def save(self):
+        _log.info("保存 SCP 人物卡数据.")
+        with open(_scp_cachepath, "w", encoding="utf-8") as f:
+            json.dump(self.data, f, ensure_ascii=False)
+
+    def load(self):
+        with open(_scp_cachepath, "r", encoding="utf-8") as f:
+            data = f.read()
+            if not data:
+                self.data = {}
+            else:
+                self.data = json.loads(data)
+
+    def update(self, message, inv_dict, qid="", save=True):
+        group_id = get_group_id(message)
+        if not self.data.get(group_id):
+            self.data[group_id] = {}
+        self.data[group_id].update(
+            {qid if qid else get_user_id(message): inv_dict}
+            )
+        if save:
+            self.save()
+
+    def get(self, message, qid=""):
+        group_id = get_group_id(message)
+        if self.data.get(group_id):
+            if self.data[group_id].get(qid if qid else get_user_id(message)):
+                return self.data[group_id].get(qid if qid else get_user_id(message))
+        else:
+            return None
+
+    def delete(self, message, qid: str = "", save: bool = True) -> bool:
+        if self.get(message, qid=qid):
+            if self.data[get_group_id(message)].get(qid if qid else get_user_id(message)):
+                self.data[get_group_id(message)].pop(
+                    qid if qid else get_user_id(message))
+            if save:
+                self.save()
+            return True
+        return False
+
+    def delete_skill(self, message, skill_name: str, qid: str = "", save: bool = True) -> bool:
+        if self.get(message, qid=qid):
+            data = self.get(message, qid=qid)
+            if data["skills"].get(skill_name):
+                data["skills"].pop(skill_name)
+                self.update(message, data, qid=qid, save=save)
+                return True
+        return False
+
+scp_cards = Cards()
+scp_cache_cards = Cards()
+scp_attrs_dict: Dict[str, List[str]] = {
+    "名字": ["name", "名字", "名称", "姓名"],
+    "性别": ["sex", "性别"],
+    "年龄": ["age", "年龄"],
+    "强度": ["str", "力量", "攻击", "强度"],
+    "灵巧": ["dex", "灵巧"],
+    "健康": ["hth", "健康"],
+    "命运": ["fte", "命运"],
+    "魅力": ["chr", "魅力"],
+    "情报": ["int", "情报"],
+    "意志": ["wil", "意志", "精神"],
+    "生命": ["hp", "生命"]
+}
```

### Comparing `dicergirl-3.0.7/dicergirl/scp/scputils.py` & `dicergirl-3.0.8/dicergirl/scp/scputils.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,18 +86,18 @@
     if len(args) == 2:
         difficulty = int(args[1])
     else:
         difficulty = 12
 
     card_data = scp_cards.get(event)
     if not card_data:
-        return "[Oracle] 在执行参数检定前, 请先完成`.scp`车卡并执行`.set`保存."
+        return "[Oracle] 在执行参数检定前, 请先执行`.scp`车卡并执行`.set`保存."
     inv = Agent().load(card_data)
     is_base = False
-    for attr, alias in attrs_dict.items():
+    for _, alias in attrs_dict.items():
         if args[0] in alias:
             dices: list = eval("inv.dices['{prop}']".format(prop=alias[0]))
             is_base = True
             break
     is_skill = False
     if not is_base:
         for skill in inv.skills:
```

### Comparing `dicergirl-3.0.7/dicergirl/utils/chat.py` & `dicergirl-3.0.8/dicergirl/utils/chat.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/utils/decorators.py` & `dicergirl-3.0.8/dicergirl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/utils/dicer.py` & `dicergirl-3.0.8/dicergirl/utils/dicer.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,17 +67,19 @@
         if self.add:
             add = sum(self.add)
         else:
             add = 0
 
         for _ in range(self.a):
             result = random.randint(1, self.b)
+
             if result == 1:
                 if self.explode:
                     result -= 1
+
             if self.explode and self.b == 8:
                 self.dices.append("D10")
                 result2 = random.randint(1, 10)
                 if result2 == 1:
                     result -= 1
                 result += result2
                 if result2 == 10:
@@ -90,14 +92,15 @@
                         self.dices.append("D20")
                         result4 = random.randint(1, 20)
                         if result4 == 1:
                             result -= 1
                         result += result4
                         if result4 == 20:
                             self.great = True
+
             self.results += [result]
 
         if self.method == "+":
             self.total = sum(self.results) + add
         else:
             self.total = sum(self.results) - add
         
@@ -131,30 +134,35 @@
         if result == 100:
             s += "大失败！"
         elif anum < 50 and result > 95:
             s += f"{result}>95 大失败！"
         elif result == 1:
             s += "大成功！"
         elif result <= anum // 5:
-            s += f"检定值{anum} {result}≤{anum//5} 极难成功"
+            s += f"检定值: {anum} {result}≤{anum//5}\n"
+            s += "检定结果: 极难成功."
         elif result <= anum // 2:
-            s += f"检定值{anum} {result}≤{anum//2} 困难成功"
+            s += f"检定值: {anum} {result}≤{anum//2}\n"
+            s += "检定结果: 困难成功."
         elif result <= anum:
-            s += f"检定值{anum} {result}≤{anum} 成功"
+            s += f"检定值: {anum} {result}≤{anum}\n"
+            s += "检定结果: 成功."
         else:
-            s += f"检定值{anum} {result}>{anum} 失败"
+            s += f"检定值: {anum} {result}>{anum}\n"
+            s += "检定结果: 失败."
     return s
 
 def scp_doc(result, difficulty, agent=None, great=False):
     if not agent:
         agent = "该特工"
     r = f"事件难度: {difficulty}\n"
     if difficulty > 25:
         r += f"检定数据: {random.randint(1, 25)}"
-        r += f"检定结果: 致命失败.\n检定结论: {agent} 在试图挑战数学、挑战科学、挑战真理, 尝试达成一个不可能事件, {agent} 毫无疑问获得了 致命失败."
+        r += f"检定结果: 致命失败.\n"
+        r += f"检定结论: {agent} 在试图挑战数学、挑战科学、挑战真理, 尝试达成一个不可能事件, {agent} 毫无疑问获得了 致命失败."
         return r
     r += f"检定数据: {result}\n"
     if great:
         r += "检定结果: 关键成功.\n"
         if result <= difficulty:
             r += "检定结论: 有时候, 一次普通的成功或许会大幅度的牵扯到整个未来, 但这并不是一件太过于值得高兴的事情, 因为它不见得是一个好的开始."
         else:
@@ -174,14 +182,41 @@
             r += "检定结果: 成功.\n"
             r += "检定结论: 小心, 你的成功完全是一次偶然, 不要试图去将这样的偶然当做希望."
         else:
             r += "检定结果: 失败.\n"
             r += "检定结论: 成功与失败宛如山顶与深渊, 无论是哪一种都是可能的, 相反, 在这个世界落入深渊是一件更加合理的事情."
     return r
 
+def dnd_doc(result, dc, adventurer=None):
+    if not adventurer:
+        adventurer = "该冒险者"
+    r = f"事件难度: {dc}\n"
+    r += f"检定数据: {result}\n"
+    if result >= 20:
+        r += "检定结果: 大成功.\n"
+        r += "检定结论: 被命运眷顾的幸运者, 这毫无疑问是一次完美的成功."
+    elif result > dc:
+        r += "检定结果: 成功.\n"
+        r += "检定结论: 前进吧, 冒险者, 异世的诗篇还在等着你."
+    elif result <= dc / 2:
+        r += "检定结果: 大失败.\n"
+        r += "检定结论: 冒险不是自寻死路, 有时候, 放弃也是一个好的选择."
+    elif result < dc:
+        r += "检定结果: 失败.\n"
+        r += "检定结论: 成功与失败总是相辅相成, 不要让一次失败打倒你."
+    else:
+        result = random.randint(0, 1)
+        if result:
+            r += "检定结果: 成功.\n"
+            r += "检定结论: 小心, 你的成功完全是一次偶然, 不要认为这样的偶然稀松平常, 冷静与冲动并存, 才是一个合格的冒险者."
+        else:
+            r += "检定结果: 失败.\n"
+            r += "检定结论: 成功与失败由于一体两面, 无论是哪一种都是可能的, 但是你不必气馁, 失败与成功都是冒险的一部分."
+    return r
+
 if __name__ == "__main__":
     try:
         roll_string = "2d1-2"
         dice = Dice().parse(roll_string).roll()
         print(f"{dice.db}={dice.detail_expr()}={dice.calc()}")
     except ValueError as e:
         print(e)
```

### Comparing `dicergirl-3.0.7/dicergirl/utils/handlers.py` & `dicergirl-3.0.8/dicergirl/utils/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,44 +315,44 @@
     return r
 
 def dnd_set_handler(message, args):
     if not args:
         if dnd_cache_cards.get(message):
             card_data = dnd_cache_cards.get(message)
             dnd_cards.update(message, inv_dict=card_data)
-            inv = Agent().load(card_data)
+            inv = Adventurer().load(card_data)
             return "[Oracle] 成功从缓存保存人物卡属性: \n" + inv.output()
         else:
             return "[Oracle] 未找到缓存数据, 请先使用`.dnd`指令进行车卡生成角色卡."
     else:
         if dnd_cards.get(message):
             card_data = dnd_cards.get(message)
-            inv = Agent().load(card_data)
+            inv = Adventurer().load(card_data)
         else:
             return "[Oracle] 未找到已保存数据, 请先使用空白`.set`指令保存角色数据."
         if len(args) % 2 != 0:
             return "[Oracle] 参数错误, 这是由于传输的数据数量错误, 我只接受为偶数的参数数量, 因为我无法连接到OpenAI, 这使得我无法使用 GPT-4 作为神经网络引擎, 我使用 TensorFlow 作为替代.\n此外, 这看起来不像是来源于我的错误."
         elif len(args) == 2:
-            for attr, alias in scp_attrs_dict.items():
+            for attr, alias in dnd_attrs_dict.items():
                 if args[0] in alias:
                     if attr in ["名字", "性别"]:
                         if attr == "性别" and not args[1] in ["男", "女"]:
-                            return "[Oracle] 欧若可拒绝将基金会特工性别将设置为 {sex}, 这是对物种的侮辱.".format(sex=args[1])
+                            return "[Oracle] 欧若可拒绝将冒险者性别将设置为 {sex}, 这是对物种的侮辱.".format(sex=args[1])
                         inv.__dict__[alias[0]] = args[1]
                     else:
                         try:
                             inv.__dict__[alias[0]] = int(args[1])
                         except ValueError:
                             return "[Oracle] 请输入正整数属性数据"
                     dnd_cards.update(message, inv.__dict__)
-                    return "[Oracle] 设置基金会特工 %s 为: %s" % (attr, args[1])
+                    return "[Oracle] 设置冒险者 %s 为: %s" % (attr, args[1])
             try:
                 inv.skills[args[0]] = int(args[1])
                 dnd_cards.update(message, inv.__dict__)
-                return "[Oracle] 设置基金会特工 %s 技能为: %s." % (args[0], args[1])
+                return "[Oracle] 设置冒险者 %s 技能为: %s." % (args[0], args[1])
             except ValueError:
                 return "[Oracle] 请输入正整数技能数据."
         elif len(args) > 2:
             reply = []
             li = []
             sub_li = []
             for arg in args:
@@ -363,67 +363,67 @@
                     sub_li.append(arg)
                     li.append(sub_li)
                     sub_li = []
                 else:
                     return "[Oracle] 参数错误, 可能是 Python 解释器的错误, 请检查该服务的 Python 版本, 我无法解析到我当前承载的服务器状态, 因为开发者并未给我提供 API 接口.\n此外, 这看起来不像是来源于我的错误."
             for sub_li in li:
                 has_set = False
-                for attr, alias in scp_attrs_dict.items():
+                for attr, alias in dnd_attrs_dict.items():
                     if sub_li[0] in alias:
                         if attr in ["名字", "性别"]:
                             if attr == "性别" and not sub_li[1] in ["男", "女"]:
-                                return "[Oracle] 欧若可拒绝将基金会特工性别将设置为 {sex}, 这是对物种的侮辱.".format(sex=sub_li[1])
+                                return "[Oracle] 欧若可拒绝将冒险者将设置为 {sex}, 这是对物种的侮辱.".format(sex=sub_li[1])
                             inv.__dict__[alias[0]] = sub_li[1]
                         else:
                             try:
                                 inv.__dict__[alias[0]] = int(sub_li[1])
                             except ValueError:
                                 reply.append("基础数据 %s 要求正整数数据, 但你传入了 %s." % (sub_li[0], sub_li[1]))
                                 continue
                         dnd_cards.update(message, inv.__dict__)
-                        reply.append("设置基金会特工基础数据 %s 为: %s" % (attr, sub_li[1]))
+                        reply.append("设置冒险者基础数据 %s 为: %s" % (attr, sub_li[1]))
                         has_set = True
                 if has_set:
                     continue
                 try:
                     inv.skills[sub_li[0]] = int(sub_li[1])
                     dnd_cards.update(message, inv.__dict__)
-                    reply.append("设置基金会特工 %s 技能为: %s." % (sub_li[0], sub_li[1]))
+                    reply.append("设置冒险者 %s 技能为: %s." % (sub_li[0], sub_li[1]))
                 except ValueError:
                     reply.append("技能 %s 要求正整数数据, 但你传入了 %s." % (sub_li[0], sub_li[1]))
             rep = "[Oracle]\n"
             for r in reply:
                 rep += r + "\n"
             return rep.rstrip("\n")
         else:
             return "[Oracle] 参数错误, 可能是由于传输的数据数量错误, 此外, 这看起来不像是来源于我的错误."
 
 def dnd_show_handler(message, args):
     r = []
     if not args:
         if dnd_cards.get(message):
             card_data = dnd_cards.get(message)
-            inv = Agent().load(card_data)
+            inv = Adventurer().load(card_data)
             data = "[Oracle] 使用中人物卡: \n" 
             data += inv.output() + "\n"
             data += inv.skills_output()
             r.append(data)
         if dnd_cache_cards.get(message):
             card_data = dnd_cache_cards.get(message)
-            inv = Agent().load(card_data)
+            inv = Adventurer().load(card_data)
             r.append("[Oracle] 已暂存人物卡: \n" + inv.output())
     elif args[0] in ["skill", "s", "skills"]:
         if dnd_cards.get(message):
             card_data = dnd_cards.get(message)
-            inv = Agent().load(card_data)
+            inv = Adventurer().load(card_data)
             r.append(inv.skills_output())
     elif args[0] == "all":
         cd = dnd_cards.data[get_group_id(message)]
         for data in cd:
-            inv = Agent().load(cd[data])
+            inv = Adventurer().load(cd[data])
             d = inv.output() + "\n"
             d += inv.skills_output()
             r.append(d)
     else:
         r.append("[Oracle] 参数异常.")
     if not r:
         r.append("[Oracle] 未查询到保存或暂存信息.")
```

### Comparing `dicergirl-3.0.7/dicergirl/utils/messages.py` & `dicergirl-3.0.8/dicergirl/utils/messages.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/utils/settings.py` & `dicergirl-3.0.8/dicergirl/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/dicergirl/utils/utils.py` & `dicergirl-3.0.8/dicergirl/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     try:
         from botpy.message import Message
     except ModuleNotFoundError:
         logger.warning("未找到依赖`qq-botpy`, 请检查你的配置.")
         class Message:
             pass
 
-version = "3.0.7"
+version = "3.0.8"
 current_dir = Path(__file__).resolve().parent
 dicer_girl_dir = Path.home() / ".dicergirl"
 data_dir = dicer_girl_dir / "data"
 _coc_cachepath = data_dir / "coc_cards.json"
 _scp_cachepath = data_dir / "scp_cards.json"
 _dnd_cachepath = data_dir / "dnd_cards.json"
 _super_user = data_dir / "super_user.json"
```

### Comparing `dicergirl-3.0.7/dicergirl.egg-info/PKG-INFO` & `dicergirl-3.0.8/dicergirl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.7
+Version: 3.0.8
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dicergirl-3.0.7/dicergirl.egg-info/SOURCES.txt` & `dicergirl-3.0.8/dicergirl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.7/setup.py` & `dicergirl-3.0.8/setup.py`

 * *Files identical despite different names*

