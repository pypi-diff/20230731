# Comparing `tmp/reflex_ui-0.1.2.tar.gz` & `tmp/reflex_ui-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_ui-0.1.2.tar", max compression
+gzip compressed data, was "reflex_ui-0.1.3.tar", max compression
```

## Comparing `reflex_ui-0.1.2.tar` & `reflex_ui-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1075 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/README.md
--rw-r--r--   0        0        0     1041 2023-07-14 08:40:45.243231 reflex_ui-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      110 2023-07-14 08:24:26.573241 reflex_ui-0.1.2/reflex/__init__.py
--rw-r--r--   0        0        0     5242 2023-07-14 08:24:26.583241 reflex_ui-0.1.2/reflex/app.py
--rw-r--r--   0        0        0    15243 2023-07-02 17:23:24.247163 reflex_ui-0.1.2/reflex/app_server.py
--rw-r--r--   0        0        0     1918 2023-07-14 07:50:58.893264 reflex_ui-0.1.2/reflex/assets.py
--rw-r--r--   0        0        0     2480 2023-07-02 17:23:24.247163 reflex_ui-0.1.2/reflex/common.py
--rw-r--r--   0        0        0       47 2023-06-02 09:45:54.484185 reflex_ui-0.1.2/reflex/errors.py
--rw-r--r--   0        0        0    36522 2023-07-02 17:49:31.901177 reflex_ui-0.1.2/reflex/generated/app.js
--rw-r--r--   0        0        0    80229 2023-07-02 17:49:31.924510 reflex_ui-0.1.2/reflex/generated/app.js.map
--rw-r--r--   0        0        0      287 2023-07-02 17:49:30.104509 reflex_ui-0.1.2/reflex/generated/index.html
--rw-r--r--   0        0        0     4350 2023-07-02 17:49:30.834510 reflex_ui-0.1.2/reflex/generated/style.css
--rw-r--r--   0        0        0     7562 2023-07-02 17:49:30.837843 reflex_ui-0.1.2/reflex/generated/style.css.map
--rw-r--r--   0        0        0    75209 2022-04-21 09:32:25.000000 reflex_ui-0.1.2/reflex/hosted-assets/showdown.min.js
--rw-r--r--   0        0        0     2521 2023-07-14 08:25:05.986574 reflex_ui-0.1.2/reflex/image_source.py
--rw-r--r--   0        0        0     1229 2023-06-02 09:31:52.003332 reflex_ui-0.1.2/reflex/messages.py
--rw-r--r--   0        0        0    38949 2023-07-14 07:51:46.796596 reflex_ui-0.1.2/reflex/session.py
--rw-r--r--   0        0        0      123 2023-07-14 08:25:08.029908 reflex_ui-0.1.2/reflex/styling/__init__.py
--rw-r--r--   0        0        0     3605 2023-07-14 07:53:45.156595 reflex_ui-0.1.2/reflex/styling/box_style.py
--rw-r--r--   0        0        0     9391 2023-06-16 18:28:59.043338 reflex_ui-0.1.2/reflex/styling/color.py
--rw-r--r--   0        0        0     2751 2023-07-14 07:53:45.159928 reflex_ui-0.1.2/reflex/styling/fills.py
--rw-r--r--   0        0        0     2673 2023-07-14 08:24:26.589908 reflex_ui-0.1.2/reflex/styling/markdown_style.py
--rw-r--r--   0        0        0     1762 2023-07-14 08:24:26.586575 reflex_ui-0.1.2/reflex/styling/text_style.py
--rw-r--r--   0        0        0      274 2023-05-30 05:41:43.000000 reflex_ui-0.1.2/reflex/theme.py
--rw-r--r--   0        0        0    12658 2023-07-14 08:24:26.576575 reflex_ui-0.1.2/reflex/validator.py
--rw-r--r--   0        0        0      466 2023-07-14 08:40:58.956564 reflex_ui-0.1.2/reflex/widgets/__init__.py
--rw-r--r--   0        0        0     2416 2023-07-14 08:25:06.019908 reflex_ui-0.1.2/reflex/widgets/auto_form.py
--rw-r--r--   0        0        0     8439 2023-07-02 17:50:56.411212 reflex_ui-0.1.2/reflex/widgets/button.py
--rw-r--r--   0        0        0     1577 2023-07-02 17:50:56.411212 reflex_ui-0.1.2/reflex/widgets/column.py
--rw-r--r--   0        0        0      226 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/reflex/widgets/container.py
--rw-r--r--   0        0        0     1827 2023-07-14 08:24:26.603242 reflex_ui-0.1.2/reflex/widgets/dropdown.py
--rw-r--r--   0        0        0      506 2023-07-14 08:25:06.009908 reflex_ui-0.1.2/reflex/widgets/image.py
--rw-r--r--   0        0        0     1175 2023-07-14 08:24:26.609908 reflex_ui-0.1.2/reflex/widgets/markdown_view.py
--rw-r--r--   0        0        0      575 2023-07-14 08:25:06.013241 reflex_ui-0.1.2/reflex/widgets/media_player.py
--rw-r--r--   0        0        0      939 2023-07-14 08:40:58.959897 reflex_ui-0.1.2/reflex/widgets/metadata.py
--rw-r--r--   0        0        0     3524 2023-06-10 18:04:23.870009 reflex_ui-0.1.2/reflex/widgets/mouse_event_listener.py
--rw-r--r--   0        0        0      498 2023-07-14 08:36:51.036567 reflex_ui-0.1.2/reflex/widgets/plot.py
--rw-r--r--   0        0        0     1665 2023-07-02 17:50:56.411212 reflex_ui-0.1.2/reflex/widgets/progress_circle.py
--rw-r--r--   0        0        0      506 2023-07-14 08:24:26.603242 reflex_ui-0.1.2/reflex/widgets/rectangle.py
--rw-r--r--   0        0        0     1594 2023-07-02 17:44:56.264397 reflex_ui-0.1.2/reflex/widgets/row.py
--rw-r--r--   0        0        0      242 2023-05-27 11:53:20.000000 reflex_ui-0.1.2/reflex/widgets/stack.py
--rw-r--r--   0        0        0     1566 2023-07-14 08:24:26.606575 reflex_ui-0.1.2/reflex/widgets/switch.py
--rw-r--r--   0        0        0      363 2023-05-28 16:37:28.000000 reflex_ui-0.1.2/reflex/widgets/text.py
--rw-r--r--   0        0        0     1894 2023-07-14 08:24:26.606575 reflex_ui-0.1.2/reflex/widgets/text_input.py
--rw-r--r--   0        0        0    20757 2023-07-02 17:50:56.414545 reflex_ui-0.1.2/reflex/widgets/widget_base.py
--rw-r--r--   0        0        0     3890 2023-07-14 08:24:26.583241 reflex_ui-0.1.2/reflex/world_units.py
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 reflex_ui-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-27 11:53:20.000000 reflex_ui-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-05-27 11:53:20.000000 reflex_ui-0.1.3/README.md
+-rw-r--r--   0        0        0     1041 2023-07-31 11:01:54.858204 reflex_ui-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-14 08:24:26.573241 reflex_ui-0.1.3/reflex/__init__.py
+-rw-r--r--   0        0        0     5242 2023-07-14 08:24:26.583241 reflex_ui-0.1.3/reflex/app.py
+-rw-r--r--   0        0        0    15243 2023-07-02 17:23:24.247163 reflex_ui-0.1.3/reflex/app_server.py
+-rw-r--r--   0        0        0     1918 2023-07-14 07:50:58.893264 reflex_ui-0.1.3/reflex/assets.py
+-rw-r--r--   0        0        0     2480 2023-07-02 17:23:24.247163 reflex_ui-0.1.3/reflex/common.py
+-rw-r--r--   0        0        0       47 2023-06-02 09:45:54.484185 reflex_ui-0.1.3/reflex/errors.py
+-rw-r--r--   0        0        0    36522 2023-07-02 17:49:31.901177 reflex_ui-0.1.3/reflex/generated/app.js
+-rw-r--r--   0        0        0    80229 2023-07-02 17:49:31.924510 reflex_ui-0.1.3/reflex/generated/app.js.map
+-rw-r--r--   0        0        0      287 2023-07-02 17:49:30.104509 reflex_ui-0.1.3/reflex/generated/index.html
+-rw-r--r--   0        0        0     4350 2023-07-02 17:49:30.834510 reflex_ui-0.1.3/reflex/generated/style.css
+-rw-r--r--   0        0        0     7562 2023-07-02 17:49:30.837843 reflex_ui-0.1.3/reflex/generated/style.css.map
+-rw-r--r--   0        0        0    75209 2022-04-21 09:32:25.000000 reflex_ui-0.1.3/reflex/hosted-assets/showdown.min.js
+-rw-r--r--   0        0        0     2521 2023-07-14 08:25:05.986574 reflex_ui-0.1.3/reflex/image_source.py
+-rw-r--r--   0        0        0     1229 2023-06-02 09:31:52.003332 reflex_ui-0.1.3/reflex/messages.py
+-rw-r--r--   0        0        0    38949 2023-07-14 07:51:46.796596 reflex_ui-0.1.3/reflex/session.py
+-rw-r--r--   0        0        0      123 2023-07-14 08:25:08.029908 reflex_ui-0.1.3/reflex/styling/__init__.py
+-rw-r--r--   0        0        0     3605 2023-07-14 07:53:45.156595 reflex_ui-0.1.3/reflex/styling/box_style.py
+-rw-r--r--   0        0        0     9391 2023-06-16 18:28:59.043338 reflex_ui-0.1.3/reflex/styling/color.py
+-rw-r--r--   0        0        0     2751 2023-07-14 07:53:45.159928 reflex_ui-0.1.3/reflex/styling/fills.py
+-rw-r--r--   0        0        0     2673 2023-07-14 08:24:26.589908 reflex_ui-0.1.3/reflex/styling/markdown_style.py
+-rw-r--r--   0        0        0     1762 2023-07-14 08:24:26.586575 reflex_ui-0.1.3/reflex/styling/text_style.py
+-rw-r--r--   0        0        0      274 2023-05-30 05:41:43.000000 reflex_ui-0.1.3/reflex/theme.py
+-rw-r--r--   0        0        0    12658 2023-07-14 08:24:26.576575 reflex_ui-0.1.3/reflex/validator.py
+-rw-r--r--   0        0        0      466 2023-07-14 08:40:58.956564 reflex_ui-0.1.3/reflex/widgets/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-14 08:25:06.019908 reflex_ui-0.1.3/reflex/widgets/auto_form.py
+-rw-r--r--   0        0        0     8439 2023-07-02 17:50:56.411212 reflex_ui-0.1.3/reflex/widgets/button.py
+-rw-r--r--   0        0        0     1577 2023-07-02 17:50:56.411212 reflex_ui-0.1.3/reflex/widgets/column.py
+-rw-r--r--   0        0        0      226 2023-05-27 11:53:20.000000 reflex_ui-0.1.3/reflex/widgets/container.py
+-rw-r--r--   0        0        0     1827 2023-07-14 08:24:26.603242 reflex_ui-0.1.3/reflex/widgets/dropdown.py
+-rw-r--r--   0        0        0      506 2023-07-14 08:25:06.009908 reflex_ui-0.1.3/reflex/widgets/image.py
+-rw-r--r--   0        0        0     1175 2023-07-14 08:24:26.609908 reflex_ui-0.1.3/reflex/widgets/markdown_view.py
+-rw-r--r--   0        0        0      575 2023-07-14 08:25:06.013241 reflex_ui-0.1.3/reflex/widgets/media_player.py
+-rw-r--r--   0        0        0      939 2023-07-14 08:40:58.959897 reflex_ui-0.1.3/reflex/widgets/metadata.py
+-rw-r--r--   0        0        0     3524 2023-06-10 18:04:23.870009 reflex_ui-0.1.3/reflex/widgets/mouse_event_listener.py
+-rw-r--r--   0        0        0      498 2023-07-14 08:36:51.036567 reflex_ui-0.1.3/reflex/widgets/plot.py
+-rw-r--r--   0        0        0     1665 2023-07-02 17:50:56.411212 reflex_ui-0.1.3/reflex/widgets/progress_circle.py
+-rw-r--r--   0        0        0      506 2023-07-14 08:24:26.603242 reflex_ui-0.1.3/reflex/widgets/rectangle.py
+-rw-r--r--   0        0        0     1594 2023-07-02 17:44:56.264397 reflex_ui-0.1.3/reflex/widgets/row.py
+-rw-r--r--   0        0        0      242 2023-05-27 11:53:20.000000 reflex_ui-0.1.3/reflex/widgets/stack.py
+-rw-r--r--   0        0        0     1566 2023-07-14 08:24:26.606575 reflex_ui-0.1.3/reflex/widgets/switch.py
+-rw-r--r--   0        0        0      363 2023-05-28 16:37:28.000000 reflex_ui-0.1.3/reflex/widgets/text.py
+-rw-r--r--   0        0        0     1894 2023-07-14 08:24:26.606575 reflex_ui-0.1.3/reflex/widgets/text_input.py
+-rw-r--r--   0        0        0    20757 2023-07-02 17:50:56.414545 reflex_ui-0.1.3/reflex/widgets/widget_base.py
+-rw-r--r--   0        0        0     3890 2023-07-14 08:24:26.583241 reflex_ui-0.1.3/reflex/world_units.py
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 reflex_ui-0.1.3/PKG-INFO
```

### Comparing `reflex_ui-0.1.2/LICENSE.txt` & `reflex_ui-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/pyproject.toml` & `reflex_ui-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex-ui"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>", "Paul Pinterits"]
 readme = "README.md"
 packages = [{ include = "reflex" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -15,15 +15,15 @@
 pillow = "^9.5.0"
 pygobject = { version = "^3.44.1", platform = "linux", optional = true }
 pytest = "^7.3.1"
 python-multipart = "^0.0.6"
 pywebview = { version = "^4.2.2", optional = true }
 timer-dict = "^1.0.0"
 typing-extensions = "^4.5.0"
-uniserde = "^0.2.5"
+uniserde = "^0.3.0"
 uvicorn = "^0.22.0"
 websockets = "^11.0.3"
 
 [tool.poetry.extras]
 window = ["cefpython3", "pygobject", "pywebview"]
```

### Comparing `reflex_ui-0.1.2/reflex/app.py` & `reflex_ui-0.1.3/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/app_server.py` & `reflex_ui-0.1.3/reflex/app_server.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/assets.py` & `reflex_ui-0.1.3/reflex/assets.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/common.py` & `reflex_ui-0.1.3/reflex/common.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/generated/app.js` & `reflex_ui-0.1.3/reflex/generated/app.js`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/generated/app.js.map` & `reflex_ui-0.1.3/reflex/generated/app.js.map`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/generated/style.css` & `reflex_ui-0.1.3/reflex/generated/style.css`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/generated/style.css.map` & `reflex_ui-0.1.3/reflex/generated/style.css.map`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/hosted-assets/showdown.min.js` & `reflex_ui-0.1.3/reflex/hosted-assets/showdown.min.js`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/image_source.py` & `reflex_ui-0.1.3/reflex/image_source.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/messages.py` & `reflex_ui-0.1.3/reflex/messages.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/session.py` & `reflex_ui-0.1.3/reflex/session.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/styling/box_style.py` & `reflex_ui-0.1.3/reflex/styling/box_style.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/styling/color.py` & `reflex_ui-0.1.3/reflex/styling/color.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/styling/fills.py` & `reflex_ui-0.1.3/reflex/styling/fills.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/styling/markdown_style.py` & `reflex_ui-0.1.3/reflex/styling/markdown_style.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/styling/text_style.py` & `reflex_ui-0.1.3/reflex/styling/text_style.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/validator.py` & `reflex_ui-0.1.3/reflex/validator.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/auto_form.py` & `reflex_ui-0.1.3/reflex/widgets/auto_form.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/button.py` & `reflex_ui-0.1.3/reflex/widgets/button.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/column.py` & `reflex_ui-0.1.3/reflex/widgets/column.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/dropdown.py` & `reflex_ui-0.1.3/reflex/widgets/dropdown.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/markdown_view.py` & `reflex_ui-0.1.3/reflex/widgets/markdown_view.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/media_player.py` & `reflex_ui-0.1.3/reflex/widgets/media_player.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/metadata.py` & `reflex_ui-0.1.3/reflex/widgets/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/mouse_event_listener.py` & `reflex_ui-0.1.3/reflex/widgets/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/progress_circle.py` & `reflex_ui-0.1.3/reflex/widgets/progress_circle.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/row.py` & `reflex_ui-0.1.3/reflex/widgets/row.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/switch.py` & `reflex_ui-0.1.3/reflex/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/text_input.py` & `reflex_ui-0.1.3/reflex/widgets/text_input.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/widgets/widget_base.py` & `reflex_ui-0.1.3/reflex/widgets/widget_base.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/reflex/world_units.py` & `reflex_ui-0.1.3/reflex/world_units.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.2/PKG-INFO` & `reflex_ui-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-ui
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,13 +16,13 @@
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pygobject (>=3.44.1,<4.0.0) ; (sys_platform == "linux") and (extra == "window")
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: pywebview (>=4.2.2,<5.0.0) ; extra == "window"
 Requires-Dist: timer-dict (>=1.0.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: uniserde (>=0.2.5,<0.3.0)
+Requires-Dist: uniserde (>=0.3.0,<0.4.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
```

