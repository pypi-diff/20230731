# Comparing `tmp/async_nec_beamer-0.1.4.tar.gz` & `tmp/async_nec_beamer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_nec_beamer-0.1.4.tar", last modified: Sun Jul 30 19:39:32 2023, max compression
+gzip compressed data, was "async_nec_beamer-0.2.0.tar", last modified: Mon Jul 31 12:22:24 2023, max compression
```

## Comparing `async_nec_beamer-0.1.4.tar` & `async_nec_beamer-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:39:32.434175 async_nec_beamer-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-30 19:39:20.000000 async_nec_beamer-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-30 19:39:32.430175 async_nec_beamer-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-30 19:39:20.000000 async_nec_beamer-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:39:32.430175 async_nec_beamer-0.1.4/async_nec_beamer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-30 19:39:20.000000 async_nec_beamer-0.1.4/async_nec_beamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-07-30 19:39:20.000000 async_nec_beamer-0.1.4/async_nec_beamer/nec_beamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:39:32.430175 async_nec_beamer-0.1.4/async_nec_beamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-30 19:39:32.000000 async_nec_beamer-0.1.4/async_nec_beamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-30 19:39:32.000000 async_nec_beamer-0.1.4/async_nec_beamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:39:32.000000 async_nec_beamer-0.1.4/async_nec_beamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 19:39:32.000000 async_nec_beamer-0.1.4/async_nec_beamer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-30 19:39:32.000000 async_nec_beamer-0.1.4/async_nec_beamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 19:39:32.000000 async_nec_beamer-0.1.4/async_nec_beamer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 19:39:32.430175 async_nec_beamer-0.1.4/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-30 19:39:20.000000 async_nec_beamer-0.1.4/bin/async_nec_beamer
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 19:39:32.434175 async_nec_beamer-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-30 19:39:20.000000 async_nec_beamer-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/async_nec_beamer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/async_nec_beamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19795 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/async_nec_beamer/nec_beamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:22:23.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 12:22:24.000000 async_nec_beamer-0.2.0/async_nec_beamer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/bin/async_nec_beamer
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:22:24.159358 async_nec_beamer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-31 12:22:14.000000 async_nec_beamer-0.2.0/setup.py
```

### Comparing `async_nec_beamer-0.1.4/LICENSE` & `async_nec_beamer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_nec_beamer-0.1.4/PKG-INFO` & `async_nec_beamer-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_nec_beamer
-Version: 0.1.4
+Version: 0.2.0
 Summary: NEC Beamer Web Interface Wrapper (Async)
 Home-page: https://github.com/heinrich-foto/async_nec_beamer
 Author: Heinrich-Foto
 Author-email: async_nec_beamer@heinrich-foto.de
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `async_nec_beamer-0.1.4/async_nec_beamer.egg-info/PKG-INFO` & `async_nec_beamer-0.2.0/async_nec_beamer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-nec-beamer
-Version: 0.1.4
+Version: 0.2.0
 Summary: NEC Beamer Web Interface Wrapper (Async)
 Home-page: https://github.com/heinrich-foto/async_nec_beamer
 Author: Heinrich-Foto
 Author-email: async_nec_beamer@heinrich-foto.de
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `async_nec_beamer-0.1.4/bin/async_nec_beamer` & `async_nec_beamer-0.2.0/bin/async_nec_beamer`

 * *Files 12% similar despite different names*

```diff
@@ -16,61 +16,61 @@
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def turn_on(ip_address, name, json):
     """Turn on the Beamer"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.turn_on())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def turn_off(ip_address, name, json):
     """Turn off the Beamer"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.turn_off())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def rgb1(ip_address, name, json):
     """Select input rgb1 (VGA)"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.source_rgb1())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def rgb2(ip_address, name, json):
     """Select input rgb2 (BNC)"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.source_rgb2())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def rgb3(ip_address, name, json):
     """Select input rgb3 (DVI)"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.source_rgb3())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
@@ -85,43 +85,87 @@
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def composite(ip_address, name, json):
     """Select input comp (Component)"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.source_comp())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def s_video(ip_address, name, json):
     """Select input svid (S-Video)"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.source_svid())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
 
 @click.command()
 @click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
 @click.option("--name", default=NAME, help="Name of the Beamer")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 def video(ip_address, name, json):
     """Select input video (Video)"""
     nec = Nec_Beamer(name=name, ip_address=ip_address)
     asyncio.run(nec.source_vidn())
-    asyncio.run(nec.update())
+    # asyncio.run(nec.update())
     nec.print_status(json)
 
-# add a verbose option to cli group
 
+@click.command()
+@click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
+@click.option("--name", default=NAME, help="Name of the Beamer")
+@click.option("--json/--no-json", default=False, help="output as JSON")
+def mute_all(ip_address, name, json):
+    """Mute the Beamer"""
+    nec = Nec_Beamer(name=name, ip_address=ip_address)
+    asyncio.run(nec.mute())
+    # asyncio.run(nec.update())
+    nec.print_status(json)
+
+@click.command()
+@click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
+@click.option("--name", default=NAME, help="Name of the Beamer")
+@click.option("--json/--no-json", default=False, help="output as JSON")
+def mute_picture(ip_address, name, json):
+    """Mute the Beamer Picture"""
+    nec = Nec_Beamer(name=name, ip_address=ip_address)
+    asyncio.run(nec.mute_picture())
+    # asyncio.run(nec.update())
+    nec.print_status(json)
+
+@click.command()
+@click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
+@click.option("--name", default=NAME, help="Name of the Beamer")
+@click.option("--json/--no-json", default=False, help="output as JSON")
+def mute_audio(ip_address, name, json):
+    """Mute the Beamer Audio"""
+    nec = Nec_Beamer(name=name, ip_address=ip_address)
+    asyncio.run(nec.mute_audio())
+    # asyncio.run(nec.update())
+    nec.print_status(json)
+
+@click.command()
+@click.option("--ip_address", default=IP_ADDRESS, help="IP Address of the Beamer")
+@click.option("--name", default=NAME, help="Name of the Beamer")
+@click.option("--json/--no-json", default=False, help="output as JSON")
+def mute_osd(ip_address, name, json):
+    """Mute the Beamer OSD"""
+    nec = Nec_Beamer(name=name, ip_address=ip_address)
+    asyncio.run(nec.mute_osd())
+    # asyncio.run(nec.update())
+    nec.print_status(json)
+
+# add a verbose option to cli group
 @click.group()
 @click.option("--verbose/--no-verbose", default=False, help="Logging with verbosity")
 @click.option("--debug/--no-debug", default=False, help="Logging with debug")
 @click.option("--json/--no-json", default=False, help="output as JSON")
 @click.pass_context
 def cli(ctx, verbose, debug, json):
     """ Control a NEC Beamer via LAN
@@ -164,14 +208,18 @@
 
 
 @ click.group()
 def select_input():
     """ Select input Source """
     pass
 
+@click.group()
+def mute():
+    """Mute the Beamer"""
+    pass
 
 cli.add_command(turn_on)
 cli.add_command(turn_off)
 cli.add_command(status)
 cli.add_command(rgb1)
 cli.add_command(rgb2)
 cli.add_command(rgb3)
@@ -181,14 +229,20 @@
 legacy_input.add_command(s_video)
 legacy_input.add_command(video)
 
 select_input.add_command(rgb1)
 select_input.add_command(rgb2)
 select_input.add_command(rgb3)
 
+mute.add_command(mute_all)
+mute.add_command(mute_picture)
+mute.add_command(mute_audio)
+mute.add_command(mute_osd)
 
 # add subgroup to main group
 cli.add_command(legacy_input)
 cli.add_command(select_input)
+cli.add_command(mute)
+cli.add_command(mute_all)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `async_nec_beamer-0.1.4/setup.py` & `async_nec_beamer-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='async_nec_beamer',
-      version='0.1.4',
+      version='0.2.0',
       description='NEC Beamer Web Interface Wrapper (Async)',
       url='https://github.com/heinrich-foto/async_nec_beamer',
       author='Heinrich-Foto',
       author_email='async_nec_beamer@heinrich-foto.de',
       license='MIT',
       packages=['async_nec_beamer'],
       install_requires=[
```

