# Comparing `tmp/xhac-0.1.2-py3-none-any.whl.zip` & `tmp/xhac-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 14808 bytes, number of entries: 11
--rw-r--r--  2.0 unx    10036 b- defN 20-Feb-02 00:00 xhac/HomeClient.py
--rw-r--r--  2.0 unx     1272 b- defN 20-Feb-02 00:00 xhac/Scanner.py
+Zip file size: 16047 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 xhac/__init__.py
--rw-r--r--  2.0 unx     3668 b- defN 20-Feb-02 00:00 xhac/cli.py
+-rw-r--r--  2.0 unx     3536 b- defN 20-Feb-02 00:00 xhac/cli.py
+-rw-r--r--  2.0 unx    12827 b- defN 20-Feb-02 00:00 xhac/client.py
+-rw-r--r--  2.0 unx     1130 b- defN 20-Feb-02 00:00 xhac/model.py
 -rw-r--r--  2.0 unx    15994 b- defN 20-Feb-02 00:00 xhac/pyparser.py
+-rw-r--r--  2.0 unx     1273 b- defN 20-Feb-02 00:00 xhac/scanner.py
 -rw-r--r--  2.0 unx     8536 b- defN 20-Feb-02 00:00 xhac/util.py
-?rw-r--r--  2.0 unx     2094 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx       39 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      812 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/RECORD
-11 files, 43611 bytes uncompressed, 13462 bytes compressed:  69.1%
+?rw-r--r--  2.0 unx     2094 b- defN 20-Feb-02 00:00 xhac-0.1.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 xhac-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx       39 b- defN 20-Feb-02 00:00 xhac-0.1.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 xhac-0.1.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      878 b- defN 20-Feb-02 00:00 xhac-0.1.3.dist-info/RECORD
+12 files, 47467 bytes uncompressed, 14607 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,34 +1,37 @@
-Filename: xhac/HomeClient.py
+Filename: xhac/__init__.py
 Comment: 
 
-Filename: xhac/Scanner.py
+Filename: xhac/cli.py
 Comment: 
 
-Filename: xhac/__init__.py
+Filename: xhac/client.py
 Comment: 
 
-Filename: xhac/cli.py
+Filename: xhac/model.py
 Comment: 
 
 Filename: xhac/pyparser.py
 Comment: 
 
+Filename: xhac/scanner.py
+Comment: 
+
 Filename: xhac/util.py
 Comment: 
 
-Filename: xhac-0.1.2.dist-info/METADATA
+Filename: xhac-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xhac-0.1.2.dist-info/WHEEL
+Filename: xhac-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xhac-0.1.2.dist-info/entry_points.txt
+Filename: xhac-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: xhac-0.1.2.dist-info/licenses/LICENSE
+Filename: xhac-0.1.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: xhac-0.1.2.dist-info/RECORD
+Filename: xhac-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xhac/cli.py

```diff
@@ -1,14 +1,14 @@
 from rich.console import Console
 from rich.table import Table
 from rich import box
 from typing import Union, Any
 import click
-from .HomeClient import HomeClient
-from .Scanner import Scanner
+from .client import HomeClient
+from .scanner import Scanner
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 def get_version():
     from pkg_resources import get_distribution
     return get_distribution("xhac").version
@@ -67,16 +67,16 @@
     console.print(table)
 
 
 @click.command()
 @click.argument("host", type=click.STRING)
 @click.argument("username", type=click.STRING)
 @click.argument("password", type=click.STRING)
-def load(host: str, username: str, password: str) -> None:
-    """Connect to MXCHIP Home Access Server and load Home model.
+def info(host: str, username: str, password: str) -> None:
+    """connect to MXCHIP Home Access Server and load Home model.
 
     Arguments:
 
         HOST : Format <IP>:<Port>, 192.168.31.66:52348.
 
         USERNAME: Username of the server.
 
@@ -85,63 +85,54 @@
     Example:
 
         $ xhac load 192.168.31.66:52348 SGW2052 mxchip123
     """
 
     ip, port = host.split(":")
 
-    def OnEvent(event):
-        print(f"OnEvent: {event}")
+    click.echo(f"Connecting to {ip}:{port} ...")
+    client = HomeClient("00:00:00:00:00:00", ip, int(port), username, password)
 
-    def OnDisconnect():
-        print("Disconnected")
-
-    homeClient = HomeClient(OnEvent, OnDisconnect)
-    homeClient.SetHost(ip, int(port))
-    homeClient.SetAccount(username, password)
-
-    if not homeClient.Connect():
+    if not client.connect():
         click.echo("Failed to connect")
         return
 
-    homeDB = homeClient.GetHome()
-
     console = Console()
 
     table = Table(title="Scenes", box=box.ROUNDED)
     table.add_column("ID")
     table.add_column("Name")
-    for scene in homeDB["scenes"]:
+    for scene in client.home_db["scenes"]:
         table.add_row(f"{scene['sid']}", scene["name"])
     console.print(table)
 
     table = Table(title="Rooms", box=box.ROUNDED)
     table.add_column("ID")
     table.add_column("Name")
-    for zone in homeDB["zones"]:
+    for zone in client.home_db["zones"]:
         table.add_row(f"{zone['zid']}", zone["name"])
     console.print(table)
 
     def FindZone(zid):
-        for zone in homeDB["zones"]:
+        for zone in client.home_db["zones"]:
             if zone["zid"] == zid:
                 return zone["name"]
         return "Unknown"
 
     table = Table(title="Devices", box=box.ROUNDED)
     table.add_column("ID")
     table.add_column("Name")
     table.add_column("Room")
-    for device in homeDB["devices"]:
+    for device in client.home_db["devices"]:
         table.add_row(f"{device['did']}", device["name"],
                       FindZone(device["zid"]))
     console.print(table)
 
 
 def main():
     cli.add_command(scan, "scan")
-    cli.add_command(load, "load")
+    cli.add_command(info, "info")
     cli()
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `xhac/Scanner.py` & `xhac/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from zeroconf import ServiceBrowser, ServiceListener, Zeroconf
 import time
 
+from zeroconf import ServiceBrowser, ServiceListener, Zeroconf
+
 
 class HomeServer:
     def __init__(self, name, ip, port, id, hostname):
         self.name = name
         self.ip = ip
         self.port = port
         self.id = id
```

## Comparing `xhac-0.1.2.dist-info/METADATA` & `xhac-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhac
-Version: 0.1.2
+Version: 0.1.3
 Summary: MXCHIP Home Access Client
 Project-URL: Homepage, https://www.mxchip.com/
 Project-URL: Documentation, https://www.mxchip.com/
 Project-URL: Repository, https://www.mxchip.com/
 Project-URL: Changelog, https://www.mxchip.com/
 Author-email: Snow Yang <yangsw@mxchip.com>
 Maintainer-email: Snow Yang <yangsw@mxchip.com>
```

## Comparing `xhac-0.1.2.dist-info/licenses/LICENSE` & `xhac-0.1.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `xhac-0.1.2.dist-info/RECORD` & `xhac-0.1.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-xhac/HomeClient.py,sha256=avRD6pvcpJ8Rcdug-OUC-HEzsN2JMls9ViUXJesc6go,10036
-xhac/Scanner.py,sha256=BM_tddVtw_EdxyeqRyqPkfsx_sROHqJVl1YwC08NrP0,1272
 xhac/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xhac/cli.py,sha256=0tstjbVGQbLyo2kG__ZkCoIfqpDA-I6YPZwOHFWuaEo,3668
+xhac/cli.py,sha256=YdJJVhRXUL8TlPGsjKMITWVLRxYlGlNeXuGF55t7pfw,3536
+xhac/client.py,sha256=o6NiXSTD5z0O9q3iSsEmcBe3a55s8g-uXQXnf7tDkq8,12827
+xhac/model.py,sha256=I2ugfctG5HCZEKPKwOcrMvrOehouFmwPOxpSfDGfUcg,1130
 xhac/pyparser.py,sha256=uPnBAJZrHVyvDaqPhxvCnL2NmVTcDglwfFNcOFsr-pA,15994
+xhac/scanner.py,sha256=z6jPta_0JlE8nlCWDesTCapR-TOC4RIkvF1pjHSC1fo,1273
 xhac/util.py,sha256=0wDCmFD4OLxUwKOgK03HkNWo5PW-K2BWierNv6ks0jY,8536
-xhac-0.1.2.dist-info/METADATA,sha256=HwGXDTZ8-tR2gNctoFWGVpo-PdoTbwzK96L3DH0aIUA,2094
-xhac-0.1.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-xhac-0.1.2.dist-info/entry_points.txt,sha256=khqPAUxrPdx8solPOTMftLurNpWL52j6gfN6dRsQq5Q,39
-xhac-0.1.2.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
-xhac-0.1.2.dist-info/RECORD,,
+xhac-0.1.3.dist-info/METADATA,sha256=80FoLEUaPwCqiyqlJtw8ZcfyWjWl9HOYfiWBMQqEM0E,2094
+xhac-0.1.3.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+xhac-0.1.3.dist-info/entry_points.txt,sha256=khqPAUxrPdx8solPOTMftLurNpWL52j6gfN6dRsQq5Q,39
+xhac-0.1.3.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
+xhac-0.1.3.dist-info/RECORD,,
```

