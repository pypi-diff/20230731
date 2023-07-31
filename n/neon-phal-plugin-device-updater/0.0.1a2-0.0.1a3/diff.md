# Comparing `tmp/neon-phal-plugin-device-updater-0.0.1a2.tar.gz` & `tmp/neon-phal-plugin-device-updater-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a2.tar", last modified: Fri Jul 28 22:26:04 2023, max compression
+gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a3.tar", last modified: Mon Jul 31 21:01:42 2023, max compression
```

## Comparing `neon-phal-plugin-device-updater-0.0.1a2.tar` & `neon-phal-plugin-device-updater-0.0.1a3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:26:04.455732 neon-phal-plugin-device-updater-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-28 22:26:00.000000 neon-phal-plugin-device-updater-0.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-28 22:26:04.451732 neon-phal-plugin-device-updater-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 22:26:00.000000 neon-phal-plugin-device-updater-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:26:04.451732 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater/
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-28 22:26:00.000000 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:26:04.451732 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-28 22:26:04.000000 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 22:26:04.000000 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:26:04.000000 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-28 22:26:04.000000 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-28 22:26:04.000000 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 22:26:04.000000 neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 22:26:04.455732 neon-phal-plugin-device-updater-0.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-28 22:26:00.000000 neon-phal-plugin-device-updater-0.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater/
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 21:01:42.000000 neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:01:42.400613 neon-phal-plugin-device-updater-0.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-31 21:01:38.000000 neon-phal-plugin-device-updater-0.0.1a3/setup.py
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a2/LICENSE.md` & `neon-phal-plugin-device-updater-0.0.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.0.1a2/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater/__init__.py` & `neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import hashlib
 import json
 import shutil
-
 import requests
 
-from typing import Optional
+from typing import Optional, Tuple
 from os import remove
 from os.path import isfile, join, dirname
 from subprocess import Popen
 from ovos_bus_client.message import Message
 from ovos_utils.log import LOG
 from ovos_plugin_manager.phal import PHALPlugin
 from neon_utils.web_utils import scrape_page_for_links
@@ -61,15 +60,17 @@
                                             "updates/")
         self.squashfs_path = self.config.get("squashfs_path",
                                              "/opt/neon/update.squashfs")
 
         self._build_info = None
 
         # Register messagebus listeners
+        self.bus.on("neon.check_update_initramfs", self.check_update_initramfs)
         self.bus.on("neon.update_initramfs", self.update_initramfs)
+        self.bus.on("neon.check_update_squashfs", self.check_update_squashfs)
         self.bus.on("neon.update_squashfs", self.update_squashfs)
 
     @property
     def build_info(self) -> dict:
         if self._build_info is None:
             try:
                 with open("/opt/neon/build_info.json") as f:
@@ -82,34 +83,34 @@
     def _get_initramfs_latest(self) -> bool:
         """
         Get the latest initramfs image and check if it is different from the
         current installed initramfs
         """
         if not self.initramfs_url:
             raise RuntimeError("No initramfs_url configured")
-        initramfs_request = requests.get(self.initramfs_url)
-        if not initramfs_request.ok:
-            raise ConnectionError(f"Unable to get updated initramfs from: "
-                                  f"{self.initramfs_url}")
-        new_hash = hashlib.md5(initramfs_request.content).hexdigest()
-        with open(self.initramfs_update_path, 'wb+') as f:
-            f.write(initramfs_request.content)
+        if isfile(self.initramfs_update_path):
+            LOG.info("update already downloaded")
+            with open(self.initramfs_update_path, 'rb') as f:
+                new_hash = hashlib.md5(f.read()).hexdigest()
+        else:
+            initramfs_request = requests.get(self.initramfs_url)
+            if not initramfs_request.ok:
+                raise ConnectionError(f"Unable to get updated initramfs from: "
+                                      f"{self.initramfs_url}")
+            new_hash = hashlib.md5(initramfs_request.content).hexdigest()
+            with open(self.initramfs_update_path, 'wb+') as f:
+                f.write(initramfs_request.content)
         with open("/boot/firmware/initramfs", 'rb') as f:
             old_hash = hashlib.md5(f.read()).hexdigest()
         if new_hash == old_hash:
             LOG.debug("initramfs not changed")
             return False
         return True
 
-    def _get_squashfs_latest(self) -> Optional[str]:
-        """
-        Get the latest squashfs image if different from the installed version
-        @returns: path to downloaded update if present, else None
-        """
-
+    def _check_squashfs_update_available(self) -> Optional[Tuple[str, str]]:
         # Get all available update files from the configured URL
         ext = '.squashfs'
         prefix = self.build_info.get("base_os", {}).get("name", "")
         links = scrape_page_for_links(self.squashfs_url)
         valid_links = [(name, uri) for name, uri in links.items()
                        if name.endswith(ext) and name.startswith(prefix)]
         valid_links.sort(key=lambda k: k[0], reverse=True)
@@ -117,14 +118,28 @@
         download_url = valid_links[0][1]
 
         # Check if the latest version matches the installed version
         installed_image_time = self.build_info.get("base_os", {}).get("time")
         if installed_image_time and installed_image_time in newest_version:
             LOG.info("Already updated")
             return None
+        return newest_version, download_url
+
+    def _get_squashfs_latest(self) -> Optional[str]:
+        """
+        Get the latest squashfs image if different from the installed version
+        @returns: path to downloaded update if present, else None
+        """
+
+        # Check for an available update
+        update = self._check_squashfs_update_available()
+        if not update:
+            # Already updated
+            return None
+        newest_version, download_url = update
 
         # Check if the updated version has already been downloaded
         download_path = join(dirname(self.initramfs_update_path),
                              newest_version)
         if isfile(download_path):
             LOG.info("Update already downloaded")
             return download_path
@@ -141,14 +156,30 @@
             shutil.move(temp_dl_path, download_path)
             return download_path
         except Exception as e:
             LOG.exception(e)
             if isfile(temp_dl_path):
                 remove(temp_dl_path)
 
+    def check_update_initramfs(self, message: Message):
+        """
+        Handle a request to check for initramfs updates
+        @param message: `neon.check_update_initramfs` Message
+        """
+        update_available = self._get_initramfs_latest()
+        self.bus.emit(message.response({"update_available": update_available}))
+
+    def check_update_squashfs(self, message: Message):
+        """
+        Handle a request to check for squash updates
+        @param message: `neon.check_update_squashfs` Message
+        """
+        update_available = self._check_squashfs_update_available() is not None
+        self.bus.emit(message.response({"update_available": update_available}))
+
     def update_squashfs(self, message: Message):
         """
         Handle a request to update squashfs
         @param message: `neon.update_squashfs` Message
         """
         try:
             LOG.info("Checking squashfs update")
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a2/neon_phal_plugin_device_updater.egg-info/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a3/neon_phal_plugin_device_updater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a2/setup.py` & `neon-phal-plugin-device-updater-0.0.1a3/setup.py`

 * *Files identical despite different names*

