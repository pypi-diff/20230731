# Comparing `tmp/ex4nicegui-0.2.6.tar.gz` & `tmp/ex4nicegui-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.2.6.tar", last modified: Sat Jul 29 10:19:35 2023, max compression
+gzip compressed data, was "ex4nicegui-0.2.7.tar", last modified: Mon Jul 31 03:23:57 2023, max compression
```

## Comparing `ex4nicegui-0.2.6.tar` & `ex4nicegui-0.2.7.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.162919 ex4nicegui-0.2.6/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-29 10:19:35.161945 ex4nicegui-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.028019 ex4nicegui-0.2.6/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-29 10:19:11.000000 ex4nicegui-0.2.6/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.043004 ex4nicegui-0.2.6/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.055945 ex4nicegui-0.2.6/ex4nicegui/reactive/
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.091067 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/
--rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.js
--rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.096053 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/
--rw-rw-rw-   0        0        0     5235 2023-07-29 10:16:43.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3501 2023-07-29 10:16:43.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/__init__.py
--rw-rw-rw-   0        0        0      412 2023-07-29 10:16:25.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.097079 ex4nicegui-0.2.6/ex4nicegui/reactive/dropZone/
--rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/dropZone/dropZone.js
--rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/local_file_picker.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.145948 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/
--rw-rw-rw-   0        0        0     1468 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/aggrid.py
--rw-rw-rw-   0        0        0     4242 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/base.py
--rw-rw-rw-   0        0        0     2250 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/button.py
--rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/card.py
--rw-rw-rw-   0        0        0     1769 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/checkbox.py
--rw-rw-rw-   0        0        0     2744 2023-07-23 13:10:30.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/color_picker.py
--rw-rw-rw-   0        0        0      413 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/column.py
--rw-rw-rw-   0        0        0     2700 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/date.py
--rw-rw-rw-   0        0        0     2443 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/drawer.py
--rw-rw-rw-   0        0        0     1783 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/echarts.py
--rw-rw-rw-   0        0        0      925 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/grid.py
--rw-rw-rw-   0        0        0     1687 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/html.py
--rw-rw-rw-   0        0        0     1600 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/icon.py
--rw-rw-rw-   0        0        0     1440 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/image.py
--rw-rw-rw-   0        0        0     3337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/input.py
--rw-rw-rw-   0        0        0     1756 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/label.py
--rw-rw-rw-   0        0        0     2058 2023-07-29 10:16:16.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/number.py
--rw-rw-rw-   0        0        0     2080 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/radio.py
--rw-rw-rw-   0        0        0      404 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/row.py
--rw-rw-rw-   0        0        0     2482 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/select.py
--rw-rw-rw-   0        0        0     2607 2023-07-23 13:10:30.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/slider.py
--rw-rw-rw-   0        0        0     1979 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/switch.py
--rw-rw-rw-   0        0        0     3903 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/table.py
--rw-rw-rw-   0        0        0     2728 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/textarea.py
--rw-rw-rw-   0        0        0     2337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/upload.py
--rw-rw-rw-   0        0        0      205 2023-07-21 14:29:40.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/officials/utils.py
--rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/rxui.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.150937 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2468 2023-07-19 08:10:43.000000 ex4nicegui-0.2.6/ex4nicegui/reactive/usePagination.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.154897 ex4nicegui-0.2.6/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.2.6/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.2.6/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.159924 ex4nicegui-0.2.6/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.6/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.2.6/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.2.6/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:19:35.038990 ex4nicegui-0.2.6/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2181 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-29 10:19:34.000000 ex4nicegui-0.2.6/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 10:19:35.162919 ex4nicegui-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-07-18 10:52:21.000000 ex4nicegui-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.176568 ex4nicegui-0.2.7/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-31 03:23:57.173609 ex4nicegui-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.005434 ex4nicegui-0.2.7/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-31 03:21:42.000000 ex4nicegui-0.2.7/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.019218 ex4nicegui-0.2.7/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.2.7/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.2.7/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.031928 ex4nicegui-0.2.7/ex4nicegui/reactive/
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.039890 ex4nicegui-0.2.7/ex4nicegui/reactive/ECharts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/ECharts/ECharts.js
+-rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/ECharts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/ECharts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.044876 ex4nicegui-0.2.7/ex4nicegui/reactive/UseDraggable/
+-rw-rw-rw-   0        0        0     5235 2023-07-29 10:16:43.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3501 2023-07-29 10:16:43.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-07-29 10:16:25.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.075710 ex4nicegui-0.2.7/ex4nicegui/reactive/dropZone/
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:21:34.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/dropZone/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-07-29 10:16:25.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/dropZone/dropZone.js
+-rw-rw-rw-   0        0        0     2582 2023-07-29 10:16:25.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/dropZone/dropZone.py
+-rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/local_file_picker.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.124581 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/
+-rw-rw-rw-   0        0        0     1468 2023-07-29 10:16:16.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/aggrid.py
+-rw-rw-rw-   0        0        0     4242 2023-07-29 10:16:16.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/base.py
+-rw-rw-rw-   0        0        0     2250 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/button.py
+-rw-rw-rw-   0        0        0     1275 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/card.py
+-rw-rw-rw-   0        0        0     1769 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/checkbox.py
+-rw-rw-rw-   0        0        0     2744 2023-07-23 13:10:30.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/color_picker.py
+-rw-rw-rw-   0        0        0      413 2023-07-29 10:16:16.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/column.py
+-rw-rw-rw-   0        0        0     2700 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/date.py
+-rw-rw-rw-   0        0        0     2443 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/drawer.py
+-rw-rw-rw-   0        0        0     1783 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/echarts.py
+-rw-rw-rw-   0        0        0      925 2023-07-29 10:16:16.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/grid.py
+-rw-rw-rw-   0        0        0     1687 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/html.py
+-rw-rw-rw-   0        0        0     1600 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/icon.py
+-rw-rw-rw-   0        0        0     1440 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/image.py
+-rw-rw-rw-   0        0        0     3337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/input.py
+-rw-rw-rw-   0        0        0     1756 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/label.py
+-rw-rw-rw-   0        0        0     2058 2023-07-29 10:16:16.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/number.py
+-rw-rw-rw-   0        0        0     2080 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/radio.py
+-rw-rw-rw-   0        0        0      404 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/row.py
+-rw-rw-rw-   0        0        0     2680 2023-07-31 03:21:34.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/select.py
+-rw-rw-rw-   0        0        0     2607 2023-07-23 13:10:30.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/slider.py
+-rw-rw-rw-   0        0        0     1979 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/switch.py
+-rw-rw-rw-   0        0        0     3903 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/table.py
+-rw-rw-rw-   0        0        0     2728 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/textarea.py
+-rw-rw-rw-   0        0        0     2337 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/upload.py
+-rw-rw-rw-   0        0        0      205 2023-07-21 14:29:40.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/officials/utils.py
+-rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/rxui.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.129569 ex4nicegui-0.2.7/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2468 2023-07-19 08:10:43.000000 ex4nicegui-0.2.7/ex4nicegui/reactive/usePagination.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.132561 ex4nicegui-0.2.7/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.2.7/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.2.7/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.169587 ex4nicegui-0.2.7/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.7/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.2.7/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-30 21:29:07.000000 ex4nicegui-0.2.7/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:23:57.016224 ex4nicegui-0.2.7/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-31 03:23:56.000000 ex4nicegui-0.2.7/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2263 2023-07-31 03:23:56.000000 ex4nicegui-0.2.7/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 03:23:56.000000 ex4nicegui-0.2.7/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-31 03:23:56.000000 ex4nicegui-0.2.7/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-31 03:23:56.000000 ex4nicegui-0.2.7/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 03:23:56.000000 ex4nicegui-0.2.7/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 03:23:57.176568 ex4nicegui-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-07-18 10:52:21.000000 ex4nicegui-0.2.7/setup.py
```

### Comparing `ex4nicegui-0.2.6/LICENSE` & `ex4nicegui-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/README.md` & `ex4nicegui-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.2.7/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.js` & `ex4nicegui-0.2.7/ex4nicegui/reactive/ECharts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/ECharts/ECharts.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/ECharts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.js` & `ex4nicegui-0.2.7/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/UseDraggable/UseDraggable.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/dropZone/dropZone.js` & `ex4nicegui-0.2.7/ex4nicegui/reactive/dropZone/dropZone.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/__init__.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/__init__.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/aggrid.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/aggrid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/base.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/base.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/button.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/button.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/card.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/card.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/checkbox.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/checkbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/color_picker.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/color_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/date.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/date.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/drawer.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/echarts.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/echarts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/grid.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/grid.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/html.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/html.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/icon.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/icon.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/image.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/image.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/input.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/input.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/label.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/label.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/number.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/number.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/radio.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/radio.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/select.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/select.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,22 @@
 
 T = TypeVar("T")
 
 
 class SelectBindableUi(SingleValueBindableUi[T, ui.select]):
     @staticmethod
     def _setup_(binder: "SelectBindableUi"):
+        opts_values = (
+            list(binder.element.options.keys())
+            if isinstance(binder.element.options, Dict)
+            else binder.element.options
+        )
+
         def onValueChanged(e):
-            binder._ref.value = e.args["label"]  # type: ignore
+            binder._ref.value = opts_values[e.args["value"]]  # type: ignore
 
         @effect
         def _():
             binder.element.value = binder.value
 
         binder.element.on("update:modelValue", handler=onValueChanged)
```

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/slider.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/slider.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/switch.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/switch.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/table.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/table.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/textarea.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/textarea.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/officials/upload.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/officials/upload.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/q_pagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.2.7/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.2.7/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/tools/debug.py` & `ex4nicegui-0.2.7/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui/utils/signals.py` & `ex4nicegui-0.2.7/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.2.6/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.2.7/ex4nicegui.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 ex4nicegui/reactive/usePagination.py
 ex4nicegui/reactive/ECharts/ECharts.js
 ex4nicegui/reactive/ECharts/ECharts.py
 ex4nicegui/reactive/ECharts/__init__.py
 ex4nicegui/reactive/UseDraggable/UseDraggable.js
 ex4nicegui/reactive/UseDraggable/UseDraggable.py
 ex4nicegui/reactive/UseDraggable/__init__.py
+ex4nicegui/reactive/dropZone/__init__.py
 ex4nicegui/reactive/dropZone/dropZone.js
+ex4nicegui/reactive/dropZone/dropZone.py
 ex4nicegui/reactive/officials/__init__.py
 ex4nicegui/reactive/officials/aggrid.py
 ex4nicegui/reactive/officials/base.py
 ex4nicegui/reactive/officials/button.py
 ex4nicegui/reactive/officials/card.py
 ex4nicegui/reactive/officials/checkbox.py
 ex4nicegui/reactive/officials/color_picker.py
```

### Comparing `ex4nicegui-0.2.6/setup.py` & `ex4nicegui-0.2.7/setup.py`

 * *Files identical despite different names*

