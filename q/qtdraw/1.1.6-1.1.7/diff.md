# Comparing `tmp/qtdraw-1.1.6.tar.gz` & `tmp/qtdraw-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdraw-1.1.6.tar", last modified: Mon Jul 31 00:15:40 2023, max compression
+gzip compressed data, was "qtdraw-1.1.7.tar", last modified: Mon Jul 31 04:49:05 2023, max compression
```

## Comparing `qtdraw-1.1.6.tar` & `qtdraw-1.1.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 00:15:40.378050 qtdraw-1.1.6/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.6/LICENSE
--rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.6/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 00:15:40.378156 qtdraw-1.1.6/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     2141 2023-07-30 16:22:53.000000 qtdraw-1.1.6/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 00:15:40.369832 qtdraw-1.1.6/qtdraw/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-31 00:09:06.000000 qtdraw-1.1.6/qtdraw/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 00:15:40.376475 qtdraw-1.1.6/qtdraw/core/
--rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.6/qtdraw/core/basic_object.py
--rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/color_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.6/qtdraw/core/color_palette.py
--rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/default_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.6/qtdraw/core/dialog_about.py
--rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/dialog_preference.py
--rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.6/qtdraw/core/editable_widget.py
--rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/group_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/group_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/group_tab.py
--rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/group_view.py
--rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.6/qtdraw/core/line_edit.py
--rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.6/qtdraw/core/pixmap_converter.py
--rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/qt_logging.py
--rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/qtdraw.png
--rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/qtdraw.ui
--rw-r--r--   0 hiro       (501) staff       (20)    17651 2023-07-30 16:22:54.000000 qtdraw-1.1.6/qtdraw/core/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/table_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/tree_item.py
--rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.6/qtdraw/core/tree_item_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.6/qtdraw/core/util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/core/validator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 00:15:40.377287 qtdraw-1.1.6/qtdraw/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.6/qtdraw/multipie/dialog_group.py
--rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.6/qtdraw/multipie/dialog_group_info.py
--rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/multipie/setting.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 00:15:40.377593 qtdraw-1.1.6/qtdraw/parser/
--rw-r--r--   0 hiro       (501) staff       (20)     5984 2023-07-30 16:22:54.000000 qtdraw-1.1.6/qtdraw/parser/element.py
--rw-r--r--   0 hiro       (501) staff       (20)     5501 2023-07-31 00:05:08.000000 qtdraw-1.1.6/qtdraw/parser/read_cif.py
--rw-r--r--   0 hiro       (501) staff       (20)    92461 2023-07-30 16:22:54.000000 qtdraw-1.1.6/qtdraw/qt_draw.py
--rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.6/qtdraw/qt_draw_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 00:15:40.377809 qtdraw-1.1.6/qtdraw/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.6/qtdraw/scripts/qtdraw.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 00:15:40.371009 qtdraw-1.1.6/qtdraw.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 00:15:40.000000 qtdraw-1.1.6/qtdraw.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1053 2023-07-31 00:15:40.000000 qtdraw-1.1.6/qtdraw.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-31 00:15:40.000000 qtdraw-1.1.6/qtdraw.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-31 00:15:40.000000 qtdraw-1.1.6/qtdraw.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)      127 2023-07-31 00:15:40.000000 qtdraw-1.1.6/qtdraw.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-31 00:15:40.000000 qtdraw-1.1.6/qtdraw.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      753 2023-07-31 00:15:40.378465 qtdraw-1.1.6/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.6/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.988092 qtdraw-1.1.7/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.7/LICENSE
+-rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.7/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 04:49:05.988185 qtdraw-1.1.7/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     2141 2023-07-30 16:22:53.000000 qtdraw-1.1.7/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.979145 qtdraw-1.1.7/qtdraw/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-31 04:39:03.000000 qtdraw-1.1.7/qtdraw/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.986284 qtdraw-1.1.7/qtdraw/core/
+-rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/basic_object.py
+-rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/color_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/color_palette.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/default_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/dialog_about.py
+-rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/dialog_preference.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/editable_widget.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_tab.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_view.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/line_edit.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/pixmap_converter.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/qt_logging.py
+-rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/qtdraw.png
+-rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/qtdraw.ui
+-rw-r--r--   0 hiro       (501) staff       (20)    17651 2023-07-30 16:22:54.000000 qtdraw-1.1.7/qtdraw/core/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/table_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/tree_item.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.7/qtdraw/core/tree_item_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.7/qtdraw/core/util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/validator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.987222 qtdraw-1.1.7/qtdraw/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.7/qtdraw/multipie/dialog_group.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.7/qtdraw/multipie/dialog_group_info.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/multipie/setting.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.987553 qtdraw-1.1.7/qtdraw/parser/
+-rw-r--r--   0 hiro       (501) staff       (20)     5984 2023-07-30 16:22:54.000000 qtdraw-1.1.7/qtdraw/parser/element.py
+-rw-r--r--   0 hiro       (501) staff       (20)     5802 2023-07-31 04:36:25.000000 qtdraw-1.1.7/qtdraw/parser/read_cif.py
+-rw-r--r--   0 hiro       (501) staff       (20)    92461 2023-07-30 16:22:54.000000 qtdraw-1.1.7/qtdraw/qt_draw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/qt_draw_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.987839 qtdraw-1.1.7/qtdraw/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.7/qtdraw/scripts/qtdraw.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.980185 qtdraw-1.1.7/qtdraw.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1053 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      127 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      753 2023-07-31 04:49:05.988500 qtdraw-1.1.7/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.7/setup.py
```

### Comparing `qtdraw-1.1.6/LICENSE` & `qtdraw-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/PKG-INFO` & `qtdraw-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.6
+Version: 1.1.7
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
```

### Comparing `qtdraw-1.1.6/README.md` & `qtdraw-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/basic_object.py` & `qtdraw-1.1.7/qtdraw/core/basic_object.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/color_dialog.py` & `qtdraw-1.1.7/qtdraw/core/color_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/color_palette.py` & `qtdraw-1.1.7/qtdraw/core/color_palette.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/default_panel.ui` & `qtdraw-1.1.7/qtdraw/core/default_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/dialog_about.py` & `qtdraw-1.1.7/qtdraw/core/dialog_about.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/dialog_preference.py` & `qtdraw-1.1.7/qtdraw/core/dialog_preference.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/editable_widget.py` & `qtdraw-1.1.7/qtdraw/core/editable_widget.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/group_model.py` & `qtdraw-1.1.7/qtdraw/core/group_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/group_panel.ui` & `qtdraw-1.1.7/qtdraw/core/group_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/group_tab.py` & `qtdraw-1.1.7/qtdraw/core/group_tab.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/group_view.py` & `qtdraw-1.1.7/qtdraw/core/group_view.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/line_edit.py` & `qtdraw-1.1.7/qtdraw/core/line_edit.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/pixmap_converter.py` & `qtdraw-1.1.7/qtdraw/core/pixmap_converter.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/qt_logging.py` & `qtdraw-1.1.7/qtdraw/core/qt_logging.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/qtdraw.png` & `qtdraw-1.1.7/qtdraw/core/qtdraw.png`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/qtdraw.ui` & `qtdraw-1.1.7/qtdraw/core/qtdraw.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/setting.py` & `qtdraw-1.1.7/qtdraw/core/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/table_dialog.py` & `qtdraw-1.1.7/qtdraw/core/table_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/tree_item.py` & `qtdraw-1.1.7/qtdraw/core/tree_item.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/tree_item_model.py` & `qtdraw-1.1.7/qtdraw/core/tree_item_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/util.py` & `qtdraw-1.1.7/qtdraw/core/util.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/core/validator.py` & `qtdraw-1.1.7/qtdraw/core/validator.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/multipie/dialog_group.py` & `qtdraw-1.1.7/qtdraw/multipie/dialog_group.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/multipie/dialog_group_info.py` & `qtdraw-1.1.7/qtdraw/multipie/dialog_group_info.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/multipie/setting.py` & `qtdraw-1.1.7/qtdraw/multipie/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/parser/element.py` & `qtdraw-1.1.7/qtdraw/parser/element.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/parser/read_cif.py` & `qtdraw-1.1.7/qtdraw/parser/read_cif.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from pymatgen.io.cif import CifParser
 from pymatgen.analysis.graphs import StructureGraph
 from pymatgen.analysis.local_env import MinimumDistanceNN
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
+from pymatgen.core.periodic_table import Element
 from qtdraw.parser.element import element_color
 from qtdraw.core.setting import rcParams
 
 color_scheme = rcParams["plotter.color_scheme"]
 digit = 6
 
 
@@ -73,28 +74,35 @@
     """
     structure = graph.structure
     eq_sites = structure.equivalent_sites
 
     # grouping equivalent sites.
     dsites = {}
     for es in eq_sites:
-        el = es[0].species_string
+        el = es[0].specie
+        if type(el) != type(Element):
+            el = str(el).replace("0+", "")
+        else:
+            el = el.symbol
         dsites[el] = dsites.get(el, []) + [es]
 
     site_info = []
     for name, v in dsites.items():
         for el_no, sl in enumerate(v):
             el_name = name + str(el_no + 1)
             for s_no, s in enumerate(sl):
                 s_name = el_name + "_" + str(s_no + 1)
-                s_element = s.species_string
                 frac_coords = s.frac_coords.round(digit)
-                radius = float(s.specie.atomic_radius)
-                color = element_color[color_scheme][s_element]
-                site_info.append((el_name, s_name, s_element, frac_coords, radius, color))
+                if name in element_color[color_scheme].keys():
+                    radius = float(s.specie.atomic_radius)
+                    color = element_color[color_scheme][name]
+                else:
+                    radius = 1.0
+                    color = "silver"
+                site_info.append((el_name, s_name, name, frac_coords, radius, color))
 
     return site_info
 
 
 # ==================================================
 def get_bond_info(graph, site_info):
     """
@@ -111,16 +119,16 @@
 
     dbonds = {}
     for tail, tail_adjacency in zip(site_info, adjacency):
         t_name, _, _, t_pos, _, t_c = tail
         for head_info in tail_adjacency:
             h_name, _, _, h_pos, _, h_c = site_info[head_info["id"]]
             h_pos = np.array(head_info["to_jimage"]) + h_pos
-            center = (t_pos + h_pos) / 2
-            vector = h_pos - t_pos
+            center = ((t_pos + h_pos) / 2).round(digit)
+            vector = (h_pos - t_pos).round(digit)
             key = t_name + "-" + h_name
             dbonds[key] = dbonds.get(key, []) + [(center, vector, t_c, h_c)]
 
     bond_info = []
     for name, v in dbonds.items():
         for no, (center, vector, t_c, h_c) in enumerate(v):
             label = name + "_" + str(no + 1)
```

### Comparing `qtdraw-1.1.6/qtdraw/qt_draw.py` & `qtdraw-1.1.7/qtdraw/qt_draw.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw/qt_draw_base.py` & `qtdraw-1.1.7/qtdraw/qt_draw_base.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/qtdraw.egg-info/PKG-INFO` & `qtdraw-1.1.7/qtdraw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.6
+Version: 1.1.7
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
```

### Comparing `qtdraw-1.1.6/qtdraw.egg-info/SOURCES.txt` & `qtdraw-1.1.7/qtdraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.6/setup.cfg` & `qtdraw-1.1.7/setup.cfg`

 * *Files identical despite different names*

