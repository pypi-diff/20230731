# Comparing `tmp/DmxOscServer-1.0.0.tar.gz` & `tmp/DmxOscServer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-x9o9v862/DmxOscServer-1.0.0.tar", last modified: Sun Jul 30 19:22:35 2023, max compression
+gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-7t31qi_v/DmxOscServer-1.0.1.tar", last modified: Mon Jul 31 18:19:19 2023, max compression
```

## Comparing `DmxOscServer-1.0.0.tar` & `DmxOscServer-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/
--rw-r--r--   0 pi        (1000) pi        (1000)     1688 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1256 2023-07-30 18:37:19.000000 DmxOscServer-1.0.0/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      861 2023-07-30 18:28:11.000000 DmxOscServer-1.0.0/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/DmxOscServer/
--rw-r--r--   0 pi        (1000) pi        (1000)     1857 2023-07-30 18:23:58.000000 DmxOscServer-1.0.0/src/DmxOscServer/DmxOscServer.py
--rw-r--r--   0 pi        (1000) pi        (1000)      731 2023-07-30 18:18:11.000000 DmxOscServer-1.0.0/src/DmxOscServer/Fixture.py
--rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.0/src/DmxOscServer/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/DmxOscServer.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1688 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/DmxOscServer.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/DmxOscServer.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/DmxOscServer.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/DmxOscServer.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-07-30 19:22:35.000000 DmxOscServer-1.0.0/src/DmxOscServer.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2265 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1829 2023-07-31 18:18:06.000000 DmxOscServer-1.0.1/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      865 2023-07-31 18:17:17.000000 DmxOscServer-1.0.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3450 2023-07-31 18:10:14.000000 DmxOscServer-1.0.1/src/DmxOscServer/DmxOscServer.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1609 2023-07-31 17:31:17.000000 DmxOscServer-1.0.1/src/DmxOscServer/Fixture.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.1/src/DmxOscServer/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2265 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/top_level.txt
```

### Comparing `DmxOscServer-1.0.0/PKG-INFO` & `DmxOscServer-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: DmxOscServer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python Lib to create a DMX compatible OSC server with handlers
-Home-page: https://github.com/Miniontoby/DmxOscServer
+Home-page: https://dmxoscserver.readthedocs.io/en/latest/
 Author: Miniontoby
 Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
 Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
 Keywords: dmx,osc,server
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # DMX OSC Server
 
 DMX OSC Server is a python lib to make it easier to create OSC Servers for the DMX Protocol.
 
 It allows you to register fixtures are the wanted universe, starting address and channels.
@@ -25,35 +25,57 @@
 ```
 
 ## Get Started
 
 To create a simple DMX OSC Server that will listen on 0.0.0.0:9000 you can use this code:
 
 ```py
-from DmxOscServer import DmxOscServer, Fixture
+from DmxOscServer import DmxOscServer
+
+server = DmxOscServer()
 
+# Register a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.new_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
     fixture.values[address] = args[0]
     print (fixture.values)
 
-server = DmxOscServer()
-server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 of universe 0
 server.run()
 ```
 
 
-To change the IP and/or port, you can add them to the DmxOscServer initializer
+To change the IP and/or port, you can specify that at the `.run()` method
+
+```py
+server.run("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
+```
+
+
+It is also possible to use the `Fixture` class and the `add_fixture` method
 
 ```py
-server = DmxOscServer("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
+from DmxOscServer import DmxOscServer, Fixture
+
+def my_rgb_handler(fixture, address, *args):
+    fixture.values[address] = args[0]
+    print (fixture.values)
+
+server = DmxOscServer()
+server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 at universe 0
 ```
 
 
-You can add multiple fixtures at once using:
+And for the `add_fixture` method, you can also add multiple fixtures at once using:
 
 ```py
+from DmxOscServer import DmxOscServer, Fixture
 server = DmxOscServer()
 server.add_fixtures(
     Fixture(0, 0, 3, my_rgb_handler), # Register a 3 channel Fixture at address 0 of universe 0
     Fixture(0, 3, 3, my_rgb_handler), # Register a 3 channel Fixture at address 3 of universe 0
 )
 ```
+
+
+# More Documentation
+
+More Documentation can be found at https://dmxoscserver.readthedocs.io/en/latest/
```

### Comparing `DmxOscServer-1.0.0/README.md` & `DmxOscServer-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -13,35 +13,57 @@
 ```
 
 ## Get Started
 
 To create a simple DMX OSC Server that will listen on 0.0.0.0:9000 you can use this code:
 
 ```py
-from DmxOscServer import DmxOscServer, Fixture
+from DmxOscServer import DmxOscServer
+
+server = DmxOscServer()
 
+# Register a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.new_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
     fixture.values[address] = args[0]
     print (fixture.values)
 
-server = DmxOscServer()
-server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 of universe 0
 server.run()
 ```
 
 
-To change the IP and/or port, you can add them to the DmxOscServer initializer
+To change the IP and/or port, you can specify that at the `.run()` method
+
+```py
+server.run("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
+```
+
+
+It is also possible to use the `Fixture` class and the `add_fixture` method
 
 ```py
-server = DmxOscServer("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
+from DmxOscServer import DmxOscServer, Fixture
+
+def my_rgb_handler(fixture, address, *args):
+    fixture.values[address] = args[0]
+    print (fixture.values)
+
+server = DmxOscServer()
+server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 at universe 0
 ```
 
 
-You can add multiple fixtures at once using:
+And for the `add_fixture` method, you can also add multiple fixtures at once using:
 
 ```py
+from DmxOscServer import DmxOscServer, Fixture
 server = DmxOscServer()
 server.add_fixtures(
     Fixture(0, 0, 3, my_rgb_handler), # Register a 3 channel Fixture at address 0 of universe 0
     Fixture(0, 3, 3, my_rgb_handler), # Register a 3 channel Fixture at address 3 of universe 0
 )
 ```
+
+
+# More Documentation
+
+More Documentation can be found at https://dmxoscserver.readthedocs.io/en/latest/
```

### Comparing `DmxOscServer-1.0.0/setup.py` & `DmxOscServer-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="DmxOscServer",
-    version="1.0.0",
+    version="1.0.1",
     description="A Python Lib to create a DMX compatible OSC server with handlers",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Miniontoby/DmxOscServer",
+    url="https://dmxoscserver.readthedocs.io/en/latest/",
     author="Miniontoby",
     keywords="dmx, osc, server",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.5",
     install_requires=["python-osc"],
     project_urls={
         "Bug Reports": "https://github.com/Miniontoby/DmxOscServer/issues",
         "Source": "https://github.com/Miniontoby/DmxOscServer",
     },
 )
```

### Comparing `DmxOscServer-1.0.0/src/DmxOscServer.egg-info/PKG-INFO` & `DmxOscServer-1.0.1/src/DmxOscServer.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: DmxOscServer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python Lib to create a DMX compatible OSC server with handlers
-Home-page: https://github.com/Miniontoby/DmxOscServer
+Home-page: https://dmxoscserver.readthedocs.io/en/latest/
 Author: Miniontoby
 Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
 Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
 Keywords: dmx,osc,server
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # DMX OSC Server
 
 DMX OSC Server is a python lib to make it easier to create OSC Servers for the DMX Protocol.
 
 It allows you to register fixtures are the wanted universe, starting address and channels.
@@ -25,35 +25,57 @@
 ```
 
 ## Get Started
 
 To create a simple DMX OSC Server that will listen on 0.0.0.0:9000 you can use this code:
 
 ```py
-from DmxOscServer import DmxOscServer, Fixture
+from DmxOscServer import DmxOscServer
+
+server = DmxOscServer()
 
+# Register a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.new_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
     fixture.values[address] = args[0]
     print (fixture.values)
 
-server = DmxOscServer()
-server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 of universe 0
 server.run()
 ```
 
 
-To change the IP and/or port, you can add them to the DmxOscServer initializer
+To change the IP and/or port, you can specify that at the `.run()` method
+
+```py
+server.run("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
+```
+
+
+It is also possible to use the `Fixture` class and the `add_fixture` method
 
 ```py
-server = DmxOscServer("10.10.123.5", 1234) # Will listen on 10.10.123.5:1234
+from DmxOscServer import DmxOscServer, Fixture
+
+def my_rgb_handler(fixture, address, *args):
+    fixture.values[address] = args[0]
+    print (fixture.values)
+
+server = DmxOscServer()
+server.add_fixture(Fixture(0, 0, 3, my_rgb_handler)) # Register a 3 channel Fixture at address 0 at universe 0
 ```
 
 
-You can add multiple fixtures at once using:
+And for the `add_fixture` method, you can also add multiple fixtures at once using:
 
 ```py
+from DmxOscServer import DmxOscServer, Fixture
 server = DmxOscServer()
 server.add_fixtures(
     Fixture(0, 0, 3, my_rgb_handler), # Register a 3 channel Fixture at address 0 of universe 0
     Fixture(0, 3, 3, my_rgb_handler), # Register a 3 channel Fixture at address 3 of universe 0
 )
 ```
+
+
+# More Documentation
+
+More Documentation can be found at https://dmxoscserver.readthedocs.io/en/latest/
```

