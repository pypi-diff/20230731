# Comparing `tmp/cumo-0.28.0.tar.gz` & `tmp/cumo-0.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumo-0.28.0.tar", max compression
+gzip compressed data, was "cumo-0.28.1.tar", max compression
```

## Comparing `cumo-0.28.0.tar` & `cumo-0.28.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1275 2023-07-31 11:19:46.815447 cumo-0.28.0/README.md
--rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/.gitignore
--rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/__init__.py
--rw-r--r--   0        0        0     3399 2023-07-31 10:43:26.850715 cumo-0.28.0/cumo/__main__.py
--rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/.gitignore
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/__init__.py
--rw-r--r--   0        0        0     1564 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/down_sample.py
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/__init__.py
--rw-r--r--   0        0        0     5041 2022-12-07 09:57:03.483743 cumo-0.28.0/cumo/_internal/members/camera.py
--rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/capture_screen.py
--rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/custom_control.py
--rw-r--r--   0        0        0     4648 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/event_handler.py
--rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/internal_utils.py
--rw-r--r--   0        0        0     6396 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/keyboard_event_handler.py
--rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/remove_object.py
--rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.28.0/cumo/_internal/members/send_object.py
--rw-r--r--   0        0        0    10336 2022-05-30 04:59:38.801405 cumo-0.28.0/cumo/_internal/members/set_custom_control.py
--rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.28.0/cumo/_internal/members/set_enable.py
--rw-r--r--   0        0        0     1164 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_internal/members/utils.py
--rw-r--r--   0        0        0        0 2023-07-31 11:18:56.284936 cumo-0.28.0/cumo/_internal/protobuf/__init__.py
--rw-r--r--   0        0        0    19981 2023-07-31 11:18:56.224936 cumo-0.28.0/cumo/_internal/protobuf/client_pb2.py
--rw-r--r--   0        0        0   100030 2023-07-31 11:18:55.384939 cumo-0.28.0/cumo/_internal/protobuf/server_pb2.py
--rw-r--r--   0        0        0     4013 2023-07-31 11:11:43.443077 cumo-0.28.0/cumo/_internal/server.py
--rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_vendor/pypcd/LICENSE
--rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/_vendor/pypcd/pypcd.py
--rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.28.0/cumo/keyboard_event.py
--rw-r--r--   0        0        0     3302 2022-12-22 06:09:32.016687 cumo-0.28.0/cumo/pointcloudviewer.py
--rw-r--r--   0        0        0  5060159 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/bundle-da8ac05a.js
--rw-r--r--   0        0        0   243028 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      515 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/index-31f52342.css
--rw-r--r--   0        0        0      281 2023-07-31 11:19:46.805447 cumo-0.28.0/cumo/public/index.html
--rw-r--r--   0        0        0     1107 2023-07-31 11:11:12.451590 cumo-0.28.0/pyproject.toml
--rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 cumo-0.28.0/PKG-INFO
+-rw-r--r--   0        0        0     1275 2023-07-31 12:56:12.454522 cumo-0.28.1/README.md
+-rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/.gitignore
+-rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-31 10:43:26.850715 cumo-0.28.1/cumo/__main__.py
+-rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/.gitignore
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/__init__.py
+-rw-r--r--   0        0        0     1564 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/down_sample.py
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/__init__.py
+-rw-r--r--   0        0        0     5041 2022-12-07 09:57:03.483743 cumo-0.28.1/cumo/_internal/members/camera.py
+-rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/capture_screen.py
+-rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/custom_control.py
+-rw-r--r--   0        0        0     4648 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/event_handler.py
+-rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/internal_utils.py
+-rw-r--r--   0        0        0     6396 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/keyboard_event_handler.py
+-rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/remove_object.py
+-rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.28.1/cumo/_internal/members/send_object.py
+-rw-r--r--   0        0        0    10336 2022-05-30 04:59:38.801405 cumo-0.28.1/cumo/_internal/members/set_custom_control.py
+-rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.28.1/cumo/_internal/members/set_enable.py
+-rw-r--r--   0        0        0     1164 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_internal/members/utils.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:55:12.618224 cumo-0.28.1/cumo/_internal/protobuf/__init__.py
+-rw-r--r--   0        0        0    19981 2023-07-31 12:55:12.578225 cumo-0.28.1/cumo/_internal/protobuf/client_pb2.py
+-rw-r--r--   0        0        0   100030 2023-07-31 12:55:11.518265 cumo-0.28.1/cumo/_internal/protobuf/server_pb2.py
+-rw-r--r--   0        0        0     4013 2023-07-31 11:11:43.443077 cumo-0.28.1/cumo/_internal/server.py
+-rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_vendor/pypcd/LICENSE
+-rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/_vendor/pypcd/pypcd.py
+-rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.28.1/cumo/keyboard_event.py
+-rw-r--r--   0        0        0     3302 2022-12-22 06:09:32.016687 cumo-0.28.1/cumo/pointcloudviewer.py
+-rw-r--r--   0        0        0  5060159 2023-07-31 12:56:12.454522 cumo-0.28.1/cumo/public/bundle-da8ac05a.js
+-rw-r--r--   0        0        0   243028 2023-07-31 12:56:12.454522 cumo-0.28.1/cumo/public/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      515 2023-07-31 12:56:12.444521 cumo-0.28.1/cumo/public/index-31f52342.css
+-rw-r--r--   0        0        0      281 2023-07-31 12:56:12.454522 cumo-0.28.1/cumo/public/index.html
+-rw-r--r--   0        0        0     1107 2023-07-31 12:55:04.858380 cumo-0.28.1/pyproject.toml
+-rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 cumo-0.28.1/PKG-INFO
```

### Comparing `cumo-0.28.0/README.md` & `cumo-0.28.1/README.md`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/__main__.py` & `cumo-0.28.1/cumo/__main__.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/down_sample.py` & `cumo-0.28.1/cumo/_internal/down_sample.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/camera.py` & `cumo-0.28.1/cumo/_internal/members/camera.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/capture_screen.py` & `cumo-0.28.1/cumo/_internal/members/capture_screen.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/custom_control.py` & `cumo-0.28.1/cumo/_internal/members/custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/event_handler.py` & `cumo-0.28.1/cumo/_internal/members/event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/internal_utils.py` & `cumo-0.28.1/cumo/_internal/members/internal_utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/keyboard_event_handler.py` & `cumo-0.28.1/cumo/_internal/members/keyboard_event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/remove_object.py` & `cumo-0.28.1/cumo/_internal/members/remove_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/send_object.py` & `cumo-0.28.1/cumo/_internal/members/send_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/set_custom_control.py` & `cumo-0.28.1/cumo/_internal/members/set_custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/set_enable.py` & `cumo-0.28.1/cumo/_internal/members/set_enable.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/members/utils.py` & `cumo-0.28.1/cumo/_internal/members/utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/protobuf/client_pb2.py` & `cumo-0.28.1/cumo/_internal/protobuf/client_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/protobuf/server_pb2.py` & `cumo-0.28.1/cumo/_internal/protobuf/server_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_internal/server.py` & `cumo-0.28.1/cumo/_internal/server.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_vendor/pypcd/LICENSE` & `cumo-0.28.1/cumo/_vendor/pypcd/LICENSE`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/_vendor/pypcd/pypcd.py` & `cumo-0.28.1/cumo/_vendor/pypcd/pypcd.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/keyboard_event.py` & `cumo-0.28.1/cumo/keyboard_event.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/pointcloudviewer.py` & `cumo-0.28.1/cumo/pointcloudviewer.py`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/public/bundle-da8ac05a.js` & `cumo-0.28.1/cumo/public/bundle-da8ac05a.js`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/public/bundle.js.LICENSE.txt` & `cumo-0.28.1/cumo/public/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/cumo/public/index-31f52342.css` & `cumo-0.28.1/cumo/public/index-31f52342.css`

 * *Files identical despite different names*

### Comparing `cumo-0.28.0/pyproject.toml` & `cumo-0.28.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 readme = "README.md"
 name = "cumo"
-version = "0.28.0"
+version = "0.28.1"
 description = "Webブラウザ上に点群を描画する python ライブラリ"
 authors = ["Kurusugawa Computer"]
 license = "BSD"
 keywords = ["point-cloud", "pcd"]
 repository = "https://github.com/kurusugawa-computer/cumo"
 classifiers = [
 	"Development Status :: 3 - Alpha",
```

### Comparing `cumo-0.28.0/PKG-INFO` & `cumo-0.28.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumo
-Version: 0.28.0
+Version: 0.28.1
 Summary: Webブラウザ上に点群を描画する python ライブラリ
 Home-page: https://github.com/kurusugawa-computer/cumo
 License: BSD
 Keywords: point-cloud,pcd
 Author: Kurusugawa Computer
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

