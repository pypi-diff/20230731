# Comparing `tmp/cumo-0.27.1.tar.gz` & `tmp/cumo-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumo-0.27.1.tar", max compression
+gzip compressed data, was "cumo-0.28.0.tar", max compression
```

## Comparing `cumo-0.27.1.tar` & `cumo-0.28.0.tar`

### file list

```diff
@@ -1,36 +1,33 @@
--rw-r--r--   0        0        0     1275 2023-05-29 11:20:13.735548 cumo-0.27.1/README.md
--rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/.gitignore
--rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/__init__.py
--rw-r--r--   0        0        0     3347 2022-12-22 05:49:06.219937 cumo-0.27.1/cumo/__main__.py
--rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/.gitignore
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/__init__.py
--rw-r--r--   0        0        0     1564 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/down_sample.py
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/__init__.py
--rw-r--r--   0        0        0     5041 2022-12-07 09:57:03.483743 cumo-0.27.1/cumo/_internal/members/camera.py
--rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/capture_screen.py
--rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/custom_control.py
--rw-r--r--   0        0        0     4648 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/event_handler.py
--rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/internal_utils.py
--rw-r--r--   0        0        0     6396 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/keyboard_event_handler.py
--rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/remove_object.py
--rw-r--r--   0        0        0    20520 2023-05-29 09:38:09.995194 cumo-0.27.1/cumo/_internal/members/send_object.py
--rw-r--r--   0        0        0    10336 2022-05-30 04:59:38.801405 cumo-0.27.1/cumo/_internal/members/set_custom_control.py
--rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.27.1/cumo/_internal/members/set_enable.py
--rw-r--r--   0        0        0     1164 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_internal/members/utils.py
--rw-r--r--   0        0        0        0 2023-05-29 11:19:43.084578 cumo-0.27.1/cumo/_internal/protobuf/__init__.py
--rw-r--r--   0        0        0    19981 2023-05-29 11:19:43.064578 cumo-0.27.1/cumo/_internal/protobuf/client_pb2.py
--rw-r--r--   0        0        0   100030 2023-05-29 11:19:42.864577 cumo-0.27.1/cumo/_internal/protobuf/server_pb2.py
--rw-r--r--   0        0        0     3638 2023-05-29 11:14:53.860776 cumo-0.27.1/cumo/_internal/server.py
--rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_vendor/pypcd/LICENSE
--rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/_vendor/pypcd/pypcd.py
--rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.27.1/cumo/keyboard_event.py
--rw-r--r--   0        0        0     3302 2022-12-22 06:09:32.016687 cumo-0.27.1/cumo/pointcloudviewer.py
--rw-r--r--   0        0        0  1314392 2023-05-29 11:20:13.725548 cumo-0.27.1/cumo/public/bundle-dfb467719784c1fd204a.js
--rw-r--r--   0        0        0     1009 2023-05-29 11:20:13.715548 cumo-0.27.1/cumo/public/bundle-dfb467719784c1fd204a.js.LICENSE.txt
--rw-r--r--   0        0        0  4003301 2023-05-29 11:20:13.735548 cumo-0.27.1/cumo/public/bundle-dfb467719784c1fd204a.js.map
--rw-r--r--   0        0        0    23075 2023-05-29 11:20:13.735548 cumo-0.27.1/cumo/public/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      269 2023-05-29 11:20:13.735548 cumo-0.27.1/cumo/public/index.html
--rw-r--r--   0        0        0      769 2023-05-29 11:20:13.735548 cumo-0.27.1/cumo/public/main.css
--rw-r--r--   0        0        0     1268 2023-05-29 11:20:13.735548 cumo-0.27.1/cumo/public/main.css.map
--rw-r--r--   0        0        0     1107 2023-05-29 11:14:53.860776 cumo-0.27.1/pyproject.toml
--rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 cumo-0.27.1/PKG-INFO
+-rw-r--r--   0        0        0     1275 2023-07-31 11:19:46.815447 cumo-0.28.0/README.md
+-rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/.gitignore
+-rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-31 10:43:26.850715 cumo-0.28.0/cumo/__main__.py
+-rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/.gitignore
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/__init__.py
+-rw-r--r--   0        0        0     1564 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/down_sample.py
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/__init__.py
+-rw-r--r--   0        0        0     5041 2022-12-07 09:57:03.483743 cumo-0.28.0/cumo/_internal/members/camera.py
+-rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/capture_screen.py
+-rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/custom_control.py
+-rw-r--r--   0        0        0     4648 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/event_handler.py
+-rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/internal_utils.py
+-rw-r--r--   0        0        0     6396 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/keyboard_event_handler.py
+-rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/remove_object.py
+-rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.28.0/cumo/_internal/members/send_object.py
+-rw-r--r--   0        0        0    10336 2022-05-30 04:59:38.801405 cumo-0.28.0/cumo/_internal/members/set_custom_control.py
+-rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.28.0/cumo/_internal/members/set_enable.py
+-rw-r--r--   0        0        0     1164 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/utils.py
+-rw-r--r--   0        0        0        0 2023-07-31 11:18:56.284936 cumo-0.28.0/cumo/_internal/protobuf/__init__.py
+-rw-r--r--   0        0        0    19981 2023-07-31 11:18:56.224936 cumo-0.28.0/cumo/_internal/protobuf/client_pb2.py
+-rw-r--r--   0        0        0   100030 2023-07-31 11:18:55.384939 cumo-0.28.0/cumo/_internal/protobuf/server_pb2.py
+-rw-r--r--   0        0        0     4013 2023-07-31 11:11:43.443077 cumo-0.28.0/cumo/_internal/server.py
+-rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_vendor/pypcd/LICENSE
+-rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_vendor/pypcd/pypcd.py
+-rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/keyboard_event.py
+-rw-r--r--   0        0        0     3302 2022-12-22 06:09:32.016687 cumo-0.28.0/cumo/pointcloudviewer.py
+-rw-r--r--   0        0        0  5060159 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/bundle-da8ac05a.js
+-rw-r--r--   0        0        0   243028 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      515 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/index-31f52342.css
+-rw-r--r--   0        0        0      281 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/index.html
+-rw-r--r--   0        0        0     1107 2023-07-31 11:11:12.451590 cumo-0.28.0/pyproject.toml
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 cumo-0.28.0/PKG-INFO
```

### Comparing `cumo-0.27.1/README.md` & `cumo-0.28.0/README.md`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/__main__.py` & `cumo-0.28.0/cumo/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     args = parser.parse_args()
 
     viewer = PointCloudViewer(
         host=host, websocket_port=websocket_port, http_port=http_port, autostart=True
     )
     print(f"open: http://{host}:{http_port}")
     print("setup...")
+    viewer.stop_render()
 
     viewer.remove_all_objects()
     viewer.remove_all_custom_controls()
 
     radius = send_pointcloud_pcd(viewer, args.pcd_filepath)
 
     points = numpy.array([
@@ -95,14 +96,15 @@
 
     viewer.add_custom_button(
         name="start", on_changed=lambda dummy: on_start_button_pushed()
     )
 
     print("resize window and press custom control button \"start\" (or press A key)")
 
+    viewer.resume_render()
     viewer.wait_forever()
 
 
 def send_pointcloud_pcd(viewer: PointCloudViewer, filename: str) -> float:
     with open(filename, "rb") as f:
         b = f.read()
         viewer.send_pointcloud_pcd(b)
```

### Comparing `cumo-0.27.1/cumo/_internal/down_sample.py` & `cumo-0.28.0/cumo/_internal/down_sample.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/camera.py` & `cumo-0.28.0/cumo/_internal/members/camera.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/capture_screen.py` & `cumo-0.28.0/cumo/_internal/members/capture_screen.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/custom_control.py` & `cumo-0.28.0/cumo/_internal/members/custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/event_handler.py` & `cumo-0.28.0/cumo/_internal/members/event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/internal_utils.py` & `cumo-0.28.0/cumo/_internal/members/internal_utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/keyboard_event_handler.py` & `cumo-0.28.0/cumo/_internal/members/keyboard_event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/remove_object.py` & `cumo-0.28.0/cumo/_internal/members/remove_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/send_object.py` & `cumo-0.28.0/cumo/_internal/members/send_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     pypcd_pc = pypcd.point_cloud_from_buffer(pcd_bytes)
     pc_data: numpy.ndarray = pypcd_pc.pc_data
 
     xyz = numpy.stack([pc_data["x"], pc_data["y"], pc_data["z"]], axis=1)
 
     rgb_u32: numpy.ndarray = pc_data["rgb"]
-    rgb_u32.dtype = "uint32"
+    rgb_u32 = rgb_u32.view("uint32")
     r_u8: numpy.ndarray = ((rgb_u32 & 0xff0000) >> 16).astype("uint8")
     g_u8: numpy.ndarray = ((rgb_u32 & 0x00ff00) >> 8).astype("uint8")
     b_u8: numpy.ndarray = (rgb_u32 & 0x0000ff).astype("uint8")
 
     rgb = numpy.stack([r_u8, g_u8, b_u8], axis=1)
 
     return self.send_pointcloud(
@@ -77,15 +77,15 @@
 
 
 def send_pointcloud(
     self: PointCloudViewer,
     xyz: Optional[numpy.ndarray] = None,
     rgb: Optional[numpy.ndarray] = None,
     xyzrgb: Optional[numpy.ndarray] = None,
-    down_sample: Optional[DownSampleStrategy] = DownSampleStrategy.RANDOM_SAMPLE,
+    down_sample: DownSampleStrategy = DownSampleStrategy.RANDOM_SAMPLE,
     max_num_points: int = DOWNSAMPLING_DEFAULT_MAX_NUM_POINTS,
     point_size: float = 1
 ) -> UUID:
     """点群をブラウザに送信し、表示させる。
 
     Args:
         xyz (Optional[numpy.ndarray], optional): shape が (num_points,3) で dtype が float32 の ndarray 。各行が点のx,y,z座標を表す。
@@ -128,15 +128,15 @@
         if rgb is not None:
             rgb_u32 = rgb.astype("uint32")
             rgb_f32: numpy.ndarray = (
                 (rgb_u32[:, 0] << 16)
                 + (rgb_u32[:, 1] << 8)
                 + rgb_u32[:, 2]
             )
-            rgb_f32.dtype = "float32"
+            rgb_f32 = rgb_f32.view("float32")
 
             concatenated: numpy.ndarray = numpy.column_stack((
                 xyz,
                 rgb_f32,
             ))
             pcd = pypcd.make_xyz_rgb_point_cloud(
                 down_sample_pointcloud(
```

### Comparing `cumo-0.27.1/cumo/_internal/members/set_custom_control.py` & `cumo-0.28.0/cumo/_internal/members/set_custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/set_enable.py` & `cumo-0.28.0/cumo/_internal/members/set_enable.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/members/utils.py` & `cumo-0.28.0/cumo/_internal/members/utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/protobuf/client_pb2.py` & `cumo-0.28.0/cumo/_internal/protobuf/client_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/protobuf/server_pb2.py` & `cumo-0.28.0/cumo/_internal/protobuf/server_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_internal/server.py` & `cumo-0.28.0/cumo/_internal/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import multiprocessing
 import pkgutil
 import asyncio
 import threading
 
 from http.server import BaseHTTPRequestHandler, HTTPServer
-from os.path import join
+from os.path import join, splitext
 from typing import Union, Optional
 
 # pylint: disable=E1101
 import websockets
 
+EXT_TO_MIME = {
+    "js": "application/javascript",
+    "html": "text/html",
+    "css": "text/css",
+}
+
 
 def _MakePointCloudViewerHTTPRequestHandler(websocket_port: int):
     class _PointCloudViewerHTTPRequestHandler(BaseHTTPRequestHandler):
         def do_GET(self):
             if self.path == "/":
                 self.redirect("index.html")
             elif self.path == "/websocket_url":
@@ -27,14 +33,17 @@
                 data: Union[bytes, None] = None
                 try:
                     data = pkgutil.get_data("cumo", path)
                 except FileNotFoundError:
                     self.send_error(404)
                 if data is not None:
                     self.send_response(200)
+                    ext = splitext(self.path)[1][1:]
+                    if ext in EXT_TO_MIME:
+                        self.send_header("content-type", EXT_TO_MIME[ext])
                     self.end_headers()
                     self.wfile.write(data)
                 else:
                     self.send_error(404)
 
         # pylint: disable=W0622
         def log_message(self, format: str, *args) -> None:
@@ -90,15 +99,17 @@
         (host, http_port),
         _MakePointCloudViewerHTTPRequestHandler(websocket_port=websocket_port),
     )
 
     start_server = websockets.serve(__websocket_handler,
                                     host=host,
                                     port=websocket_port,
-                                    max_size=None)
+                                    max_size=None,
+                                    ping_timeout=60,
+                                    )
     loop.run_until_complete(start_server)
 
     threads = [
         threading.Thread(
             target=loop.run_forever
         ),
         threading.Thread(
```

### Comparing `cumo-0.27.1/cumo/_vendor/pypcd/LICENSE` & `cumo-0.28.0/cumo/_vendor/pypcd/LICENSE`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/_vendor/pypcd/pypcd.py` & `cumo-0.28.0/cumo/_vendor/pypcd/pypcd.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/keyboard_event.py` & `cumo-0.28.0/cumo/keyboard_event.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/cumo/pointcloudviewer.py` & `cumo-0.28.0/cumo/pointcloudviewer.py`

 * *Files identical despite different names*

### Comparing `cumo-0.27.1/pyproject.toml` & `cumo-0.28.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 readme = "README.md"
 name = "cumo"
-version = "0.27.1"
+version = "0.28.0"
 description = "Webブラウザ上に点群を描画する python ライブラリ"
 authors = ["Kurusugawa Computer"]
 license = "BSD"
 keywords = ["point-cloud", "pcd"]
 repository = "https://github.com/kurusugawa-computer/cumo"
 classifiers = [
 	"Development Status :: 3 - Alpha",
```

### Comparing `cumo-0.27.1/PKG-INFO` & `cumo-0.28.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumo
-Version: 0.27.1
+Version: 0.28.0
 Summary: Webブラウザ上に点群を描画する python ライブラリ
 Home-page: https://github.com/kurusugawa-computer/cumo
 License: BSD
 Keywords: point-cloud,pcd
 Author: Kurusugawa Computer
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

