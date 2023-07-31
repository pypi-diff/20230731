# Comparing `tmp/e2D-0.1.0.tar.gz` & `tmp/e2D-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2D-0.1.0.tar", last modified: Mon Jul 31 16:53:51 2023, max compression
+gzip compressed data, was "e2D-0.1.1.tar", last modified: Mon Jul 31 17:12:11 2023, max compression
```

## Comparing `e2D-0.1.0.tar` & `e2D-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:53:51.593240 e2D-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3081 2023-07-31 16:53:51.593240 e2D-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2488 2023-07-31 16:30:45.000000 e2D-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:53:51.567230 e2D-0.1.0/e2D/
--rw-rw-rw-   0        0        0    39663 2023-07-31 16:41:56.000000 e2D-0.1.0/e2D/__init__.py
--rw-rw-rw-   0        0        0    10446 2023-07-31 16:52:35.000000 e2D-0.1.0/e2D/envs.py
--rw-rw-rw-   0        0        0     3899 2023-07-31 14:51:50.000000 e2D-0.1.0/e2D/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:53:51.591232 e2D-0.1.0/e2D.egg-info/
--rw-rw-rw-   0        0        0     3081 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 16:53:51.000000 e2D-0.1.0/e2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      729 2023-07-31 16:53:51.595228 e2D-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 17:12:11.969078 e2D-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3081 2023-07-31 17:12:11.969078 e2D-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2023-07-31 16:30:45.000000 e2D-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 17:12:11.949453 e2D-0.1.1/e2D/
+-rw-rw-rw-   0        0        0    39663 2023-07-31 16:41:56.000000 e2D-0.1.1/e2D/__init__.py
+-rw-rw-rw-   0        0        0    10427 2023-07-31 17:10:49.000000 e2D-0.1.1/e2D/envs.py
+-rw-rw-rw-   0        0        0     3918 2023-07-31 17:10:43.000000 e2D-0.1.1/e2D/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:12:11.969078 e2D-0.1.1/e2D.egg-info/
+-rw-rw-rw-   0        0        0     3081 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-07-31 17:12:11.969078 e2D-0.1.1/setup.cfg
```

### Comparing `e2D-0.1.0/LICENSE` & `e2D-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e2D-0.1.0/PKG-INFO` & `e2D-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-0.1.0/README.md` & `e2D-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `e2D-0.1.0/e2D/__init__.py` & `e2D-0.1.1/e2D/__init__.py`

 * *Files identical despite different names*

### Comparing `e2D-0.1.0/e2D/envs.py` & `e2D-0.1.1/e2D/envs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .utils import *
-from e2D import *
 import pygame as pg
 
 """  CODE EXAMPLE FOR RootEnv
 from e2D.envs import *
 
 class Env:
     def __init__(self) -> None:
```

### Comparing `e2D-0.1.0/e2D/utils.py` & `e2D-0.1.1/e2D/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pygame as pg
+from e2D import *
 
 KEY_MODE_PRESSED = 0
 KEY_MODE_JUST_PRESSED = 1
 KEY_MODE_JUST_RELEASED = 2
 
 SCANCODES = {"":0,"backspace":8,"tab":9,"return":13,"escape":27,"space":32,"!":33,"\"":34,"#":35,"$":36,"%":37,"&":38,"'":39,"(":40,")":41,"*":42,"+":43,",":44,"-":45,".":46,"/":47,"0":48,"1":49,"2":50,"3":51,"4":52,"5":53,"6":54,"7":55,"8":56,"9":57,":":58,";":59,"<":60,"=":61,">":62,"?":63,"@":64,"[":91,"\\":92,"]":93,"^":94,"_":95,"`":96,"a":97,"b":98,"c":99,"d":100,"e":101,"f":102,"g":103,"h":104,"i":105,"j":106,"k":107,"l":108,"m":109,"n":110,"o":111,"p":112,"q":113,"r":114,"s":115,"t":116,"u":117,"v":118,"w":119,"x":120,"y":121,"z":122,"delete":127,"caps lock":1073741881,"f1":1073741882,"f2":1073741883,"f3":1073741884,"f4":1073741885,"f5":1073741886,"f6":1073741887,"f7":1073741888,"f8":1073741889,"f9":1073741890,"f10":1073741891,"f11":1073741892,"f12":1073741893,"print screen":1073741894,"scroll lock":1073741895,"break":1073741896,"insert":1073741897,"home":1073741898,"page up":1073741899,"end":1073741901,"page down":1073741902,"right":1073741903,"left":1073741904,"down":1073741905,"up":1073741906,"numlock":1073741907,"[/]":1073741908,"[*]":1073741909,"[-]":1073741910,"[+]":1073741911,"enter":1073741912,"[1]":1073741913,"[2]":1073741914,"[3]":1073741915,"[4]":1073741916,"[5]":1073741917,"[6]":1073741918,"[7]":1073741919,"[8]":1073741920,"[9]":1073741921,"[0]":1073741922,"[.]":1073741923,"power":1073741926,"equals":1073741927,"f13":1073741928,"f14":1073741929,"f15":1073741930,"help":1073741941,"menu":1073741942,"sys req":1073741978,"clear":1073741980,"euro":1073742004,"CurrencySubUnit":1073742005,"left ctrl":1073742048,"left shift":1073742049,"left alt":1073742050,"left meta":1073742051,"right ctrl":1073742052,"right shift":1073742053,"right alt":1073742054,"right meta":1073742055,"alt gr":1073742081,"AC Back":1073742094}
 SCANCODES_NUMS = [i for i in SCANCODES.values()]
```

### Comparing `e2D-0.1.0/e2D.egg-info/PKG-INFO` & `e2D-0.1.1/e2D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-0.1.0/setup.cfg` & `e2D-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 3244 0d0a 7665 7273 696f 6e20   = e2D..version 
-00000020: 3d20 302e 312e 300d 0a61 7574 686f 7220  = 0.1.0..author 
+00000020: 3d20 302e 312e 310d 0a61 7574 686f 7220  = 0.1.1..author 
 00000030: 3d20 5269 6363 6172 646f 204d 6172 6961  = Riccardo Maria
 00000040: 6e69 0d0a 6175 7468 6f72 5f65 6d61 696c  ni..author_email
 00000050: 203d 2072 6963 6f6d 6172 6932 3030 3640   = ricomari2006@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
 00000080: 6c69 6272 6172 7920 666f 7220 3244 2067  library for 2D g
 00000090: 616d 6573 2e20 5374 7265 616d 6c69 6e65  ames. Streamline
```

