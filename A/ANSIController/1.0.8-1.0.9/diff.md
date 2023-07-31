# Comparing `tmp/ANSIController-1.0.8.tar.gz` & `tmp/ANSIController-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANSIController-1.0.8.tar", last modified: Sun Jul 30 09:51:15 2023, max compression
+gzip compressed data, was "ANSIController-1.0.9.tar", last modified: Mon Jul 31 10:41:49 2023, max compression
```

## Comparing `ANSIController-1.0.8.tar` & `ANSIController-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 09:51:15.810635 ANSIController-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-07-30 09:51:15.785279 ANSIController-1.0.8/ANSIController/
--rw-rw-rw-   0        0        0    10863 2023-07-30 09:46:20.000000 ANSIController-1.0.8/ANSIController/__init__.py
--rw-rw-rw-   0        0        0     2307 2023-07-30 09:37:17.000000 ANSIController-1.0.8/ANSIController/__main__.py
--rw-rw-rw-   0        0        0     2280 2023-07-29 12:47:36.000000 ANSIController-1.0.8/ANSIController/const.py
--rw-rw-rw-   0        0        0     8681 2023-07-30 09:32:45.000000 ANSIController-1.0.8/ANSIController/controls.py
--rw-rw-rw-   0        0        0     3776 2023-07-30 08:38:37.000000 ANSIController-1.0.8/ANSIController/tcolor.py
--rw-rw-rw-   0        0        0      457 2023-07-30 09:32:51.000000 ANSIController-1.0.8/ANSIController/tparser.py
--rw-rw-rw-   0        0        0     2993 2023-07-30 08:38:33.000000 ANSIController-1.0.8/ANSIController/tstyles.py
-drwxrwxrwx   0        0        0        0 2023-07-30 09:51:15.808870 ANSIController-1.0.8/ANSIController.egg-info/
--rw-rw-rw-   0        0        0    11509 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-30 09:51:15.000000 ANSIController-1.0.8/ANSIController.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-07-30 01:37:14.000000 ANSIController-1.0.8/LICENSE
--rw-rw-rw-   0        0        0    11509 2023-07-30 09:51:15.811157 ANSIController-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    10524 2023-07-30 01:33:45.000000 ANSIController-1.0.8/README.md
--rw-rw-rw-   0        0        0       86 2023-07-30 09:51:15.812169 ANSIController-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1686 2023-07-30 09:51:08.000000 ANSIController-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:41:49.087089 ANSIController-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-31 10:41:49.058537 ANSIController-1.0.9/ANSIController/
+-rw-rw-rw-   0        0        0    11325 2023-07-31 10:05:13.000000 ANSIController-1.0.9/ANSIController/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-07-31 07:25:02.000000 ANSIController-1.0.9/ANSIController/__main__.py
+-rw-rw-rw-   0        0        0     2280 2023-07-30 11:30:05.000000 ANSIController-1.0.9/ANSIController/const.py
+-rw-rw-rw-   0        0        0     9287 2023-07-31 07:26:10.000000 ANSIController-1.0.9/ANSIController/controls.py
+-rw-rw-rw-   0        0        0     3776 2023-07-31 07:26:13.000000 ANSIController-1.0.9/ANSIController/tcolor.py
+-rw-rw-rw-   0        0        0      457 2023-07-31 07:26:16.000000 ANSIController-1.0.9/ANSIController/tparser.py
+-rw-rw-rw-   0        0        0     5950 2023-07-31 09:58:23.000000 ANSIController-1.0.9/ANSIController/tprogress.py
+-rw-rw-rw-   0        0        0     2993 2023-07-31 07:26:20.000000 ANSIController-1.0.9/ANSIController/tstyles.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:41:49.087089 ANSIController-1.0.9/ANSIController.egg-info/
+-rw-rw-rw-   0        0        0    16306 2023-07-31 10:41:48.000000 ANSIController-1.0.9/ANSIController.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-07-31 10:41:48.000000 ANSIController-1.0.9/ANSIController.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:41:48.000000 ANSIController-1.0.9/ANSIController.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-31 10:41:48.000000 ANSIController-1.0.9/ANSIController.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 10:41:48.000000 ANSIController-1.0.9/ANSIController.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-31 10:41:48.000000 ANSIController-1.0.9/ANSIController.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-07-30 01:37:14.000000 ANSIController-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    16306 2023-07-31 10:41:49.087089 ANSIController-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15321 2023-07-31 10:37:56.000000 ANSIController-1.0.9/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-31 10:41:49.087089 ANSIController-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-07-31 09:17:34.000000 ANSIController-1.0.9/setup.py
```

### Comparing `ANSIController-1.0.8/ANSIController/__init__.py` & `ANSIController-1.0.9/ANSIController/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,24 +208,37 @@
 from time import sleep
 import keyboard
 from ANSIController.controls import (
     _ColorsControls, _CursorControls,
     _print,_RESET,_1ATTR,_256_BG,
     _256_FG,_PARSER
 )
+from ANSIController.tprogress import _ProgressManage
 
-class Terminal(_CursorControls,_ColorsControls):
+class Terminal(_CursorControls,_ColorsControls,_ProgressManage):
     __colors = _PARSER._COLORS
     __styles = _PARSER._STYLES
     def __init__(self) -> None:
         super().__init__()
+
     def get_color(self,char:str,style:int=0,bg:bool=False) -> str:
         return _PARSER.get_color(char,style,bg)
     def get_reset(self) -> str:
         return _RESET
+    def print_multi_colorize(self,text:str|list):
+        if isinstance(text,str):
+            text = text.split('\n')
+        for t in text:
+            self.clear_line()
+            self.print_colorize(t+'\n') 
+    def print_progress(self):
+        txts = self._get_ptexts()
+        self.print_multi_colorize(txts)
+        self.force_move_to_up(len(txts),self.is_progress_finish())
+
     @staticmethod
     def game(row:int=40,col:int=40,move_steps:int=1):
         control = Terminal()
         for r in range(row):
             print("|"+'-'*col+"|")
         while True:
             try:
@@ -280,14 +293,13 @@
     @staticmethod
     def print_colors_styles():
         _print(f"{_1ATTR.format(s=1)}\n[-] Test Colors With Styles: \n{_RESET}")
         for color in Terminal.__colors:
             color.test_with_every_style(Terminal.__styles)
         _print("="*40+"\n")
         _print(_RESET+'\n')
-    
     @staticmethod
     def print_test():
         Terminal.print_styles()
         Terminal.print_colors()
         Terminal.print_id_colors()
         Terminal.print_colors_styles()
```

### Comparing `ANSIController-1.0.8/ANSIController/__main__.py` & `ANSIController-1.0.9/ANSIController/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 #!/data/data/com.termux/files/usr/bin/env python3
+from time import sleep
 from ANSIController import Terminal,_print
 
 ## more info `https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797#escape`
 
 __author__ = 'JoOx01'
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
@@ -28,14 +29,15 @@
 [4] Print IDs
 [5] Print All
 [6] X O   # soon 
 [7] Snake # soon
 [8] Move Game
 [9] Colorize Text
 [10] Clear Screen
+[11] Progress
 [-1] End
 -----------------------
 >>> 
 -----------------------""")
         t.force_move_to_up()
         t.move_to_left(50)
         # t.move_to_up(start_line=True)
@@ -60,14 +62,36 @@
         if choice == "9":
             text = str(input(f"Text `[your_color_code]`: {t.get_color('green')}"))
             t.get_reset()
             t.print_colorize(text)
             input()
         if choice == "10":
             t.clear_screen()
+        if choice == "11":
+            t.move_to_down(1)
+            max_value = int(input("Max Value: "))
+            increase = int(input("Increase Value: "))
+            texts = []
+            c = 1
+            _print("[Rules] %c% current , %m% max , %p% percent , %b% bar\n")
+            while True:
+                txt = str(input(f"Text Progress Line ({c}) [-1 To End] : "))
+                if txt == "-1":
+                    break
+                texts.append(txt)
+                c+=1
+            t.add_progress(texts,max_value,increase)
+            while not t.is_progress_finish():
+                t.increase_progress(all=True)
+                c = 0
+                for text in texts:
+                    t.set_progress_inc_value(10+c,c,False)
+                    c+=1
+                t.print_progress()
+                sleep(.2)
         if choice == '-1':
             t.clear_line()
             _print("\nThx For Using Bye\n")
             break
 if __name__ == '__main__':
     try:
         main()
```

### Comparing `ANSIController-1.0.8/ANSIController/const.py` & `ANSIController-1.0.9/ANSIController/const.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.8/ANSIController/controls.py` & `ANSIController-1.0.9/ANSIController/controls.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,19 @@
         self.__parse_escape(f"{steps}{'F' if start_line else 'B'}")
     def move_to_left(self, steps: int = 1):
         "moves cursor left {steps} lines"
         self.__parse_escape(f"{steps}D")
     def move_to_right(self, steps: int = 1):
         "moves cursor right {steps} lines"
         self.__parse_escape(f"{steps}C")
-    def force_move_to_up(self):
-        self.__parse_default("M")
+    def force_move_to_up(self,steps:int=1,clear=False):
+        for _ in range(steps):
+            self.__parse_default("M")
+            if clear:
+                self.clear_line()
 
     def save_cursor_postion(self):
         self.__parse_default("7")
     def restor_cursor_postion(self):
         self.__parse_default("8")
 
     def hide_cursor(self):
@@ -82,14 +85,18 @@
         self.__parse_escape("K")  # 0K
     def clear_before_cursor(self):
         self.__parse_escape("1J")
     def clear_after_cursor(self):
         self.__parse_escape("J")  # 0J
     def clear_line(self):
         self.__parse_escape("2K\r") # type: ignore
+    def clear_up_lines(self,steps:int=1):
+        self.save_cursor_postion()
+        self.force_move_to_up(steps,clear=True)
+        self.restor_cursor_postion()
 
 class _ColorsControls:
     def __init__(self) -> None:
         pass
 
     def __get_colors_escape(self,style:str,colors:tuple) -> str:
         if style == None and all(c is None for c in colors):
@@ -129,15 +136,15 @@
             else:
                 data.append(text)
         return data
     def __swap(self,text:str,texts) -> str:
         texts = self.__replace(texts)
         for t in texts:
             if isinstance(t,tuple):
-                text = text.replace(t[0],self.__get_colors_escape(t[1],t[2]))
+                text = text.replace(t[0],self.__get_colors_escape(t[1],t[2]),1)
         return text
 
     def colorize(self,text:str,sep:str="[]") -> str:
         """
         ##### @text: text u want to colorize in terminal
         ##### @sep: set special code of colors styles `[]` `!$` `{}` `()` `$$` `??` `}{` and so on
         - ##### if terminal not support colorize the string will just remove from string
@@ -198,11 +205,19 @@
         """
         fsep,esep = sep,sep
         if len(sep) == 2:
             fsep,esep = sep[0],sep[1]
         fsep = re.escape(fsep)
         esep = re.escape(esep)
         text = _convert_hex_colors(text)
-        return self.__swap(text,re.compile(rf"({fsep}.*?{esep})").findall(text))
+        _re = fr"{fsep}[^{fsep}{esep}].*?{esep}"
+        _found = re.compile(rf"({_re})").findall(text)
+        _manual_replacment = []
+        for r in _found:
+            if '/' in r:
+                _found.remove(r)
+                _manual_replacment.append(r)
+        for m in _manual_replacment:
+            text = text.replace(m,m.replace('/',''))
+        return self.__swap(text,_found)
     def print_colorize(self,text:str,sep:str="[]") -> None:
         _print(self.colorize(text,sep))
-
```

### Comparing `ANSIController-1.0.8/ANSIController/tcolor.py` & `ANSIController-1.0.9/ANSIController/tcolor.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.8/ANSIController/tstyles.py` & `ANSIController-1.0.9/ANSIController/tstyles.py`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.8/ANSIController.egg-info/PKG-INFO` & `ANSIController-1.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,720 +1,958 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2041 4e53  : 2.1..Name: ANS
-00000020: 4943 6f6e 7472 6f6c 6c65 720d 0a56 6572  IController..Ver
-00000030: 7369 6f6e 3a20 312e 302e 380d 0a53 756d  sion: 1.0.8..Sum
-00000040: 6d61 7279 3a20 4261 7369 6320 5079 7468  mary: Basic Pyth
-00000050: 6f6e 204d 6f64 756c 6520 746f 2063 6f6e  on Module to con
-00000060: 7472 6f6c 2026 2063 6f6c 6f72 2026 2073  trol & color & s
-00000070: 7479 6c65 2074 6578 7420 696e 2074 6572  tyle text in ter
-00000080: 6d69 6e61 6c0d 0a48 6f6d 652d 7061 6765  minal..Home-page
-00000090: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-000000a0: 2e63 6f6d 2f6a 6f30 7830 312f 616e 7369  .com/jo0x01/ansi
-000000b0: 636f 6e74 726f 6c6c 6572 0d0a 4175 7468  controller..Auth
-000000c0: 6f72 3a20 4a6f 4f78 3031 0d0a 4175 7468  or: JoOx01..Auth
-000000d0: 6f72 2d65 6d61 696c 3a20 666f 7273 656c  or-email: forsel
-000000e0: 6c34 3530 4067 6d61 696c 2e63 6f6d 0d0a  l450@gmail.com..
-000000f0: 4c69 6365 6e73 653a 204d 4954 0d0a 4b65  License: MIT..Ke
-00000100: 7977 6f72 6473 3a20 616e 7369 2c74 6572  ywords: ansi,ter
-00000110: 6d69 6e61 6c2c 616e 7369 5f74 6572 6d69  minal,ansi_termi
-00000120: 6e61 6c2c 414e 5349 436f 6e74 726f 6c2c  nal,ANSIControl,
-00000130: 414e 5349 436f 6e74 726f 6c6c 6572 2c41  ANSIController,A
-00000140: 534e 492c 616e 7369 636f 6e74 726f 6c6c  SNI,ansicontroll
-00000150: 6572 0d0a 436c 6173 7369 6669 6572 3a20  er..Classifier: 
-00000160: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000170: 7573 203a 3a20 3320 2d20 416c 7068 610d  us :: 3 - Alpha.
-00000180: 0a43 6c61 7373 6966 6965 723a 2045 6e76  .Classifier: Env
-00000190: 6972 6f6e 6d65 6e74 203a 3a20 436f 6e73  ironment :: Cons
-000001a0: 6f6c 650d 0a43 6c61 7373 6966 6965 723a  ole..Classifier:
-000001b0: 2045 6e76 6972 6f6e 6d65 6e74 203a 3a20   Environment :: 
-000001c0: 436f 6e73 6f6c 6520 3a3a 2043 7572 7365  Console :: Curse
-000001d0: 730d 0a43 6c61 7373 6966 6965 723a 2045  s..Classifier: E
-000001e0: 6e76 6972 6f6e 6d65 6e74 203a 3a20 436f  nvironment :: Co
-000001f0: 6e73 6f6c 6520 3a3a 2046 7261 6d65 6275  nsole :: Framebu
-00000200: 6666 6572 0d0a 436c 6173 7369 6669 6572  ffer..Classifier
-00000210: 3a20 456e 7669 726f 6e6d 656e 7420 3a3a  : Environment ::
-00000220: 2043 6f6e 736f 6c65 203a 3a20 4e65 7774   Console :: Newt
-00000230: 0d0a 436c 6173 7369 6669 6572 3a20 496e  ..Classifier: In
-00000240: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000250: 3a3a 2044 6576 656c 6f70 6572 730d 0a43  :: Developers..C
-00000260: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-00000270: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000280: 656c 6f70 6d65 6e74 203a 3a20 4275 696c  elopment :: Buil
-00000290: 6420 546f 6f6c 730d 0a43 6c61 7373 6966  d Tools..Classif
-000002a0: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-000002b0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000002c0: 4d49 5420 4c69 6365 6e73 650d 0a43 6c61  MIT License..Cla
-000002d0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000002e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002f0: 2050 7974 686f 6e20 3a3a 2033 0d0a 436c   Python :: 3..Cl
-00000300: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 340d  : Python :: 3.4.
-00000330: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000340: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000350: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000360: 2e35 0d0a 436c 6173 7369 6669 6572 3a20  .5..Classifier: 
-00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000390: 3a20 332e 360d 0a44 6573 6372 6970 7469  : 3.6..Descripti
-000003a0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000003b0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-000003c0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000003d0: 4345 4e53 450d 0a0d 0a60 6060 7368 0d0a  CENSE....```sh..
-000003e0: 0d0a 2320 2020 2020 2020 2020 6438 3838  ..#         d888
-000003f0: 3820 3838 3862 2020 2020 3838 3820 202e  8 888b    888  .
-00000400: 6438 3838 3862 2e20 3838 3838 3838 3820  d8888b. 8888888 
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000000: 6060 6073 680d 0a0d 0a23 2020 2020 2020  ```sh....#      
+00000010: 2020 2064 3838 3838 2038 3838 6220 2020     d8888 888b   
+00000020: 2038 3838 2020 2e64 3838 3838 622e 2038   888  .d8888b. 8
+00000030: 3838 3838 3838 2020 2020 2020 2020 2020  888888          
+00000040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000060: 2020 2020 0d0a 2320 2020 2020 2020 2064      ..#        d
+00000070: 3838 3838 3820 3838 3838 6220 2020 3838  88888 8888b   88
+00000080: 3820 6438 3850 2020 5938 3862 2020 3838  8 d88P  Y88b  88
+00000090: 3820 2020 2020 2020 2020 2020 2020 2020  8               
+000000a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000000b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000000c0: 200d 0a23 2020 2020 2020 2064 3838 5038   ..#       d88P8
+000000d0: 3838 2038 3838 3838 6220 2038 3838 2059  88 88888b  888 Y
+000000e0: 3838 622e 2020 2020 2020 2038 3838 2020  88b.       888  
+000000f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000110: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00000120: 2320 2020 2020 2064 3838 5020 3838 3820  #      d88P 888 
+00000130: 3838 3859 3838 6220 3838 3820 2022 5938  888Y88b 888  "Y8
+00000140: 3838 622e 2020 2020 3838 3820 2020 2020  88b.    888     
+00000150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000170: 2020 2020 2020 2020 2020 200d 0a23 2020             ..#  
+00000180: 2020 2064 3838 5020 2038 3838 2038 3838     d88P  888 888
+00000190: 2059 3838 6238 3838 2020 2020 2022 5938   Y88b888     "Y8
+000001a0: 3862 2e20 2038 3838 2020 2020 2020 2020  8b.  888        
+000001b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001d0: 2020 2020 2020 2020 0d0a 2320 2020 2064          ..#    d
+000001e0: 3838 5020 2020 3838 3820 3838 3820 2059  88P   888 888  Y
+000001f0: 3838 3838 3820 2020 2020 2020 2238 3838  88888       "888
+00000200: 2020 3838 3820 2020 2020 2020 2020 2020    888           
+00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000230: 2020 2020 200d 0a23 2020 2064 3838 3838       ..#   d8888
+00000240: 3838 3838 3838 2038 3838 2020 2059 3838  888888 888   Y88
+00000250: 3838 2059 3838 6220 2064 3838 5020 2038  88 Y88b  d88P  8
+00000260: 3838 2020 2020 2020 2020 2020 2020 2020  88              
+00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000290: 2020 0d0a 2320 2064 3838 5020 2020 2020    ..#  d88P     
+000002a0: 3838 3820 3838 3820 2020 2059 3838 3820  888 888    Y888 
+000002b0: 2022 5938 3838 3850 2220 3838 3838 3838   "Y8888P" 888888
+000002c0: 3820 2020 2020 2020 2020 2020 2020 2020  8               
+000002d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002e0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000002f0: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
+00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 2020 2020 2020 2020 2020 2020 0d0a 2320              ..# 
+00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003a0: 2020 2020 2020 2020 200d 0a23 2020 2020           ..#    
+000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000400: 2020 2020 2020 0d0a 2320 2020 2020 2020        ..#       
+00000410: 2020 2020 2020 202e 6438 3838 3862 2e20         .d8888b. 
 00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 2020 2020 2020 2020 2020 2020 200d 0a23               ..#
-00000440: 2020 2020 2020 2020 6438 3838 3838 2038          d88888 8
-00000450: 3838 3862 2020 2038 3838 2064 3838 5020  888b   888 d88P 
-00000460: 2059 3838 6220 2038 3838 2020 2020 2020   Y88b  888      
-00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000430: 2020 2038 3838 2020 2020 2020 2020 2020     888          
+00000440: 2020 2020 2020 2020 2020 3838 3820 3838            888 88
+00000450: 3820 2020 2020 2020 2020 2020 2020 2020  8               
+00000460: 2020 200d 0a23 2020 2020 2020 2020 2020     ..#          
+00000470: 2020 2064 3838 5020 2059 3838 6220 2020     d88P  Y88b   
 00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000490: 2020 2020 2020 2020 2020 0d0a 2320 2020            ..#   
-000004a0: 2020 2020 6438 3850 3838 3820 3838 3838      d88P888 8888
-000004b0: 3862 2020 3838 3820 5938 3862 2e20 2020  8b  888 Y88b.   
-000004c0: 2020 2020 3838 3820 2020 2020 2020 2020      888         
-000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004f0: 2020 2020 2020 200d 0a23 2020 2020 2020         ..#      
-00000500: 6438 3850 2038 3838 2038 3838 5938 3862  d88P 888 888Y88b
-00000510: 2038 3838 2020 2259 3838 3862 2e20 2020   888  "Y888b.   
-00000520: 2038 3838 2020 2020 2020 2020 2020 2020   888            
-00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000550: 2020 2020 0d0a 2320 2020 2020 6438 3850      ..#     d88P
-00000560: 2020 3838 3820 3838 3820 5938 3862 3838    888 888 Y88b88
-00000570: 3820 2020 2020 2259 3838 622e 2020 3838  8     "Y88b.  88
-00000580: 3820 2020 2020 2020 2020 2020 2020 2020  8               
-00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 200d 0a23 2020 2020 6438 3850 2020 2038   ..#    d88P   8
-000005c0: 3838 2038 3838 2020 5938 3838 3838 2020  88 888  Y88888  
-000005d0: 2020 2020 2022 3838 3820 2038 3838 2020       "888  888  
-000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00000610: 2320 2020 6438 3838 3838 3838 3838 3820  #   d8888888888 
-00000620: 3838 3820 2020 5938 3838 3820 5938 3862  888   Y8888 Y88b
-00000630: 2020 6438 3850 2020 3838 3820 2020 2020    d88P  888     
-00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 2020 2020 2020 2020 2020 200d 0a23 2020             ..#  
-00000670: 6438 3850 2020 2020 2038 3838 2038 3838  d88P     888 888
-00000680: 2020 2020 5938 3838 2020 2259 3838 3838      Y888  "Y8888
-00000690: 5022 2038 3838 3838 3838 2020 2020 2020  P" 8888888      
-000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006c0: 2020 2020 2020 2020 0d0a 2320 2020 2020          ..#     
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000490: 3838 3820 2020 2020 2020 2020 2020 2020  888             
+000004a0: 2020 2020 2020 2038 3838 2038 3838 2020         888 888  
+000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004c0: 0d0a 2320 2020 2020 2020 2020 2020 2020  ..#             
+000004d0: 3838 3820 2020 2038 3838 2020 2020 2020  888    888      
+000004e0: 2020 2020 2020 2020 2020 2020 2038 3838               888
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 2020 2020 3838 3820 3838 3820 2020 2020      888 888     
+00000510: 2020 2020 2020 2020 2020 2020 200d 0a23               ..#
+00000520: 2020 2020 2020 2020 2020 2020 2038 3838               888
+00000530: 2020 2020 2020 2020 202e 6438 3862 2e20           .d88b. 
+00000540: 2038 3838 3838 622e 2020 3838 3838 3838   88888b.  888888
+00000550: 2038 3838 6438 3838 202e 6438 3862 2e20   888d888 .d88b. 
+00000560: 2038 3838 2038 3838 2020 2e64 3838 622e   888 888  .d88b.
+00000570: 2020 3838 3864 3838 3820 0d0a 2320 2020    888d888 ..#   
+00000580: 2020 2020 2020 2020 2020 3838 3820 2020            888   
+00000590: 2020 2020 2064 3838 2222 3838 6220 3838       d88""88b 88
+000005a0: 3820 2238 3862 2038 3838 2020 2020 3838  8 "88b 888    88
+000005b0: 3850 2220 2064 3838 2222 3838 6220 3838  8P"  d88""88b 88
+000005c0: 3820 3838 3820 6438 5020 2059 3862 2038  8 888 d8P  Y8b 8
+000005d0: 3838 5022 2020 200d 0a23 2020 2020 2020  88P"   ..#      
+000005e0: 2020 2020 2020 2038 3838 2020 2020 3838         888    88
+000005f0: 3820 3838 3820 2038 3838 2038 3838 2020  8 888  888 888  
+00000600: 3838 3820 3838 3820 2020 2038 3838 2020  888 888    888  
+00000610: 2020 3838 3820 2038 3838 2038 3838 2038    888  888 888 8
+00000620: 3838 2038 3838 3838 3838 3820 3838 3820  88 88888888 888 
+00000630: 2020 2020 0d0a 2320 2020 2020 2020 2020      ..#         
+00000640: 2020 2020 5938 3862 2020 6438 3850 2059      Y88b  d88P Y
+00000650: 3838 2e2e 3838 5020 3838 3820 2038 3838  88..88P 888  888
+00000660: 2059 3838 622e 2020 3838 3820 2020 2059   Y88b.  888    Y
+00000670: 3838 2e2e 3838 5020 3838 3820 3838 3820  88..88P 888 888 
+00000680: 5938 622e 2020 2020 2038 3838 2020 2020  Y8b.     888    
+00000690: 200d 0a23 2020 2020 2020 2020 2020 2020   ..#            
+000006a0: 2020 2259 3838 3838 5022 2020 2022 5938    "Y8888P"   "Y8
+000006b0: 3850 2220 2038 3838 2020 3838 3820 2022  8P"  888  888  "
+000006c0: 5938 3838 2038 3838 2020 2020 2022 5938  Y888 888     "Y8
+000006d0: 3850 2220 2038 3838 2038 3838 2020 2259  8P"  888 888  "Y
+000006e0: 3838 3838 2020 3838 3820 2020 2020 0d0a  8888  888     ..
+000006f0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
 00000700: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 200d 0a23 2020 2020 2020 2020       ..#        
+00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000780: 2020 0d0a 2320 2020 2020 2020 2020 2020    ..#           
-00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000007e0: 0a23 2020 2020 2020 2020 2020 2020 2020  .#              
-000007f0: 2e64 3838 3838 622e 2020 2020 2020 2020  .d8888b.        
-00000800: 2020 2020 2020 2020 2020 2020 3838 3820              888 
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2020 2038 3838 2038 3838 2020 2020 2020     888 888      
-00000830: 2020 2020 2020 2020 2020 2020 0d0a 2320              ..# 
-00000840: 2020 2020 2020 2020 2020 2020 6438 3850              d88P
-00000850: 2020 5938 3862 2020 2020 2020 2020 2020    Y88b          
-00000860: 2020 2020 2020 2020 2038 3838 2020 2020           888    
-00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000880: 3838 3820 3838 3820 2020 2020 2020 2020  888 888         
-00000890: 2020 2020 2020 2020 200d 0a23 2020 2020           ..#    
-000008a0: 2020 2020 2020 2020 2038 3838 2020 2020           888    
-000008b0: 3838 3820 2020 2020 2020 2020 2020 2020  888             
-000008c0: 2020 2020 2020 3838 3820 2020 2020 2020        888       
-000008d0: 2020 2020 2020 2020 2020 2020 2038 3838               888
-000008e0: 2038 3838 2020 2020 2020 2020 2020 2020   888            
-000008f0: 2020 2020 2020 0d0a 2320 2020 2020 2020        ..#       
-00000900: 2020 2020 2020 3838 3820 2020 2020 2020        888       
-00000910: 2020 2e64 3838 622e 2020 3838 3838 3862    .d88b.  88888b
-00000920: 2e20 2038 3838 3838 3820 3838 3864 3838  .  888888 888d88
-00000930: 3820 2e64 3838 622e 2020 3838 3820 3838  8 .d88b.  888 88
-00000940: 3820 202e 6438 3862 2e20 2038 3838 6438  8  .d88b.  888d8
-00000950: 3838 200d 0a23 2020 2020 2020 2020 2020  88 ..#          
-00000960: 2020 2038 3838 2020 2020 2020 2020 6438     888        d8
-00000970: 3822 2238 3862 2038 3838 2022 3838 6220  8""88b 888 "88b 
-00000980: 3838 3820 2020 2038 3838 5022 2020 6438  888    888P"  d8
-00000990: 3822 2238 3862 2038 3838 2038 3838 2064  8""88b 888 888 d
-000009a0: 3850 2020 5938 6220 3838 3850 2220 2020  8P  Y8b 888P"   
-000009b0: 0d0a 2320 2020 2020 2020 2020 2020 2020  ..#             
-000009c0: 3838 3820 2020 2038 3838 2038 3838 2020  888    888 888  
-000009d0: 3838 3820 3838 3820 2038 3838 2038 3838  888 888  888 888
-000009e0: 2020 2020 3838 3820 2020 2038 3838 2020      888    888  
-000009f0: 3838 3820 3838 3820 3838 3820 3838 3838  888 888 888 8888
-00000a00: 3838 3838 2038 3838 2020 2020 200d 0a23  8888 888     ..#
-00000a10: 2020 2020 2020 2020 2020 2020 2059 3838               Y88
-00000a20: 6220 2064 3838 5020 5938 382e 2e38 3850  b  d88P Y88..88P
-00000a30: 2038 3838 2020 3838 3820 5938 3862 2e20   888  888 Y88b. 
-00000a40: 2038 3838 2020 2020 5938 382e 2e38 3850   888    Y88..88P
-00000a50: 2038 3838 2038 3838 2059 3862 2e20 2020   888 888 Y8b.   
-00000a60: 2020 3838 3820 2020 2020 0d0a 2320 2020    888     ..#   
-00000a70: 2020 2020 2020 2020 2020 2022 5938 3838             "Y888
-00000a80: 3850 2220 2020 2259 3838 5022 2020 3838  8P"   "Y88P"  88
-00000a90: 3820 2038 3838 2020 2259 3838 3820 3838  8  888  "Y888 88
-00000aa0: 3820 2020 2020 2259 3838 5022 2020 3838  8     "Y88P"  88
-00000ab0: 3820 3838 3820 2022 5938 3838 3820 2038  8 888  "Y8888  8
-00000ac0: 3838 2020 2020 200d 0a23 2020 2020 2020  88     ..#      
-00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2020 200d 0a60 6060 0d0a 2320 414e 5349     ..```..# ANSI
-00000b30: 2043 6f6e 7472 6f6c 6c65 720d 0a3e 2042   Controller..> B
-00000b40: 6173 6963 2050 7974 686f 6e20 5363 7269  asic Python Scri
-00000b50: 7074 2074 6f20 636f 6e74 726f 6c20 6375  pt to control cu
-00000b60: 7273 6f72 2070 6f73 7469 6f6e 2069 6e20  rsor postion in 
-00000b70: 7465 726d 696e 616c 0d0a 3e20 616e 6420  terminal..> and 
-00000b80: 636f 6c6f 7269 7a65 2061 6e79 2074 6578  colorize any tex
-00000b90: 7420 696e 2074 6572 6d69 6e61 6c20 2c20  t in terminal , 
-00000ba0: 616e 6420 6164 6420 616e 7920 7374 796c  and add any styl
-00000bb0: 6520 746f 2067 7261 7068 6963 206d 6f64  e to graphic mod
-00000bc0: 6520 696e 2074 6572 6d69 6e61 6c0d 0a3c  e in terminal..<
-00000bd0: 6469 7620 7374 796c 653d 220d 0a20 2020  div style="..   
-00000be0: 2063 6f6c 6f72 3a20 7768 6974 653b 0d0a   color: white;..
-00000bf0: 2020 2020 6261 636b 6772 6f75 6e64 2d63      background-c
-00000c00: 6f6c 6f72 3a20 2338 4230 3030 303b 0d0a  olor: #8B0000;..
-00000c10: 2020 2020 7061 6464 696e 673a 2031 3070      padding: 10p
-00000c20: 783b 0d0a 2020 2020 616c 6967 6e6d 656e  x;..    alignmen
-00000c30: 743a 2063 656e 7465 723b 0d0a 2020 2020  t: center;..    
-00000c40: 7465 7874 2d61 6c69 676e 3a20 6365 6e74  text-align: cent
-00000c50: 6572 3b0d 0a22 3e0d 0a3c 623e 4e6f 7465  er;..">..<b>Note
-00000c60: 3c2f 623e 3c62 723e 0d0a 2120 5468 6973  </b><br>..! This
-00000c70: 204d 6f64 756c 6520 776f 726b 2044 6570   Module work Dep
-00000c80: 656e 6473 206f 6620 5465 726d 696e 616c  ends of Terminal
-00000c90: 2054 7970 6520 6f66 2073 7570 706f 7274   Type of support
-00000ca0: 2041 4e53 4920 6573 6361 7065 2063 6861   ANSI escape cha
-00000cb0: 7261 6374 6572 7320 6f72 206e 6f74 2021  racters or not !
-00000cc0: 0d0a 3c68 723e 0d0a 6966 2075 2066 6163  ..<hr>..if u fac
-00000cd0: 6520 616e 7920 6973 7375 6520 7772 6974  e any issue writ
-00000ce0: 6520 6974 0d0a 3c2f 6469 763e 0d0a 3c62  e it..</div>..<b
-00000cf0: 723e 0d0a 0d0a 5b21 5b50 7950 695d 2868  r>....[![PyPi](h
-00000d00: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000d10: 6473 2e69 6f2f 6261 6467 652f 2d50 7950  ds.io/badge/-PyP
-00000d20: 692d 626c 7565 2e73 7667 3f6c 6f67 6f3d  i-blue.svg?logo=
-00000d30: 7079 7069 266c 6162 656c 436f 6c6f 723d  pypi&labelColor=
-00000d40: 3535 3535 3535 2673 7479 6c65 3d66 6f72  555555&style=for
-00000d50: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
-00000d60: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000d70: 6f6a 6563 742f 414e 5349 436f 6e74 726f  oject/ANSIContro
-00000d80: 6c6c 6572 2022 5079 5069 2229 205b 215b  ller "PyPi") [![
-00000d90: 4c69 6365 6e73 653a 206c 6963 656e 7365  License: license
-00000da0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000db0: 6965 6c64 732e 696f 2f62 6164 6765 2f2d  ields.io/badge/-
-00000dc0: 6c69 6365 6e73 652d 626c 7565 2e73 7667  license-blue.svg
-00000dd0: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
-00000de0: 6164 6765 295d 284c 4943 454e 5345 2022  adge)](LICENSE "
-00000df0: 4c69 6365 6e73 6522 290d 0a0d 0a5b 4d6f  License")....[Mo
-00000e00: 7265 2049 6e66 6f20 4162 6f75 7420 414e  re Info About AN
-00000e10: 5349 2045 7363 6170 6520 436f 6465 735d  SI Escape Codes]
-00000e20: 2860 6874 7470 733a 2f2f 6769 7374 2e67  (`https://gist.g
-00000e30: 6974 6875 622e 636f 6d2f 666e 6b79 2f34  ithub.com/fnky/4
-00000e40: 3538 3731 3933 3433 6161 6264 3031 6366  58719343aabd01cf
-00000e50: 6231 3761 3361 3466 3732 3936 3739 3723  b17a3a4f7296797#
-00000e60: 6573 6361 7065 6029 0d0a 2323 2046 6561  escape`)..## Fea
-00000e70: 7475 7265 730d 0a2d 2d2d 2d2d 2d2d 2d2d  tures..---------
-00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e90: 2d2d 2d2d 2d0d 0a60 414e 5349 2043 6f6e  -----..`ANSI Con
-00000ea0: 7472 6f6c 6c65 7260 2046 6561 7475 7265  troller` Feature
-00000eb0: 733a 0d0a 2d20 4d6f 7665 2043 7572 736f  s:..- Move Curso
-00000ec0: 7220 5269 6768 7420 6f72 206c 6566 7420  r Right or left 
-00000ed0: 6f72 2074 6f70 206f 7220 646f 776e 206f  or top or down o
-00000ee0: 7220 706f 7374 696f 6e20 696e 2074 6572  r postion in ter
-00000ef0: 6d69 6e61 6c20 7363 7265 656e 0d0a 2d20  minal screen..- 
-00000f00: 436f 6c6f 7269 7a65 2061 6e79 2074 6578  Colorize any tex
-00000f10: 7420 7520 7761 6e74 2069 6e20 7465 726d  t u want in term
-00000f20: 696e 616c 0d0a 2d20 4368 616e 6765 2053  inal..- Change S
-00000f30: 7479 6c65 206f 6620 7465 726d 696e 616c  tyle of terminal
-00000f40: 2070 7269 6e74 696e 6720 7465 7874 202c   printing text ,
-00000f50: 2062 6f6c 6420 2c69 7461 6c69 6320 2c20   bold ,italic , 
-00000f60: 6574 632e 2e2e 0d0a 0d0a 2323 2054 6563  etc.......## Tec
-00000f70: 680d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  h..-------------
-00000f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000f90: 2d0d 0a0d 0a5b 4d6f 7265 2049 6e66 6f20  -....[More Info 
-00000fa0: 4162 6f75 7420 414e 5349 2045 7363 6170  About ANSI Escap
-00000fb0: 6520 436f 6465 735d 2860 6874 7470 733a  e Codes](`https:
-00000fc0: 2f2f 6769 7374 2e67 6974 6875 622e 636f  //gist.github.co
-00000fd0: 6d2f 666e 6b79 2f34 3538 3731 3933 3433  m/fnky/458719343
-00000fe0: 6161 6264 3031 6366 6231 3761 3361 3466  aabd01cfb17a3a4f
-00000ff0: 3732 3936 3739 3723 6573 6361 7065 6029  7296797#escape`)
-00001000: 0d0a 6041 4e53 4920 436f 6e74 726f 6c6c  ..`ANSI Controll
-00001010: 6572 6020 7573 6573 2061 206e 756d 6265  er` uses a numbe
-00001020: 7220 6f66 206f 7065 6e20 736f 7572 6365  r of open source
-00001030: 2070 726f 6a65 6374 7320 746f 2077 6f72   projects to wor
-00001040: 6b20 7072 6f70 6572 6c79 3a0d 0a2d 205b  k properly:..- [
-00001050: 6b65 7962 6f61 7264 5d20 2d20 7079 7069  keyboard] - pypi
-00001060: 206d 6f64 756c 6520 6068 7474 7073 3a2f   module `https:/
-00001070: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00001080: 742f 6b65 7962 6f61 7264 2f60 0d0a 2d20  t/keyboard/`..- 
-00001090: 416e 6420 6f66 2063 6f75 7273 6520 6041  And of course `A
-000010a0: 4e53 4920 436f 6e74 726f 6c6c 6572 6020  NSI Controller` 
-000010b0: 6974 7365 6c66 2069 7320 6f70 656e 2073  itself is open s
-000010c0: 6f75 7263 652e 0d0a 206f 6e20 4769 7448  ource... on GitH
-000010d0: 7562 2e0d 0a0d 0a23 2320 496e 7374 616c  ub.....## Instal
-000010e0: 6c61 7469 6f6e 0d0a 2d2d 2d2d 2d2d 2d2d  lation..--------
-000010f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001100: 2d2d 2d2d 2d2d 0d0a 0d0a 6041 4e53 4920  ------....`ANSI 
-00001110: 436f 6e74 726f 6c6c 6572 6020 7265 7175  Controller` requ
-00001120: 6972 6573 205b 7069 705d 2868 7474 7073  ires [pip](https
-00001130: 3a2f 2f70 7970 692e 6f72 672f 2920 746f  ://pypi.org/) to
-00001140: 2069 6e73 7461 6c6c 2e0d 0a49 6e73 7461   install...Insta
-00001150: 6c6c 2074 6865 2064 6570 656e 6465 6e63  ll the dependenc
-00001160: 6965 7320 616e 6420 6465 7644 6570 656e  ies and devDepen
-00001170: 6465 6e63 6965 7320 616e 6420 7374 6172  dencies and star
-00001180: 7420 7468 6520 7363 7269 7074 2e0d 0a23  t the script...#
-00001190: 2323 2057 696e 646f 7773 0d0a 6060 6062  ## Windows..```b
-000011a0: 6173 680d 0a70 6970 2069 6e73 7461 6c6c  ash..pip install
-000011b0: 2041 4e53 4943 6f6e 7472 6f6c 6c65 720d   ANSIController.
-000011c0: 0a60 6060 0d0a 2323 2320 4c69 6e75 7820  .```..### Linux 
-000011d0: 2626 2054 6572 6d75 780d 0a60 6060 6261  && Termux..```ba
-000011e0: 7368 0d0a 7069 7033 2069 6e73 7461 6c6c  sh..pip3 install
-000011f0: 2041 4e53 4943 6f6e 7472 6f6c 6c65 720d   ANSIController.
-00001200: 0a60 6060 0d0a 2320 5461 626c 6520 6f66  .```..# Table of
-00001210: 2063 6f6c 6f72 7320 2620 7374 796c 650d   colors & style.
-00001220: 0a2d 2023 2323 2320 6966 2074 6572 6d69  .- #### if termi
-00001230: 6e61 6c20 6e6f 7420 7375 7070 6f72 7420  nal not support 
-00001240: 636f 6c6f 7269 7a65 2074 6865 2073 7472  colorize the str
-00001250: 696e 6720 7769 6c6c 206a 7573 7420 7265  ing will just re
-00001260: 6d6f 7665 2066 726f 6d20 7374 7269 6e67  move from string
-00001270: 0d0a 2d20 2323 2320 4e6f 7465 3a20 4164  ..- ### Note: Ad
-00001280: 6420 4375 7374 6f6d 2056 616c 7565 732c  d Custom Values,
-00001290: 2074 6f20 7374 7269 6e67 2074 6f20 636f   to string to co
-000012a0: 6c6f 7269 7a65 2074 6865 206f 7574 7075  lorize the outpu
-000012b0: 740d 0a2d 2023 2323 2320 4944 2d2d 2d2d  t..- #### ID----
-000012c0: 2d2d 2d2d 2d2d 3a20 603c 7b69 647d 3e60  ------: `<{id}>`
-000012d0: 2020 6672 6f6d 2030 2074 6f20 3235 3520    from 0 to 255 
-000012e0: 2c20 603c 3235 353e 6020 2c20 603c 3135  , `<255>` , `<15
-000012f0: 3e60 0d0a 2d20 2323 2323 2052 4742 2d2d  >`..- #### RGB--
-00001300: 2d2d 2d2d 2d2d 2d3a 2060 2872 6564 5f76  -------: `(red_v
-00001310: 616c 7565 2c67 7265 656e 5f76 616c 7565  alue,green_value
-00001320: 2c62 6c75 655f 7661 6c75 6529 6020 6672  ,blue_value)` fr
-00001330: 6f6d 2030 2074 6f20 3235 3520 202c 2060  om 0 to 255  , `
-00001340: 2832 3133 2c32 3031 2c32 3530 2960 0d0a  (213,201,250)`..
-00001350: 2d20 2323 2323 2052 4742 2d2d 2d2d 2d2d  - #### RGB------
-00001360: 2d2d 2d3a 2060 2346 4646 4646 4660 2075  ---: `#FFFFFF` u
-00001370: 7369 6e67 2068 6578 202c 2060 2334 6166  sing hex , `#4af
-00001380: 6661 3160 0d0a 2d20 2323 2323 2042 6163  fa1`..- #### Bac
-00001390: 6b67 726f 756e 642d 2d3a 2060 582c 7860  kground--: `X,x`
-000013a0: 0d0a 2d20 2323 2323 2052 6573 6574 2d2d  ..- #### Reset--
-000013b0: 2d2d 2d2d 2d3a 2060 5a2c 302c 7265 7365  -----: `Z,0,rese
-000013c0: 742c 5265 7365 7460 0d0a 2d20 2323 2323  t,Reset`..- ####
-000013d0: 2043 6f6c 6f72 733a 0d0a 2020 2020 2d20   Colors:..    - 
-000013e0: 5b2b 5d20 6062 6c61 636b 3a60 2020 2020  [+] `black:`    
-000013f0: 2020 2020 2020 2020 2020 6062 2c62 6c61            `b,bla
-00001400: 636b 2c33 3060 0d0a 2020 2020 2d20 5b2b  ck,30`..    - [+
-00001410: 5d20 6072 6564 3a60 2020 2020 2020 2020  ] `red:`        
-00001420: 2020 2020 2020 2020 6072 2c72 6564 2c33          `r,red,3
-00001430: 3160 0d0a 2020 2020 2d20 5b2b 5d20 6067  1`..    - [+] `g
-00001440: 7265 656e 3a60 2020 2020 2020 2020 2020  reen:`          
-00001450: 2020 2020 6067 2c67 7265 656e 2c33 3260      `g,green,32`
-00001460: 0d0a 2020 2020 2d20 5b2b 5d20 6079 656c  ..    - [+] `yel
-00001470: 6c6f 773a 6020 2020 2020 2020 2020 2020  low:`           
-00001480: 2020 6079 2c79 656c 6c6f 772c 3333 600d    `y,yellow,33`.
-00001490: 0a20 2020 202d 205b 2b5d 2060 626c 7565  .    - [+] `blue
-000014a0: 3a60 2020 2020 2020 2020 2020 2020 2020  :`              
-000014b0: 2060 6c2c 626c 7565 2c33 3460 0d0a 2020   `l,blue,34`..  
-000014c0: 2020 2d20 5b2b 5d20 606d 6167 656e 7461    - [+] `magenta
-000014d0: 3a60 2020 2020 2020 2020 2020 2020 606d  :`            `m
-000014e0: 2c6d 6167 656e 7461 2c33 3560 0d0a 2020  ,magenta,35`..  
-000014f0: 2020 2d20 5b2b 5d20 6063 7961 6e3a 6020    - [+] `cyan:` 
-00001500: 2020 2020 2020 2020 2020 2020 2020 6063                `c
-00001510: 2c63 7961 6e2c 3336 600d 0a20 2020 202d  ,cyan,36`..    -
-00001520: 205b 2b5d 2060 7768 6974 653a 6020 2020   [+] `white:`   
-00001530: 2020 2020 2020 2020 2020 2060 772c 7768             `w,wh
-00001540: 6974 652c 3337 600d 0a20 2020 202d 205b  ite,37`..    - [
-00001550: 2b5d 2060 6465 6661 756c 743a 6020 2020  +] `default:`   
-00001560: 2020 2020 2020 2020 2060 642c 6465 6661           `d,defa
-00001570: 756c 742c 3339 600d 0a20 2020 202d 205b  ult,39`..    - [
-00001580: 2b5d 2060 6272 6967 6874 2062 6c61 636b  +] `bright black
-00001590: 3a60 2020 2020 2020 2060 6262 2c62 626c  :`       `bb,bbl
-000015a0: 6163 6b2c 3930 600d 0a20 2020 202d 205b  ack,90`..    - [
-000015b0: 2b5d 2060 6272 6967 6874 2072 6564 3a60  +] `bright red:`
-000015c0: 2020 2020 2020 2020 2060 6272 2c62 7265           `br,bre
-000015d0: 642c 3931 600d 0a20 2020 202d 205b 2b5d  d,91`..    - [+]
-000015e0: 2060 6272 6967 6874 2067 7265 656e 3a60   `bright green:`
-000015f0: 2020 2020 2020 2060 6267 2c62 6772 6565         `bg,bgree
-00001600: 6e2c 3932 600d 0a20 2020 202d 205b 2b5d  n,92`..    - [+]
-00001610: 2060 6272 6967 6874 2079 656c 6c6f 773a   `bright yellow:
-00001620: 6020 2020 2020 2060 6279 2c62 7965 6c6c  `      `by,byell
-00001630: 6f77 2c39 3360 0d0a 2020 2020 2d20 5b2b  ow,93`..    - [+
-00001640: 5d20 6062 7269 6768 7420 626c 7565 3a60  ] `bright blue:`
-00001650: 2020 2020 2020 2020 6062 6c2c 6262 6c75          `bl,bblu
-00001660: 652c 3934 600d 0a20 2020 202d 205b 2b5d  e,94`..    - [+]
-00001670: 2060 6272 6967 6874 206d 6167 656e 7461   `bright magenta
-00001680: 6020 2020 2020 2060 626d 2c62 6d61 6765  `      `bm,bmage
-00001690: 6e74 612c 3935 600d 0a20 2020 202d 205b  nta,95`..    - [
-000016a0: 2b5d 2060 6272 6967 6874 2063 7961 6e3a  +] `bright cyan:
-000016b0: 6020 2020 2020 2020 2060 6263 2c62 6379  `        `bc,bcy
-000016c0: 616e 2c39 3660 0d0a 2020 2020 2d20 5b2b  an,96`..    - [+
-000016d0: 5d20 6062 7269 6768 7420 7768 6974 653a  ] `bright white:
-000016e0: 6020 2020 2020 2020 6062 772c 6277 6869  `       `bw,bwhi
-000016f0: 7465 2c39 3760 0d0a 2d20 2323 2323 2053  te,97`..- #### S
-00001700: 7479 6c65 733a 0d0a 2020 2020 2d20 5b2b  tyles:..    - [+
-00001710: 5d20 6062 6f6c 643a 6020 2020 2020 2020  ] `bold:`       
-00001720: 2020 2020 2020 2020 6042 2c62 6f6c 642c          `B,bold,
-00001730: 3160 0d0a 2020 2020 2d20 5b2b 5d20 6064  1`..    - [+] `d
-00001740: 696d 3a60 2020 2020 2020 2020 2020 2020  im:`            
-00001750: 2020 2020 6044 2c64 696d 2c32 600d 0a20      `D,dim,2`.. 
-00001760: 2020 202d 205b 2b5d 2060 6974 616c 6963     - [+] `italic
-00001770: 3a60 2020 2020 2020 2020 2020 2020 2060  :`             `
-00001780: 492c 6974 616c 6963 2c33 600d 0a20 2020  I,italic,3`..   
-00001790: 202d 205b 2b5d 2060 756e 6465 726c 696e   - [+] `underlin
-000017a0: 653a 6020 2020 2020 2020 2020 2060 552c  e:`          `U,
-000017b0: 756e 6465 726c 696e 652c 3460 0d0a 2020  underline,4`..  
-000017c0: 2020 2d20 5b2b 5d20 6062 6c69 6e6b 696e    - [+] `blinkin
-000017d0: 673a 6020 2020 2020 2020 2020 2020 604c  g:`           `L
-000017e0: 2c62 6c69 6e6b 696e 672c 3560 0d0a 2020  ,blinking,5`..  
-000017f0: 2020 2d20 5b2b 5d20 6072 6576 6572 7365    - [+] `reverse
-00001800: 3a60 2020 2020 2020 2020 2020 2020 6052  :`            `R
-00001810: 2c72 6576 6572 7365 2c37 600d 0a20 2020  ,reverse,7`..   
-00001820: 202d 205b 2b5d 2060 6869 6464 656e 3a60   - [+] `hidden:`
-00001830: 2020 2020 2020 2020 2020 2020 2060 482c               `H,
-00001840: 6869 6464 656e 2c38 600d 0a20 2020 202d  hidden,8`..    -
-00001850: 205b 2b5d 2060 7374 7269 6b65 7468 726f   [+] `strikethro
-00001860: 7567 683a 6020 2020 2020 2060 532c 7374  ugh:`      `S,st
-00001870: 7269 6b65 7468 726f 7567 682c 3960 0d0a  rikethrough,9`..
-00001880: 0d0a 2323 2045 7861 6d70 6c65 7320 2620  ..## Examples & 
-00001890: 5573 6167 650d 0a5f 5f5f 5f5f 5f5f 5f5f  Usage.._________
-000018a0: 5f5f 5f0d 0a3e 2054 6572 6d69 6e61 6c20  ___..> Terminal 
-000018b0: 4578 6563 7574 650d 0a23 2323 2077 696e  Execute..### win
-000018c0: 646f 7773 0d0a 6060 6073 6865 6c6c 0d0a  dows..```shell..
-000018d0: 7079 7468 6f6e 202d 6d20 414e 5349 436f  python -m ANSICo
-000018e0: 6e74 726f 6c6c 6572 0d0a 6060 600d 0a3e  ntroller..```..>
-000018f0: 204f 520d 0a60 6060 7368 656c 6c0d 0a61   OR..```shell..a
-00001900: 6e73 6963 6f6e 7472 6f6c 6c65 720d 0a60  nsicontroller..`
-00001910: 6060 0d0a 2323 2320 4c69 6e75 7820 2626  ``..### Linux &&
-00001920: 2054 6572 6d75 780d 0a60 6060 7368 656c   Termux..```shel
-00001930: 6c0d 0a70 7974 686f 6e33 202d 6d20 414e  l..python3 -m AN
-00001940: 5349 436f 6e74 726f 6c6c 6572 0d0a 6060  SIController..``
-00001950: 600d 0a3e 204f 520d 0a60 6060 7368 656c  `..> OR..```shel
-00001960: 6c0d 0a61 6e73 6963 6f6e 7472 6f6c 6c65  l..ansicontrolle
-00001970: 720d 0a60 6060 0d0a 3e20 5079 7468 6f6e  r..```..> Python
-00001980: 2043 6f64 650d 0a20 6060 6020 7079 7468   Code.. ``` pyth
-00001990: 6f6e 0d0a 6672 6f6d 2041 4e53 4943 6f6e  on..from ANSICon
-000019a0: 7472 6f6c 6c65 7220 696d 706f 7274 2054  troller import T
-000019b0: 6572 6d69 6e61 6c20 2023 2049 6d70 6f72  erminal  # Impor
-000019c0: 7420 4e65 6564 6564 2043 6c61 7373 0d0a  t Needed Class..
-000019d0: 7465 726d 696e 616c 5f63 6f6e 7472 6f6c  terminal_control
-000019e0: 203d 2054 6572 6d69 6e61 6c28 2920 2020   = Terminal()   
-000019f0: 2020 2020 2023 2043 7265 6174 6520 4f62       # Create Ob
-00001a00: 6a65 6374 2046 726f 6d20 436c 6173 7320  ject From Class 
-00001a10: 5465 726d 696e 616c 0d0a 6060 600d 0a3e  Terminal..```..>
-00001a20: 2054 6f20 7365 6520 616c 6c20 7465 7374   To see all test
-00001a30: 200d 0a60 6060 7079 7468 6f6e 0d0a 2320   ..```python..# 
-00001a40: 7072 696e 7420 616c 6c20 7374 796c 6573  print all styles
-00001a50: 2077 6974 6820 7465 7374 2065 7861 6d70   with test examp
-00001a60: 6c65 0d0a 5465 726d 696e 616c 2e70 7269  le..Terminal.pri
-00001a70: 6e74 5f73 7479 6c65 7328 290d 0a23 2070  nt_styles()..# p
-00001a80: 7269 6e74 2061 6c6c 2063 6f6c 6f72 7320  rint all colors 
-00001a90: 7769 7468 2074 6573 7420 6578 616d 706c  with test exampl
-00001aa0: 6520 666f 7220 6261 636b 6772 6f75 6e64  e for background
-00001ab0: 2074 6f6f 2061 6e64 2063 6f64 6573 0d0a   too and codes..
-00001ac0: 5465 726d 696e 616c 2e70 7269 6e74 5f63  Terminal.print_c
-00001ad0: 6f6c 6f72 7328 290d 0a23 2070 7269 6e74  olors()..# print
-00001ae0: 2061 6c6c 2063 6f6c 6f72 7320 2620 7374   all colors & st
-00001af0: 796c 6573 2077 6974 6820 636f 6465 730d  yles with codes.
-00001b00: 0a54 6572 6d69 6e61 6c2e 7072 696e 745f  .Terminal.print_
-00001b10: 636f 6c6f 7273 5f73 7479 6c65 7328 290d  colors_styles().
-00001b20: 0a23 2070 7269 6e74 2069 6473 2063 6f6c  .# print ids col
-00001b30: 6f72 7320 6261 636b 6772 6f75 6e64 2061  ors background a
-00001b40: 6e64 206e 6f72 6d61 6c20 6672 6f6d 2030  nd normal from 0
-00001b50: 2074 6f20 3235 350d 0a54 6572 6d69 6e61   to 255..Termina
-00001b60: 6c2e 7072 696e 745f 6964 5f63 6f6c 6f72  l.print_id_color
-00001b70: 7328 290d 0a23 2077 696c 6c20 7072 696e  s()..# will prin
-00001b80: 7420 616c 6c20 7065 7276 696f 7573 2069  t all pervious i
-00001b90: 6e20 7361 6d65 2074 696d 650d 0a54 6572  n same time..Ter
-00001ba0: 6d69 6e61 6c2e 7072 696e 745f 7465 7374  minal.print_test
-00001bb0: 2829 0d0a 2320 5472 7920 6974 0d0a 5465  ()..# Try it..Te
-00001bc0: 726d 696e 616c 2e67 616d 6528 290d 0a60  rminal.game()..`
-00001bd0: 6060 0d0a 2323 2320 746f 206d 6f76 6520  ``..### to move 
-00001be0: 6375 7273 6f72 0d0a 6060 6070 7974 686f  cursor..```pytho
-00001bf0: 6e0d 0a23 2074 6869 7320 7769 6c6c 206d  n..# this will m
-00001c00: 616b 6520 6375 7273 6f72 206d 6f76 6520  ake cursor move 
-00001c10: 746f 2075 7020 3320 6c69 6e65 730d 0a74  to up 3 lines..t
-00001c20: 6572 6d69 6e61 6c5f 636f 6e74 726f 6c2e  erminal_control.
-00001c30: 6d6f 7665 5f74 6f5f 7570 2873 7465 7073  move_to_up(steps
-00001c40: 3d33 2920 2020 200d 0a0d 0a23 2041 6674  =3)    ....# Aft
-00001c50: 6572 206d 6f76 6520 746f 2075 7020 3320  er move to up 3 
-00001c60: 6c69 6e65 7320 2c20 6375 7273 6f72 2077  lines , cursor w
-00001c70: 696c 6c20 7374 6172 7420 6672 6f6d 2030  ill start from 0
-00001c80: 2070 6f73 7469 6f6e 206f 6620 6c69 6e65   postion of line
-00001c90: 0d0a 7465 726d 696e 616c 5f63 6f6e 7472  ..terminal_contr
-00001ca0: 6f6c 2e6d 6f76 655f 746f 5f75 7028 7374  ol.move_to_up(st
-00001cb0: 6570 733d 332c 7374 6172 745f 6c69 6e65  eps=3,start_line
-00001cc0: 3d54 7275 6529 0d0a 0d0a 2320 7468 6973  =True)....# this
-00001cd0: 2077 696c 6c20 6d61 6b65 2063 7572 736f   will make curso
-00001ce0: 7220 6d6f 7665 2074 6f20 646f 776e 2031  r move to down 1
-00001cf0: 206c 696e 650d 0a74 6572 6d69 6e61 6c5f   line..terminal_
-00001d00: 636f 6e74 726f 6c2e 6d6f 7665 5f74 6f5f  control.move_to_
-00001d10: 646f 776e 2873 7465 7073 3d31 2920 200d  down(steps=1)  .
-00001d20: 0a0d 0a23 2073 6f6d 6574 696d 6573 2074  ...# sometimes t
-00001d30: 6572 6d69 6e61 6c20 6e6f 7420 6163 6365  erminal not acce
-00001d40: 7074 2074 6f20 6d6f 7665 2074 6f20 7570  pt to move to up
-00001d50: 2074 6869 7320 6675 6e63 7469 6f6e 2077   this function w
-00001d60: 696c 6c20 666f 7263 6520 7465 726d 696e  ill force termin
-00001d70: 616c 2074 6f20 6d6f 7665 2075 7020 3120  al to move up 1 
-00001d80: 6c69 6e65 0d0a 7465 726d 696e 616c 5f63  line..terminal_c
-00001d90: 6f6e 7472 6f6c 2e66 6f72 6365 5f6d 6f76  ontrol.force_mov
-00001da0: 655f 746f 5f75 7028 2920 0d0a 0d0a 2320  e_to_up() ....# 
-00001db0: 6d6f 7665 2063 7572 736f 7220 746f 2068  move cursor to h
-00001dc0: 6f6d 6520 706f 7374 696f 6e20 2c20 6d61  ome postion , ma
-00001dd0: 6b65 2063 7572 736f 7220 696e 2072 6f77  ke cursor in row
-00001de0: 2030 2061 6e64 2063 6f6c 2030 0d0a 7465   0 and col 0..te
-00001df0: 726d 696e 616c 5f63 6f6e 7472 6f6c 2e6d  rminal_control.m
-00001e00: 6f76 655f 746f 5f68 6f6d 655f 706f 7374  ove_to_home_post
-00001e10: 696f 6e28 290d 0a0d 0a23 206d 6f76 6520  ion()....# move 
-00001e20: 6375 7273 6f72 2074 6f20 6375 7374 6f6d  cursor to custom
-00001e30: 2070 6f73 7469 6f6e 2072 6f77 207b 6e75   postion row {nu
-00001e40: 6d7d 2063 6f6c 207b 6e75 6d7d 2069 6e20  m} col {num} in 
-00001e50: 7465 726d 696e 616c 2073 6372 6565 6e0d  terminal screen.
-00001e60: 0a23 2068 6572 6520 7468 6520 6375 7273  .# here the curs
-00001e70: 6f72 2077 696c 6c20 6d6f 7665 2074 6f20  or will move to 
-00001e80: 726f 7720 3134 202c 636f 6c75 6d6e 2032  row 14 ,column 2
-00001e90: 300d 0a74 6572 6d69 6e61 6c5f 636f 6e74  0..terminal_cont
-00001ea0: 726f 6c2e 6d6f 7665 5f74 6f5f 6c69 6e65  rol.move_to_line
-00001eb0: 2872 6f77 3d31 342c 636f 6c3d 3230 2920  (row=14,col=20) 
-00001ec0: 0d0a 6060 600d 0a23 2323 2074 6f20 6869  ..```..### to hi
-00001ed0: 6465 2063 7572 736f 720d 0a60 6060 7079  de cursor..```py
-00001ee0: 7468 6f6e 0d0a 2320 6869 6465 2063 7572  thon..# hide cur
-00001ef0: 736f 7220 2c20 7472 7920 6974 0d0a 7465  sor , try it..te
-00001f00: 726d 696e 616c 5f63 6f6e 7472 6f6c 2e68  rminal_control.h
-00001f10: 6964 655f 6375 7273 6f72 2829 0d0a 2320  ide_cursor()..# 
-00001f20: 7368 6f77 2063 7572 736f 7220 6966 2068  show cursor if h
-00001f30: 6964 6465 6e0d 0a74 6572 6d69 6e61 6c5f  idden..terminal_
-00001f40: 636f 6e74 726f 6c2e 7368 6f77 5f63 7572  control.show_cur
-00001f50: 736f 7228 290d 0a23 2073 686f 7720 6375  sor()..# show cu
-00001f60: 7273 6f72 2069 6620 6869 6464 656e 2061  rsor if hidden a
-00001f70: 6e64 2068 6964 6520 6966 2073 686f 7765  nd hide if showe
-00001f80: 6e0d 0a74 6572 6d69 6e61 6c5f 636f 6e74  n..terminal_cont
-00001f90: 726f 6c2e 746f 6767 6c65 5f63 7572 736f  rol.toggle_curso
-00001fa0: 7228 290d 0a60 6060 0d0a 2323 2320 546f  r()..```..### To
-00001fb0: 2073 6176 6520 6375 7273 6f72 2070 6f73   save cursor pos
-00001fc0: 7469 6f6e 206f 7220 7265 7374 6f72 6520  tion or restore 
-00001fd0: 6375 7273 726f 7220 706f 7374 696f 6e0d  cursror postion.
-00001fe0: 0a60 6060 7079 7468 6f6e 0d0a 7465 726d  .```python..term
-00001ff0: 696e 616c 5f63 6f6e 7472 6f6c 2e73 6176  inal_control.sav
-00002000: 655f 6375 7273 6f72 5f70 6f73 7469 6f6e  e_cursor_postion
-00002010: 2829 2020 2023 2053 6176 6520 4375 7272  ()   # Save Curr
-00002020: 656e 7420 4375 7273 6f72 2070 6f73 7469  ent Cursor posti
-00002030: 6f6e 2072 6f77 202c 2063 6f6c 756d 6e0d  on row , column.
-00002040: 0a23 2052 6573 746f 7265 204c 6173 7420  .# Restore Last 
-00002050: 5361 7665 6420 4375 7273 6f72 2070 6f73  Saved Cursor pos
-00002060: 7469 6f6e 0d0a 7465 726d 696e 616c 5f63  tion..terminal_c
-00002070: 6f6e 7472 6f6c 2e72 6573 746f 725f 6375  ontrol.restor_cu
-00002080: 7273 6f72 5f70 6f73 7469 6f6e 2829 2023  rsor_postion() #
-00002090: 2063 7572 736f 7220 7769 6c6c 206d 6f76   cursor will mov
-000020a0: 6520 6175 746f 2074 6f20 7361 7665 6420  e auto to saved 
-000020b0: 706f 7374 696f 6e0d 0a60 6060 0d0a 2323  postion..```..##
-000020c0: 2320 6c65 7473 2073 6179 2069 2077 616e  # lets say i wan
-000020d0: 7420 746f 2063 6c65 6172 2073 6f6d 6520  t to clear some 
-000020e0: 7465 7874 2066 726f 6d20 7465 726d 696e  text from termin
-000020f0: 616c 2060 5c72 206e 6f60 0d0a 6060 6070  al `\r no`..```p
-00002100: 7974 686f 6e0d 0a74 6572 6d69 6e61 6c5f  ython..terminal_
-00002110: 636f 6e74 726f 6c2e 636c 6561 725f 7363  control.clear_sc
-00002120: 7265 656e 2829 2020 2020 2020 2020 2020  reen()          
-00002130: 2020 2023 2043 6c65 6172 2054 6572 6d69     # Clear Termi
-00002140: 6e61 6c20 5363 7265 656e 2069 7420 636c  nal Screen it cl
-00002150: 6f73 6520 746f 2063 6f6d 6d61 6e64 2060  ose to command `
-00002160: 636c 7360 2061 6e64 2060 636c 6561 7260  cls` and `clear`
-00002170: 0d0a 7465 726d 696e 616c 5f63 6f6e 7472  ..terminal_contr
-00002180: 6f6c 2e63 6c65 6172 5f61 6674 6572 5f63  ol.clear_after_c
-00002190: 7572 736f 7228 2920 2020 2020 2020 2320  ursor()       # 
-000021a0: 436c 6561 7220 5465 726d 696e 616c 2053  Clear Terminal S
-000021b0: 6372 6565 6e20 616c 6c20 7465 7874 2061  creen all text a
-000021c0: 6674 6572 2063 7572 736f 7220 706f 7374  fter cursor post
-000021d0: 696f 6e0d 0a74 6572 6d69 6e61 6c5f 636f  ion..terminal_co
-000021e0: 6e74 726f 6c2e 636c 6561 725f 6265 666f  ntrol.clear_befo
-000021f0: 7265 5f63 7572 736f 7228 2920 2020 2020  re_cursor()     
-00002200: 2023 2043 6c65 6172 2054 6572 6d69 6e61   # Clear Termina
-00002210: 6c20 5363 7265 656e 2061 6c6c 2074 6578  l Screen all tex
-00002220: 7420 6166 7465 7220 6375 7273 6f72 2070  t after cursor p
-00002230: 6f73 7469 6f6e 0d0a 7465 726d 696e 616c  ostion..terminal
-00002240: 5f63 6f6e 7472 6f6c 2e63 6c65 6172 5f6c  _control.clear_l
-00002250: 696e 6528 2920 2020 2020 2020 2020 2020  ine()           
-00002260: 2020 2020 2320 436c 6561 7220 4375 7272      # Clear Curr
-00002270: 656e 7420 6c69 6e65 2c20 6f66 2063 7572  ent line, of cur
-00002280: 736f 7220 706f 7374 696f 6e20 726f 7720  sor postion row 
-00002290: 616e 6420 7374 6172 7420 6672 6f6d 2066  and start from f
-000022a0: 6972 7374 206c 696e 650d 0a74 6572 6d69  irst line..termi
-000022b0: 6e61 6c5f 636f 6e74 726f 6c2e 636c 6561  nal_control.clea
-000022c0: 725f 6c69 6e65 5f61 6674 6572 5f63 7572  r_line_after_cur
-000022d0: 736f 7228 2920 2023 2043 6c65 6172 2043  sor()  # Clear C
-000022e0: 7572 7265 6e74 206c 696e 652c 2061 6c6c  urrent line, all
-000022f0: 2074 6578 7420 6166 7465 7220 6375 7273   text after curs
-00002300: 6f72 2070 6f73 7469 6f6e 2069 6e20 7361  or postion in sa
-00002310: 6d65 206c 696e 650d 0a74 6572 6d69 6e61  me line..termina
-00002320: 6c5f 636f 6e74 726f 6c2e 636c 6561 725f  l_control.clear_
-00002330: 6c69 6e65 5f62 6566 6f72 655f 6375 7273  line_before_curs
-00002340: 6f72 2829 2023 2043 6c65 6172 2043 7572  or() # Clear Cur
-00002350: 7265 6e74 206c 696e 652c 2061 6c6c 2074  rent line, all t
-00002360: 6578 7420 6265 666f 7265 2063 7572 736f  ext before curso
-00002370: 7220 706f 7374 696f 6e20 696e 2073 616d  r postion in sam
-00002380: 6520 6c69 6e65 0d0a 6060 600d 0a23 2323  e line..```..###
-00002390: 206c 6574 7320 7361 7920 6920 7761 6e74   lets say i want
-000023a0: 2074 6f20 636f 6c6f 7269 7a65 2073 6f6d   to colorize som
-000023b0: 6520 7465 7874 0d0a 6042 7920 5573 696e  e text..`By Usin
-000023c0: 6720 436f 6e63 6570 7420 6f66 202d 2054  g Concept of - T
-000023d0: 6162 6c65 206f 6620 636f 6c6f 7273 2026  able of colors &
-000023e0: 2073 7479 6c65 600d 0a3e 2055 7369 6e67   style`..> Using
-000023f0: 2043 6f6c 6f72 7320 6f6e 6c79 206e 6f20   Colors only no 
-00002400: 7374 796c 6573 206f 7220 6261 636b 6772  styles or backgr
-00002410: 6f75 6e64 0d0a 3e20 436f 6c6f 7269 7a65  ound..> Colorize
-00002420: 2066 756e 6374 696f 6e20 7461 6b65 203a   function take :
-00002430: 2074 6578 7420 616e 6420 7365 7072 6174   text and seprat
-00002440: 6f72 0d0a 3e20 0d0a 3e20 7379 6e74 6178  or..> ..> syntax
-00002450: 3a0d 0a3e 200d 0a3e 2060 7365 7020 736f  :..> ..> `sep so
-00002460: 6d65 5f73 7479 6c65 5f63 6f64 6573 5f6f  me_style_codes_o
-00002470: 725f 636f 6c6f 725f 636f 6465 2073 6570  r_color_code sep
-00002480: 600d 0a3e 200d 0a3e 2066 6f72 2065 7861  `..> ..> for exa
-00002490: 6d70 6c65 2060 7365 7020 6973 205b 5d60  mple `sep is []`
-000024a0: 0d0a 3e20 0d0a 3e20 7379 6e74 6178 2077  ..> ..> syntax w
-000024b0: 696c 6c20 6265 3a20 2060 5b73 6f6d 655f  ill be:  `[some_
-000024c0: 7374 796c 655f 636f 6465 735f 6f72 5f63  style_codes_or_c
-000024d0: 6f6c 6f72 5f63 6f64 655d 600d 0a3e 200d  olor_code]`..> .
-000024e0: 0a60 6060 7079 7468 6f6e 0d0a 7365 7020  .```python..sep 
-000024f0: 3d20 225b 5d22 0d0a 636f 6c6f 7269 7a65  = "[]"..colorize
-00002500: 5f74 6578 7473 5f75 7369 6e67 5f63 6f6c  _texts_using_col
-00002510: 6f72 5f63 6861 7220 3d20 5b0d 0a20 2020  or_char = [..   
-00002520: 2022 5b72 5d54 6869 7320 6973 2052 6564   "[r]This is Red
-00002530: 5b30 5d22 2c0d 0a20 2020 2022 5b67 5d54  [0]",..    "[g]T
-00002540: 6869 7320 6973 2047 7265 656e 5b30 5d22  his is Green[0]"
-00002550: 2c0d 0a20 2020 2022 5b79 5d54 6869 7320  ,..    "[y]This 
-00002560: 6973 2059 656c 6c6f 775b 305d 222c 0d0a  is Yellow[0]",..
-00002570: 2020 2020 225b 625d 5468 6973 2069 7320      "[b]This is 
-00002580: 426c 6163 6b5b 305d 222c 0d0a 2020 2020  Black[0]",..    
-00002590: 225b 6c5d 5468 6973 2069 7320 426c 7565  "[l]This is Blue
-000025a0: 5b30 5d22 2c0d 0a20 2020 2022 5b6d 5d54  [0]",..    "[m]T
-000025b0: 6869 7320 6973 204d 6567 656e 7461 5b30  his is Megenta[0
-000025c0: 5d22 2c0d 0a20 2020 2022 5b63 5d54 6869  ]",..    "[c]Thi
-000025d0: 7320 6973 2043 7961 6e5b 305d 222c 0d0a  s is Cyan[0]",..
-000025e0: 2020 2020 225b 775d 5468 6973 2069 7320      "[w]This is 
-000025f0: 5768 6974 655b 305d 222c 0d0a 2020 2020  White[0]",..    
-00002600: 225b 645d 5468 6973 2069 7320 6465 6661  "[d]This is defa
-00002610: 756c 745b 305d 222c 0d0a 2020 2020 225b  ult[0]",..    "[
-00002620: 6262 5d54 6869 7320 6973 2042 7269 6768  bb]This is Brigh
-00002630: 7420 426c 6163 6b5b 305d 222c 0d0a 2020  t Black[0]",..  
-00002640: 2020 225b 6272 5d54 6869 7320 6973 2042    "[br]This is B
-00002650: 7269 6768 7420 5265 645b 305d 222c 0d0a  right Red[0]",..
-00002660: 5d0d 0a66 6f72 2074 6578 7420 696e 2063  ]..for text in c
-00002670: 6f6c 6f72 697a 655f 7465 7874 735f 7573  olorize_texts_us
-00002680: 696e 675f 636f 6c6f 725f 6368 6172 3a0d  ing_color_char:.
-00002690: 0a20 2020 2070 7269 6e74 2874 6572 6d69  .    print(termi
-000026a0: 6e61 6c5f 636f 6e74 726f 6c2e 636f 6c6f  nal_control.colo
-000026b0: 7269 7a65 2874 6578 742c 7365 7029 290d  rize(text,sep)).
-000026c0: 0a60 6060 0d0a 3e20 4e6f 7720 5573 696e  .```..> Now Usin
-000026d0: 6720 7374 796c 6520 6f6e 6c79 0d0a 3e20  g style only..> 
-000026e0: 0d0a 6060 6070 7974 686f 6e0d 0a73 6570  ..```python..sep
-000026f0: 203d 2022 5b5d 220d 0a63 6f6c 6f72 697a   = "[]"..coloriz
-00002700: 655f 7465 7874 735f 7573 696e 675f 7374  e_texts_using_st
-00002710: 796c 655f 6368 6172 203d 205b 0d0a 2020  yle_char = [..  
-00002720: 2020 225b 425d 5468 6973 2069 7320 426f    "[B]This is Bo
-00002730: 6c64 5b30 5d22 2c0d 0a20 2020 2022 5b44  ld[0]",..    "[D
-00002740: 5d54 6869 7320 6973 2044 696d 5b30 5d22  ]This is Dim[0]"
-00002750: 2c0d 0a20 2020 2022 5b49 5d54 6869 7320  ,..    "[I]This 
-00002760: 6973 2049 7461 6c69 635b 305d 222c 0d0a  is Italic[0]",..
-00002770: 2020 2020 225b 555d 5468 6973 2069 7320      "[U]This is 
-00002780: 556e 6465 726c 696e 655b 305d 222c 0d0a  Underline[0]",..
-00002790: 2020 2020 225b 4c5d 5468 6973 2069 7320      "[L]This is 
-000027a0: 426c 696e 6b69 6e67 5b30 5d22 2c0d 0a20  Blinking[0]",.. 
-000027b0: 2020 2022 5b52 5d54 6869 7320 6973 2072     "[R]This is r
-000027c0: 6576 6572 7365 5b30 5d22 2c0d 0a20 2020  everse[0]",..   
-000027d0: 2022 5b48 5d54 6869 7320 6973 2048 6964   "[H]This is Hid
-000027e0: 6465 6e5b 305d 222c 0d0a 2020 2020 225b  den[0]",..    "[
-000027f0: 535d 5468 6973 2069 7320 5374 7269 6b65  S]This is Strike
-00002800: 7468 726f 6768 5b30 5d22 2c0d 0a5d 0d0a  throgh[0]",..]..
-00002810: 666f 7220 7465 7874 2069 6e20 636f 6c6f  for text in colo
-00002820: 7269 7a65 5f74 6578 7473 5f75 7369 6e67  rize_texts_using
-00002830: 5f73 7479 6c65 5f63 6861 723a 0d0a 2020  _style_char:..  
-00002840: 2020 7072 696e 7428 7465 726d 696e 616c    print(terminal
-00002850: 5f63 6f6e 7472 6f6c 2e63 6f6c 6f72 697a  _control.coloriz
-00002860: 6528 7465 7874 2c73 6570 2929 0d0a 6060  e(text,sep))..``
-00002870: 600d 0a3e 204e 6f77 2055 7369 6e67 2043  `..> Now Using C
-00002880: 6f6c 6f72 7320 2620 7374 796c 650d 0a3e  olors & style..>
-00002890: 200d 0a60 6060 7079 7468 6f6e 0d0a 7365   ..```python..se
-000028a0: 7020 3d20 225b 5d22 0d0a 636f 6c6f 7269  p = "[]"..colori
-000028b0: 7a65 5f74 6578 7473 5f75 7369 6e67 5f73  ze_texts_using_s
-000028c0: 7479 6c65 5f63 6f6c 6f72 5f63 6861 7220  tyle_color_char 
-000028d0: 3d20 5b0d 0a20 2020 2022 5b42 725d 5468  = [..    "[Br]Th
-000028e0: 6973 2069 7320 426f 6c64 2061 6e64 2052  is is Bold and R
-000028f0: 6564 5b30 5d22 2c0d 0a20 2020 2022 5b44  ed[0]",..    "[D
-00002900: 795d 5468 6973 2069 7320 4469 6d20 616e  y]This is Dim an
-00002910: 6420 5965 6c6c 6f77 5b30 5d22 2c0d 0a20  d Yellow[0]",.. 
-00002920: 2020 2022 5b49 6c5d 5468 6973 2069 7320     "[Il]This is 
-00002930: 4974 616c 6963 2061 6e64 2042 6c75 655b  Italic and Blue[
-00002940: 305d 222c 0d0a 2020 2020 225b 5567 5d54  0]",..    "[Ug]T
-00002950: 6869 7320 6973 2055 6e64 6572 6c69 6e65  his is Underline
-00002960: 2061 6e64 2047 7265 656e 5b30 5d22 2c0d   and Green[0]",.
-00002970: 0a20 2020 2022 5b4c 625d 5468 6973 2069  .    "[Lb]This i
-00002980: 7320 426c 696e 6b69 6e67 2061 6e64 2062  s Blinking and b
-00002990: 6c61 636b 5b30 5d22 2c0d 0a20 2020 2022  lack[0]",..    "
-000029a0: 5b52 6272 5d54 6869 7320 6973 2072 6576  [Rbr]This is rev
-000029b0: 6572 7365 2061 6e64 2042 7269 6768 7420  erse and Bright 
-000029c0: 5265 645b 305d 222c 0d0a 2020 2020 225b  Red[0]",..    "[
-000029d0: 4862 795d 5468 6973 2069 7320 4869 6464  Hby]This is Hidd
-000029e0: 656e 2061 6e64 2042 7269 6768 7420 5965  en and Bright Ye
-000029f0: 6c6c 6f77 5b30 5d22 2c0d 0a20 2020 2022  llow[0]",..    "
-00002a00: 5b53 6263 5d54 6869 7320 6973 2053 7472  [Sbc]This is Str
-00002a10: 696b 6574 6872 6f67 6820 616e 6420 4272  ikethrogh and Br
-00002a20: 6967 6874 2043 7961 6e5b 305d 222c 0d0a  ight Cyan[0]",..
-00002a30: 5d0d 0a66 6f72 2074 6578 7420 696e 2063  ]..for text in c
-00002a40: 6f6c 6f72 697a 655f 7465 7874 735f 7573  olorize_texts_us
-00002a50: 696e 675f 7374 796c 655f 636f 6c6f 725f  ing_style_color_
-00002a60: 6368 6172 3a0d 0a20 2020 2070 7269 6e74  char:..    print
-00002a70: 2874 6572 6d69 6e61 6c5f 636f 6e74 726f  (terminal_contro
-00002a80: 6c2e 636f 6c6f 7269 7a65 2874 6578 742c  l.colorize(text,
-00002a90: 7365 7029 290d 0a60 6060 0d0a 3e20 546f  sep))..```..> To
-00002aa0: 2061 6464 2042 6163 6b67 726f 756e 6420   add Background 
-00002ab0: 206a 7573 7420 6164 6420 6058 2c78 6020   just add `X,x` 
-00002ac0: 746f 2074 6865 2062 6c6f 636b 2060 5b78  to the block `[x
-00002ad0: 7242 5d60 2069 2077 616e 7420 6261 636b  rB]` i want back
-00002ae0: 6772 6f75 6e64 2072 6564 2061 6e64 2062  ground red and b
-00002af0: 6f6c 6420 7374 796c 650d 0a3e 200d 0a3e  old style..> ..>
-00002b00: 204e 6f74 653a 2079 6f75 2063 616e 2075   Note: you can u
-00002b10: 7365 2060 7465 726d 696e 616c 5f63 6f6e  se `terminal_con
-00002b20: 7472 6f6c 2e70 7269 6e74 5f63 6f6c 6f72  trol.print_color
-00002b30: 697a 6560 2077 6974 686f 7574 2070 7269  ize` without pri
-00002b40: 6e74 0d0a 3e20 0d0a 3e20 605b 305d 2c5b  nt..> ..> `[0],[
-00002b50: 7a5d 2c5b 5a5d 2c5b 5265 7365 745d 6020  z],[Z],[Reset]` 
-00002b60: 6973 2074 6f20 7265 7365 7420 746f 2064  is to reset to d
-00002b70: 6566 6175 6c74 2063 6f6c 6f72 2673 7479  efault color&sty
-00002b80: 6c65 2069 6e20 7465 726d 696e 616c 0d0a  le in terminal..
-00002b90: 0d0a 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ..______________
-00002ba0: 5f5f 0d0a 2323 2054 6573 7473 0d0a 2a20  __..## Tests..* 
-00002bb0: e29c 8520 6057 696e 646f 7773 2031 3120  ... `Windows 11 
-00002bc0: 2620 3130 2026 2037 600d 0a20 202a 2077  & 10 & 7`..  * w
-00002bd0: 6f72 6b20 7769 7468 206e 6f20 6973 7375  ork with no issu
-00002be0: 650d 0a2a 20f0 9f91 8d20 604c 696e 7578  e..* .... `Linux
-00002bf0: 600d 0a20 202a 2077 6f72 6b20 6275 7420  `..  * work but 
-00002c00: 2c20 6d61 7962 6520 6973 7375 6520 6170  , maybe issue ap
-00002c10: 7065 6172 0d0a 2020 2a20 5374 696c 6c20  pear..  * Still 
-00002c20: 576f 726b 206f 6e20 6974 0d0a 2a20 f09f  Work on it..* ..
-00002c30: 94a7 2060 5465 726d 7578 600d 0a20 202a  .. `Termux`..  *
-00002c40: 2053 6f6d 6520 4665 6174 7572 6573 204e   Some Features N
-00002c50: 6565 6420 526f 6f74 6564 2044 6576 6963  eed Rooted Devic
-00002c60: 650d 0a20 202a 2053 7469 6c6c 2057 6f72  e..  * Still Wor
-00002c70: 6b20 6f6e 2069 740d 0a5f 5f5f 5f5f 5f5f  k on it.._______
-00002c80: 5f5f 5f5f 5f5f 5f5f 5f0d 0a23 2323 2060  _________..### `
-00002c90: 6966 2075 2066 6163 6520 616e 7920 6973  if u face any is
-00002ca0: 7375 6520 646f 6e74 2062 6520 7368 7920  sue dont be shy 
-00002cb0: 2c20 7361 7920 6974 600d 0a23 2320 4c69  , say it`..## Li
-00002cc0: 6365 6e73 650d 0a0d 0a2a 2a4d 4954 2a2a  cense....**MIT**
-00002cd0: 0d0a 2a2a 436f 7079 7269 6768 7420 2863  ..**Copyright (c
-00002ce0: 2920 3230 3233 205b 4a6f 4f78 3031 5d2a  ) 2023 [JoOx01]*
-00002cf0: 2a0d 0a0d 0a                             *....
+00000740: 2020 2020 2020 2020 2020 0d0a 6060 600d            ..```.
+00000750: 0a23 2041 4e53 4920 436f 6e74 726f 6c6c  .# ANSI Controll
+00000760: 6572 0d0a 3e20 4261 7369 6320 5079 7468  er..> Basic Pyth
+00000770: 6f6e 2053 6372 6970 7420 746f 2063 6f6e  on Script to con
+00000780: 7472 6f6c 2063 7572 736f 7220 706f 7374  trol cursor post
+00000790: 696f 6e20 696e 2074 6572 6d69 6e61 6c0d  ion in terminal.
+000007a0: 0a3e 2061 6e64 2063 6f6c 6f72 697a 6520  .> and colorize 
+000007b0: 616e 7920 7465 7874 2069 6e20 7465 726d  any text in term
+000007c0: 696e 616c 202c 2061 6e64 2061 6464 2061  inal , and add a
+000007d0: 6e79 2073 7479 6c65 2074 6f20 6772 6170  ny style to grap
+000007e0: 6869 6320 6d6f 6465 2069 6e20 7465 726d  hic mode in term
+000007f0: 696e 616c 0d0a 3c64 6976 2073 7479 6c65  inal..<div style
+00000800: 3d22 0d0a 2020 2020 636f 6c6f 723a 2077  ="..    color: w
+00000810: 6869 7465 3b0d 0a20 2020 2062 6163 6b67  hite;..    backg
+00000820: 726f 756e 642d 636f 6c6f 723a 2023 3842  round-color: #8B
+00000830: 3030 3030 3b0d 0a20 2020 2070 6164 6469  0000;..    paddi
+00000840: 6e67 3a20 3130 7078 3b0d 0a20 2020 2061  ng: 10px;..    a
+00000850: 6c69 676e 6d65 6e74 3a20 6365 6e74 6572  lignment: center
+00000860: 3b0d 0a20 2020 2074 6578 742d 616c 6967  ;..    text-alig
+00000870: 6e3a 2063 656e 7465 723b 0d0a 223e 0d0a  n: center;..">..
+00000880: 3c62 3e4e 6f74 653c 2f62 3e3c 6272 3e0d  <b>Note</b><br>.
+00000890: 0a21 2054 6869 7320 4d6f 6475 6c65 2077  .! This Module w
+000008a0: 6f72 6b20 4465 7065 6e64 7320 6f66 2054  ork Depends of T
+000008b0: 6572 6d69 6e61 6c20 5479 7065 206f 6620  erminal Type of 
+000008c0: 7375 7070 6f72 7420 414e 5349 2065 7363  support ANSI esc
+000008d0: 6170 6520 6368 6172 6163 7465 7273 206f  ape characters o
+000008e0: 7220 6e6f 7420 210d 0a3c 6872 3e0d 0a69  r not !..<hr>..i
+000008f0: 6620 7520 6661 6365 2061 6e79 2069 7373  f u face any iss
+00000900: 7565 2077 7269 7465 2069 740d 0a3c 2f64  ue write it..</d
+00000910: 6976 3e0d 0a3c 6272 3e0d 0a0d 0a5b 215b  iv>..<br>....[![
+00000920: 5079 5069 5d28 6874 7470 733a 2f2f 696d  PyPi](https://im
+00000930: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000940: 6765 2f2d 5079 5069 2d62 6c75 652e 7376  ge/-PyPi-blue.sv
+00000950: 673f 6c6f 676f 3d70 7970 6926 6c61 6265  g?logo=pypi&labe
+00000960: 6c43 6f6c 6f72 3d35 3535 3535 3526 7374  lColor=555555&st
+00000970: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00000980: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
+00000990: 2e6f 7267 2f70 726f 6a65 6374 2f41 4e53  .org/project/ANS
+000009a0: 4943 6f6e 7472 6f6c 6c65 7220 2250 7950  IController "PyP
+000009b0: 6922 2920 5b21 5b4c 6963 656e 7365 3a20  i") [![License: 
+000009c0: 6c69 6365 6e73 655d 2868 7474 7073 3a2f  license](https:/
+000009d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000009e0: 6261 6467 652f 2d6c 6963 656e 7365 2d62  badge/-license-b
+000009f0: 6c75 652e 7376 673f 7374 796c 653d 666f  lue.svg?style=fo
+00000a00: 722d 7468 652d 6261 6467 6529 5d28 4c49  r-the-badge)](LI
+00000a10: 4345 4e53 4520 224c 6963 656e 7365 2229  CENSE "License")
+00000a20: 0d0a 0d0a 5b4d 6f72 6520 496e 666f 2041  ....[More Info A
+00000a30: 626f 7574 2041 4e53 4920 4573 6361 7065  bout ANSI Escape
+00000a40: 2043 6f64 6573 5d28 6068 7474 7073 3a2f   Codes](`https:/
+00000a50: 2f67 6973 742e 6769 7468 7562 2e63 6f6d  /gist.github.com
+00000a60: 2f66 6e6b 792f 3435 3837 3139 3334 3361  /fnky/458719343a
+00000a70: 6162 6430 3163 6662 3137 6133 6134 6637  abd01cfb17a3a4f7
+00000a80: 3239 3637 3937 2365 7363 6170 6560 290d  296797#escape`).
+00000a90: 0a0d 0a23 2320 546f 6f6c 2053 6e61 700d  ...## Tool Snap.
+00000aa0: 0a5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ._______________
+00000ab0: 0d0a 215b 416c 7420 5465 7874 5d28 6874  ..![Alt Text](ht
+00000ac0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000ad0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000ae0: 4a6f 3058 3031 2f41 4e53 4943 6f6e 7472  Jo0X01/ANSIContr
+00000af0: 6f6c 6c65 722f 6d61 696e 2f74 6573 7473  oller/main/tests
+00000b00: 2f74 6f6f 6c2e 706e 6729 0d0a 0d0a 2323  /tool.png)....##
+00000b10: 2046 6561 7475 7265 730d 0a2d 2d2d 2d2d   Features..-----
+00000b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b30: 2d2d 2d2d 2d2d 2d2d 2d0d 0a60 414e 5349  ---------..`ANSI
+00000b40: 2043 6f6e 7472 6f6c 6c65 7260 2046 6561   Controller` Fea
+00000b50: 7475 7265 733a 0d0a 2d20 4d6f 7665 2043  tures:..- Move C
+00000b60: 7572 736f 7220 5269 6768 7420 6f72 206c  ursor Right or l
+00000b70: 6566 7420 6f72 2074 6f70 206f 7220 646f  eft or top or do
+00000b80: 776e 206f 7220 706f 7374 696f 6e20 696e  wn or postion in
+00000b90: 2074 6572 6d69 6e61 6c20 7363 7265 656e   terminal screen
+00000ba0: 0d0a 2d20 436f 6c6f 7269 7a65 2061 6e79  ..- Colorize any
+00000bb0: 2074 6578 7420 7520 7761 6e74 2069 6e20   text u want in 
+00000bc0: 7465 726d 696e 616c 0d0a 2d20 4368 616e  terminal..- Chan
+00000bd0: 6765 2053 7479 6c65 206f 6620 7465 726d  ge Style of term
+00000be0: 696e 616c 2070 7269 6e74 696e 6720 7465  inal printing te
+00000bf0: 7874 202c 2062 6f6c 6420 2c69 7461 6c69  xt , bold ,itali
+00000c00: 6320 2c20 6574 632e 2e2e 0d0a 2d20 4d75  c , etc.....- Mu
+00000c10: 6c74 6950 726f 6772 6573 7320 696e 2073  ltiProgress in s
+00000c20: 616d 6520 7469 6d65 0d0a 2323 2054 6563  ame time..## Tec
+00000c30: 680d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  h..-------------
+00000c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000c50: 2d0d 0a60 414e 5349 2043 6f6e 7472 6f6c  -..`ANSI Control
+00000c60: 6c65 7260 2075 7365 7320 6120 6e75 6d62  ler` uses a numb
+00000c70: 6572 206f 6620 6f70 656e 2073 6f75 7263  er of open sourc
+00000c80: 6520 7072 6f6a 6563 7473 2074 6f20 776f  e projects to wo
+00000c90: 726b 2070 726f 7065 726c 793a 0d0a 2d20  rk properly:..- 
+00000ca0: 5b6b 6579 626f 6172 645d 202d 2070 7970  [keyboard] - pyp
+00000cb0: 6920 6d6f 6475 6c65 2060 6874 7470 733a  i module `https:
+00000cc0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000cd0: 6374 2f6b 6579 626f 6172 642f 600d 0a2d  ct/keyboard/`..-
+00000ce0: 2060 414e 5349 2043 6f6e 7472 6f6c 6c65   `ANSI Controlle
+00000cf0: 7260 2069 7473 656c 6620 6973 206f 7065  r` itself is ope
+00000d00: 6e20 736f 7572 6365 206f 6e20 4769 7448  n source on GitH
+00000d10: 7562 2e0d 0a2d 2060 4d6f 7265 2049 6e66  ub...- `More Inf
+00000d20: 6f20 4162 6f75 7420 414e 5349 2045 7363  o About ANSI Esc
+00000d30: 6170 6520 436f 6465 733a 2060 6874 7470  ape Codes: `http
+00000d40: 733a 2f2f 6769 7374 2e67 6974 6875 622e  s://gist.github.
+00000d50: 636f 6d2f 666e 6b79 2f34 3538 3731 3933  com/fnky/4587193
+00000d60: 3433 6161 6264 3031 6366 6231 3761 3361  43aabd01cfb17a3a
+00000d70: 3466 3732 3936 3739 3723 6573 6361 7065  4f7296797#escape
+00000d80: 0d0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000d90: 6e0d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  n..-------------
+00000da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000db0: 2d0d 0a0d 0a60 414e 5349 2043 6f6e 7472  -....`ANSI Contr
+00000dc0: 6f6c 6c65 7260 2072 6571 7569 7265 7320  oller` requires 
+00000dd0: 5b70 6970 5d28 6874 7470 733a 2f2f 7079  [pip](https://py
+00000de0: 7069 2e6f 7267 2f29 2074 6f20 696e 7374  pi.org/) to inst
+00000df0: 616c 6c2e 0d0a 496e 7374 616c 6c20 7468  all...Install th
+00000e00: 6520 6465 7065 6e64 656e 6369 6573 2061  e dependencies a
+00000e10: 6e64 2064 6576 4465 7065 6e64 656e 6369  nd devDependenci
+00000e20: 6573 2061 6e64 2073 7461 7274 2074 6865  es and start the
+00000e30: 2073 6372 6970 742e 0d0a 2323 2320 5769   script...### Wi
+00000e40: 6e64 6f77 730d 0a60 6060 6261 7368 0d0a  ndows..```bash..
+00000e50: 7069 7020 696e 7374 616c 6c20 414e 5349  pip install ANSI
+00000e60: 436f 6e74 726f 6c6c 6572 0d0a 6060 600d  Controller..```.
+00000e70: 0a23 2323 204c 696e 7578 2026 2620 5465  .### Linux && Te
+00000e80: 726d 7578 0d0a 6060 6062 6173 680d 0a70  rmux..```bash..p
+00000e90: 6970 3320 696e 7374 616c 6c20 414e 5349  ip3 install ANSI
+00000ea0: 436f 6e74 726f 6c6c 6572 0d0a 6060 600d  Controller..```.
+00000eb0: 0a23 2054 6162 6c65 206f 6620 636f 6c6f  .# Table of colo
+00000ec0: 7273 2026 2073 7479 6c65 0d0a 2d20 2323  rs & style..- ##
+00000ed0: 2323 2069 6620 7465 726d 696e 616c 206e  ## if terminal n
+00000ee0: 6f74 2073 7570 706f 7274 2063 6f6c 6f72  ot support color
+00000ef0: 697a 6520 7468 6520 7374 7269 6e67 2077  ize the string w
+00000f00: 696c 6c20 6a75 7374 2072 656d 6f76 6520  ill just remove 
+00000f10: 6672 6f6d 2073 7472 696e 670d 0a2d 2023  from string..- #
+00000f20: 2323 204e 6f74 653a 2041 6464 2043 7573  ## Note: Add Cus
+00000f30: 746f 6d20 5661 6c75 6573 2c20 746f 2073  tom Values, to s
+00000f40: 7472 696e 6720 746f 2063 6f6c 6f72 697a  tring to coloriz
+00000f50: 6520 7468 6520 6f75 7470 7574 0d0a 2d20  e the output..- 
+00000f60: 2323 2323 2049 442d 2d2d 2d2d 2d2d 2d2d  #### ID---------
+00000f70: 2d3a 2060 3c7b 6964 7d3e 6020 2066 726f  -: `<{id}>`  fro
+00000f80: 6d20 3020 746f 2032 3535 202c 2060 3c32  m 0 to 255 , `<2
+00000f90: 3535 3e60 202c 2060 3c31 353e 600d 0a2d  55>` , `<15>`..-
+00000fa0: 2023 2323 2320 5247 422d 2d2d 2d2d 2d2d   #### RGB-------
+00000fb0: 2d2d 3a20 6028 7265 645f 7661 6c75 652c  --: `(red_value,
+00000fc0: 6772 6565 6e5f 7661 6c75 652c 626c 7565  green_value,blue
+00000fd0: 5f76 616c 7565 2960 2066 726f 6d20 3020  _value)` from 0 
+00000fe0: 746f 2032 3535 2020 2c20 6028 3231 332c  to 255  , `(213,
+00000ff0: 3230 312c 3235 3029 600d 0a2d 2023 2323  201,250)`..- ###
+00001000: 2320 5247 422d 2d2d 2d2d 2d2d 2d2d 3a20  # RGB---------: 
+00001010: 6023 4646 4646 4646 6020 7573 696e 6720  `#FFFFFF` using 
+00001020: 6865 7820 2c20 6023 3461 6666 6131 600d  hex , `#4affa1`.
+00001030: 0a2d 2023 2323 2320 4261 636b 6772 6f75  .- #### Backgrou
+00001040: 6e64 2d2d 3a20 6058 2c78 600d 0a2d 2023  nd--: `X,x`..- #
+00001050: 2323 2320 5265 7365 742d 2d2d 2d2d 2d2d  ### Reset-------
+00001060: 3a20 605a 2c30 2c72 6573 6574 2c52 6573  : `Z,0,reset,Res
+00001070: 6574 600d 0a2d 2023 2323 2320 436f 6c6f  et`..- #### Colo
+00001080: 7273 3a0d 0a20 2020 202d 205b 2b5d 2060  rs:..    - [+] `
+00001090: 626c 6163 6b3a 6020 2020 2020 2020 2020  black:`         
+000010a0: 2020 2020 2060 622c 626c 6163 6b2c 3330       `b,black,30
+000010b0: 600d 0a20 2020 202d 205b 2b5d 2060 7265  `..    - [+] `re
+000010c0: 643a 6020 2020 2020 2020 2020 2020 2020  d:`             
+000010d0: 2020 2060 722c 7265 642c 3331 600d 0a20     `r,red,31`.. 
+000010e0: 2020 202d 205b 2b5d 2060 6772 6565 6e3a     - [+] `green:
+000010f0: 6020 2020 2020 2020 2020 2020 2020 2060  `              `
+00001100: 672c 6772 6565 6e2c 3332 600d 0a20 2020  g,green,32`..   
+00001110: 202d 205b 2b5d 2060 7965 6c6c 6f77 3a60   - [+] `yellow:`
+00001120: 2020 2020 2020 2020 2020 2020 2060 792c               `y,
+00001130: 7965 6c6c 6f77 2c33 3360 0d0a 2020 2020  yellow,33`..    
+00001140: 2d20 5b2b 5d20 6062 6c75 653a 6020 2020  - [+] `blue:`   
+00001150: 2020 2020 2020 2020 2020 2020 606c 2c62              `l,b
+00001160: 6c75 652c 3334 600d 0a20 2020 202d 205b  lue,34`..    - [
+00001170: 2b5d 2060 6d61 6765 6e74 613a 6020 2020  +] `magenta:`   
+00001180: 2020 2020 2020 2020 2060 6d2c 6d61 6765           `m,mage
+00001190: 6e74 612c 3335 600d 0a20 2020 202d 205b  nta,35`..    - [
+000011a0: 2b5d 2060 6379 616e 3a60 2020 2020 2020  +] `cyan:`      
+000011b0: 2020 2020 2020 2020 2060 632c 6379 616e           `c,cyan
+000011c0: 2c33 3660 0d0a 2020 2020 2d20 5b2b 5d20  ,36`..    - [+] 
+000011d0: 6077 6869 7465 3a60 2020 2020 2020 2020  `white:`        
+000011e0: 2020 2020 2020 6077 2c77 6869 7465 2c33        `w,white,3
+000011f0: 3760 0d0a 2020 2020 2d20 5b2b 5d20 6064  7`..    - [+] `d
+00001200: 6566 6175 6c74 3a60 2020 2020 2020 2020  efault:`        
+00001210: 2020 2020 6064 2c64 6566 6175 6c74 2c33      `d,default,3
+00001220: 3960 0d0a 2020 2020 2d20 5b2b 5d20 6062  9`..    - [+] `b
+00001230: 7269 6768 7420 626c 6163 6b3a 6020 2020  right black:`   
+00001240: 2020 2020 6062 622c 6262 6c61 636b 2c39      `bb,bblack,9
+00001250: 3060 0d0a 2020 2020 2d20 5b2b 5d20 6062  0`..    - [+] `b
+00001260: 7269 6768 7420 7265 643a 6020 2020 2020  right red:`     
+00001270: 2020 2020 6062 722c 6272 6564 2c39 3160      `br,bred,91`
+00001280: 0d0a 2020 2020 2d20 5b2b 5d20 6062 7269  ..    - [+] `bri
+00001290: 6768 7420 6772 6565 6e3a 6020 2020 2020  ght green:`     
+000012a0: 2020 6062 672c 6267 7265 656e 2c39 3260    `bg,bgreen,92`
+000012b0: 0d0a 2020 2020 2d20 5b2b 5d20 6062 7269  ..    - [+] `bri
+000012c0: 6768 7420 7965 6c6c 6f77 3a60 2020 2020  ght yellow:`    
+000012d0: 2020 6062 792c 6279 656c 6c6f 772c 3933    `by,byellow,93
+000012e0: 600d 0a20 2020 202d 205b 2b5d 2060 6272  `..    - [+] `br
+000012f0: 6967 6874 2062 6c75 653a 6020 2020 2020  ight blue:`     
+00001300: 2020 2060 626c 2c62 626c 7565 2c39 3460     `bl,bblue,94`
+00001310: 0d0a 2020 2020 2d20 5b2b 5d20 6062 7269  ..    - [+] `bri
+00001320: 6768 7420 6d61 6765 6e74 6160 2020 2020  ght magenta`    
+00001330: 2020 6062 6d2c 626d 6167 656e 7461 2c39    `bm,bmagenta,9
+00001340: 3560 0d0a 2020 2020 2d20 5b2b 5d20 6062  5`..    - [+] `b
+00001350: 7269 6768 7420 6379 616e 3a60 2020 2020  right cyan:`    
+00001360: 2020 2020 6062 632c 6263 7961 6e2c 3936      `bc,bcyan,96
+00001370: 600d 0a20 2020 202d 205b 2b5d 2060 6272  `..    - [+] `br
+00001380: 6967 6874 2077 6869 7465 3a60 2020 2020  ight white:`    
+00001390: 2020 2060 6277 2c62 7768 6974 652c 3937     `bw,bwhite,97
+000013a0: 600d 0a2d 2023 2323 2320 5374 796c 6573  `..- #### Styles
+000013b0: 3a0d 0a20 2020 202d 205b 2b5d 2060 626f  :..    - [+] `bo
+000013c0: 6c64 3a60 2020 2020 2020 2020 2020 2020  ld:`            
+000013d0: 2020 2060 422c 626f 6c64 2c31 600d 0a20     `B,bold,1`.. 
+000013e0: 2020 202d 205b 2b5d 2060 6469 6d3a 6020     - [+] `dim:` 
+000013f0: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00001400: 442c 6469 6d2c 3260 0d0a 2020 2020 2d20  D,dim,2`..    - 
+00001410: 5b2b 5d20 6069 7461 6c69 633a 6020 2020  [+] `italic:`   
+00001420: 2020 2020 2020 2020 2020 6049 2c69 7461            `I,ita
+00001430: 6c69 632c 3360 0d0a 2020 2020 2d20 5b2b  lic,3`..    - [+
+00001440: 5d20 6075 6e64 6572 6c69 6e65 3a60 2020  ] `underline:`  
+00001450: 2020 2020 2020 2020 6055 2c75 6e64 6572          `U,under
+00001460: 6c69 6e65 2c34 600d 0a20 2020 202d 205b  line,4`..    - [
+00001470: 2b5d 2060 626c 696e 6b69 6e67 3a60 2020  +] `blinking:`  
+00001480: 2020 2020 2020 2020 2060 4c2c 626c 696e           `L,blin
+00001490: 6b69 6e67 2c35 600d 0a20 2020 202d 205b  king,5`..    - [
+000014a0: 2b5d 2060 7265 7665 7273 653a 6020 2020  +] `reverse:`   
+000014b0: 2020 2020 2020 2020 2060 522c 7265 7665           `R,reve
+000014c0: 7273 652c 3760 0d0a 2020 2020 2d20 5b2b  rse,7`..    - [+
+000014d0: 5d20 6068 6964 6465 6e3a 6020 2020 2020  ] `hidden:`     
+000014e0: 2020 2020 2020 2020 6048 2c68 6964 6465          `H,hidde
+000014f0: 6e2c 3860 0d0a 2020 2020 2d20 5b2b 5d20  n,8`..    - [+] 
+00001500: 6073 7472 696b 6574 6872 6f75 6768 3a60  `strikethrough:`
+00001510: 2020 2020 2020 6053 2c73 7472 696b 6574        `S,striket
+00001520: 6872 6f75 6768 2c39 600d 0a2d 2023 2323  hrough,9`..- ###
+00001530: 2320 5072 6f67 7265 7373 4261 723a 2061  # ProgressBar: a
+00001540: 6464 2060 257b 6368 6172 7d25 600d 0a20  dd `%{char}%`.. 
+00001550: 2020 202d 205b 2b5d 2060 633a 6020 2020     - [+] `c:`   
+00001560: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00001570: 6375 7272 656e 7420 7072 6f67 7265 7373  current progress
+00001580: 2076 616c 7565 600d 0a20 2020 202d 205b   value`..    - [
+00001590: 2b5d 2060 6d3a 6020 2020 2020 2020 2020  +] `m:`         
+000015a0: 2020 2020 2020 2020 2060 6d61 7820 7072           `max pr
+000015b0: 6f67 7265 7373 2076 616c 7565 600d 0a20  ogress value`.. 
+000015c0: 2020 202d 205b 2b5d 2060 703a 6020 2020     - [+] `p:`   
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+000015e0: 7065 7263 656e 7420 7072 6f67 7265 7373  percent progress
+000015f0: 2076 616c 7565 600d 0a20 2020 202d 205b   value`..    - [
+00001600: 2b5d 2060 623a 6020 2020 2020 2020 2020  +] `b:`         
+00001610: 2020 2020 2020 2020 2060 6261 7220 7072           `bar pr
+00001620: 6f67 7265 7373 2076 616c 7565 600d 0a20  ogress value`.. 
+00001630: 2020 202d 205b 2b5d 2060 663a 6020 2020     - [+] `f:`   
+00001640: 2020 2020 2020 2020 2020 2020 2020 2060                 `
+00001650: 7072 696e 7420 6675 6c6c 2062 6172 2077  print full bar w
+00001660: 6974 6820 616c 6c20 696e 666f 600d 0a20  ith all info`.. 
+00001670: 2020 202d 205b 2b5d 2060 796f 7572 5f63     - [+] `your_c
+00001680: 7573 746f 6d5f 6b65 793a 6020 2020 2060  ustom_key:`    `
+00001690: 796f 7572 5f63 7573 746f 6d5f 7661 6c75  your_custom_valu
+000016a0: 6560 0d0a 2d20 2323 2323 204d 6f72 6520  e`..- #### More 
+000016b0: 436f 6e74 726f 6c20 696e 2050 726f 6772  Control in Progr
+000016c0: 6573 7342 6172 3a0d 0a20 2020 202d 205b  essBar:..    - [
+000016d0: 2b5d 2060 7478 743a 6020 2020 2020 2020  +] `txt:`       
+000016e0: 2020 2020 2020 2020 2060 6b65 7920 6f66           `key of
+000016f0: 2073 7472 696e 6720 7661 6c75 6520 696e   string value in
+00001700: 7369 6465 600d 0a20 2020 202d 205b 2b5d  side`..    - [+]
+00001710: 2060 6d78 3a60 2020 2020 2020 2020 2020   `mx:`          
+00001720: 2020 2020 2020 2060 6d61 7820 7661 6c75         `max valu
+00001730: 6520 6465 6661 756c 7420 6973 2031 3030  e default is 100
+00001740: 600d 0a20 2020 202d 205b 2b5d 2060 696e  `..    - [+] `in
+00001750: 633a 6020 2020 2020 2020 2020 2020 2020  c:`             
+00001760: 2020 2060 696e 6372 6561 6d6e 7420 7661     `increamnt va
+00001770: 6c75 6520 6465 6675 616c 7420 6973 2031  lue defualt is 1
+00001780: 600d 0a20 2020 202d 205b 2b5d 2060 6375  `..    - [+] `cu
+00001790: 7374 6f6d 3a60 2020 2020 2020 2020 2020  stom:`          
+000017a0: 2020 2060 6469 6374 206f 626a 6563 7420     `dict object 
+000017b0: 7769 7468 2063 7573 746f 6d20 6b65 7973  with custom keys
+000017c0: 600d 0a23 2320 4578 616d 706c 6573 2026  `..## Examples &
+000017d0: 2055 7361 6765 0d0a 5f5f 5f5f 5f5f 5f5f   Usage..________
+000017e0: 5f5f 5f5f 0d0a 3e20 5465 726d 696e 616c  ____..> Terminal
+000017f0: 2045 7865 6375 7465 0d0a 2323 2320 7769   Execute..### wi
+00001800: 6e64 6f77 730d 0a60 6060 7368 656c 6c0d  ndows..```shell.
+00001810: 0a70 7974 686f 6e20 2d6d 2041 4e53 4943  .python -m ANSIC
+00001820: 6f6e 7472 6f6c 6c65 720d 0a60 6060 0d0a  ontroller..```..
+00001830: 3e20 4f52 0d0a 6060 6073 6865 6c6c 0d0a  > OR..```shell..
+00001840: 616e 7369 636f 6e74 726f 6c6c 6572 0d0a  ansicontroller..
+00001850: 6060 600d 0a23 2323 204c 696e 7578 2026  ```..### Linux &
+00001860: 2620 5465 726d 7578 0d0a 6060 6073 6865  & Termux..```she
+00001870: 6c6c 0d0a 7079 7468 6f6e 3320 2d6d 2041  ll..python3 -m A
+00001880: 4e53 4943 6f6e 7472 6f6c 6c65 720d 0a60  NSIController..`
+00001890: 6060 0d0a 3e20 4f52 0d0a 6060 6073 6865  ``..> OR..```she
+000018a0: 6c6c 0d0a 616e 7369 636f 6e74 726f 6c6c  ll..ansicontroll
+000018b0: 6572 0d0a 6060 600d 0a3e 2050 7974 686f  er..```..> Pytho
+000018c0: 6e20 436f 6465 0d0a 2060 6060 2070 7974  n Code.. ``` pyt
+000018d0: 686f 6e0d 0a66 726f 6d20 414e 5349 436f  hon..from ANSICo
+000018e0: 6e74 726f 6c6c 6572 2069 6d70 6f72 7420  ntroller import 
+000018f0: 5465 726d 696e 616c 2020 2320 496d 706f  Terminal  # Impo
+00001900: 7274 204e 6565 6465 6420 436c 6173 730d  rt Needed Class.
+00001910: 0a74 6572 6d69 6e61 6c5f 636f 6e74 726f  .terminal_contro
+00001920: 6c20 3d20 5465 726d 696e 616c 2829 2020  l = Terminal()  
+00001930: 2020 2020 2020 2320 4372 6561 7465 204f        # Create O
+00001940: 626a 6563 7420 4672 6f6d 2043 6c61 7373  bject From Class
+00001950: 2054 6572 6d69 6e61 6c0d 0a60 6060 0d0a   Terminal..```..
+00001960: 3e20 546f 2073 6565 2061 6c6c 2074 6573  > To see all tes
+00001970: 7420 0d0a 6060 6070 7974 686f 6e0d 0a23  t ..```python..#
+00001980: 2070 7269 6e74 2061 6c6c 2073 7479 6c65   print all style
+00001990: 7320 7769 7468 2074 6573 7420 6578 616d  s with test exam
+000019a0: 706c 650d 0a54 6572 6d69 6e61 6c2e 7072  ple..Terminal.pr
+000019b0: 696e 745f 7374 796c 6573 2829 0d0a 2320  int_styles()..# 
+000019c0: 7072 696e 7420 616c 6c20 636f 6c6f 7273  print all colors
+000019d0: 2077 6974 6820 7465 7374 2065 7861 6d70   with test examp
+000019e0: 6c65 2066 6f72 2062 6163 6b67 726f 756e  le for backgroun
+000019f0: 6420 746f 6f20 616e 6420 636f 6465 730d  d too and codes.
+00001a00: 0a54 6572 6d69 6e61 6c2e 7072 696e 745f  .Terminal.print_
+00001a10: 636f 6c6f 7273 2829 0d0a 2320 7072 696e  colors()..# prin
+00001a20: 7420 616c 6c20 636f 6c6f 7273 2026 2073  t all colors & s
+00001a30: 7479 6c65 7320 7769 7468 2063 6f64 6573  tyles with codes
+00001a40: 0d0a 5465 726d 696e 616c 2e70 7269 6e74  ..Terminal.print
+00001a50: 5f63 6f6c 6f72 735f 7374 796c 6573 2829  _colors_styles()
+00001a60: 0d0a 2320 7072 696e 7420 6964 7320 636f  ..# print ids co
+00001a70: 6c6f 7273 2062 6163 6b67 726f 756e 6420  lors background 
+00001a80: 616e 6420 6e6f 726d 616c 2066 726f 6d20  and normal from 
+00001a90: 3020 746f 2032 3535 0d0a 5465 726d 696e  0 to 255..Termin
+00001aa0: 616c 2e70 7269 6e74 5f69 645f 636f 6c6f  al.print_id_colo
+00001ab0: 7273 2829 0d0a 2320 7769 6c6c 2070 7269  rs()..# will pri
+00001ac0: 6e74 2061 6c6c 2070 6572 7669 6f75 7320  nt all pervious 
+00001ad0: 696e 2073 616d 6520 7469 6d65 0d0a 5465  in same time..Te
+00001ae0: 726d 696e 616c 2e70 7269 6e74 5f74 6573  rminal.print_tes
+00001af0: 7428 290d 0a23 2054 7279 2069 740d 0a54  t()..# Try it..T
+00001b00: 6572 6d69 6e61 6c2e 6761 6d65 2829 0d0a  erminal.game()..
+00001b10: 6060 600d 0a23 2320 4f75 7470 7574 3a0d  ```..## Output:.
+00001b20: 0a21 5b41 6c74 2054 6578 745d 2868 7474  .![Alt Text](htt
+00001b30: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00001b40: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f4a  sercontent.com/J
+00001b50: 6f30 5830 312f 414e 5349 436f 6e74 726f  o0X01/ANSIContro
+00001b60: 6c6c 6572 2f6d 6169 6e2f 7465 7374 732f  ller/main/tests/
+00001b70: 7465 7374 5f73 7479 6c65 732e 706e 6729  test_styles.png)
+00001b80: 0d0a 215b 416c 7420 5465 7874 5d28 6874  ..![Alt Text](ht
+00001b90: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00001ba0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00001bb0: 4a6f 3058 3031 2f41 4e53 4943 6f6e 7472  Jo0X01/ANSIContr
+00001bc0: 6f6c 6c65 722f 6d61 696e 2f74 6573 7473  oller/main/tests
+00001bd0: 2f74 6573 745f 636f 6c6f 7273 2e70 6e67  /test_colors.png
+00001be0: 290d 0a21 5b41 6c74 2054 6578 745d 2868  )..![Alt Text](h
+00001bf0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00001c00: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001c10: 2f4a 6f30 5830 312f 414e 5349 436f 6e74  /Jo0X01/ANSICont
+00001c20: 726f 6c6c 6572 2f6d 6169 6e2f 7465 7374  roller/main/test
+00001c30: 732f 7465 7374 5f69 6473 2e70 6e67 290d  s/test_ids.png).
+00001c40: 0a23 2323 2074 6f20 6d6f 7665 2063 7572  .### to move cur
+00001c50: 736f 720d 0a60 6060 7079 7468 6f6e 0d0a  sor..```python..
+00001c60: 2320 7468 6973 2077 696c 6c20 6d61 6b65  # this will make
+00001c70: 2063 7572 736f 7220 6d6f 7665 2074 6f20   cursor move to 
+00001c80: 7570 2033 206c 696e 6573 0d0a 7465 726d  up 3 lines..term
+00001c90: 696e 616c 5f63 6f6e 7472 6f6c 2e6d 6f76  inal_control.mov
+00001ca0: 655f 746f 5f75 7028 7374 6570 733d 3329  e_to_up(steps=3)
+00001cb0: 2020 2020 0d0a 0d0a 2320 4166 7465 7220      ....# After 
+00001cc0: 6d6f 7665 2074 6f20 7570 2033 206c 696e  move to up 3 lin
+00001cd0: 6573 202c 2063 7572 736f 7220 7769 6c6c  es , cursor will
+00001ce0: 2073 7461 7274 2066 726f 6d20 3020 706f   start from 0 po
+00001cf0: 7374 696f 6e20 6f66 206c 696e 650d 0a74  stion of line..t
+00001d00: 6572 6d69 6e61 6c5f 636f 6e74 726f 6c2e  erminal_control.
+00001d10: 6d6f 7665 5f74 6f5f 7570 2873 7465 7073  move_to_up(steps
+00001d20: 3d33 2c73 7461 7274 5f6c 696e 653d 5472  =3,start_line=Tr
+00001d30: 7565 290d 0a0d 0a23 2074 6869 7320 7769  ue)....# this wi
+00001d40: 6c6c 206d 616b 6520 6375 7273 6f72 206d  ll make cursor m
+00001d50: 6f76 6520 746f 2064 6f77 6e20 3120 6c69  ove to down 1 li
+00001d60: 6e65 0d0a 7465 726d 696e 616c 5f63 6f6e  ne..terminal_con
+00001d70: 7472 6f6c 2e6d 6f76 655f 746f 5f64 6f77  trol.move_to_dow
+00001d80: 6e28 7374 6570 733d 3129 2020 0d0a 0d0a  n(steps=1)  ....
+00001d90: 2320 736f 6d65 7469 6d65 7320 7465 726d  # sometimes term
+00001da0: 696e 616c 206e 6f74 2061 6363 6570 7420  inal not accept 
+00001db0: 746f 206d 6f76 6520 746f 2075 7020 7468  to move to up th
+00001dc0: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
+00001dd0: 2066 6f72 6365 2074 6572 6d69 6e61 6c20   force terminal 
+00001de0: 746f 206d 6f76 6520 7570 2031 206c 696e  to move up 1 lin
+00001df0: 650d 0a74 6572 6d69 6e61 6c5f 636f 6e74  e..terminal_cont
+00001e00: 726f 6c2e 666f 7263 655f 6d6f 7665 5f74  rol.force_move_t
+00001e10: 6f5f 7570 2829 200d 0a0d 0a23 206d 6f76  o_up() ....# mov
+00001e20: 6520 6375 7273 6f72 2074 6f20 686f 6d65  e cursor to home
+00001e30: 2070 6f73 7469 6f6e 202c 206d 616b 6520   postion , make 
+00001e40: 6375 7273 6f72 2069 6e20 726f 7720 3020  cursor in row 0 
+00001e50: 616e 6420 636f 6c20 300d 0a74 6572 6d69  and col 0..termi
+00001e60: 6e61 6c5f 636f 6e74 726f 6c2e 6d6f 7665  nal_control.move
+00001e70: 5f74 6f5f 686f 6d65 5f70 6f73 7469 6f6e  _to_home_postion
+00001e80: 2829 0d0a 0d0a 2320 6d6f 7665 2063 7572  ()....# move cur
+00001e90: 736f 7220 746f 2063 7573 746f 6d20 706f  sor to custom po
+00001ea0: 7374 696f 6e20 726f 7720 7b6e 756d 7d20  stion row {num} 
+00001eb0: 636f 6c20 7b6e 756d 7d20 696e 2074 6572  col {num} in ter
+00001ec0: 6d69 6e61 6c20 7363 7265 656e 0d0a 2320  minal screen..# 
+00001ed0: 6865 7265 2074 6865 2063 7572 736f 7220  here the cursor 
+00001ee0: 7769 6c6c 206d 6f76 6520 746f 2072 6f77  will move to row
+00001ef0: 2031 3420 2c63 6f6c 756d 6e20 3230 0d0a   14 ,column 20..
+00001f00: 7465 726d 696e 616c 5f63 6f6e 7472 6f6c  terminal_control
+00001f10: 2e6d 6f76 655f 746f 5f6c 696e 6528 726f  .move_to_line(ro
+00001f20: 773d 3134 2c63 6f6c 3d32 3029 200d 0a60  w=14,col=20) ..`
+00001f30: 6060 0d0a 2323 2320 746f 2068 6964 6520  ``..### to hide 
+00001f40: 6375 7273 6f72 0d0a 6060 6070 7974 686f  cursor..```pytho
+00001f50: 6e0d 0a23 2068 6964 6520 6375 7273 6f72  n..# hide cursor
+00001f60: 202c 2074 7279 2069 740d 0a74 6572 6d69   , try it..termi
+00001f70: 6e61 6c5f 636f 6e74 726f 6c2e 6869 6465  nal_control.hide
+00001f80: 5f63 7572 736f 7228 290d 0a23 2073 686f  _cursor()..# sho
+00001f90: 7720 6375 7273 6f72 2069 6620 6869 6464  w cursor if hidd
+00001fa0: 656e 0d0a 7465 726d 696e 616c 5f63 6f6e  en..terminal_con
+00001fb0: 7472 6f6c 2e73 686f 775f 6375 7273 6f72  trol.show_cursor
+00001fc0: 2829 0d0a 2320 7368 6f77 2063 7572 736f  ()..# show curso
+00001fd0: 7220 6966 2068 6964 6465 6e20 616e 6420  r if hidden and 
+00001fe0: 6869 6465 2069 6620 7368 6f77 656e 0d0a  hide if showen..
+00001ff0: 7465 726d 696e 616c 5f63 6f6e 7472 6f6c  terminal_control
+00002000: 2e74 6f67 676c 655f 6375 7273 6f72 2829  .toggle_cursor()
+00002010: 0d0a 6060 600d 0a23 2323 2054 6f20 7361  ..```..### To sa
+00002020: 7665 2063 7572 736f 7220 706f 7374 696f  ve cursor postio
+00002030: 6e20 6f72 2072 6573 746f 7265 2063 7572  n or restore cur
+00002040: 7372 6f72 2070 6f73 7469 6f6e 0d0a 6060  sror postion..``
+00002050: 6070 7974 686f 6e0d 0a74 6572 6d69 6e61  `python..termina
+00002060: 6c5f 636f 6e74 726f 6c2e 7361 7665 5f63  l_control.save_c
+00002070: 7572 736f 725f 706f 7374 696f 6e28 2920  ursor_postion() 
+00002080: 2020 2320 5361 7665 2043 7572 7265 6e74    # Save Current
+00002090: 2043 7572 736f 7220 706f 7374 696f 6e20   Cursor postion 
+000020a0: 726f 7720 2c20 636f 6c75 6d6e 0d0a 2320  row , column..# 
+000020b0: 5265 7374 6f72 6520 4c61 7374 2053 6176  Restore Last Sav
+000020c0: 6564 2043 7572 736f 7220 706f 7374 696f  ed Cursor postio
+000020d0: 6e0d 0a74 6572 6d69 6e61 6c5f 636f 6e74  n..terminal_cont
+000020e0: 726f 6c2e 7265 7374 6f72 5f63 7572 736f  rol.restor_curso
+000020f0: 725f 706f 7374 696f 6e28 2920 2320 6375  r_postion() # cu
+00002100: 7273 6f72 2077 696c 6c20 6d6f 7665 2061  rsor will move a
+00002110: 7574 6f20 746f 2073 6176 6564 2070 6f73  uto to saved pos
+00002120: 7469 6f6e 0d0a 6060 600d 0a23 2323 206c  tion..```..### l
+00002130: 6574 7320 7361 7920 6920 7761 6e74 2074  ets say i want t
+00002140: 6f20 636c 6561 7220 736f 6d65 2074 6578  o clear some tex
+00002150: 7420 6672 6f6d 2074 6572 6d69 6e61 6c20  t from terminal 
+00002160: 605c 7220 6e6f 600d 0a60 6060 7079 7468  `\r no`..```pyth
+00002170: 6f6e 0d0a 7465 726d 696e 616c 5f63 6f6e  on..terminal_con
+00002180: 7472 6f6c 2e63 6c65 6172 5f73 6372 6565  trol.clear_scree
+00002190: 6e28 2920 2020 2020 2020 2020 2020 2020  n()             
+000021a0: 2320 436c 6561 7220 5465 726d 696e 616c  # Clear Terminal
+000021b0: 2053 6372 6565 6e20 6974 2063 6c6f 7365   Screen it close
+000021c0: 2074 6f20 636f 6d6d 616e 6420 6063 6c73   to command `cls
+000021d0: 6020 616e 6420 6063 6c65 6172 600d 0a74  ` and `clear`..t
+000021e0: 6572 6d69 6e61 6c5f 636f 6e74 726f 6c2e  erminal_control.
+000021f0: 636c 6561 725f 6166 7465 725f 6375 7273  clear_after_curs
+00002200: 6f72 2829 2020 2020 2020 2023 2043 6c65  or()       # Cle
+00002210: 6172 2054 6572 6d69 6e61 6c20 5363 7265  ar Terminal Scre
+00002220: 656e 2061 6c6c 2074 6578 7420 6166 7465  en all text afte
+00002230: 7220 6375 7273 6f72 2070 6f73 7469 6f6e  r cursor postion
+00002240: 0d0a 7465 726d 696e 616c 5f63 6f6e 7472  ..terminal_contr
+00002250: 6f6c 2e63 6c65 6172 5f62 6566 6f72 655f  ol.clear_before_
+00002260: 6375 7273 6f72 2829 2020 2020 2020 2320  cursor()      # 
+00002270: 436c 6561 7220 5465 726d 696e 616c 2053  Clear Terminal S
+00002280: 6372 6565 6e20 616c 6c20 7465 7874 2061  creen all text a
+00002290: 6674 6572 2063 7572 736f 7220 706f 7374  fter cursor post
+000022a0: 696f 6e0d 0a74 6572 6d69 6e61 6c5f 636f  ion..terminal_co
+000022b0: 6e74 726f 6c2e 636c 6561 725f 6c69 6e65  ntrol.clear_line
+000022c0: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
+000022d0: 2023 2043 6c65 6172 2043 7572 7265 6e74   # Clear Current
+000022e0: 206c 696e 652c 206f 6620 6375 7273 6f72   line, of cursor
+000022f0: 2070 6f73 7469 6f6e 2072 6f77 2061 6e64   postion row and
+00002300: 2073 7461 7274 2066 726f 6d20 6669 7273   start from firs
+00002310: 7420 6c69 6e65 0d0a 7465 726d 696e 616c  t line..terminal
+00002320: 5f63 6f6e 7472 6f6c 2e63 6c65 6172 5f6c  _control.clear_l
+00002330: 696e 655f 6166 7465 725f 6375 7273 6f72  ine_after_cursor
+00002340: 2829 2020 2320 436c 6561 7220 4375 7272  ()  # Clear Curr
+00002350: 656e 7420 6c69 6e65 2c20 616c 6c20 7465  ent line, all te
+00002360: 7874 2061 6674 6572 2063 7572 736f 7220  xt after cursor 
+00002370: 706f 7374 696f 6e20 696e 2073 616d 6520  postion in same 
+00002380: 6c69 6e65 0d0a 7465 726d 696e 616c 5f63  line..terminal_c
+00002390: 6f6e 7472 6f6c 2e63 6c65 6172 5f6c 696e  ontrol.clear_lin
+000023a0: 655f 6265 666f 7265 5f63 7572 736f 7228  e_before_cursor(
+000023b0: 2920 2320 436c 6561 7220 4375 7272 656e  ) # Clear Curren
+000023c0: 7420 6c69 6e65 2c20 616c 6c20 7465 7874  t line, all text
+000023d0: 2062 6566 6f72 6520 6375 7273 6f72 2070   before cursor p
+000023e0: 6f73 7469 6f6e 2069 6e20 7361 6d65 206c  ostion in same l
+000023f0: 696e 650d 0a60 6060 0d0a 2323 2320 6c65  ine..```..### le
+00002400: 7473 2073 6179 2069 2077 616e 7420 746f  ts say i want to
+00002410: 2063 6f6c 6f72 697a 6520 736f 6d65 2074   colorize some t
+00002420: 6578 740d 0a60 4279 2055 7369 6e67 2043  ext..`By Using C
+00002430: 6f6e 6365 7074 206f 6620 2d20 5461 626c  oncept of - Tabl
+00002440: 6520 6f66 2063 6f6c 6f72 7320 2620 7374  e of colors & st
+00002450: 796c 6560 0d0a 3e20 5573 696e 6720 436f  yle`..> Using Co
+00002460: 6c6f 7273 206f 6e6c 7920 6e6f 2073 7479  lors only no sty
+00002470: 6c65 7320 6f72 2062 6163 6b67 726f 756e  les or backgroun
+00002480: 640d 0a3e 2043 6f6c 6f72 697a 6520 6675  d..> Colorize fu
+00002490: 6e63 7469 6f6e 2074 616b 6520 3a20 7465  nction take : te
+000024a0: 7874 2061 6e64 2073 6570 7261 746f 720d  xt and seprator.
+000024b0: 0a3e 200d 0a3e 2073 796e 7461 783a 0d0a  .> ..> syntax:..
+000024c0: 3e20 0d0a 3e20 6073 6570 2073 6f6d 655f  > ..> `sep some_
+000024d0: 7374 796c 655f 636f 6465 735f 6f72 5f63  style_codes_or_c
+000024e0: 6f6c 6f72 5f63 6f64 6520 7365 7060 0d0a  olor_code sep`..
+000024f0: 3e20 0d0a 3e20 666f 7220 6578 616d 706c  > ..> for exampl
+00002500: 6520 6073 6570 2069 7320 5b5d 600d 0a3e  e `sep is []`..>
+00002510: 200d 0a3e 2073 796e 7461 7820 7769 6c6c   ..> syntax will
+00002520: 2062 653a 2020 605b 736f 6d65 5f73 7479   be:  `[some_sty
+00002530: 6c65 5f63 6f64 6573 5f6f 725f 636f 6c6f  le_codes_or_colo
+00002540: 725f 636f 6465 5d60 0d0a 3e20 0d0a 6060  r_code]`..> ..``
+00002550: 6070 7974 686f 6e0d 0a73 6570 203d 2022  `python..sep = "
+00002560: 5b5d 220d 0a63 6f6c 6f72 697a 655f 7465  []"..colorize_te
+00002570: 7874 735f 7573 696e 675f 636f 6c6f 725f  xts_using_color_
+00002580: 6368 6172 203d 205b 0d0a 2020 2020 225b  char = [..    "[
+00002590: 725d 5468 6973 2069 7320 5265 645b 305d  r]This is Red[0]
+000025a0: 222c 0d0a 2020 2020 225b 675d 5468 6973  ",..    "[g]This
+000025b0: 2069 7320 4772 6565 6e5b 305d 222c 0d0a   is Green[0]",..
+000025c0: 2020 2020 225b 795d 5468 6973 2069 7320      "[y]This is 
+000025d0: 5965 6c6c 6f77 5b30 5d22 2c0d 0a20 2020  Yellow[0]",..   
+000025e0: 2022 5b62 5d54 6869 7320 6973 2042 6c61   "[b]This is Bla
+000025f0: 636b 5b30 5d22 2c0d 0a20 2020 2022 5b6c  ck[0]",..    "[l
+00002600: 5d54 6869 7320 6973 2042 6c75 655b 305d  ]This is Blue[0]
+00002610: 222c 0d0a 2020 2020 225b 6d5d 5468 6973  ",..    "[m]This
+00002620: 2069 7320 4d65 6765 6e74 615b 305d 222c   is Megenta[0]",
+00002630: 0d0a 2020 2020 225b 635d 5468 6973 2069  ..    "[c]This i
+00002640: 7320 4379 616e 5b30 5d22 2c0d 0a20 2020  s Cyan[0]",..   
+00002650: 2022 5b77 5d54 6869 7320 6973 2057 6869   "[w]This is Whi
+00002660: 7465 5b30 5d22 2c0d 0a20 2020 2022 5b64  te[0]",..    "[d
+00002670: 5d54 6869 7320 6973 2064 6566 6175 6c74  ]This is default
+00002680: 5b30 5d22 2c0d 0a20 2020 2022 5b62 625d  [0]",..    "[bb]
+00002690: 5468 6973 2069 7320 4272 6967 6874 2042  This is Bright B
+000026a0: 6c61 636b 5b30 5d22 2c0d 0a20 2020 2022  lack[0]",..    "
+000026b0: 5b62 725d 5468 6973 2069 7320 4272 6967  [br]This is Brig
+000026c0: 6874 2052 6564 5b30 5d22 2c0d 0a5d 0d0a  ht Red[0]",..]..
+000026d0: 666f 7220 7465 7874 2069 6e20 636f 6c6f  for text in colo
+000026e0: 7269 7a65 5f74 6578 7473 5f75 7369 6e67  rize_texts_using
+000026f0: 5f63 6f6c 6f72 5f63 6861 723a 0d0a 2020  _color_char:..  
+00002700: 2020 7072 696e 7428 7465 726d 696e 616c    print(terminal
+00002710: 5f63 6f6e 7472 6f6c 2e63 6f6c 6f72 697a  _control.coloriz
+00002720: 6528 7465 7874 2c73 6570 2929 0d0a 6060  e(text,sep))..``
+00002730: 600d 0a23 2320 4f75 7470 7574 3a0d 0a21  `..## Output:..!
+00002740: 5b41 6c74 2054 6578 745d 2868 7474 7073  [Alt Text](https
+00002750: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00002760: 7263 6f6e 7465 6e74 2e63 6f6d 2f4a 6f30  rcontent.com/Jo0
+00002770: 5830 312f 414e 5349 436f 6e74 726f 6c6c  X01/ANSIControll
+00002780: 6572 2f6d 6169 6e2f 7465 7374 732f 7465  er/main/tests/te
+00002790: 7374 5f63 6f6c 6f72 735f 6f75 742e 706e  st_colors_out.pn
+000027a0: 6729 0d0a 3e20 4e6f 7720 5573 696e 6720  g)..> Now Using 
+000027b0: 7374 796c 6520 6f6e 6c79 0d0a 3e20 0d0a  style only..> ..
+000027c0: 6060 6070 7974 686f 6e0d 0a73 6570 203d  ```python..sep =
+000027d0: 2022 5b5d 220d 0a63 6f6c 6f72 697a 655f   "[]"..colorize_
+000027e0: 7465 7874 735f 7573 696e 675f 7374 796c  texts_using_styl
+000027f0: 655f 6368 6172 203d 205b 0d0a 2020 2020  e_char = [..    
+00002800: 225b 425d 5468 6973 2069 7320 426f 6c64  "[B]This is Bold
+00002810: 5b30 5d22 2c0d 0a20 2020 2022 5b44 5d54  [0]",..    "[D]T
+00002820: 6869 7320 6973 2044 696d 5b30 5d22 2c0d  his is Dim[0]",.
+00002830: 0a20 2020 2022 5b49 5d54 6869 7320 6973  .    "[I]This is
+00002840: 2049 7461 6c69 635b 305d 222c 0d0a 2020   Italic[0]",..  
+00002850: 2020 225b 555d 5468 6973 2069 7320 556e    "[U]This is Un
+00002860: 6465 726c 696e 655b 305d 222c 0d0a 2020  derline[0]",..  
+00002870: 2020 225b 4c5d 5468 6973 2069 7320 426c    "[L]This is Bl
+00002880: 696e 6b69 6e67 5b30 5d22 2c0d 0a20 2020  inking[0]",..   
+00002890: 2022 5b52 5d54 6869 7320 6973 2072 6576   "[R]This is rev
+000028a0: 6572 7365 5b30 5d22 2c0d 0a20 2020 2022  erse[0]",..    "
+000028b0: 5b48 5d54 6869 7320 6973 2048 6964 6465  [H]This is Hidde
+000028c0: 6e5b 305d 222c 0d0a 2020 2020 225b 535d  n[0]",..    "[S]
+000028d0: 5468 6973 2069 7320 5374 7269 6b65 7468  This is Striketh
+000028e0: 726f 6768 5b30 5d22 2c0d 0a5d 0d0a 666f  rogh[0]",..]..fo
+000028f0: 7220 7465 7874 2069 6e20 636f 6c6f 7269  r text in colori
+00002900: 7a65 5f74 6578 7473 5f75 7369 6e67 5f73  ze_texts_using_s
+00002910: 7479 6c65 5f63 6861 723a 0d0a 2020 2020  tyle_char:..    
+00002920: 7072 696e 7428 7465 726d 696e 616c 5f63  print(terminal_c
+00002930: 6f6e 7472 6f6c 2e63 6f6c 6f72 697a 6528  ontrol.colorize(
+00002940: 7465 7874 2c73 6570 2929 0d0a 6060 600d  text,sep))..```.
+00002950: 0a23 2320 4f75 7470 7574 3a0d 0a21 5b41  .## Output:..![A
+00002960: 6c74 2054 6578 745d 2868 7474 7073 3a2f  lt Text](https:/
+00002970: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00002980: 6f6e 7465 6e74 2e63 6f6d 2f4a 6f30 5830  ontent.com/Jo0X0
+00002990: 312f 414e 5349 436f 6e74 726f 6c6c 6572  1/ANSIController
+000029a0: 2f6d 6169 6e2f 7465 7374 732f 7465 7374  /main/tests/test
+000029b0: 5f73 7479 6c65 735f 6f75 742e 706e 6729  _styles_out.png)
+000029c0: 0d0a 3e20 4e6f 7720 5573 696e 6720 436f  ..> Now Using Co
+000029d0: 6c6f 7273 2026 2073 7479 6c65 0d0a 3e20  lors & style..> 
+000029e0: 0d0a 6060 6070 7974 686f 6e0d 0a73 6570  ..```python..sep
+000029f0: 203d 2022 5b5d 220d 0a63 6f6c 6f72 697a   = "[]"..coloriz
+00002a00: 655f 7465 7874 735f 7573 696e 675f 7374  e_texts_using_st
+00002a10: 796c 655f 636f 6c6f 725f 6368 6172 203d  yle_color_char =
+00002a20: 205b 0d0a 2020 2020 225b 4272 5d54 6869   [..    "[Br]Thi
+00002a30: 7320 6973 2042 6f6c 6420 616e 6420 5265  s is Bold and Re
+00002a40: 645b 305d 222c 0d0a 2020 2020 225b 4479  d[0]",..    "[Dy
+00002a50: 5d54 6869 7320 6973 2044 696d 2061 6e64  ]This is Dim and
+00002a60: 2059 656c 6c6f 775b 305d 222c 0d0a 2020   Yellow[0]",..  
+00002a70: 2020 225b 496c 5d54 6869 7320 6973 2049    "[Il]This is I
+00002a80: 7461 6c69 6320 616e 6420 426c 7565 5b30  talic and Blue[0
+00002a90: 5d22 2c0d 0a20 2020 2022 5b55 675d 5468  ]",..    "[Ug]Th
+00002aa0: 6973 2069 7320 556e 6465 726c 696e 6520  is is Underline 
+00002ab0: 616e 6420 4772 6565 6e5b 305d 222c 0d0a  and Green[0]",..
+00002ac0: 2020 2020 225b 4c62 5d54 6869 7320 6973      "[Lb]This is
+00002ad0: 2042 6c69 6e6b 696e 6720 616e 6420 626c   Blinking and bl
+00002ae0: 6163 6b5b 305d 222c 0d0a 2020 2020 225b  ack[0]",..    "[
+00002af0: 5262 725d 5468 6973 2069 7320 7265 7665  Rbr]This is reve
+00002b00: 7273 6520 616e 6420 4272 6967 6874 2052  rse and Bright R
+00002b10: 6564 5b30 5d22 2c0d 0a20 2020 2022 5b48  ed[0]",..    "[H
+00002b20: 6279 5d54 6869 7320 6973 2048 6964 6465  by]This is Hidde
+00002b30: 6e20 616e 6420 4272 6967 6874 2059 656c  n and Bright Yel
+00002b40: 6c6f 775b 305d 222c 0d0a 2020 2020 225b  low[0]",..    "[
+00002b50: 5362 635d 5468 6973 2069 7320 5374 7269  Sbc]This is Stri
+00002b60: 6b65 7468 726f 6768 2061 6e64 2042 7269  kethrogh and Bri
+00002b70: 6768 7420 4379 616e 5b30 5d22 2c0d 0a5d  ght Cyan[0]",..]
+00002b80: 0d0a 666f 7220 7465 7874 2069 6e20 636f  ..for text in co
+00002b90: 6c6f 7269 7a65 5f74 6578 7473 5f75 7369  lorize_texts_usi
+00002ba0: 6e67 5f73 7479 6c65 5f63 6f6c 6f72 5f63  ng_style_color_c
+00002bb0: 6861 723a 0d0a 2020 2020 7072 696e 7428  har:..    print(
+00002bc0: 7465 726d 696e 616c 5f63 6f6e 7472 6f6c  terminal_control
+00002bd0: 2e63 6f6c 6f72 697a 6528 7465 7874 2c73  .colorize(text,s
+00002be0: 6570 2929 0d0a 6060 600d 0a23 2320 4f75  ep))..```..## Ou
+00002bf0: 7470 7574 3a0d 0a21 5b41 6c74 2054 6578  tput:..![Alt Tex
+00002c00: 745d 2868 7474 7073 3a2f 2f72 6177 2e67  t](https://raw.g
+00002c10: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00002c20: 2e63 6f6d 2f4a 6f30 5830 312f 414e 5349  .com/Jo0X01/ANSI
+00002c30: 436f 6e74 726f 6c6c 6572 2f6d 6169 6e2f  Controller/main/
+00002c40: 7465 7374 732f 7465 7374 5f63 6f6c 6f72  tests/test_color
+00002c50: 735f 7374 796c 655f 6f75 742e 706e 6729  s_style_out.png)
+00002c60: 0d0a 3e20 546f 2061 6464 2042 6163 6b67  ..> To add Backg
+00002c70: 726f 756e 6420 206a 7573 7420 6164 6420  round  just add 
+00002c80: 6058 2c78 6020 746f 2074 6865 2062 6c6f  `X,x` to the blo
+00002c90: 636b 2060 5b78 7242 5d60 2069 2077 616e  ck `[xrB]` i wan
+00002ca0: 7420 6261 636b 6772 6f75 6e64 2072 6564  t background red
+00002cb0: 2061 6e64 2062 6f6c 6420 7374 796c 650d   and bold style.
+00002cc0: 0a3e 200d 0a3e 204e 6f74 653a 2079 6f75  .> ..> Note: you
+00002cd0: 2063 616e 2075 7365 2060 7465 726d 696e   can use `termin
+00002ce0: 616c 5f63 6f6e 7472 6f6c 2e70 7269 6e74  al_control.print
+00002cf0: 5f63 6f6c 6f72 697a 6560 2077 6974 686f  _colorize` witho
+00002d00: 7574 2070 7269 6e74 0d0a 3e20 0d0a 3e20  ut print..> ..> 
+00002d10: 605b 305d 2c5b 7a5d 2c5b 5a5d 2c5b 5265  `[0],[z],[Z],[Re
+00002d20: 7365 745d 6020 6973 2074 6f20 7265 7365  set]` is to rese
+00002d30: 7420 746f 2064 6566 6175 6c74 2063 6f6c  t to default col
+00002d40: 6f72 2673 7479 6c65 2069 6e20 7465 726d  or&style in term
+00002d50: 696e 616c 0d0a 3e20 0d0a 3e20 0d0a 2323  inal..> ..> ..##
+00002d60: 2320 2d20 5573 696e 6720 6d75 6c74 6970  # - Using multip
+00002d70: 726f 6772 6573 7362 6172 0d0a 6060 6070  rogressbar..```p
+00002d80: 7974 686f 6e0d 0a23 2061 6464 5f70 726f  ython..# add_pro
+00002d90: 6772 6573 733a 2074 616b 6520 6c69 7374  gress: take list
+00002da0: 206f 6620 7465 7874 0d0a 2320 7461 6b65   of text..# take
+00002db0: 2074 6f6f 2064 6963 740d 0a23 6578 616d   too dict..#exam
+00002dc0: 706c 6520 7769 7468 206c 6973 740d 0a74  ple with list..t
+00002dd0: 6572 6d69 6e61 6c5f 636f 6e74 726f 6c2e  erminal_control.
+00002de0: 6164 645f 7072 6f67 7265 7373 285b 0d0a  add_progress([..
+00002df0: 2020 2020 225b 7242 5d74 6573 7431 5b30      "[rB]test1[0
+00002e00: 5d22 2c0d 0a20 2020 2022 5b77 5d74 6573  ]",..    "[w]tes
+00002e10: 7432 5b30 5d22 2c0d 0a20 2020 2022 5b63  t2[0]",..    "[c
+00002e20: 495d 7465 7374 335b 305d 222c 0d0a 2020  I]test3[0]",..  
+00002e30: 2020 225b 7944 5d74 6573 7434 5b30 5d22    "[yD]test4[0]"
+00002e40: 2c0d 0a5d 290d 0a23 2065 7861 6d70 6c65  ,..])..# example
+00002e50: 2077 6974 6820 6469 6374 0d0a 2320 7461   with dict..# ta
+00002e60: 6b65 2060 7072 6f67 7265 7373 5f6e 616d  ke `progress_nam
+00002e70: 6560 6020 746f 2061 6363 6573 7320 6c61  e`` to access la
+00002e80: 7465 720d 0a23 2060 7478 7460 206b 6579  ter..# `txt` key
+00002e90: 2069 7320 7468 6520 7072 6f67 7265 7373   is the progress
+00002ea0: 2074 6578 740d 0a74 6572 6d69 6e61 6c5f   text..terminal_
+00002eb0: 636f 6e74 726f 6c2e 6164 645f 7072 6f67  control.add_prog
+00002ec0: 7265 7373 287b 0d0a 2020 2020 2270 726f  ress({..    "pro
+00002ed0: 6772 6573 7331 223a 7b22 7478 7422 3a20  gress1":{"txt": 
+00002ee0: 225b 7242 5d74 6573 7431 5b30 5d22 7d2c  "[rB]test1[0]"},
+00002ef0: 0d0a 2020 2020 2270 726f 6772 6573 7332  ..    "progress2
+00002f00: 223a 7b22 7478 7422 3a20 225b 775d 7465  ":{"txt": "[w]te
+00002f10: 7374 325b 305d 227d 2c0d 0a20 2020 2022  st2[0]"},..    "
+00002f20: 7072 6f67 7265 7373 3322 3a7b 2274 7874  progress3":{"txt
+00002f30: 223a 2022 5b63 495d 7465 7374 335b 305d  ": "[cI]test3[0]
+00002f40: 227d 2c0d 0a20 2020 2022 7072 6f67 7265  "},..    "progre
+00002f50: 7373 3422 3a7b 2274 7874 223a 2022 5b79  ss4":{"txt": "[y
+00002f60: 445d 7465 7374 345b 305d 227d 2c0d 0a7d  D]test4[0]"},..}
+00002f70: 290d 0a23 206e 6f77 2069 6620 6920 7761  )..# now if i wa
+00002f80: 6e74 2074 6f20 6164 6420 7072 6f67 7265  nt to add progre
+00002f90: 7373 2076 616c 7565 2061 6e64 2075 7064  ss value and upd
+00002fa0: 6174 6520 7661 6c75 6573 0d0a 2365 7861  ate values..#exa
+00002fb0: 6d70 6c65 2077 6974 6820 6c69 7374 0d0a  mple with list..
+00002fc0: 2320 6163 6365 7373 2062 7920 696e 6465  # access by inde
+00002fd0: 780d 0a74 6572 6d69 6e61 6c5f 636f 6e74  x..terminal_cont
+00002fe0: 726f 6c2e 6164 645f 7072 6f67 7265 7373  rol.add_progress
+00002ff0: 285b 0d0a 2020 2020 225b 7242 5d74 6573  ([..    "[rB]tes
+00003000: 7431 3a20 2825 6325 2f25 6d25 295b 305d  t1: (%c%/%m%)[0]
+00003010: 222c 0d0a 2020 2020 225b 775d 7465 7374  ",..    "[w]test
+00003020: 323a 2025 6225 2028 2563 252f 256d 2529  2: %b% (%c%/%m%)
+00003030: 5b30 5d22 2c0d 0a20 2020 2022 5b63 495d  [0]",..    "[cI]
+00003040: 7465 7374 333a 2025 6225 2025 7025 2028  test3: %b% %p% (
+00003050: 2563 252f 256d 2529 5b30 5d22 2c0d 0a20  %c%/%m%)[0]",.. 
+00003060: 2020 2022 5b79 445d 7465 7374 343a 2025     "[yD]test4: %
+00003070: 6625 205b 305d 222c 0d0a 5d29 0d0a 2365  f% [0]",..])..#e
+00003080: 7861 6d70 6c65 2077 6974 6820 6d6f 7265  xample with more
+00003090: 2063 6f6e 7472 6f6c 2064 6963 740d 0a74   control dict..t
+000030a0: 6572 6d69 6e61 6c5f 636f 6e74 726f 6c2e  erminal_control.
+000030b0: 6164 645f 7072 6f67 7265 7373 287b 0d0a  add_progress({..
+000030c0: 2020 2020 2270 726f 6772 6573 7331 223a      "progress1":
+000030d0: 7b0d 0a20 2020 2020 2020 2022 7478 7422  {..        "txt"
+000030e0: 3a20 225b 7242 5d74 6573 7431 3a20 2825  : "[rB]test1: (%
+000030f0: 6325 2f25 6d25 2920 2d20 2825 6b65 7931  c%/%m%) - (%key1
+00003100: 252c 256b 6579 3225 2c25 7374 6174 7573  %,%key2%,%status
+00003110: 5f74 6573 7425 295b 305d 222c 0d0a 2020  _test%)[0]",..  
+00003120: 2020 2020 2020 226d 7822 3a32 3030 2c0d        "mx":200,.
+00003130: 0a20 2020 2020 2020 2022 696e 6322 3a35  .        "inc":5
+00003140: 2c0d 0a20 2020 2020 2020 2022 6375 7374  ,..        "cust
+00003150: 6f6d 223a 7b0d 0a20 2020 2020 2020 2020  om":{..         
+00003160: 2020 2022 6b65 7931 223a 3130 2c0d 0a20     "key1":10,.. 
+00003170: 2020 2020 2020 2020 2020 2022 6b65 7932             "key2
+00003180: 223a 2274 6573 7422 2c0d 0a20 2020 2020  ":"test",..     
+00003190: 2020 2020 2020 2022 7374 6174 7573 5f74         "status_t
+000031a0: 6573 7422 3a22 476f 6f64 220d 0a20 2020  est":"Good"..   
+000031b0: 2020 2020 207d 0d0a 2020 2020 7d2c 0d0a       }..    },..
+000031c0: 2020 2020 2320 736f 6d65 7469 6d65 7320      # sometimes 
+000031d0: 6e6f 206e 6565 6420 666f 7220 606d 7860  no need for `mx`
+000031e0: 206f 7220 6069 6e63 600d 0a20 2020 2022   or `inc`..    "
+000031f0: 7072 6f67 7265 7373 3222 3a7b 0d0a 2020  progress2":{..  
+00003200: 2020 2020 2020 2274 7874 223a 2022 5b77        "txt": "[w
+00003210: 5d74 6573 7432 3a20 2562 2520 2825 6325  ]test2: %b% (%c%
+00003220: 2f25 6d25 292d 2028 256b 6579 3125 2c25  /%m%)- (%key1%,%
+00003230: 6b65 7932 2529 5b30 5d22 2c0d 0a20 2020  key2%)[0]",..   
+00003240: 2020 2020 2022 6375 7374 6f6d 223a 7b0d       "custom":{.
+00003250: 0a20 2020 2020 2020 2020 2020 2022 6b65  .            "ke
+00003260: 7931 223a 3130 2c0d 0a20 2020 2020 2020  y1":10,..       
+00003270: 2020 2020 2022 6b65 7932 223a 2274 6573       "key2":"tes
+00003280: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
+00003290: 2022 7374 6174 7573 5f74 6573 7422 3a22   "status_test":"
+000032a0: 476f 6f64 220d 0a20 2020 2020 2020 207d  Good"..        }
+000032b0: 0d0a 2020 2020 7d0d 0a7d 290d 0a0d 0a23  ..    }..})....#
+000032c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000032d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000032e0: 2d2d 2d2d 2d2d 2d2d 0d0a 2320 6e6f 7720  --------..# now 
+000032f0: 746f 2075 7064 6174 6520 7072 6f67 7265  to update progre
+00003300: 7373 2062 6172 2076 616c 7565 730d 0a0d  ss bar values...
+00003310: 0a23 2070 726f 6772 6573 735f 6b65 7920  .# progress_key 
+00003320: 3d20 6069 6620 6c69 7374 2077 696c 6c20  = `if list will 
+00003330: 6265 2069 6e64 6578 600d 0a23 2070 726f  be index`..# pro
+00003340: 6772 6573 735f 6b65 7920 3d20 6069 6620  gress_key = `if 
+00003350: 6469 6374 2077 696c 6c20 6265 206e 616d  dict will be nam
+00003360: 6560 0d0a 2320 6061 6c6c 6020 6172 6775  e`..# `all` argu
+00003370: 6d65 6e74 206d 6561 6e20 6966 2075 2077  ment mean if u w
+00003380: 616e 7420 746f 2063 6861 6e67 6520 696e  ant to change in
+00003390: 2061 6c6c 2074 6578 7473 0d0a 2320 6465   all texts..# de
+000033a0: 6661 756c 7420 6f66 2061 6c6c 2069 7320  fault of all is 
+000033b0: 4661 6c73 650d 0a0d 0a23 2074 6f20 6368  False....# to ch
+000033c0: 616e 6765 206d 6178 2076 616c 7565 206f  ange max value o
+000033d0: 6620 6375 7374 6f6d 2074 6578 7473 0d0a  f custom texts..
+000033e0: 7465 726d 696e 616c 5f63 6f6e 7472 6f6c  terminal_control
+000033f0: 2e73 6574 5f70 726f 6772 6573 735f 6d61  .set_progress_ma
+00003400: 785f 7661 6c75 6528 3135 302c 2270 726f  x_value(150,"pro
+00003410: 6772 6573 735f 6b65 7922 290d 0a74 6572  gress_key")..ter
+00003420: 6d69 6e61 6c5f 636f 6e74 726f 6c2e 7365  minal_control.se
+00003430: 745f 7072 6f67 7265 7373 5f6d 6178 5f76  t_progress_max_v
+00003440: 616c 7565 2831 3530 2c61 6c6c 3d54 7275  alue(150,all=Tru
+00003450: 6529 0d0a 0d0a 2320 746f 2063 6861 6e67  e)....# to chang
+00003460: 6520 6175 746f 2069 6e63 7265 6d65 6e74  e auto increment
+00003470: 2076 616c 7565 206f 6620 6375 7374 6f6d   value of custom
+00003480: 2074 6578 7473 0d0a 7465 726d 696e 616c   texts..terminal
+00003490: 5f63 6f6e 7472 6f6c 2e73 6574 5f70 726f  _control.set_pro
+000034a0: 6772 6573 735f 696e 635f 7661 6c75 6528  gress_inc_value(
+000034b0: 352c 2270 726f 6772 6573 735f 6b65 7922  5,"progress_key"
+000034c0: 290d 0a74 6572 6d69 6e61 6c5f 636f 6e74  )..terminal_cont
+000034d0: 726f 6c2e 7365 745f 7072 6f67 7265 7373  rol.set_progress
+000034e0: 5f69 6e63 5f76 616c 7565 2835 2c61 6c6c  _inc_value(5,all
+000034f0: 3d54 7275 6529 0d0a 0d0a 2320 746f 2063  =True)....# to c
+00003500: 6861 6e67 6520 7465 7874 2076 616c 7565  hange text value
+00003510: 206f 6620 6375 7374 6f6d 2074 6578 7473   of custom texts
+00003520: 0d0a 7465 726d 696e 616c 5f63 6f6e 7472  ..terminal_contr
+00003530: 6f6c 2e73 6574 5f70 726f 6772 6573 735f  ol.set_progress_
+00003540: 7465 7874 2822 5b72 445d 5468 6973 2069  text("[rD]This i
+00003550: 7320 5465 7874 5b30 5d22 2c22 7072 6f67  s Text[0]","prog
+00003560: 7265 7373 5f6b 6579 2229 0d0a 7465 726d  ress_key")..term
+00003570: 696e 616c 5f63 6f6e 7472 6f6c 2e73 6574  inal_control.set
+00003580: 5f70 726f 6772 6573 735f 7465 7874 2822  _progress_text("
+00003590: 5b72 445d 5468 6973 2069 7320 5465 7874  [rD]This is Text
+000035a0: 5b30 5d22 2c61 6c6c 3d54 7275 6529 0d0a  [0]",all=True)..
+000035b0: 0d0a 2320 746f 2063 6861 6e67 6520 6f72  ..# to change or
+000035c0: 2061 6464 2063 7573 746f 6d20 7661 6c75   add custom valu
+000035d0: 6520 6f66 2063 7573 746f 6d20 7465 7874  e of custom text
+000035e0: 730d 0a74 6572 6d69 6e61 6c5f 636f 6e74  s..terminal_cont
+000035f0: 726f 6c2e 7365 745f 6375 7374 6f6d 5f76  rol.set_custom_v
+00003600: 616c 7565 2822 6b65 7931 222c 2276 616c  alue("key1","val
+00003610: 7565 3122 2c22 7072 6f67 7265 7373 5f6b  ue1","progress_k
+00003620: 6579 2229 0d0a 7465 726d 696e 616c 5f63  ey")..terminal_c
+00003630: 6f6e 7472 6f6c 2e73 6574 5f63 7573 746f  ontrol.set_custo
+00003640: 6d5f 7661 6c75 6528 226b 6579 3122 2c22  m_value("key1","
+00003650: 7661 6c75 6531 222c 616c 6c3d 5472 7565  value1",all=True
+00003660: 290d 0a0d 0a23 2d2d 2d2d 2d2d 2d2d 2d2d  )....#----------
+00003670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+00003690: 2320 6e6f 7720 746f 2075 7064 6174 6520  # now to update 
+000036a0: 7072 6f67 7265 7373 2076 616c 7565 0d0a  progress value..
+000036b0: 0d0a 2320 7468 6973 2066 756e 6374 696f  ..# this functio
+000036c0: 6e20 6d6f 7265 2063 6f6e 7472 6f6c 2069  n more control i
+000036d0: 6e20 7570 6461 7465 0d0a 7465 726d 696e  n update..termin
+000036e0: 616c 5f63 6f6e 7472 6f6c 2e75 7064 6174  al_control.updat
+000036f0: 6528 0d0a 2020 2020 7661 6c75 6520 3d20  e(..    value = 
+00003700: 3133 2c20 2320 6966 206e 6f20 7072 6f67  13, # if no prog
+00003710: 7265 7373 2076 616c 7565 2c20 6c65 6176  ress value, leav
+00003720: 6520 6974 0d0a 2020 2020 7072 6f67 7265  e it..    progre
+00003730: 7373 5f6b 6579 3d22 7072 6f67 7265 7373  ss_key="progress
+00003740: 5f6b 6579 222c 2023 2069 6620 6e6f 2061  _key", # if no a
+00003750: 6c6c 2c20 6c65 6176 6520 6974 0d0a 2020  ll, leave it..  
+00003760: 2020 616c 6c3d 5472 7565 206f 7220 4661    all=True or Fa
+00003770: 6c73 652c 0d0a 2020 2020 6375 7374 6f6d  lse,..    custom
+00003780: 5f76 616c 7565 733d 7b0d 0a20 2020 2020  _values={..     
+00003790: 2020 2022 6b65 7931 223a 2276 616c 7565     "key1":"value
+000037a0: 3122 2c0d 0a20 2020 2020 2020 2022 6b65  1",..        "ke
+000037b0: 7932 223a 2276 616c 7565 3222 0d0a 2020  y2":"value2"..  
+000037c0: 2020 7d0d 0a29 0d0a 2320 6966 2075 2077    }..)..# if u w
+000037d0: 616e 7420 746f 2061 7574 6f20 7570 6461  ant to auto upda
+000037e0: 7465 2075 7369 6e67 2060 696e 6360 2076  te using `inc` v
+000037f0: 616c 7565 206a 7573 7420 6361 6c6c 2074  alue just call t
+00003800: 6869 730d 0a74 6572 6d69 6e61 6c5f 636f  his..terminal_co
+00003810: 6e74 726f 6c2e 696e 6372 6561 7365 5f70  ntrol.increase_p
+00003820: 726f 6772 6573 7328 2270 726f 6772 6573  rogress("progres
+00003830: 735f 6b65 7922 290d 0a74 6572 6d69 6e61  s_key")..termina
+00003840: 6c5f 636f 6e74 726f 6c2e 696e 6372 6561  l_control.increa
+00003850: 7365 5f70 726f 6772 6573 7328 616c 6c3d  se_progress(all=
+00003860: 5472 7565 290d 0a0d 0a23 2d2d 2d2d 2d2d  True)....#------
+00003870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003890: 2d2d 0d0a 2320 6e6f 7720 746f 2070 7269  --..# now to pri
+000038a0: 6e74 2026 2063 6865 636b 2070 726f 6772  nt & check progr
+000038b0: 6573 7320 7661 6c75 650d 0a23 2074 6f20  ess value..# to 
+000038c0: 7072 696e 7420 616c 6c20 7072 6f67 7265  print all progre
+000038d0: 7373 2074 6578 7420 7769 7468 2063 6f6c  ss text with col
+000038e0: 6f72 697a 6520 6d6f 6465 0d0a 7465 726d  orize mode..term
+000038f0: 696e 616c 5f63 6f6e 7472 6f6c 2e70 7269  inal_control.pri
+00003900: 6e74 5f70 726f 6772 6573 7328 290d 0a23  nt_progress()..#
+00003910: 2074 6f20 6368 6563 6b20 6973 2070 726f   to check is pro
+00003920: 6772 6573 7320 6669 6e69 7368 206f 7220  gress finish or 
+00003930: 6e6f 740d 0a74 6572 6d69 6e61 6c5f 636f  not..terminal_co
+00003940: 6e74 726f 6c2e 6973 5f70 726f 6772 6573  ntrol.is_progres
+00003950: 735f 6669 6e69 7368 2822 7072 6f67 7265  s_finish("progre
+00003960: 7373 5f6b 6579 2229 0d0a 7465 726d 696e  ss_key")..termin
+00003970: 616c 5f63 6f6e 7472 6f6c 2e69 735f 7072  al_control.is_pr
+00003980: 6f67 7265 7373 5f66 696e 6973 6828 616c  ogress_finish(al
+00003990: 6c3d 5472 7565 290d 0a60 6060 0d0a 2323  l=True)..```..##
+000039a0: 204f 7574 7075 743a 0d0a 215b 5072 6f67   Output:..![Prog
+000039b0: 7265 7373 4261 7220 4749 465d 2868 7474  ressBar GIF](htt
+000039c0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000039d0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f4a  sercontent.com/J
+000039e0: 6f30 5830 312f 414e 5349 436f 6e74 726f  o0X01/ANSIContro
+000039f0: 6c6c 6572 2f6d 6169 6e2f 7465 7374 732f  ller/main/tests/
+00003a00: 7465 7374 5f70 726f 6772 6573 732e 6769  test_progress.gi
+00003a10: 6629 0d0a 2323 2052 6566 0d0a 5f5f 5f5f  f)..## Ref..____
+00003a20: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 0d0a 2d20  ____________..- 
+00003a30: 6874 7470 733a 2f2f 6769 7374 2e67 6974  https://gist.git
+00003a40: 6875 622e 636f 6d2f 666e 6b79 2f34 3538  hub.com/fnky/458
+00003a50: 3731 3933 3433 6161 6264 3031 6366 6231  719343aabd01cfb1
+00003a60: 3761 3361 3466 3732 3936 3739 3723 6573  7a3a4f7296797#es
+00003a70: 6361 7065 0d0a 5f5f 5f5f 5f5f 5f5f 5f5f  cape..__________
+00003a80: 5f5f 5f5f 5f5f 0d0a 2323 2054 6573 7473  ______..## Tests
+00003a90: 0d0a 2a20 e29c 8520 6057 696e 646f 7773  ..* ... `Windows
+00003aa0: 2031 3120 2620 3130 2026 2037 600d 0a20   11 & 10 & 7`.. 
+00003ab0: 202a 2077 6f72 6b20 7769 7468 206e 6f20   * work with no 
+00003ac0: 6973 7375 650d 0a2a 20f0 9f91 8d20 604c  issue..* .... `L
+00003ad0: 696e 7578 600d 0a20 202a 2077 6f72 6b20  inux`..  * work 
+00003ae0: 6275 7420 2c20 6d61 7962 6520 6973 7375  but , maybe issu
+00003af0: 6520 6170 7065 6172 0d0a 2020 2a20 5374  e appear..  * St
+00003b00: 696c 6c20 576f 726b 206f 6e20 6974 0d0a  ill Work on it..
+00003b10: 2a20 f09f 94a7 2060 5465 726d 7578 600d  * .... `Termux`.
+00003b20: 0a20 202a 2053 6f6d 6520 4665 6174 7572  .  * Some Featur
+00003b30: 6573 204e 6565 6420 526f 6f74 6564 2044  es Need Rooted D
+00003b40: 6576 6963 650d 0a20 202a 2053 7469 6c6c  evice..  * Still
+00003b50: 2057 6f72 6b20 6f6e 2069 740d 0a5f 5f5f   Work on it..___
+00003b60: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f0d 0a23  _____________..#
+00003b70: 2323 2060 6966 2075 2066 6163 6520 616e  ## `if u face an
+00003b80: 7920 6973 7375 6520 646f 6e74 2062 6520  y issue dont be 
+00003b90: 7368 7920 2c20 7361 7920 6974 600d 0a23  shy , say it`..#
+00003ba0: 2320 4c69 6365 6e73 650d 0a0d 0a2a 2a4d  # License....**M
+00003bb0: 4954 2a2a 0d0a 2a2a 436f 7079 7269 6768  IT**..**Copyrigh
+00003bc0: 7420 2863 2920 3230 3233 205b 4a6f 4f78  t (c) 2023 [JoOx
+00003bd0: 3031 5d2a 2a0d 0a0d 0a                   01]**....
```

### Comparing `ANSIController-1.0.8/LICENSE` & `ANSIController-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ANSIController-1.0.8/PKG-INFO` & `ANSIController-1.0.9/ANSIController.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANSIController
-Version: 1.0.8
+Version: 1.0.9
 Summary: Basic Python Module to control & color & style text in terminal
 Home-page: https://github.com/jo0x01/ansicontroller
 Author: JoOx01
 Author-email: forsell450@gmail.com
 License: MIT
 Keywords: ansi,terminal,ansi_terminal,ANSIControl,ANSIController,ASNI,ansicontroller
 Classifier: Development Status :: 3 - Alpha
@@ -61,30 +61,32 @@
 if u face any issue write it
 </div>
 <br>
 
 [![PyPi](https://img.shields.io/badge/-PyPi-blue.svg?logo=pypi&labelColor=555555&style=for-the-badge)](https://pypi.org/project/ANSIController "PyPi") [![License: license](https://img.shields.io/badge/-license-blue.svg?style=for-the-badge)](LICENSE "License")
 
 [More Info About ANSI Escape Codes](`https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797#escape`)
+
+## Tool Snap
+_______________
+![Alt Text](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/tool.png)
+
 ## Features
 ------------------------------
 `ANSI Controller` Features:
 - Move Cursor Right or left or top or down or postion in terminal screen
 - Colorize any text u want in terminal
 - Change Style of terminal printing text , bold ,italic , etc...
-
+- MultiProgress in same time
 ## Tech
 ------------------------------
-
-[More Info About ANSI Escape Codes](`https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797#escape`)
 `ANSI Controller` uses a number of open source projects to work properly:
 - [keyboard] - pypi module `https://pypi.org/project/keyboard/`
-- And of course `ANSI Controller` itself is open source.
- on GitHub.
-
+- `ANSI Controller` itself is open source on GitHub.
+- `More Info About ANSI Escape Codes: `https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797#escape
 ## Installation
 ------------------------------
 
 `ANSI Controller` requires [pip](https://pypi.org/) to install.
 Install the dependencies and devDependencies and start the script.
 ### Windows
 ```bash
@@ -125,15 +127,26 @@
     - [+] `dim:`                `D,dim,2`
     - [+] `italic:`             `I,italic,3`
     - [+] `underline:`          `U,underline,4`
     - [+] `blinking:`           `L,blinking,5`
     - [+] `reverse:`            `R,reverse,7`
     - [+] `hidden:`             `H,hidden,8`
     - [+] `strikethrough:`      `S,strikethrough,9`
-
+- #### ProgressBar: add `%{char}%`
+    - [+] `c:`                  `current progress value`
+    - [+] `m:`                  `max progress value`
+    - [+] `p:`                  `percent progress value`
+    - [+] `b:`                  `bar progress value`
+    - [+] `f:`                  `print full bar with all info`
+    - [+] `your_custom_key:`    `your_custom_value`
+- #### More Control in ProgressBar:
+    - [+] `txt:`                `key of string value inside`
+    - [+] `mx:`                 `max value default is 100`
+    - [+] `inc:`                `increamnt value defualt is 1`
+    - [+] `custom:`             `dict object with custom keys`
 ## Examples & Usage
 ____________
 > Terminal Execute
 ### windows
 ```shell
 python -m ANSIController
 ```
@@ -165,14 +178,18 @@
 # print ids colors background and normal from 0 to 255
 Terminal.print_id_colors()
 # will print all pervious in same time
 Terminal.print_test()
 # Try it
 Terminal.game()
 ```
+## Output:
+![Alt Text](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/test_styles.png)
+![Alt Text](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/test_colors.png)
+![Alt Text](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/test_ids.png)
 ### to move cursor
 ```python
 # this will make cursor move to up 3 lines
 terminal_control.move_to_up(steps=3)    
 
 # After move to up 3 lines , cursor will start from 0 postion of line
 terminal_control.move_to_up(steps=3,start_line=True)
@@ -241,14 +258,16 @@
     "[d]This is default[0]",
     "[bb]This is Bright Black[0]",
     "[br]This is Bright Red[0]",
 ]
 for text in colorize_texts_using_color_char:
     print(terminal_control.colorize(text,sep))
 ```
+## Output:
+![Alt Text](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/test_colors_out.png)
 > Now Using style only
 > 
 ```python
 sep = "[]"
 colorize_texts_using_style_char = [
     "[B]This is Bold[0]",
     "[D]This is Dim[0]",
@@ -258,14 +277,16 @@
     "[R]This is reverse[0]",
     "[H]This is Hidden[0]",
     "[S]This is Strikethrogh[0]",
 ]
 for text in colorize_texts_using_style_char:
     print(terminal_control.colorize(text,sep))
 ```
+## Output:
+![Alt Text](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/test_styles_out.png)
 > Now Using Colors & style
 > 
 ```python
 sep = "[]"
 colorize_texts_using_style_color_char = [
     "[Br]This is Bold and Red[0]",
     "[Dy]This is Dim and Yellow[0]",
@@ -275,20 +296,129 @@
     "[Rbr]This is reverse and Bright Red[0]",
     "[Hby]This is Hidden and Bright Yellow[0]",
     "[Sbc]This is Strikethrogh and Bright Cyan[0]",
 ]
 for text in colorize_texts_using_style_color_char:
     print(terminal_control.colorize(text,sep))
 ```
+## Output:
+![Alt Text](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/test_colors_style_out.png)
 > To add Background  just add `X,x` to the block `[xrB]` i want background red and bold style
 > 
 > Note: you can use `terminal_control.print_colorize` without print
 > 
 > `[0],[z],[Z],[Reset]` is to reset to default color&style in terminal
-
+> 
+> 
+### - Using multiprogressbar
+```python
+# add_progress: take list of text
+# take too dict
+#example with list
+terminal_control.add_progress([
+    "[rB]test1[0]",
+    "[w]test2[0]",
+    "[cI]test3[0]",
+    "[yD]test4[0]",
+])
+# example with dict
+# take `progress_name`` to access later
+# `txt` key is the progress text
+terminal_control.add_progress({
+    "progress1":{"txt": "[rB]test1[0]"},
+    "progress2":{"txt": "[w]test2[0]"},
+    "progress3":{"txt": "[cI]test3[0]"},
+    "progress4":{"txt": "[yD]test4[0]"},
+})
+# now if i want to add progress value and update values
+#example with list
+# access by index
+terminal_control.add_progress([
+    "[rB]test1: (%c%/%m%)[0]",
+    "[w]test2: %b% (%c%/%m%)[0]",
+    "[cI]test3: %b% %p% (%c%/%m%)[0]",
+    "[yD]test4: %f% [0]",
+])
+#example with more control dict
+terminal_control.add_progress({
+    "progress1":{
+        "txt": "[rB]test1: (%c%/%m%) - (%key1%,%key2%,%status_test%)[0]",
+        "mx":200,
+        "inc":5,
+        "custom":{
+            "key1":10,
+            "key2":"test",
+            "status_test":"Good"
+        }
+    },
+    # sometimes no need for `mx` or `inc`
+    "progress2":{
+        "txt": "[w]test2: %b% (%c%/%m%)- (%key1%,%key2%)[0]",
+        "custom":{
+            "key1":10,
+            "key2":"test",
+            "status_test":"Good"
+        }
+    }
+})
+
+#----------------------------------------
+# now to update progress bar values
+
+# progress_key = `if list will be index`
+# progress_key = `if dict will be name`
+# `all` argument mean if u want to change in all texts
+# default of all is False
+
+# to change max value of custom texts
+terminal_control.set_progress_max_value(150,"progress_key")
+terminal_control.set_progress_max_value(150,all=True)
+
+# to change auto increment value of custom texts
+terminal_control.set_progress_inc_value(5,"progress_key")
+terminal_control.set_progress_inc_value(5,all=True)
+
+# to change text value of custom texts
+terminal_control.set_progress_text("[rD]This is Text[0]","progress_key")
+terminal_control.set_progress_text("[rD]This is Text[0]",all=True)
+
+# to change or add custom value of custom texts
+terminal_control.set_custom_value("key1","value1","progress_key")
+terminal_control.set_custom_value("key1","value1",all=True)
+
+#----------------------------------------
+# now to update progress value
+
+# this function more control in update
+terminal_control.update(
+    value = 13, # if no progress value, leave it
+    progress_key="progress_key", # if no all, leave it
+    all=True or False,
+    custom_values={
+        "key1":"value1",
+        "key2":"value2"
+    }
+)
+# if u want to auto update using `inc` value just call this
+terminal_control.increase_progress("progress_key")
+terminal_control.increase_progress(all=True)
+
+#----------------------------------------
+# now to print & check progress value
+# to print all progress text with colorize mode
+terminal_control.print_progress()
+# to check is progress finish or not
+terminal_control.is_progress_finish("progress_key")
+terminal_control.is_progress_finish(all=True)
+```
+## Output:
+![ProgressBar GIF](https://raw.githubusercontent.com/Jo0X01/ANSIController/main/tests/test_progress.gif)
+## Ref
+________________
+- https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797#escape
 ________________
 ## Tests
 * ✅ `Windows 11 & 10 & 7`
   * work with no issue
 * 👍 `Linux`
   * work but , maybe issue appear
   * Still Work on it
```

### Comparing `ANSIController-1.0.8/setup.py` & `ANSIController-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 __author__ = "JoOx01"
 __pkg_name__ = "ANSIController"
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __desc__ = """Basic Python Module to control & color & style text in terminal"""
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=__pkg_name__,
```

