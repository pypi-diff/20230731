# Comparing `tmp/pyDuotecno-2023.7.3.tar.gz` & `tmp/pyDuotecno-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDuotecno-2023.7.3.tar", last modified: Tue Jul 25 05:50:55 2023, max compression
+gzip compressed data, was "pyDuotecno-2023.7.4.tar", last modified: Mon Jul 31 14:54:51 2023, max compression
```

## Comparing `pyDuotecno-2023.7.3.tar` & `pyDuotecno-2023.7.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.203315 pyDuotecno-2023.7.3/
--rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.7.3/LICENSE
--rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.7.3/MANIFEST.in
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1119 2023-07-25 05:50:55.199981 pyDuotecno-2023.7.3/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)       53 2023-07-25 05:45:41.000000 pyDuotecno-2023.7.3/README.md
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.173313 pyDuotecno-2023.7.3/duotecno/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     5252 2023-07-25 05:50:01.000000 pyDuotecno-2023.7.3/duotecno/controller.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)      125 2023-07-25 04:44:21.000000 pyDuotecno-2023.7.3/duotecno/exceptions.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     2909 2023-07-11 13:11:31.000000 pyDuotecno-2023.7.3/duotecno/node.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     7610 2023-05-15 11:00:00.000000 pyDuotecno-2023.7.3/duotecno/protocol.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     4395 2023-07-25 04:46:29.000000 pyDuotecno-2023.7.3/duotecno/unit.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.176646 pyDuotecno-2023.7.3/examples/
--rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.7.3/examples/read.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.183313 pyDuotecno-2023.7.3/pyDuotecno.egg-info/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1119 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)      626 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1682 2023-07-25 05:45:09.000000 pyDuotecno-2023.7.3/pyproject.toml
--rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.7.3/requirements.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-07-25 05:50:55.203315 pyDuotecno-2023.7.3/setup.cfg
--rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.7.3/setup.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.159978 pyDuotecno-2023.7.3/venv/
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.199981 pyDuotecno-2023.7.3/venv/bin/
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      616 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2html.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      738 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2html4.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1083 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2html5.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      815 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2latex.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      638 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2man.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      804 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2odt.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1742 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      623 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      659 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2s5.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      895 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2xetex.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      624 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2xml.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      692 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rstpep2html.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-31 14:54:51.141186 pyDuotecno-2023.7.4/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.7.4/LICENSE
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.7.4/MANIFEST.in
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1119 2023-07-31 14:54:51.141186 pyDuotecno-2023.7.4/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       53 2023-07-25 05:45:41.000000 pyDuotecno-2023.7.4/README.md
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-31 14:54:51.111184 pyDuotecno-2023.7.4/duotecno/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     4990 2023-07-27 11:08:55.000000 pyDuotecno-2023.7.4/duotecno/controller.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      125 2023-07-25 04:44:21.000000 pyDuotecno-2023.7.4/duotecno/exceptions.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     2909 2023-07-27 11:16:18.000000 pyDuotecno-2023.7.4/duotecno/node.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     7610 2023-05-15 11:00:00.000000 pyDuotecno-2023.7.4/duotecno/protocol.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     4398 2023-07-27 11:18:40.000000 pyDuotecno-2023.7.4/duotecno/unit.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-31 14:54:51.114517 pyDuotecno-2023.7.4/examples/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.7.4/examples/read.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-31 14:54:51.121184 pyDuotecno-2023.7.4/pyDuotecno.egg-info/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1119 2023-07-31 14:54:51.000000 pyDuotecno-2023.7.4/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      626 2023-07-31 14:54:51.000000 pyDuotecno-2023.7.4/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-07-31 14:54:51.000000 pyDuotecno-2023.7.4/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.7.4/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-07-31 14:54:51.000000 pyDuotecno-2023.7.4/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1536 2023-07-31 14:53:58.000000 pyDuotecno-2023.7.4/pyproject.toml
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.7.4/requirements.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-07-31 14:54:51.141186 pyDuotecno-2023.7.4/setup.cfg
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.7.4/setup.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-31 14:54:51.094516 pyDuotecno-2023.7.4/venv/
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-31 14:54:51.137852 pyDuotecno-2023.7.4/venv/bin/
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      616 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      738 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1083 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      815 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      638 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      804 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1742 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      623 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      659 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      895 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      624 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      692 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.4/venv/bin/rstpep2html.py
```

### Comparing `pyDuotecno-2023.7.3/LICENSE` & `pyDuotecno-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/PKG-INFO` & `pyDuotecno-2023.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.7.3/duotecno/controller.py` & `pyDuotecno-2023.7.4/duotecno/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     """
 
     writer: asyncio.StreamWriter = None
     reader: asyncio.StreamReader = None
     readerTask: asyncio.Task
     loginOK: asyncio.Event
     connectionOK: asyncio.Event
-    loadOK: asyncio.Event
     nodes: dict = {}
 
     def get_units(self, unit_type) -> list:
         res = []
         for node in self.nodes.values():
             for unit in node.get_unit_by_type(unit_type):
                 res.append(unit)
@@ -43,19 +42,17 @@
         try:
             self.reader, self.writer = await asyncio.open_connection(host, port)
         except ConnectionError or TimeoutError:
             raise
         # events
         self.connectionOK = asyncio.Event()
         self.loginOK = asyncio.Event()
-        self.loadOK = asyncio.Event()
         # at this point the connection should be ok
         self.connectionOK.set()
         self.loginOK.clear()
-        self.loadOK.clear()
         # start the bus reading task
         self.readerTask = asyncio.Task(self.readTask())
         # start loading, this task will kill itself once finished
         passw = [str(ord(i)) for i in password]
         # send login info
         await self.write(f"[214,3,{len(passw)},{','.join(passw)}]")
         # wait for the login to be ok
@@ -63,46 +60,42 @@
             await asyncio.wait_for(self.loginOK.wait(), timeout=1.0)
             await self.loginOK.wait()
         except TimeoutError:
             raise InvalidPassword()
         # if we are not testing the connection, start scanning
         if not testOnly:
             await self.write("[209,0]")
-            _loadTask = asyncio.Task(self._loadTask())
             try:
-                await asyncio.wait_for(self.loadOK.wait(), timeout=15.0)
+                await asyncio.wait_for(self._loadTask(), timeout=30.0)
             except TimeoutError:
                 raise LoadFailure()
-            finally:
-                _loadTask.cancel()
+            self._log.info("Loading finished")
 
     async def write(self, msg) -> None:
         """Send a message."""
         if self.writer.transport._conn_lost:
             self.connectionOK.clear()
             self._log("ERROR CONNECTION LOST")
             return
         self._log.debug(f"Send: {msg}")
         msg = f"{msg}{chr(10)}"
         self.writer.write(msg.encode())
         await self.writer.drain()
 
     async def _loadTask(self):
         while len(self.nodes) < 1:
-            await asyncio.sleep(1)
-        while not self.loadOK.is_set():
+            await asyncio.sleep(3)
+        while True:
             c = 0
             for n in self.nodes.values():
                 if n.isLoaded.is_set():
                     c += 1
             if c == len(self.nodes):
-                self.loadOK.set()
-                self._log.info("Loading finished")
-            else:
-                await asyncio.sleep(1)
+                return
+            await asyncio.sleep(1)
 
     async def readTask(self):
         """Reader task."""
         while self.connectionOK.is_set():
             tmp = await self.reader.readline()
             tmp = tmp.decode().rstrip()
             if not tmp.startswith("["):
```

### Comparing `pyDuotecno-2023.7.3/duotecno/node.py` & `pyDuotecno-2023.7.4/duotecno/node.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/duotecno/protocol.py` & `pyDuotecno-2023.7.4/duotecno/protocol.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/duotecno/unit.py` & `pyDuotecno-2023.7.4/duotecno/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,20 +140,20 @@
         return False
 
     def is_closed(self):
         if self._state == 1:
             return True
         return False
 
-    async def up(self):
+    async def open(self):
         """Move up."""
         await self.stop()
         await self.writer(f"[182,0,{self.node.address},{self.unit},4]")
 
-    async def down(self):
+    async def close(self):
         """Move down."""
         await self.stop()
         await self.writer(f"[182,0,{self.node.address},{self.unit},5]")
 
     async def stop(self):
         """Stop the motor."""
         await self.writer(f"[182,0,{self.node.address},{self.unit},3]")
```

### Comparing `pyDuotecno-2023.7.3/examples/read.py` & `pyDuotecno-2023.7.4/examples/read.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/pyDuotecno.egg-info/PKG-INFO` & `pyDuotecno-2023.7.4/pyDuotecno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyDuotecno-2023.7.3/pyDuotecno.egg-info/SOURCES.txt` & `pyDuotecno-2023.7.4/pyDuotecno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/pyproject.toml` & `pyDuotecno-2023.7.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
-name        = "pyDuotecno"
-license     = {text = "Apache"}
-version     = "2023.7.3"
+name = "pyDuotecno"
+license = {text = "Apache"}
+version = "2023.7.4"
 description = "Open-source home automation platform running on Python 3."
-readme      = "README.md"
-authors     = [
+readme = "README.md"
+authors = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
-keywords    = ["home", "duotecno", "automation"]
+keywords = ["home", "duotecno", "automation"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -22,43 +22,34 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Home Automation",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.9.0"
-dependencies    = [
-]
+dependencies = []
 
 [project.urls]
 "Source Code" = "https://github.com/Cereal2nd/pyDuotecno"
 "Bug Reports" = "https://github.com/Cereal2nd/pyDuotecno/issues"
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*"]
 
 [tool.bumpver]
-current_version = "2023.7.3"
+current_version = "2023.7.4"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'version = "{version}"',
-    'current_version = "{version}"',
-]
-"setup.py" = [
-    "{version}",
-    "{pep440_version}",
-]
-"README.md" = [
-    "{version}",
-    "{pep440_version}",
+    '^version = "{version}"',
+    '^current_version = "{version}"',
 ]
```

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2html.py` & `pyDuotecno-2023.7.4/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2html4.py` & `pyDuotecno-2023.7.4/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2html5.py` & `pyDuotecno-2023.7.4/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2latex.py` & `pyDuotecno-2023.7.4/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2man.py` & `pyDuotecno-2023.7.4/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2odt.py` & `pyDuotecno-2023.7.4/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2odt_prepstyles.py` & `pyDuotecno-2023.7.4/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2pseudoxml.py` & `pyDuotecno-2023.7.4/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2s5.py` & `pyDuotecno-2023.7.4/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2xetex.py` & `pyDuotecno-2023.7.4/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rst2xml.py` & `pyDuotecno-2023.7.4/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.3/venv/bin/rstpep2html.py` & `pyDuotecno-2023.7.4/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

