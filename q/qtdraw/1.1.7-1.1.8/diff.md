# Comparing `tmp/qtdraw-1.1.7.tar.gz` & `tmp/qtdraw-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdraw-1.1.7.tar", last modified: Mon Jul 31 04:49:05 2023, max compression
+gzip compressed data, was "qtdraw-1.1.8.tar", last modified: Mon Jul 31 11:56:17 2023, max compression
```

## Comparing `qtdraw-1.1.7.tar` & `qtdraw-1.1.8.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.988092 qtdraw-1.1.7/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.7/LICENSE
--rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.7/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 04:49:05.988185 qtdraw-1.1.7/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     2141 2023-07-30 16:22:53.000000 qtdraw-1.1.7/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.979145 qtdraw-1.1.7/qtdraw/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-31 04:39:03.000000 qtdraw-1.1.7/qtdraw/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.986284 qtdraw-1.1.7/qtdraw/core/
--rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/basic_object.py
--rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/color_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/color_palette.py
--rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/default_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/dialog_about.py
--rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/dialog_preference.py
--rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/editable_widget.py
--rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_tab.py
--rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/group_view.py
--rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/line_edit.py
--rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.7/qtdraw/core/pixmap_converter.py
--rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/qt_logging.py
--rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/qtdraw.png
--rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/qtdraw.ui
--rw-r--r--   0 hiro       (501) staff       (20)    17651 2023-07-30 16:22:54.000000 qtdraw-1.1.7/qtdraw/core/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/table_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/tree_item.py
--rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.7/qtdraw/core/tree_item_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.7/qtdraw/core/util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/core/validator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.987222 qtdraw-1.1.7/qtdraw/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.7/qtdraw/multipie/dialog_group.py
--rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.7/qtdraw/multipie/dialog_group_info.py
--rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/multipie/setting.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.987553 qtdraw-1.1.7/qtdraw/parser/
--rw-r--r--   0 hiro       (501) staff       (20)     5984 2023-07-30 16:22:54.000000 qtdraw-1.1.7/qtdraw/parser/element.py
--rw-r--r--   0 hiro       (501) staff       (20)     5802 2023-07-31 04:36:25.000000 qtdraw-1.1.7/qtdraw/parser/read_cif.py
--rw-r--r--   0 hiro       (501) staff       (20)    92461 2023-07-30 16:22:54.000000 qtdraw-1.1.7/qtdraw/qt_draw.py
--rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.7/qtdraw/qt_draw_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.987839 qtdraw-1.1.7/qtdraw/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.7/qtdraw/scripts/qtdraw.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 04:49:05.980185 qtdraw-1.1.7/qtdraw.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1053 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)      127 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-31 04:49:05.000000 qtdraw-1.1.7/qtdraw.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      753 2023-07-31 04:49:05.988500 qtdraw-1.1.7/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.7/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.670512 qtdraw-1.1.8/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.8/LICENSE
+-rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.8/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 11:56:17.670595 qtdraw-1.1.8/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     2141 2023-07-30 16:22:53.000000 qtdraw-1.1.8/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.662486 qtdraw-1.1.8/qtdraw/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2023-07-31 11:33:10.000000 qtdraw-1.1.8/qtdraw/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.668797 qtdraw-1.1.8/qtdraw/core/
+-rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/basic_object.py
+-rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/color_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/color_palette.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/default_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/dialog_about.py
+-rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/dialog_preference.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/editable_widget.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_tab.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/group_view.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/line_edit.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.8/qtdraw/core/pixmap_converter.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/qt_logging.py
+-rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/qtdraw.png
+-rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/qtdraw.ui
+-rw-r--r--   0 hiro       (501) staff       (20)    17651 2023-07-30 16:22:54.000000 qtdraw-1.1.8/qtdraw/core/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/table_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/tree_item.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-24 14:55:28.000000 qtdraw-1.1.8/qtdraw/core/tree_item_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7490 2023-07-29 10:18:46.000000 qtdraw-1.1.8/qtdraw/core/util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/core/validator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.669552 qtdraw-1.1.8/qtdraw/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)    48651 2023-07-29 13:47:38.000000 qtdraw-1.1.8/qtdraw/multipie/dialog_group.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.8/qtdraw/multipie/dialog_group_info.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/multipie/setting.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.670066 qtdraw-1.1.8/qtdraw/parser/
+-rw-r--r--   0 hiro       (501) staff       (20)     5984 2023-07-30 16:22:54.000000 qtdraw-1.1.8/qtdraw/parser/element.py
+-rw-r--r--   0 hiro       (501) staff       (20)     6330 2023-07-31 11:45:17.000000 qtdraw-1.1.8/qtdraw/parser/read_cif_vesta.py
+-rw-------   0 hiro       (501) staff       (20)     2983 2023-07-31 11:45:03.000000 qtdraw-1.1.8/qtdraw/parser/vesta.py
+-rw-r--r--   0 hiro       (501) staff       (20)    92584 2023-07-31 11:36:18.000000 qtdraw-1.1.8/qtdraw/qt_draw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.8/qtdraw/qt_draw_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.670283 qtdraw-1.1.8/qtdraw/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      486 2023-05-26 22:04:11.000000 qtdraw-1.1.8/qtdraw/scripts/qtdraw.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-07-31 11:56:17.663480 qtdraw-1.1.8/qtdraw.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2521 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1082 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       53 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      127 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        7 2023-07-31 11:56:17.000000 qtdraw-1.1.8/qtdraw.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      753 2023-07-31 11:56:17.670845 qtdraw-1.1.8/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.8/setup.py
```

### Comparing `qtdraw-1.1.7/LICENSE` & `qtdraw-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/PKG-INFO` & `qtdraw-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.7
+Version: 1.1.8
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # QtDraw
 
 3D drawing tool for molecules and crystals based on [PyVista](https://docs.pyvista.org/) and [Qt](https://www.riverbankcomputing.com/static/Docs/PyQt5/#).
```

### Comparing `qtdraw-1.1.7/README.md` & `qtdraw-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/basic_object.py` & `qtdraw-1.1.8/qtdraw/core/basic_object.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/color_dialog.py` & `qtdraw-1.1.8/qtdraw/core/color_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/color_palette.py` & `qtdraw-1.1.8/qtdraw/core/color_palette.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/default_panel.ui` & `qtdraw-1.1.8/qtdraw/core/default_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/dialog_about.py` & `qtdraw-1.1.8/qtdraw/core/dialog_about.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/dialog_preference.py` & `qtdraw-1.1.8/qtdraw/core/dialog_preference.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/editable_widget.py` & `qtdraw-1.1.8/qtdraw/core/editable_widget.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/group_model.py` & `qtdraw-1.1.8/qtdraw/core/group_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/group_panel.ui` & `qtdraw-1.1.8/qtdraw/core/group_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/group_tab.py` & `qtdraw-1.1.8/qtdraw/core/group_tab.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/group_view.py` & `qtdraw-1.1.8/qtdraw/core/group_view.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/line_edit.py` & `qtdraw-1.1.8/qtdraw/core/line_edit.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/pixmap_converter.py` & `qtdraw-1.1.8/qtdraw/core/pixmap_converter.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/qt_logging.py` & `qtdraw-1.1.8/qtdraw/core/qt_logging.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/qtdraw.png` & `qtdraw-1.1.8/qtdraw/core/qtdraw.png`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/qtdraw.ui` & `qtdraw-1.1.8/qtdraw/core/qtdraw.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/setting.py` & `qtdraw-1.1.8/qtdraw/core/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/table_dialog.py` & `qtdraw-1.1.8/qtdraw/core/table_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/tree_item.py` & `qtdraw-1.1.8/qtdraw/core/tree_item.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/tree_item_model.py` & `qtdraw-1.1.8/qtdraw/core/tree_item_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/util.py` & `qtdraw-1.1.8/qtdraw/core/util.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/core/validator.py` & `qtdraw-1.1.8/qtdraw/core/validator.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/multipie/dialog_group.py` & `qtdraw-1.1.8/qtdraw/multipie/dialog_group.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/multipie/dialog_group_info.py` & `qtdraw-1.1.8/qtdraw/multipie/dialog_group_info.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/multipie/setting.py` & `qtdraw-1.1.8/qtdraw/multipie/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/parser/element.py` & `qtdraw-1.1.8/qtdraw/parser/element.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw/parser/read_cif.py` & `qtdraw-1.1.8/qtdraw/parser/read_cif_vesta.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pymatgen.io.cif import CifParser
 from pymatgen.analysis.graphs import StructureGraph
 from pymatgen.analysis.local_env import MinimumDistanceNN
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.core.periodic_table import Element
 from qtdraw.parser.element import element_color
 from qtdraw.core.setting import rcParams
+from qtdraw.parser.vesta import parse_vesta, create_vesta_graph
 
 color_scheme = rcParams["plotter.color_scheme"]
 digit = 6
 
 
 # ==================================================
 def get_graph(file):
@@ -186,7 +187,24 @@
         filename (str): filename.
     """
     graph = get_graph(filename)
     name, cell, volume = get_model_cell(graph)
     site_info = get_site_info(graph)
     bond_info = get_bond_info(graph, site_info)
     plot_site_bond(qtdraw, name, cell, volume, site_info, bond_info)
+
+
+# ==================================================
+def plot_vesta(qtdraw, filename):
+    """
+    read and plot VESTA file.
+
+    Args:
+        filename (str): filename.
+    """
+    vesta_dict = parse_vesta(filename)
+    graph = create_vesta_graph(vesta_dict)
+
+    name, cell, volume = get_model_cell(graph)
+    site_info = get_site_info(graph)
+    bond_info = get_bond_info(graph, site_info)
+    plot_site_bond(qtdraw, name, cell, volume, site_info, bond_info)
```

### Comparing `qtdraw-1.1.7/qtdraw/qt_draw.py` & `qtdraw-1.1.8/qtdraw/qt_draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     create_plane,
     create_box,
     create_polygon,
     create_text,
     create_spline,
 )
 from qtdraw.core.color_palette import all_colors, custom_colormap, check_color
-from qtdraw.parser.read_cif import plot_cif
+from qtdraw.parser.read_cif_vesta import plot_cif, plot_vesta
 from qtdraw import __version__
 
 from qtdraw.core.qt_logging import UncaughtHook
 
 CHOP = 1e-4
 qt_exception_hook = UncaughtHook()
 global QT_EXCEPTION_HOOK
@@ -1647,15 +1647,15 @@
             self.tab.deselectedData.connect(self._remove_spotlight)
             self.tab.finished["int"].connect(self._close_dialog)
             self.tab.show()
 
     # ==================================================
     def _load(self):
         default_ext = rcParams["plotter.ext"]
-        loadable_ext = rcParams["plotter.cif"]  # +" "+rcParams["plotter.vesta"]
+        loadable_ext = rcParams["plotter.cif"] + " " + rcParams["plotter.vesta"]
         default_file = os.getcwd()
         ext_str = default_ext + " " + loadable_ext
         filename, _ = QFileDialog.getOpenFileName(
             self, "Load QtDraw", default_file, "QtDraw file (" + ext_str.replace(".", "*.") + ")"
         )
         if filename:
             _, ext = os.path.splitext(filename)
@@ -1673,14 +1673,17 @@
     def _load_file(self, filename, ext):
         self._homedir = os.path.dirname(filename)
         os.chdir(self._homedir)
 
         if ext == rcParams["plotter.cif"]:
             plot_cif(self, filename)
             return
+        elif ext == rcParams["plotter.vesta"]:
+            plot_vesta(self, filename)
+            return
 
         load_dict = read_dict(filename)
 
         self.preference = load_dict["preference"]
         self.setting = load_dict["setting"]
         self._remove_all_actor()
         self._init_all()
```

### Comparing `qtdraw-1.1.7/qtdraw/qt_draw_base.py` & `qtdraw-1.1.8/qtdraw/qt_draw_base.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.7/qtdraw.egg-info/PKG-INFO` & `qtdraw-1.1.8/qtdraw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.7
+Version: 1.1.8
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # QtDraw
 
 3D drawing tool for molecules and crystals based on [PyVista](https://docs.pyvista.org/) and [Qt](https://www.riverbankcomputing.com/static/Docs/PyQt5/#).
```

### Comparing `qtdraw-1.1.7/qtdraw.egg-info/SOURCES.txt` & `qtdraw-1.1.8/qtdraw.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -34,9 +34,10 @@
 qtdraw/core/tree_item_model.py
 qtdraw/core/util.py
 qtdraw/core/validator.py
 qtdraw/multipie/dialog_group.py
 qtdraw/multipie/dialog_group_info.py
 qtdraw/multipie/setting.py
 qtdraw/parser/element.py
-qtdraw/parser/read_cif.py
+qtdraw/parser/read_cif_vesta.py
+qtdraw/parser/vesta.py
 qtdraw/scripts/qtdraw.py
```

### Comparing `qtdraw-1.1.7/setup.cfg` & `qtdraw-1.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = pyvista, qtpy5
 license = MIT
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.9
 install_requires = 
 	matplotlib
 	seaborn
 	pyqt5
 	pyvista
 	pyvistaqt
 	click
```

