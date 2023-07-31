# Comparing `tmp/cm2py-0.2.7.tar.gz` & `tmp/cm2py-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.2.7.tar", last modified: Tue Jul 25 10:50:57 2023, max compression
+gzip compressed data, was "cm2py-0.2.8.tar", last modified: Mon Jul 31 08:14:04 2023, max compression
```

## Comparing `cm2py-0.2.7.tar` & `cm2py-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.207667 cm2py-0.2.7/
--rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     3012 2023-07-25 10:50:57.206671 cm2py-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1189 2023-07-15 07:50:59.000000 cm2py-0.2.7/README.md
--rw-rw-rw-   0        0        0      675 2023-07-25 10:50:32.000000 cm2py-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 10:50:57.208669 cm2py-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.142669 cm2py-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.161672 cm2py-0.2.7/src/cm2py/
--rw-rw-rw-   0        0        0      237 2023-07-19 11:34:20.000000 cm2py-0.2.7/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     6419 2023-07-25 10:50:18.000000 cm2py-0.2.7/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.201673 cm2py-0.2.7/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0     3012 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.204672 cm2py-0.2.7/tests/
--rw-rw-rw-   0        0        0     2374 2023-07-19 09:48:55.000000 cm2py-0.2.7/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:14:04.294495 cm2py-0.2.8/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-07-31 08:14:04.293495 cm2py-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-07-15 07:50:59.000000 cm2py-0.2.8/README.md
+-rw-rw-rw-   0        0        0      675 2023-07-31 08:13:23.000000 cm2py-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 08:14:04.294495 cm2py-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 08:14:04.234496 cm2py-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 08:14:04.255496 cm2py-0.2.8/src/cm2py/
+-rw-rw-rw-   0        0        0      237 2023-07-25 10:54:54.000000 cm2py-0.2.8/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     6612 2023-07-31 08:13:27.000000 cm2py-0.2.8/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:14:04.286503 cm2py-0.2.8/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-07-31 08:14:04.000000 cm2py-0.2.8/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-31 08:14:04.000000 cm2py-0.2.8/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 08:14:04.000000 cm2py-0.2.8/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-31 08:14:04.000000 cm2py-0.2.8/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 08:14:04.000000 cm2py-0.2.8/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 08:14:04.290499 cm2py-0.2.8/tests/
+-rw-rw-rw-   0        0        0     2553 2023-07-31 08:13:15.000000 cm2py-0.2.8/tests/test_app.py
```

### Comparing `cm2py-0.2.7/LICENSE` & `cm2py-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.7/PKG-INFO` & `cm2py-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.7
+Version: 0.2.8
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.2.7/README.md` & `cm2py-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.7/pyproject.toml` & `cm2py-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `cm2py-0.2.7/src/cm2py/cm2py.py` & `cm2py-0.2.8/src/cm2py/cm2py.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,44 +10,48 @@
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/05/21"
 __deprecated__ = False
 __email__ = "qestudios17@example.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 import re
 from uuid import UUID, uuid4
 import math
 
 
 class Save:
     """A class to represent a save, which can be modified."""
 
     def __init__(self):
         self.blocks = []
         self.connections = {}
+        self.blockCount = 0
+        self.connectionCount = 0
 
     def addBlock(self, blockId, pos, state=False, properties=None, snapToGrid=True):
         """Add a block to the save."""
         if snapToGrid:
             newBlock = Block(blockId, tuple([int(math.floor(i)) for i in pos]), state=state, properties=properties)
         else:
             newBlock = Block(blockId, pos, state=state, properties=properties)
         self.blocks.append(newBlock)
+        self.blockCount += 1
         return newBlock
 
     def addConnection(self, source, target):
         """Add a connection to the save."""
         newConnection = Connection(source, target)
         if str(newConnection.target.uuid) in self.connections:
             self.connections[str(newConnection.target.uuid)].append(newConnection)
         else:
             self.connections[str(newConnection.target.uuid)] = [newConnection]
+        self.connectionCount += 1
         return newConnection
 
     def exportSave(self):
         """Export the save to a Circuit Maker 2 save string."""
         string = ""
         for b in self.blocks:
             if b.properties:
@@ -70,24 +74,26 @@
         assert blockRef in self.blocks, "block does not exist in save"
         for c in self.connections.values():
             for n in c:
                 if n.source.uuid == blockRef.uuid or n.target.uuid == blockRef.uuid:
                     del self.connections[str(n.target.uuid)][self.connections[str(n.target.uuid)].index(n)]
                     break
         del self.blocks[self.blocks.index(blockRef)]
+        self.blockCount -= 1
         return
 
     def deleteConnection(self, connectionRef):
         """Delete a connection from the save."""
         assert isinstance(connectionRef, Connection), "connectionRef must be a Connection object"
         assert connectionRef in (n for c in self.connections.values() for n in c)
         for c in self.connections.values():
             for n in c:
                 if connectionRef == n:
                     del self.connections[str(n.target.uuid)][self.connections[str(n.target.uuid)].index(n)]
+        self.connectionCount -= 1
 
 
 class Block:
     def __init__(self, blockId, pos, state=False, properties=None):
         assert isinstance(blockId, int) and 0 <= blockId <= 13, "blockId must be an integer between 0 and 11"
         assert (
             isinstance(pos, tuple)
```

### Comparing `cm2py-0.2.7/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.2.8/src/cm2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.7
+Version: 0.2.8
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.2.7/tests/test_app.py` & `cm2py-0.2.8/tests/test_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
 from src import cm2py as cm2
 
-
 def test_addBlocks():
     save = cm2.Save()
 
     save.addBlock(cm2.NOR, (0, 0, 0))
     save.addBlock(cm2.AND, (1, 0, 0))
     save.addBlock(cm2.OR, (2, 0, 0))
     save.addBlock(cm2.XOR, (3, 0, 0))
@@ -77,10 +76,19 @@
 
     b1 = save.addBlock(cm2.LED, (0, 0, 0), properties=[255, 0, 0])
 
     save.exportSave()
 
 
 def test_importSave():
-    string = "7,1,17,0,6,;7,0,-9,0,3,1.00;7,0,20,0,6,1.00;7,0,4,0,-8,10000.00;7,0,19,0,4,;7,0,0,0,-4,100.00;7,0,17,0,2,;7,1,20,0,2,;7,0,17,0,4,;7,1,20,0,5,;7,0,-1,0,-5,;7,0,0,0,-6,1000.00;7,1,18,0,4,;7,0,6,0,-8,10000.00;7,0,-5,0,-5,1.00;7,1,17,0,5,;7,0,0,0,-2,10.00;7,1,20,0,4,;7,0,17,0,3,;7,0,8,0,-8,;7,0,-9,0,1,10.00;7,0,2,0,-8,10000.00;7,0,0,0,-8,10000.00;7,0,-9,0,-1,100.00;7,0,-9,0,-5,10000.00;7,0,0,0,0,1.00;7,1,20,0,3,;7,0,-7,0,-5,10000.00;7,0,-3,0,-5,10000.00;7,0,-9,0,-3,1000.00?16,1;29,11;6,12;24,30;19,9;28,15;21,24;9,16;22,4;25,28;14,20;2,21;26,17;27,8;8,5;1,3;23,22;10,18;30,25;5,13;3,10;7,19;13,7;12,23;18,27;17,6;15,29??"
+    string = ("0,0,0,0,3,;0,0,1,0,3,;0,0,2,0,3,;7,1,17,0,6,;7,0,-9,0,3,1.00;"
+              "7,0,20,0,6,1.00;7,0,4,0,-8,10000.00;7,0,19,0,4,;7,0,0,0,-4,100.00;7,0,17,0,2,;"
+              "7,1,20,0,2,;7,0,17,0,4,;7,1,20,0,5,;7,0,-1,0,-5,;7,0,0,0,-6,1000.00;"
+              "7,1,18,0,4,;7,0,6,0,-8,10000.00;7,0,-5,0,-5,1.00;7,1,17,0,5,;7,0,0,0,-2,10.00;"
+              "7,1,20,0,4,;7,0,17,0,3,;7,0,8,0,-8,;7,0,-9,0,1,10.00;7,0,2,0,-8,10000.00;"
+              "7,0,0,0,-8,10000.00;7,0,-9,0,-1,100.00;7,0,-9,0,-5,10000.00;7,0,0,0,0,1.00;"
+              "7,1,20,0,3,;7,0,-7,0,-5,10000.00;7,0,-3,0,-5,10000.00;7,0,-9,0,-3,1000.00?"
+              "16,1;29,11;6,12;24,30;19,9;28,15;21,24;9,16;22,4;25,28;14,20;2,21;26,17;"
+              "27,8;8,5;1,3;23,22;10,18;30,25;5,13;3,10;7,19;13,7;12,23;18,27;17,6;15,29??")
 
     save = cm2.importSave(string)
+
```

