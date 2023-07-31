# Comparing `tmp/tablate-0.0.7.tar.gz` & `tmp/tablate-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablate-0.0.7.tar", last modified: Sun Jul 23 05:01:03 2023, max compression
+gzip compressed data, was "tablate-0.0.8.tar", last modified: Mon Jul 31 08:45:20 2023, max compression
```

## Comparing `tablate-0.0.7.tar` & `tablate-0.0.8.tar`

### file list

```diff
@@ -1,143 +1,200 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.493357 tablate-0.0.7/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.7/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      553 2023-07-23 05:01:03.493357 tablate-0.0.7/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 00:33:05.000000 tablate-0.0.7/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      627 2023-07-23 05:00:53.000000 tablate-0.0.7/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-23 05:01:03.494356 tablate-0.0.7/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.470357 tablate-0.0.7/tablate/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      366 2023-07-23 04:53:06.000000 tablate-0.0.7/tablate/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.471356 tablate-0.0.7/tablate/api/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     7168 2023-07-23 04:59:42.000000 tablate-0.0.7/tablate/api/Tablate.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.7/tablate/api/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.471356 tablate-0.0.7/tablate/api/functions/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 04:48:05.000000 tablate-0.0.7/tablate/api/functions/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1015 2023-07-23 04:56:02.000000 tablate-0.0.7/tablate/api/functions/concat.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.472357 tablate-0.0.7/tablate/api/modules/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2147 2023-07-23 04:24:03.000000 tablate-0.0.7/tablate/api/modules/Grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3763 2023-07-23 04:24:03.000000 tablate-0.0.7/tablate/api/modules/Table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2063 2023-07-23 04:24:03.000000 tablate-0.0.7/tablate/api/modules/Text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 01:25:25.000000 tablate-0.0.7/tablate/api/modules/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.472357 tablate-0.0.7/tablate/classes/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:53:19.000000 tablate-0.0.7/tablate/classes/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.473357 tablate-0.0.7/tablate/classes/bases/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1736 2023-07-23 04:41:22.000000 tablate-0.0.7/tablate/classes/bases/TablateApi.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      172 2023-07-23 02:12:14.000000 tablate-0.0.7/tablate/classes/bases/TablateBase.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1316 2023-07-23 04:52:22.000000 tablate-0.0.7/tablate/classes/bases/TablateSet.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:25:16.000000 tablate-0.0.7/tablate/classes/bases/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.473357 tablate-0.0.7/tablate/classes/options/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.7/tablate/classes/options/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.473357 tablate-0.0.7/tablate/classes/options/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.7/tablate/classes/options/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.473357 tablate-0.0.7/tablate/classes/options/html/style/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4529 2023-07-23 04:41:22.000000 tablate-0.0.7/tablate/classes/options/html/style/StyleCss.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.7/tablate/classes/options/html/style/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.474357 tablate-0.0.7/tablate/classes/options/html/style/mixins/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      508 2023-07-22 10:49:03.000000 tablate-0.0.7/tablate/classes/options/html/style/mixins/AddStyleMixin.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      515 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/classes/options/html/style/mixins/ClassNameMixin.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 01:07:40.000000 tablate-0.0.7/tablate/classes/options/html/style/mixins/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.475356 tablate-0.0.7/tablate/classes/options/html/style/subclasses/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2399 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/classes/options/html/style/subclasses/ElementStyle.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      583 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/classes/options/html/style/subclasses/TableStyle.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      674 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/classes/options/html/style/subclasses/TextStyle.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.7/tablate/classes/options/html/style/subclasses/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.477357 tablate-0.0.7/tablate/classes/options/html/style/utilities/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 15:13:12.000000 tablate-0.0.7/tablate/classes/options/html/style/utilities/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      231 2023-07-22 10:49:03.000000 tablate-0.0.7/tablate/classes/options/html/style/utilities/base_names.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2281 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/classes/options/html/style/utilities/css_factory.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      876 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/classes/options/html/style/utilities/selectors.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      881 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/classes/options/html/style/utilities/style_dict.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.477357 tablate-0.0.7/tablate/library/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.7/tablate/library/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.477357 tablate-0.0.7/tablate/library/calcs/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.7/tablate/library/calcs/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      801 2023-07-23 04:58:20.000000 tablate-0.0.7/tablate/library/calcs/calc_column_percent.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2599 2023-07-23 04:37:08.000000 tablate-0.0.7/tablate/library/calcs/calc_column_widths.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.7/tablate/library/calcs/get_row_colspan.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-23 04:37:08.000000 tablate-0.0.7/tablate/library/calcs/random_string.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.478356 tablate-0.0.7/tablate/library/chars/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.7/tablate/library/chars/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.7/tablate/library/chars/corners.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.7/tablate/library/chars/line_h.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.7/tablate/library/chars/line_v.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.7/tablate/library/chars/matrix_cross.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.7/tablate/library/chars/matrix_side.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.479357 tablate-0.0.7/tablate/library/checkers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.7/tablate/library/checkers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.7/tablate/library/checkers/is_last_element.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.479357 tablate-0.0.7/tablate/library/formatters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.7/tablate/library/formatters/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.480357 tablate-0.0.7/tablate/library/formatters/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.7/tablate/library/formatters/console/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4579 2023-07-20 08:05:59.000000 tablate-0.0.7/tablate/library/formatters/console/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      545 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/formatters/console/row_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3107 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/formatters/console/row_divider.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.480357 tablate-0.0.7/tablate/library/formatters/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.7/tablate/library/formatters/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.481356 tablate-0.0.7/tablate/library/formatters/html/element/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.7/tablate/library/formatters/html/element/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      717 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/formatters/html/element/column.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      486 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/formatters/html/element/frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      115 2023-07-22 11:20:40.000000 tablate-0.0.7/tablate/library/formatters/html/element/row.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      275 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/formatters/html/element/text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.481356 tablate-0.0.7/tablate/library/formatters/html/style/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.7/tablate/library/formatters/html/style/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      416 2023-07-19 23:18:14.000000 tablate-0.0.7/tablate/library/formatters/html/style/border_style.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.481356 tablate-0.0.7/tablate/library/formatters/html/style/elements/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:02:02.000000 tablate-0.0.7/tablate/library/formatters/html/style/elements/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      706 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/formatters/html/style/elements/column_style.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      389 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/formatters/html/style/elements/frame_style.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      734 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/formatters/html/style/elements/text_style.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.482357 tablate-0.0.7/tablate/library/initializers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2111 2023-07-23 04:24:03.000000 tablate-0.0.7/tablate/library/initializers/grid_init.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3653 2023-07-23 03:30:08.000000 tablate-0.0.7/tablate/library/initializers/table_init.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      917 2023-07-23 04:37:08.000000 tablate-0.0.7/tablate/library/initializers/text_init.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.483357 tablate-0.0.7/tablate/library/renderers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.7/tablate/library/renderers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.484356 tablate-0.0.7/tablate/library/renderers/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.7/tablate/library/renderers/console/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.486357 tablate-0.0.7/tablate/library/renderers/console/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.7/tablate/library/renderers/console/frames/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2039 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/renderers/console/frames/render_console_columns.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2490 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/renderers/console/frames/render_console_frame_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3829 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/renderers/console/frames/render_string_frame_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1893 2023-07-23 04:37:08.000000 tablate-0.0.7/tablate/library/renderers/console/frames/render_string_frame_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      765 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/renderers/console/render_console.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      803 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/renderers/console/render_console_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2320 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/renderers/console/render_console_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      780 2023-07-22 22:49:28.000000 tablate-0.0.7/tablate/library/renderers/console/render_console_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.488356 tablate-0.0.7/tablate/library/renderers/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.7/tablate/library/renderers/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.489357 tablate-0.0.7/tablate/library/renderers/html/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3024 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/renderers/html/frames/render_html_columns.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6150 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/renderers/html/frames/render_html_table_body.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2532 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/library/renderers/html/frames/render_html_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1340 2023-07-23 04:41:22.000000 tablate-0.0.7/tablate/library/renderers/html/render_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.7/tablate/library/renderers/html/render_html_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1698 2023-07-23 04:41:22.000000 tablate-0.0.7/tablate/library/renderers/html/render_html_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1797 2023-07-23 04:41:22.000000 tablate-0.0.7/tablate/library/renderers/html/render_html_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.489357 tablate-0.0.7/tablate/library/validators/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:45.000000 tablate-0.0.7/tablate/library/validators/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.491356 tablate-0.0.7/tablate/tests/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 00:41:48.000000 tablate-0.0.7/tablate/tests/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.491356 tablate-0.0.7/tablate/tests/playpen/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      303 2023-07-23 02:37:58.000000 tablate-0.0.7/tablate/tests/playpen/func_sigs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      362 2023-07-23 04:53:06.000000 tablate-0.0.7/tablate/tests/test_api_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3569 2023-07-22 12:51:12.000000 tablate-0.0.7/tablate/tests/test_defs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8000 2023-07-22 23:55:35.000000 tablate-0.0.7/tablate/tests/test_objs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 22:51:46.000000 tablate-0.0.7/tablate/tests/test_out_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.7/tablate/tests/test_out_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      951 2023-07-22 23:05:00.000000 tablate-0.0.7/tablate/tests/test_styles.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.493357 tablate-0.0.7/tablate/type/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.7/tablate/type/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      414 2023-07-20 10:49:54.000000 tablate-0.0.7/tablate/type/primitives.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      312 2023-07-23 04:56:17.000000 tablate-0.0.7/tablate/type/type_class.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2370 2023-07-23 04:37:08.000000 tablate-0.0.7/tablate/type/type_frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      156 2023-07-22 12:45:12.000000 tablate-0.0.7/tablate/type/type_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      626 2023-07-20 23:50:14.000000 tablate-0.0.7/tablate/type/type_input.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      725 2023-07-23 04:41:22.000000 tablate-0.0.7/tablate/type/type_options.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1024 2023-07-22 08:41:42.000000 tablate-0.0.7/tablate/type/type_style.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 05:01:03.470357 tablate-0.0.7/tablate.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      553 2023-07-23 05:01:03.000000 tablate-0.0.7/tablate.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4529 2023-07-23 05:01:03.000000 tablate-0.0.7/tablate.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-23 05:01:03.000000 tablate-0.0.7/tablate.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-23 05:01:03.000000 tablate-0.0.7/tablate.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.552162 tablate-0.0.8/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.8/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      554 2023-07-31 08:45:20.552162 tablate-0.0.8/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-24 14:23:22.000000 tablate-0.0.8/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      628 2023-07-31 08:44:51.000000 tablate-0.0.8/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-31 08:45:20.552162 tablate-0.0.8/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.524162 tablate-0.0.8/tablate/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      392 2023-07-25 22:27:18.000000 tablate-0.0.8/tablate/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.529162 tablate-0.0.8/tablate/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    18347 2023-07-31 07:08:49.000000 tablate-0.0.8/tablate/api/Future.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:31:19.000000 tablate-0.0.8/tablate/api/ITablate.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8378 2023-07-31 05:10:14.000000 tablate-0.0.8/tablate/api/Tablate.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.8/tablate/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.529162 tablate-0.0.8/tablate/api/functions/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 04:48:05.000000 tablate-0.0.8/tablate/api/functions/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      993 2023-07-25 19:43:31.000000 tablate-0.0.8/tablate/api/functions/concat.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.530161 tablate-0.0.8/tablate/api/modules/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2115 2023-07-26 02:21:08.000000 tablate-0.0.8/tablate/api/modules/Grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3627 2023-07-28 12:18:13.000000 tablate-0.0.8/tablate/api/modules/Table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2031 2023-07-25 02:00:37.000000 tablate-0.0.8/tablate/api/modules/Text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 01:25:25.000000 tablate-0.0.8/tablate/api/modules/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.530161 tablate-0.0.8/tablate/classes/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:53:19.000000 tablate-0.0.8/tablate/classes/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/bases/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:32:45.000000 tablate-0.0.8/tablate/classes/bases/ITablateApi.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     5597 2023-07-31 04:47:30.000000 tablate-0.0.8/tablate/classes/bases/TablateApi.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      173 2023-07-26 01:09:49.000000 tablate-0.0.8/tablate/classes/bases/TablateBase.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 03:32:13.000000 tablate-0.0.8/tablate/classes/bases/TablateInit.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1329 2023-07-25 00:08:00.000000 tablate-0.0.8/tablate/classes/bases/TablateSet.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 22:25:16.000000 tablate-0.0.8/tablate/classes/bases/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      311 2023-07-25 22:32:01.000000 tablate-0.0.8/tablate/classes/classes.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/options/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.8/tablate/classes/options/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/options/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.8/tablate/classes/options/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.531162 tablate-0.0.8/tablate/classes/options/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4877 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/CssStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.8/tablate/classes/options/html/style/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.532162 tablate-0.0.8/tablate/classes/options/html/style/mixins/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      611 2023-07-30 04:43:48.000000 tablate-0.0.8/tablate/classes/options/html/style/mixins/AddStyleMixin.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      549 2023-07-25 00:34:59.000000 tablate-0.0.8/tablate/classes/options/html/style/mixins/ClassNameMixin.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 01:07:40.000000 tablate-0.0.8/tablate/classes/options/html/style/mixins/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.532162 tablate-0.0.8/tablate/classes/options/html/style/subclasses/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2587 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/ElementStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      616 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/TableStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      717 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/TextStyler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 13:24:20.000000 tablate-0.0.8/tablate/classes/options/html/style/subclasses/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.533161 tablate-0.0.8/tablate/classes/options/html/style/utilities/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-21 15:13:12.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      286 2023-07-25 00:34:59.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/base_values.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3007 2023-07-30 03:15:25.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/css_factory.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1210 2023-07-25 00:34:59.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/selectors.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      876 2023-07-30 03:03:58.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/style_dict.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1102 2023-07-30 03:00:29.000000 tablate-0.0.8/tablate/classes/options/html/style/utilities/style_types.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.533161 tablate-0.0.8/tablate/library/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.8/tablate/library/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.533161 tablate-0.0.8/tablate/library/ascii/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 07:07:45.000000 tablate-0.0.8/tablate/library/ascii/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.534162 tablate-0.0.8/tablate/library/ascii/chars/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.8/tablate/library/ascii/chars/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.8/tablate/library/ascii/chars/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.8/tablate/library/ascii/chars/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.8/tablate/library/ascii/chars/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.8/tablate/library/ascii/chars/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.8/tablate/library/ascii/chars/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.534162 tablate-0.0.8/tablate/library/ascii/colors/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      479 2023-07-31 05:59:34.000000 tablate-0.0.8/tablate/library/ascii/colors/background.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      471 2023-07-31 05:59:34.000000 tablate-0.0.8/tablate/library/ascii/colors/characters.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.535162 tablate-0.0.8/tablate/library/ascii/styles/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      110 2023-07-31 05:58:51.000000 tablate-0.0.8/tablate/library/ascii/styles/styles.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.535162 tablate-0.0.8/tablate/library/calcs/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.8/tablate/library/calcs/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      833 2023-07-29 00:59:58.000000 tablate-0.0.8/tablate/library/calcs/calc_column_percent.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3035 2023-07-30 04:43:48.000000 tablate-0.0.8/tablate/library/calcs/calc_column_widths.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.8/tablate/library/calcs/get_row_colspan.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-23 04:37:08.000000 tablate-0.0.8/tablate/library/calcs/random_string.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.536162 tablate-0.0.8/tablate/library/checkers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.8/tablate/library/checkers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.8/tablate/library/checkers/is_last_element.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      256 2023-07-30 03:50:35.000000 tablate-0.0.8/tablate/library/checkers/set_attr_resolver.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      174 2023-07-31 06:00:43.000000 tablate-0.0.8/tablate/library/checkers/set_key_resolver.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.536162 tablate-0.0.8/tablate/library/formatters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.8/tablate/library/formatters/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.537161 tablate-0.0.8/tablate/library/formatters/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.8/tablate/library/formatters/console/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1065 2023-07-31 06:41:45.000000 tablate-0.0.8/tablate/library/formatters/console/ascii_styler.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     5248 2023-07-31 06:38:14.000000 tablate-0.0.8/tablate/library/formatters/console/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      648 2023-07-31 06:55:06.000000 tablate-0.0.8/tablate/library/formatters/console/row_colors.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3458 2023-07-28 21:39:04.000000 tablate-0.0.8/tablate/library/formatters/console/row_line_divider.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      826 2023-07-28 20:40:34.000000 tablate-0.0.8/tablate/library/formatters/console/row_outer_border.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.537161 tablate-0.0.8/tablate/library/formatters/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.8/tablate/library/formatters/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.538162 tablate-0.0.8/tablate/library/formatters/html/element/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.8/tablate/library/formatters/html/element/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      721 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/formatters/html/element/column.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      490 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/formatters/html/element/frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      273 2023-07-30 04:59:45.000000 tablate-0.0.8/tablate/library/formatters/html/element/row.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      278 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/formatters/html/element/text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.538162 tablate-0.0.8/tablate/library/formatters/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.8/tablate/library/formatters/html/style/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.539162 tablate-0.0.8/tablate/library/formatters/html/style/attributes/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-29 02:34:03.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1144 2023-07-31 07:15:41.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/color.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      546 2023-07-31 02:08:02.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/divider.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      161 2023-07-29 02:49:27.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/padding.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      387 2023-07-29 07:37:01.000000 tablate-0.0.8/tablate/library/formatters/html/style/attributes/text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.540161 tablate-0.0.8/tablate/library/formatters/html/style/elements/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 12:02:02.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4439 2023-07-31 02:13:45.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_column.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2128 2023-07-31 01:51:02.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1734 2023-07-31 06:57:10.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_rows.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1364 2023-07-31 01:27:34.000000 tablate-0.0.8/tablate/library/formatters/html/style/elements/style_text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-23 07:32:48.000000 tablate-0.0.8/tablate/library/initializers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4324 2023-07-31 04:59:57.000000 tablate-0.0.8/tablate/library/initializers/grid_init.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/mappers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:39.000000 tablate-0.0.8/tablate/library/initializers/mappers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/mappers/attribute/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-28 12:24:21.000000 tablate-0.0.8/tablate/library/initializers/mappers/attribute/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4880 2023-07-31 06:57:30.000000 tablate-0.0.8/tablate/library/initializers/mappers/attribute/column_attr.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.541162 tablate-0.0.8/tablate/library/initializers/mappers/element/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-28 12:21:58.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.543161 tablate-0.0.8/tablate/library/initializers/mappers/element/base/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:39.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1520 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_column_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2980 2023-07-31 04:59:31.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_frame_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1895 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_rows_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1930 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/base/base_text_mapper.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.544161 tablate-0.0.8/tablate/library/initializers/mappers/element/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-27 09:01:47.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2241 2023-07-31 01:48:15.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_column_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3128 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_frame_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2758 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_outer_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2500 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_rows_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2485 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/html/html_text_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3889 2023-07-31 01:04:05.000000 tablate-0.0.8/tablate/library/initializers/mappers/element/style_mapper.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    11255 2023-07-31 04:59:14.000000 tablate-0.0.8/tablate/library/initializers/table_init.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4780 2023-07-31 04:59:41.000000 tablate-0.0.8/tablate/library/initializers/text_init.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.544161 tablate-0.0.8/tablate/library/renderers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.8/tablate/library/renderers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.545162 tablate-0.0.8/tablate/library/renderers/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.8/tablate/library/renderers/console/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.545162 tablate-0.0.8/tablate/library/renderers/console/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.8/tablate/library/renderers/console/frames/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1783 2023-07-29 00:45:05.000000 tablate-0.0.8/tablate/library/renderers/console/frames/render_console_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1991 2023-07-29 00:52:54.000000 tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3950 2023-07-31 06:56:57.000000 tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      766 2023-07-26 01:09:49.000000 tablate-0.0.8/tablate/library/renderers/console/render_console.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      848 2023-07-28 20:40:34.000000 tablate-0.0.8/tablate/library/renderers/console/render_console_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2059 2023-07-30 07:09:26.000000 tablate-0.0.8/tablate/library/renderers/console/render_console_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      825 2023-07-28 20:40:34.000000 tablate-0.0.8/tablate/library/renderers/console/render_console_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.546162 tablate-0.0.8/tablate/library/renderers/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.8/tablate/library/renderers/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.547161 tablate-0.0.8/tablate/library/renderers/html/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2752 2023-07-31 01:22:49.000000 tablate-0.0.8/tablate/library/renderers/html/frames/render_html_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2757 2023-07-31 01:28:00.000000 tablate-0.0.8/tablate/library/renderers/html/frames/render_html_table_body.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1330 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/library/renderers/html/render_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.8/tablate/library/renderers/html/render_html_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1517 2023-07-31 01:59:19.000000 tablate-0.0.8/tablate/library/renderers/html/render_html_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2078 2023-07-29 08:51:58.000000 tablate-0.0.8/tablate/library/renderers/html/render_html_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.548162 tablate-0.0.8/tablate/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-22 00:41:48.000000 tablate-0.0.8/tablate/tests/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.550161 tablate-0.0.8/tablate/tests/old/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      121 2023-07-23 05:13:34.000000 tablate-0.0.8/tablate/tests/old/test_api_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      362 2023-07-23 04:53:06.000000 tablate-0.0.8/tablate/tests/old/test_api_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       71 2023-07-23 05:12:51.000000 tablate-0.0.8/tablate/tests/old/test_api_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3544 2023-07-24 00:06:28.000000 tablate-0.0.8/tablate/tests/old/test_defs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8030 2023-07-23 07:18:53.000000 tablate-0.0.8/tablate/tests/old/test_objs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 22:51:46.000000 tablate-0.0.8/tablate/tests/old/test_out_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.8/tablate/tests/old/test_out_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      954 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/tests/old/test_styles.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.551162 tablate-0.0.8/tablate/tests/playpen/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-26 21:51:22.000000 tablate-0.0.8/tablate/tests/playpen/classsy.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-25 00:44:00.000000 tablate-0.0.8/tablate/tests/playpen/func_maps.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      273 2023-07-27 06:35:01.000000 tablate-0.0.8/tablate/tests/playpen/func_sigs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-25 00:44:00.000000 tablate-0.0.8/tablate/tests/playpen/key_of_dict.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2448 2023-07-23 08:39:36.000000 tablate-0.0.8/tablate/tests/playpen/loopy_test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       95 2023-07-31 06:17:44.000000 tablate-0.0.8/tablate/tests/playpen/modulus.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      195 2023-07-25 23:32:08.000000 tablate-0.0.8/tablate/tests/playpen/prototype_test.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      121 2023-07-23 05:13:34.000000 tablate-0.0.8/tablate/tests/test_api_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      362 2023-07-23 04:53:06.000000 tablate-0.0.8/tablate/tests/test_api_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       71 2023-07-23 05:12:51.000000 tablate-0.0.8/tablate/tests/test_api_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3544 2023-07-24 00:06:28.000000 tablate-0.0.8/tablate/tests/test_defs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8030 2023-07-23 07:18:53.000000 tablate-0.0.8/tablate/tests/test_objs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       74 2023-07-22 22:51:46.000000 tablate-0.0.8/tablate/tests/test_out_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-21 00:20:53.000000 tablate-0.0.8/tablate/tests/test_out_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      954 2023-07-29 21:18:27.000000 tablate-0.0.8/tablate/tests/test_styles.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.552162 tablate-0.0.8/tablate/type/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.8/tablate/type/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2774 2023-07-31 03:58:54.000000 tablate-0.0.8/tablate/type/defaults.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2280 2023-07-31 03:58:54.000000 tablate-0.0.8/tablate/type/primitives.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3558 2023-07-31 01:00:20.000000 tablate-0.0.8/tablate/type/type_base.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      914 2023-07-31 04:59:15.000000 tablate-0.0.8/tablate/type/type_global.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3847 2023-07-30 04:43:48.000000 tablate-0.0.8/tablate/type/type_input.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2652 2023-07-31 04:59:14.000000 tablate-0.0.8/tablate/type/type_store.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-31 08:45:20.528162 tablate-0.0.8/tablate.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      554 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     6883 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-31 08:45:20.000000 tablate-0.0.8/tablate.egg-info/top_level.txt
```

### Comparing `tablate-0.0.7/LICENCE` & `tablate-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `tablate-0.0.7/PKG-INFO` & `tablate-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.7
-Summary: A highly customizable and dynamic table renderer for IPython & CLI application.
+Version: 0.0.8
+Summary: A highly customizable and dynamic table renderer for IPython & CLI applications.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablate
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `tablate-0.0.7/pyproject.toml` & `tablate-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablate"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
-description = "A highly customizable and dynamic table renderer for IPython & CLI application."
+description = "A highly customizable and dynamic table renderer for IPython & CLI applications."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `tablate-0.0.7/tablate/api/functions/concat.py` & `tablate-0.0.8/tablate/api/functions/concat.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List
 
 from tablate.classes.bases.TablateSet import TablateSet
-from tablate.type.primitives import BaseDivider, Border
-from tablate.type.type_class import TablateUnion
+from tablate.type.primitives import FrameDivider, OuterBorder, TablateUnion
+
 
 def concat(tablate_set: List[TablateUnion],
-           border_style: Border = "thick",
-           frame_padding: int = 1,
-           frame_divider: BaseDivider = "thick",
-           frame_width: int = None,
+           outer_border: OuterBorder = "thick",
+           outer_padding: int = 1,
+           frame_divider: FrameDivider = "thick",
+           outer_width: int = None,
            html_px_size: int = 6,
            html_text_size: int = 12,
-           html_frame_width: str = "100%",
+           html_outer_width: str = "100%",
            html_css_injection: str = ""):
 
     return TablateSet(tablate_set=tablate_set,
-                      border_style=border_style,
-                      frame_padding=frame_padding,
+                      outer_border=outer_border,
+                      outer_padding=outer_padding,
                       frame_divider=frame_divider,
-                      frame_width=frame_width,
+                      outer_width=outer_width,
                       html_px_size=html_px_size,
                       html_text_size=html_text_size,
-                      html_frame_width=html_frame_width,
+                      html_outer_width=html_outer_width,
                       html_css_injection=html_css_injection)
```

### Comparing `tablate-0.0.7/tablate/api/modules/Grid.py` & `tablate-0.0.8/tablate/api/modules/Grid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 from typing import List, Union
 
 from tablate.classes.bases.TablateApi import TablateApi
 from tablate.library.initializers.grid_init import grid_init
-from tablate.type.primitives import BaseDivider, ColumnDivider, Border
-from tablate.type.type_input import GridInputColumnDict
+from tablate.type.primitives import FrameDivider, ColumnDivider, OuterBorder
+from tablate.type.type_input import GridColumnInput
 
 
 class Grid(TablateApi):
 
     def __init__(self,
                  # TablateGrid args
-                 columns: List[Union[str, GridInputColumnDict]],
+                 columns: List[Union[str, GridColumnInput]],
                  column_padding: int = 1,
                  column_divider: ColumnDivider = "thin",
-                 frame_base_divider: BaseDivider = "thick",
+                 frame_divider: FrameDivider = "thick",  # todo: doesn't make sense here
                  multiline: bool = True,
                  max_lines: int = None,
                  trunc_value: str = "...",
                  # TablateApi args
-                 border_style: Border = "thick",
-                 frame_padding: int = 1,
-                 frame_divider: BaseDivider = "thick",
-                 frame_width: int = None,
+                 outer_border: OuterBorder = "thick",
+                 outer_padding: int = 1,
+                 outer_width: int = None,
                  html_px_size: int = 6,
                  html_text_size: int = 12,
-                 html_frame_width: str = "100%",
+                 html_outer_width: str = "100%",
                  html_css_injection: str = "") -> None:
 
         TablateApi.__init__(self=self,
-                            border_style=border_style,
-                            frame_padding=frame_padding,
+                            outer_border=outer_border,
+                            outer_padding=outer_padding,
                             frame_divider=frame_divider,
-                            frame_width=frame_width,
+                            outer_width=outer_width,
                             html_px_size=html_px_size,
                             html_text_size=html_text_size,
-                            html_frame_width=html_frame_width,
+                            html_outer_width=html_outer_width,
                             html_css_injection=html_css_injection)
 
         grid_dict = grid_init(columns=columns,
                               column_padding=column_padding,
                               column_divider=column_divider,
-                              frame_base_divider=frame_base_divider,
+                              frame_divider=frame_divider,
                               multiline=multiline,
                               max_lines=max_lines,
                               trunc_value=trunc_value,
-                              frame_width=self._options["common"]["frame_width"])
+                              outer_width=self._options["console"]["outer_width"])
 
         self._frame_list.append(grid_dict)
```

### Comparing `tablate-0.0.7/tablate/api/modules/Table.py` & `tablate-0.0.8/tablate/api/modules/Table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 from typing import List, Dict, Union
 
 from tablate.classes.bases.TablateApi import TablateApi
 from tablate.library.initializers.table_init import table_init
-from tablate.type.primitives import BaseDivider, ColumnDivider, HeaderAlignment, HeaderColumnDivider, Border
-from tablate.type.type_input import TableInputColumnDict
+from tablate.type.primitives import FrameDivider, ColumnDivider, HeaderAlignment, HeaderColumnDivider, OuterBorder
+from tablate.type.type_input import TableColumnInput
 
 
 class Table(TablateApi):
 
     def __init__(self,
                  # TablateTable args
-                 columns: List[TableInputColumnDict],
+                 columns: List[TableColumnInput],
                  rows: List[Dict[str, Union[str, int, float]]],
-                 column_padding: int = 1,
-                 row_line_divider: BaseDivider = "thin",
-                 row_column_divider: ColumnDivider = "thin",
-                 frame_base_divider: BaseDivider = "thick",
-                 header_align: HeaderAlignment = "column",
-                 header_column_divider: HeaderColumnDivider = "rows",
-                 header_base_divider: BaseDivider = "thick",
+                 column_padding: int = None,
+                 row_line_divider: FrameDivider = None,
+                 row_column_divider: ColumnDivider = None,
+                 frame_divider: FrameDivider = None,  # todo: doesn't make sense here
+                 header_text_align: HeaderAlignment = None,
+                 header_column_divider: HeaderColumnDivider = None,
+                 header_frame_divider: FrameDivider = None,
                  multiline: bool = False,
                  max_lines: int = None,
                  multiline_header: bool = False,
                  max_lines_header: int = None,
                  hide_header: bool = False,
-                 head_trunc_value: str = ".",
-                 row_trunc_value: str = "...",
                  # TablateApi args
-                 border_style: Border = "thick",
-                 frame_padding: int = 1,
-                 frame_divider: BaseDivider = "thick",
-                 frame_width: int = None,
-                 html_px_size: int = 6,
-                 html_text_size: int = 12,
-                 html_frame_width: str = "100%",
+                 outer_border: OuterBorder = None,
+                 outer_padding: int = None,
+                 outer_width: int = None,
+                 html_px_size: int = None,
+                 html_text_size: int = None,
+                 html_outer_width: str = None,
                  html_css_injection: str = "") -> None:
 
         TablateApi.__init__(self=self,
-                            border_style=border_style,
-                            frame_padding=frame_padding,
+                            outer_border=outer_border,
+                            outer_padding=outer_padding,
                             frame_divider=frame_divider,
-                            frame_width=frame_width,
+                            outer_width=outer_width,
                             html_px_size=html_px_size,
                             html_text_size=html_text_size,
-                            html_frame_width=html_frame_width,
+                            html_outer_width=html_outer_width,
                             html_css_injection=html_css_injection)
 
         table_head_dict, table_rows_dict = table_init(columns=columns,
                                                       rows=rows,
                                                       column_padding=column_padding,
                                                       row_line_divider=row_line_divider,
                                                       row_column_divider=row_column_divider,
-                                                      frame_base_divider=frame_base_divider,
-                                                      header_align=header_align,
+                                                      frame_divider=frame_divider,
+                                                      header_text_align=header_text_align,
                                                       header_column_divider=header_column_divider,
-                                                      header_base_divider=header_base_divider,
+                                                      header_frame_divider=header_frame_divider,
                                                       multiline=multiline,
                                                       max_lines=max_lines,
                                                       multiline_header=multiline_header,
                                                       max_lines_header=max_lines_header,
                                                       hide_header=hide_header,
-                                                      head_trunc_value=head_trunc_value,
-                                                      row_trunc_value=row_trunc_value,
-                                                      frame_width=self._options["common"]["frame_width"])
+                                                      head_trunc_value="...",
+                                                      row_trunc_value="...",
+                                                      outer_width=self._options["console"]["outer_width"])
 
         if table_head_dict:
             self._frame_list.append(table_head_dict)
 
         self._frame_list.append(table_rows_dict)
```

### Comparing `tablate-0.0.7/tablate/classes/options/html/style/mixins/ClassNameMixin.py` & `tablate-0.0.8/tablate/classes/options/html/style/mixins/ClassNameMixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from tablate.classes.options.html.style.utilities.base_names import base_class
-from tablate.type.type_style import SelectorDictUnion
+from tablate.classes.options.html.style.utilities.base_values import base_class
+from tablate.classes.options.html.style.utilities.style_types import SelectorDictUnion
 
 
 class ClassNameMixin:
 
     _selector_dict: SelectorDictUnion
 
     def generate_class_names(self) -> str:
```

### Comparing `tablate-0.0.7/tablate/classes/options/html/style/subclasses/ElementStyle.py` & `tablate-0.0.8/tablate/classes/options/html/style/subclasses/ElementStyler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from copy import copy
-from typing import Callable, Union, List
+from typing import Callable, Union, List, Tuple, Optional
 
 from tablate.classes.options.html.style.mixins.AddStyleMixin import AddStyleMixin
 from tablate.classes.options.html.style.mixins.ClassNameMixin import ClassNameMixin
-from tablate.classes.options.html.style.subclasses.TextStyle import TextStyle
-from tablate.classes.options.html.style.utilities.selectors import column_selector, row_selector, \
-    element_append
-from tablate.type.type_style import SelectorDictUnion, ElementSelectorDict, ElementSelectorDictKeys
+from tablate.classes.options.html.style.subclasses.TextStyler import TextStyler
+from tablate.classes.options.html.style.utilities.selectors import column_selector, row_selector
+from tablate.classes.options.html.style.utilities.style_types import ElementSelectorDict, SelectorDictUnion, \
+    ElementSelectorDictKeys, StyleItem
 
 
-class ElementStyle(ClassNameMixin, AddStyleMixin):
+class ElementStyler(ClassNameMixin, AddStyleMixin):
 
     def __init__(self,
                  selector: ElementSelectorDict,
-                 create_style: Callable[[SelectorDictUnion, Union[str, List[str]]], None]) -> None:
+                 create_style: Callable[[SelectorDictUnion, StyleItem], None]) -> None:
         self._selector_dict = selector
         self._create_style = create_style
 
-    def column(self, column_index):
-        selector = self.__create_selector_dict(column_index=column_index)
-        return ElementStyle(selector=selector, create_style=self._create_style)
-
-    def row(self, row_index):
-        selector = self.__create_selector_dict(row_index=row_index)
-        return ElementStyle(selector=selector, create_style=self._create_style)
+    def column(self, column_index: int = None):
+        selector = self.__create_selector_dict(column=True, column_index=column_index)
+        return ElementStyler(selector=selector, create_style=self._create_style)
+
+    def row(self, row_index: int = None):
+        selector = self.__create_selector_dict(row=True, row_index=row_index)
+        return ElementStyler(selector=selector, create_style=self._create_style)
 
     @property
     def text(self):
         selector = self.__create_selector_dict(text_cell=True)
-        return TextStyle(selector=selector, create_style=self._create_style)
+        return TextStyler(selector=selector, create_style=self._create_style)
 
     def __create_selector_dict(self,
+                               column: bool = False,
                                column_index: int = None,
+                               row: bool = None,
                                row_index: int = None,
                                text_cell: bool = False) -> ElementSelectorDict:
         new_selector_dict: ElementSelectorDict = copy(self._selector_dict)
-        if column_index is not None:
-            base_type: ElementSelectorDictKeys = "tablate_column"
-            new_selector_dict["element_type"] = element_append(base_type)
+        if column:
+            # base_type: ElementSelectorDictKeys = "tablate_column"
+            new_selector_dict["element_type"]: ElementSelectorDictKeys = "tablate_column"
             new_selector_dict["tablate_column"] = column_selector(index=column_index)
-        if row_index is not None:
-            base_type: ElementSelectorDictKeys = "tablate_row"
-            new_selector_dict["element_type"] = element_append(base_type)
+        if row:
+            # base_type: ElementSelectorDictKeys = "tablate_row"
+            new_selector_dict["element_type"]: ElementSelectorDictKeys = "tablate_row"
             new_selector_dict["tablate_row"] = row_selector(index=row_index)
-        if text_cell is not False:
-            base_type: ElementSelectorDictKeys = "tablate_text"
-            new_selector_dict["element_type"] = element_append(base_type)
+        if text_cell:
+            # base_type: ElementSelectorDictKeys = "tablate_text"
+            new_selector_dict["element_type"]: ElementSelectorDictKeys = "tablate_text"
         return new_selector_dict
```

### Comparing `tablate-0.0.7/tablate/classes/options/html/style/subclasses/TableStyle.py` & `tablate-0.0.8/tablate/classes/options/html/style/subclasses/TableStyler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Union, List
 
 from tablate.classes.options.html.style.mixins.AddStyleMixin import AddStyleMixin
 from tablate.classes.options.html.style.mixins.ClassNameMixin import ClassNameMixin
-from tablate.type.type_style import TableSelectorDict, SelectorDictUnion
+from tablate.classes.options.html.style.utilities.style_types import TableSelectorDict, SelectorDictUnion, StyleItem
 
 
-class TableStyle(ClassNameMixin, AddStyleMixin):
+class TableStyler(ClassNameMixin, AddStyleMixin):
 
     def __init__(self,
                  selector: TableSelectorDict,
-                 create_style: Callable[[SelectorDictUnion, Union[str, List[str]]], None]) -> None:
+                 create_style: Callable[[SelectorDictUnion, StyleItem], None]) -> None:
         self._selector_dict = selector
         self._create_style = create_style
```

### Comparing `tablate-0.0.7/tablate/classes/options/html/style/subclasses/TextStyle.py` & `tablate-0.0.8/tablate/classes/options/html/style/subclasses/TextStyler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Callable, Union, List
+from typing import Callable, Union, List, Tuple, Optional
 
 from tablate.classes.options.html.style.mixins.AddStyleMixin import AddStyleMixin
 from tablate.classes.options.html.style.mixins.ClassNameMixin import ClassNameMixin
-from tablate.type.type_style import SelectorDictUnion
-from tablate.type.primitives import TextAlignment
+from tablate.classes.options.html.style.utilities.style_types import SelectorDictUnion, StyleItem
+from tablate.type.primitives import TextAlign
 
 
-class TextStyle(ClassNameMixin, AddStyleMixin):
+class TextStyler(ClassNameMixin, AddStyleMixin):
 
     def __init__(self, selector: SelectorDictUnion,
-                 create_style: Callable[[SelectorDictUnion, Union[str, List[str]]], None]) -> None:
+                 create_style: Callable[[SelectorDictUnion, StyleItem], None]) -> None:
         self._selector_dict: SelectorDictUnion = selector
         self._create_style = create_style
 
-    def alignment(self, align=TextAlignment):
-        pass
+    def alignment(self, align=TextAlign):
+        pass
```

### Comparing `tablate-0.0.7/tablate/classes/options/html/style/utilities/style_dict.py` & `tablate-0.0.8/tablate/classes/options/html/style/utilities/style_dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-from typing import Union
+from typing import Union, List, Optional, Tuple
 
-from tablate.classes.options.html.style.utilities.base_names import styles_key
-from tablate.type.type_style import SelectorDictUnion, SelectorDictKeysUnion
+from tablate.classes.options.html.style.utilities.base_values import styles_key
+from tablate.classes.options.html.style.utilities.style_types import SelectorDictUnion, SelectorDictKeysUnion, StyleItem
 
 
 def style_dict_key_builder(style_dict: dict, selector_dict: SelectorDictUnion, key: SelectorDictKeysUnion) -> Union[dict, list]:
     if key in selector_dict:
         if selector_dict[key] in style_dict:
             style_dict = style_dict[selector_dict[key]]
         else:
             style_dict[selector_dict[key]] = {}
             style_dict = style_dict[selector_dict[key]]
     return style_dict
 
 
-def style_dict_css_append(style_dict: dict, css: Union[str, list]):
-    if type(css) == str:
-        css = [css]
+def style_dict_css_append(style_dict: dict, css_item: StyleItem):
     if styles_key in style_dict:
-        for css_item in css:
-            style_dict[styles_key].append(css_item)
+        style_dict[styles_key].append(css_item)
     else:
-        style_dict[styles_key] = css
+        style_dict[styles_key] = [css_item]
     return style_dict
```

### Comparing `tablate-0.0.7/tablate/library/calcs/calc_column_widths.py` & `tablate-0.0.8/tablate/library/calcs/calc_column_widths.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,91 @@
-import copy
 import math
-from typing import List, TypeVar
+from typing import List, overload, TypeVar, Type
+
+from tablate.type.type_global import Options
+from tablate.type.type_input import BaseColumnInput, GridColumnInput, TableColumnInput
 
-T = TypeVar("T")
 
 def calc_column_width_error():
     raise Exception(
         f"Error computing width values. Please input check widths.")
 
-def calc_column_widths(columns: List[T], frame_width: int, column_padding: int) -> List[T]:
 
-    # todo: check keys are all in place => validator (probably not here though)
+@overload
+def calc_column_widths(columns: List[BaseColumnInput], options: Options) -> List[BaseColumnInput]:
+    ...
+
+
+@overload
+def calc_column_widths(columns: List[GridColumnInput], options: Options) -> List[GridColumnInput]:
+    ...
+
+
+@overload
+def calc_column_widths(columns: List[TableColumnInput], options: Options) -> List[TableColumnInput]:
+    ...
 
-    columns = copy.deepcopy(columns)
 
-    min_column_width = (column_padding * 2) + 1
+T = TypeVar("T", BaseColumnInput, GridColumnInput, TableColumnInput)
+
+
+def calc_column_widths(columns: List[Type[T]], options: Options) -> List[T]:
+
+    outer_width = options.console.outer_styles.outer_width
 
     total_defined_column_width = 0
     undefined_width_columns = []
 
     error = False
 
     for column_index, column_item in enumerate(columns):
 
         if "width" in column_item:
             validated_value = False
             if type(column_item["width"]) == str and column_item["width"][-1] == "%":
                 try:
-                    width_percentage = math.floor(frame_width / (100 / int(column_item["width"][0:-1]))) - 2
+                    width_percentage = math.floor(outer_width / (100 / int(column_item["width"][0:-1]))) - 2
                     column_item["width"] = width_percentage
                     validated_value = True
                 except TypeError:
                     error = True
             if type(column_item["width"]) == int:
-                if column_item["width"] < min_column_width:
-                    error = True
+                # if column_item["width"] < min_column_width:
+                #     error = True
                 total_defined_column_width += column_item["width"]
                 validated_value = True
             if not validated_value:
                 error = True
         else:
             undefined_width_columns.append(column_index)
 
     if error:
         calc_column_width_error()
 
     total_column_width = 0
 
     if len(undefined_width_columns):
-        calculated_width_total = frame_width - (total_defined_column_width + len(columns) + 1)
+        calculated_width_total = outer_width - (total_defined_column_width + len(columns) + 1)
         calculated_column_width = math.floor((calculated_width_total / len(undefined_width_columns)))
-        if calculated_column_width < min_column_width:
-            error = True
+        # if calculated_column_width < min_column_width:
+        #     error = True
         for column_index, column_item in enumerate(columns):
             if column_index in undefined_width_columns:
                 column_item["width"] = calculated_column_width
             total_column_width += column_item["width"]
     else:
         total_column_width = total_defined_column_width
 
     if error:
         calc_column_width_error()
 
-    if total_column_width + len(columns) + 1 > frame_width:
+    if total_column_width + len(columns) + 1 > outer_width:
         calc_column_width_error()
-    if total_column_width + len(columns) + 1 < frame_width:
+    if total_column_width + len(columns) + 1 < outer_width:
         if len(undefined_width_columns) > 0:
-            columns[undefined_width_columns[0]]["width"] += (frame_width - total_column_width) - (
+            columns[undefined_width_columns[0]]["width"] += (outer_width - total_column_width) - (
                     len(columns) + 1)
         else:
             calc_column_width_error()
 
     return columns
```

### Comparing `tablate-0.0.7/tablate/library/calcs/get_row_colspan.py` & `tablate-0.0.8/tablate/library/calcs/get_row_colspan.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.7/tablate/library/chars/matrix_cross.py` & `tablate-0.0.8/tablate/library/ascii/chars/matrix_cross.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.7/tablate/library/chars/matrix_side.py` & `tablate-0.0.8/tablate/library/ascii/chars/matrix_side.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.7/tablate/library/formatters/console/cell_string.py` & `tablate-0.0.8/tablate/library/formatters/console/cell_string.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 import math
 from typing import List, Optional
 
-from tablate.type.primitives import TextAlignment
+from tablate.library.formatters.console.ascii_styler import ascii_background_styler, \
+    ascii_text_styler, ascii_terminator
+from tablate.type.type_input import BaseColumnStyles
+from tablate.type.type_store import BaseColumnStore
 
 
 def cell_string_single_line(string: str,
-                            width: int,
-                            padding: int,
-                            align: TextAlignment,
+                            column_item: BaseColumnStore,
                             trunc_value: str = "...") -> str:
 
     string = str(string)
 
     string = string.split("\n")[0]
     string = " ".join(string.split("\t"))
 
-    if len(string) + (padding * 2) > width:
-        slice_outer_index = width - ((padding * 2) + len(trunc_value))
+    if "background_padding" in column_item and "background" in column_item and column_item["background_padding"] is not None and column_item["background"] is not None:
+        string = f"{' ' * column_item['background_padding']}{string}{' ' * column_item['background_padding']}"
+
+    if len(string) + (column_item["padding"] * 2) > column_item["width"]:
+        slice_outer_index = column_item["width"] - ((column_item["padding"] * 2) + len(trunc_value))
         if slice_outer_index < 1:
             trunc_value = trunc_value[0:len(trunc_value) - abs(slice_outer_index - 1)]
             slice_outer_index = 1
         string = f"{string[0:slice_outer_index]}{trunc_value}"
 
     return_string = ""
 
-    white_space = width - ((padding * 2) + len(string))
-
-    return_string += " " * padding
+    white_space = column_item["width"] - ((column_item["padding"] * 2) + len(string))
+    if column_item["text_color"] is not None or column_item["text_style"] is not None:
+        fore_space = len(string) - len(string.lstrip())
+        back_space = len(string) - len(string.rstrip())
+        string = (" " * fore_space) + ascii_text_styler(string=string.strip(), column_dict=column_item) + (" " * back_space)
 
-    if align == "left":
+    if column_item["text_align"] == "left":
         return_string += string
+        # return_string += ascii_text_styler_open(string=string, column_dict=column_styles)
         return_string += " " * white_space
-    if align == "center":
+    if column_item["text_align"] == "center":
         if white_space % 2 != 0:
             left_space = int(math.floor(white_space / 2))
             right_space = int(math.floor(white_space / 2) + 1)
         else:
             left_space = int(white_space / 2)
             right_space = int(white_space / 2)
         return_string += " " * left_space
         return_string += string
         return_string += " " * right_space
-    if align == "right":
+    if column_item["text_align"] == "right":
         return_string += " " * white_space
         return_string += string
 
-    return_string += " " * padding
+    if column_item["background"] is not None:
+        return_string = ascii_background_styler(string=return_string, column_dict=column_item)
+
+    padding = " " * column_item["padding"]
+    return_string = f"{padding}{return_string}{ascii_terminator()}{padding}"
 
     return return_string
 
 
 def cell_string_multi_line(string: str,
-                           width: int,
-                           padding: int,
-                           align: TextAlignment = "left",
+                           column_item: BaseColumnStyles,
                            max_lines: Optional[int] = None,
                            trunc_value: str = "...") -> List[str]:
 
     return_string_array = []
 
     string = str(string)
 
@@ -69,39 +78,33 @@
     for initial_string_item in initial_string_array:
         word_string_array = initial_string_item.split(" ")
         character_count = 0
         current_line_array = []
         for word_string_index, word_string_item in enumerate(word_string_array):
             last_line = max_lines is not None and len(return_string_array) == max_lines - 1
             character_count += len(word_string_item)
-            if (character_count + (padding * 2) < width) or (last_line and character_count + (padding * 2) < width + len(trunc_value)):
+            if (character_count + (column_item["padding"] * 2) < column_item["width"]) or (last_line and character_count + (column_item["padding"] * 2) < column_item["width"] + len(trunc_value)):
                 current_line_array.append(word_string_item)
             else:
                 if last_line:
                     current_line_array.append(word_string_item)
                     current_line_string = " ".join(current_line_array)
                     return_string_array.append(cell_string_single_line(string=current_line_string,
-                                                                       width=width,
-                                                                       padding=padding,
-                                                                       align=align,
+                                                                       column_item=column_item,
                                                                        trunc_value=trunc_value))
                     reached_max_lines = True
                     break
                 else:
                     current_line_string = " ".join(current_line_array)
                     return_string_array.append(cell_string_single_line(string=current_line_string,
-                                                                       width=width,
-                                                                       padding=padding,
-                                                                       align=align,
+                                                                       column_item=column_item,
                                                                        trunc_value=trunc_value))
                     current_line_array = [word_string_item]
                     character_count = len(word_string_item)
             character_count += 1
         if reached_max_lines:
             break
         current_line_string = " ".join(current_line_array)
         return_string_array.append(cell_string_single_line(string=current_line_string,
-                                                           width=width,
-                                                           padding=padding,
-                                                           align=align,
+                                                           column_item=column_item,
                                                            trunc_value=trunc_value))
     return return_string_array
```

### Comparing `tablate-0.0.7/tablate/library/formatters/console/row_border.py` & `tablate-0.0.8/tablate/library/formatters/console/row_outer_border.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,18 @@
-from tablate.library.chars.line_v import v_line
-from tablate.library.chars.matrix_side import left_side_matrix, right_side_matrix
-from tablate.type.primitives import Border, BaseDivider
+from tablate.library.ascii.chars.line_v import v_line
+from tablate.library.ascii.chars.matrix_side import left_side_matrix, right_side_matrix
+from tablate.type.primitives import FrameDivider
+from tablate.type.type_global import Options
 
 
-def row_border(row_string: str, outer_border: Border, row_divider: BaseDivider = None) -> str:
+def row_outer_border(row_string: str, options: Options, row_divider: FrameDivider = None) -> str:
+
+    outer_padding = options.console.outer_styles.outer_padding
+    outer_border = options.console.outer_styles.outer_border
+
     left_border = left_side_matrix[outer_border][row_divider] if row_divider else v_line[outer_border]
     right_border = right_side_matrix[outer_border][row_divider] if row_divider else v_line[outer_border]
-    return f"{left_border}{row_string}{right_border}"
+
+    grid_line_inner = f"{left_border}{row_string}{right_border}"
+    return_string = f"{' ' * outer_padding}{grid_line_inner}\n"
+
+    return return_string
```

### Comparing `tablate-0.0.7/tablate/library/formatters/html/element/column.py` & `tablate-0.0.8/tablate/library/formatters/html/element/column.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
-from tablate.classes.options.html.style.subclasses.ElementStyle import ElementStyle
-from tablate.type.type_html import HtmlCellElement
+from tablate.classes.options.html.style.subclasses.ElementStyler import ElementStyler
+from tablate.type.primitives import HtmlCellElement
 
 
-def html_column_head_formatter(column_styler: ElementStyle,
+def html_column_head_formatter(column_styler: ElementStyler,
                                column_index: int,
                                colspans: List[int],
                                column_element: HtmlCellElement = 'td'):
 
     return_html = ''
 
     column_classnames = column_styler.generate_class_names()
```

### Comparing `tablate-0.0.7/tablate/library/renderers/console/frames/render_console_columns.py` & `tablate-0.0.8/tablate/library/renderers/console/frames/render_console_columns.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 from typing import List
 
-from tablate.library.chars.line_v import v_line
+from tablate.library.ascii.chars.line_v import v_line
 from tablate.library.checkers.is_last_element import is_last_element
 from tablate.library.formatters.console.cell_string import cell_string_single_line
-from tablate.library.formatters.console.row_border import row_border
-from tablate.type.type_frame import BaseFrameDict
-from tablate.type.type_options import Options
+from tablate.library.formatters.console.row_outer_border import row_outer_border
+from tablate.type.type_store import FrameStoreUnion
+from tablate.type.type_global import Options
 
 
-def column_console_multiline(formatted_columns_array: List[List[str]], frame_dict: BaseFrameDict, options: Options):
-
-    frame_padding = options["common"]["frame_padding"]
-    frame_border = options["common"]["border_style"]
-
+def column_console_multiline(formatted_columns_array: List[List[str]], frame_dict: FrameStoreUnion, options: Options):
     line_count = 0
 
     for column_item in formatted_columns_array:
         line_count = len(column_item) if len(column_item) > line_count else line_count
 
-    line_count = line_count if frame_dict["max_lines"] is None or frame_dict["max_lines"] > line_count else frame_dict["max_lines"]
+    line_count = line_count if frame_dict.frame_styles.max_lines is None \
+                               or frame_dict.frame_styles.max_lines > line_count else frame_dict.frame_styles.max_lines
 
     return_string = ""
 
     for grid_line_index in range(line_count):
         grid_line_string = ""
-        for column_index, column_item in enumerate(frame_dict["column_list"]):
+        for column_index, column_item in enumerate(frame_dict.column_list):
             if grid_line_index < len(formatted_columns_array[column_index]):
                 grid_line_string += formatted_columns_array[column_index][grid_line_index]
             else:
-                grid_line_string += cell_string_single_line(string="",
-                                                           width=column_item["width"],
-                                                           padding=column_item["padding"],
-                                                           align=column_item["align"],
-                                                           trunc_value=column_item["trunc_value"])
-            if not is_last_element(column_index, frame_dict["column_list"]):
+                grid_line_string += cell_string_single_line(string=column_item["string"],
+                                                            column_item=column_item,
+                                                            trunc_value=frame_dict.frame_styles.trunc_value)
+            if not is_last_element(column_index, frame_dict.column_list):
                 grid_line_string += v_line[column_item["divider"]]
-        grid_line_inner = row_border(row_string=grid_line_string, outer_border=frame_border)
-        return_string += f"{' ' * frame_padding}{grid_line_inner}\n"
+        return_string += row_outer_border(row_string=grid_line_string, options=options)
+
     return return_string
```

### Comparing `tablate-0.0.7/tablate/library/renderers/console/frames/render_console_frame_grid.py` & `tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,37 @@
 
-from tablate.library.chars.line_v import v_line
+from tablate.library.ascii.chars.line_v import v_line
 from tablate.library.checkers.is_last_element import is_last_element
 from tablate.library.formatters.console.cell_string import cell_string_single_line, cell_string_multi_line
 from tablate.library.renderers.console.frames.render_console_columns import column_console_multiline
-from tablate.library.formatters.console.row_border import row_border
-from tablate.type.type_frame import GridFrameDict
-from tablate.type.type_options import Options
+from tablate.library.formatters.console.row_outer_border import row_outer_border
+from tablate.type.type_store import GridFrameStore
+from tablate.type.type_global import Options
 
 
-def render_console_single_line_grid(grid_frame_dict: GridFrameDict, options: Options):
-
-    frame_padding = options["common"]["frame_padding"]
-    frame_border = options["common"]["border_style"]
+def render_console_single_line_grid(grid_frame_dict: GridFrameStore, options: Options):
 
     grid_line_string = ""
-    for column_index, column_item in enumerate(grid_frame_dict["column_list"]):
+    for column_index, column_item in enumerate(grid_frame_dict.column_list):
         grid_line_string += cell_string_single_line(string=column_item["string"],
-                                                    width=column_item["width"],
-                                                    padding=column_item["padding"],
-                                                    align=column_item["align"],
-                                                    trunc_value=column_item["trunc_value"])
-        if not is_last_element(column_index, grid_frame_dict["column_list"]):
+                                                    column_item=column_item,
+                                                    trunc_value=grid_frame_dict.frame_styles.trunc_value)
+        if not is_last_element(column_index, grid_frame_dict.column_list):
             grid_line_string += v_line[column_item["divider"]]
 
-    grid_line_inner = row_border(row_string=grid_line_string, outer_border=frame_border)
-    return_string = f"{' ' * frame_padding}{grid_line_inner}\n"
-    return return_string
+    return row_outer_border(row_string=grid_line_string, options=options)
+
 
-def render_console_multi_line_grid(grid_frame_dict: GridFrameDict, options: Options):
+def render_console_multi_line_grid(grid_frame_dict: GridFrameStore, options: Options):
 
     formatted_columns_array = []
 
-    for column_item in grid_frame_dict["column_list"]:
+    for column_item in grid_frame_dict.column_list:
         column_string_array = cell_string_multi_line(string=column_item["string"],
-                                                     width=column_item["width"],
-                                                     padding=column_item["padding"],
-                                                     align=column_item["align"],
-                                                     trunc_value=column_item["trunc_value"],
-                                                     max_lines=grid_frame_dict["max_lines"])
+                                                     column_item=column_item,
+                                                     trunc_value=grid_frame_dict.frame_styles.trunc_value,
+                                                     max_lines=grid_frame_dict.frame_styles.max_lines)
         formatted_columns_array.append(column_string_array)
 
     return column_console_multiline(formatted_columns_array=formatted_columns_array,
                                     frame_dict=grid_frame_dict,
                                     options=options)
```

### Comparing `tablate-0.0.7/tablate/library/renderers/console/frames/render_string_frame_table.py` & `tablate-0.0.8/tablate/library/renderers/console/frames/render_console_frame_table.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,65 @@
-from tablate.library.chars.line_v import v_line
+from copy import copy
+
+from tablate.library.ascii.chars.line_v import v_line
 from tablate.library.checkers.is_last_element import is_last_element
 from tablate.library.formatters.console.cell_string import cell_string_single_line, cell_string_multi_line
+from tablate.library.formatters.console.row_colors import row_colors
 from tablate.library.renderers.console.frames.render_console_columns import column_console_multiline
-from tablate.library.formatters.console.row_divider import row_divider
-from tablate.library.formatters.console.row_border import row_border
-from tablate.type.type_frame import TableRowsFrameDict
-from tablate.type.type_options import Options
-
+from tablate.library.formatters.console.row_line_divider import row_line_divider
+from tablate.library.formatters.console.row_outer_border import row_outer_border
+from tablate.type.type_store import TableBodyFrameStore
+from tablate.type.type_global import Options
 
-def render_console_table_frame(table_frame_dict: TableRowsFrameDict, options: Options) -> str:
 
-    frame_padding = options["common"]["frame_padding"]
-    frame_border = options["common"]["border_style"]
+def render_console_table_frame(table_frame_store: TableBodyFrameStore, options: Options) -> str:
 
     return_string = ""
     line_divider_string = None
 
-    if table_frame_dict["row_line_divider"] != "none":
-        line_divider_row_string = row_divider(divider=table_frame_dict["row_line_divider"],
-                                              column_list_top=table_frame_dict["column_list"],
-                                              column_list_bottom=table_frame_dict["column_list"])
-        line_divider_inner_string = row_border(row_string=line_divider_row_string, outer_border=frame_border, row_divider=table_frame_dict["row_line_divider"])
-        line_divider_string = f"{' ' * frame_padding}{line_divider_inner_string}\n"
+    if table_frame_store.row_styles.row_line_divider != "none":
+        line_divider_row_string = row_line_divider(divider=table_frame_store.row_styles.row_line_divider,
+                                                   column_list_top=table_frame_store.column_list,
+                                                   column_list_bottom=table_frame_store.column_list)
+        line_divider_string = row_outer_border(row_string=line_divider_row_string,
+                                               options=options,
+                                               row_divider=table_frame_store.row_styles.row_line_divider)
 
-    for row_index, row_item in enumerate(table_frame_dict["table_row_list"]):
-        if table_frame_dict["multiline"] is False or table_frame_dict["max_lines"] == 1:
+    for row_index, row_item in enumerate(table_frame_store.row_list):
+        if table_frame_store.frame_styles.multiline is False or table_frame_store.frame_styles.max_lines == 1:
             row_line_string = ""
-            for column_index, column_item in enumerate(table_frame_dict["column_list"]):
-                row_line_string += cell_string_single_line(string=row_item[column_item["key"]],
-                                                           width=column_item["width"],
-                                                           padding=column_item["padding"],
-                                                           align=column_item["align"],
-                                                           trunc_value=column_item["trunc_value"])
-                if not is_last_element(column_index, table_frame_dict["column_list"]):
+            for column_index, column_item in enumerate(table_frame_store.column_list):
+                row_column_item = row_colors(column_item=column_item,
+                                            row_index=row_index,
+                                            table_frame_store=table_frame_store)
+                row_line_string += cell_string_single_line(string=row_column_item[column_item["key"]],
+                                                           column_item=row_column_item,
+                                                           trunc_value=table_frame_store.frame_styles.trunc_value)
+                if not is_last_element(column_index, table_frame_store.column_list):
                     row_line_string += v_line[column_item["divider"]]
-            line_string_inner = row_border(row_string=row_line_string, outer_border=frame_border)
-            return_string += f"{' ' * frame_padding}{line_string_inner}\n"
+            return_string += row_outer_border(row_string=row_line_string, options=options)
         else:
             formatted_columns_array = []
 
-            for column_item in table_frame_dict["column_list"]:
-                column_string_array = cell_string_multi_line(string=row_item[column_item["key"]],
-                                                             width=column_item["width"],
-                                                             padding=column_item["padding"],
-                                                             align=column_item["align"],
-                                                             trunc_value=column_item["trunc_value"],
-                                                             max_lines=table_frame_dict["max_lines"])
+            for column_item in table_frame_store.column_list:
+                row_column_item = row_colors(column_item=column_item,
+                                                 row_index=row_index,
+                                                 table_frame_store=table_frame_store)
+
+
+
+                column_string_array = cell_string_multi_line(string=row_item[row_column_item["key"]],
+                                                             column_item=row_column_item,
+                                                             trunc_value=table_frame_store.frame_styles.trunc_value,
+                                                             max_lines=table_frame_store.frame_styles.max_lines)
                 formatted_columns_array.append(column_string_array)
 
             return_string += column_console_multiline(formatted_columns_array=formatted_columns_array,
-                                                      frame_dict=table_frame_dict,
+                                                      frame_dict=table_frame_store,
                                                       options=options)
 
-        if not is_last_element(row_index, table_frame_dict["table_row_list"]) and line_divider_string:
+        if not is_last_element(row_index, table_frame_store.row_list) and line_divider_string:
             return_string += line_divider_string
-    if table_frame_dict["row_line_divider"] == "blank":
+    if table_frame_store.row_styles.row_line_divider == "blank":
         return_string = f"{line_divider_string}{return_string}{line_divider_string}"
 
-    return return_string
+    return return_string
```

### Comparing `tablate-0.0.7/tablate/library/renderers/console/frames/render_string_frame_text.py` & `tablate-0.0.8/tablate/library/renderers/console/render_console_frames.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from tablate.library.formatters.console.cell_string import cell_string_multi_line, cell_string_single_line
-from tablate.library.formatters.console.row_border import row_border
-from tablate.type.type_frame import TextFrameDict
-from tablate.type.type_options import Options
-
-
-def render_console_text_frame(text_frame_dict: TextFrameDict, options: Options) -> str:
-
-    frame_padding = options["common"]["frame_padding"]
-    frame_border = options["common"]["border_style"]
-
-    line_strings_array = []
-
-    if text_frame_dict["multiline"] == False or text_frame_dict["max_lines"] == 1:
-        row_string_inner = cell_string_single_line(string=text_frame_dict["string"],
-                                                   width=text_frame_dict["column_list"][0]["width"],
-                                                   padding=text_frame_dict["padding"],
-                                                   align=text_frame_dict["align"],
-                                                   trunc_value=text_frame_dict["trunc_value"])
-        line_strings_array.append(row_border(row_string=row_string_inner, outer_border=frame_border))
-    else:
-        multiline_array = cell_string_multi_line(string=text_frame_dict["string"],
-                                                 width=text_frame_dict["column_list"][0]["width"],
-                                                 padding=text_frame_dict["padding"],
-                                                 align=text_frame_dict["align"],
-                                                 max_lines=text_frame_dict["max_lines"])
-        for multiline_item in multiline_array:
-            line_strings_array.append(row_border(row_string=multiline_item, outer_border=frame_border))
+from tablate.library.checkers.is_last_element import is_last_element
+from tablate.library.formatters.console.row_line_divider import row_line_divider
+from tablate.library.formatters.console.row_outer_border import row_outer_border
+from tablate.library.renderers.console.frames.render_console_frame_grid import render_console_single_line_grid, \
+    render_console_multi_line_grid
+from tablate.library.renderers.console.frames.render_console_frame_table import render_console_table_frame
+from tablate.type.type_store import FrameStoreList
+from tablate.type.type_global import Options
+
+
+def render_console_frames(frame_list: FrameStoreList, options: Options) -> str:
+
     return_string = ""
 
-    for line_string in line_strings_array:
-        return_string += f"{' ' * frame_padding}{line_string}\n"
+    for frame_index, frame_item in enumerate(frame_list):
 
+        if frame_item.type == "grid" or frame_item.type == "table_header":
+            if frame_item.frame_styles.multiline is False or frame_item.frame_styles.max_lines == 1:
+                return_string += render_console_single_line_grid(grid_frame_dict=frame_item, options=options)
+            else:
+                return_string += render_console_multi_line_grid(grid_frame_dict=frame_item, options=options)
+
+        if frame_item.type == "table_body":
+            return_string += render_console_table_frame(table_frame_store=frame_item, options=options)
+
+        if not is_last_element(frame_index, frame_list):
+            if frame_list[frame_index].frame_styles.frame_divider != 'none':
+                frame_divider_inner = row_line_divider(column_list_top=frame_list[frame_index].column_list,
+                                                       column_list_bottom=frame_list[frame_index + 1].column_list,
+                                                       divider=frame_list[frame_index].frame_styles.frame_divider)
+                return_string += row_outer_border(row_string=frame_divider_inner,
+                                                  options=options,
+                                                  row_divider=frame_item.frame_styles.frame_divider)
 
-    return return_string
+    return return_string
```

### Comparing `tablate-0.0.7/tablate/library/renderers/console/render_console.py` & `tablate-0.0.8/tablate/library/renderers/console/render_console.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from tablate.library.renderers.console.render_console_foot import render_console_foot
 from tablate.library.renderers.console.render_console_frames import render_console_frames
 from tablate.library.renderers.console.render_console_head import render_console_head
-from tablate.type.type_frame import FrameDictList
-from tablate.type.type_options import Options
+from tablate.type.type_store import FrameStoreList
+from tablate.type.type_global import Options
 
 
-def render_console(frame_list: FrameDictList, options: Options) -> str:
+def render_console(frame_list: FrameStoreList, options: Options) -> str:
     return_string = ""
     if len(frame_list) > 0:
         return_string += render_console_head(frame_list=frame_list, options=options)
         return_string += render_console_frames(frame_list=frame_list, options=options)
         return_string += render_console_foot(frame_list=frame_list, options=options)
     return return_string
```

### Comparing `tablate-0.0.7/tablate/library/renderers/console/render_console_foot.py` & `tablate-0.0.8/tablate/library/renderers/console/render_console_foot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from tablate.library.chars.corners import bottom_left, bottom_right
-from tablate.library.formatters.console.row_divider import row_divider
-from tablate.type.type_frame import FrameDictList
-from tablate.type.type_options import Options
+from tablate.library.ascii.chars.corners import bottom_left, bottom_right
+from tablate.library.formatters.console.row_line_divider import row_line_divider
+from tablate.type.type_store import FrameStoreList
+from tablate.type.type_global import Options
 
 
-def render_console_foot(frame_list: FrameDictList, options: Options) -> str:
+def render_console_foot(frame_list: FrameStoreList, options: Options) -> str:
 
     return_string = ""
 
-    frame_padding = options["common"]["frame_padding"]
-    frame_border = options["common"]["border_style"]
+    outer_padding = options.console.outer_styles.outer_padding
+    frame_border = options.console.outer_styles.outer_border
 
-    bottom_border_inner = row_divider(column_list_top=frame_list[-1]["column_list"],
-                                      column_list_bottom=[],
-                                      divider=frame_border)
-    return_string += f"{' ' * frame_padding}{bottom_left[frame_border]}{bottom_border_inner}{bottom_right[frame_border]}\n"
+    bottom_border_inner = row_line_divider(column_list_top=frame_list[-1].column_list,
+                                           column_list_bottom=[],
+                                           divider=frame_border)
+    return_string += f"{' ' * outer_padding}{bottom_left[frame_border]}{bottom_border_inner}{bottom_right[frame_border]}\n"
 
     return return_string
```

### Comparing `tablate-0.0.7/tablate/library/renderers/html/frames/render_html_columns.py` & `tablate-0.0.8/tablate/library/renderers/html/frames/render_html_columns.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,58 @@
-from tablate.classes.options.html.style.subclasses.ElementStyle import ElementStyle
+from tablate.classes.options.html.style.subclasses.ElementStyler import ElementStyler
 from tablate.library.calcs.get_row_colspan import get_row_colspans
 from tablate.library.formatters.html.element.column import html_column_head_formatter, html_column_foot_formatter
 from tablate.library.formatters.html.element.frame import html_frame_head_formatter, html_frame_foot_formatter
 from tablate.library.formatters.html.element.row import html_row_head_formatter, html_row_foot_formatter
 from tablate.library.formatters.html.element.text import html_text_formatter
-from tablate.library.formatters.html.style.elements.column_style import column_style
-from tablate.library.formatters.html.style.elements.frame_style import frame_style
-from tablate.library.formatters.html.style.elements.text_style import text_style
-from tablate.type.type_frame import BaseFrameDict
-from tablate.type.type_html import HtmlFrameType, HtmlRowGroupElement, HtmlCellElement
-from tablate.type.type_options import Options
+from tablate.library.formatters.html.style.elements.style_column import style_column_dict
+from tablate.library.formatters.html.style.elements.style_frame import style_frame
+from tablate.type.primitives import HtmlRowGroupElement, HtmlCellElement, HtmlFrameType
+from tablate.type.type_store import BaseFrameStore, FrameStoreUnion
+from tablate.type.type_global import Options
 
 
-def render_html_column(frame_dict: BaseFrameDict, options: Options, frame_styler: ElementStyle, frame_type: HtmlFrameType = "body") -> str:
+def render_html_column(frame_dict: FrameStoreUnion, options: Options, frame_styler: ElementStyler, frame_type: HtmlFrameType = "body") -> str:
 
     frame_element: HtmlRowGroupElement
     column_element: HtmlCellElement
 
     if frame_type == "head":
-        frame_element = "thead"
+        frame_element = "tbody"
         column_element = 'th'
     else:
         frame_element = "tbody"
         column_element = 'td'
 
+    column_baselines = options.html.column_baselines
+    html_px = options.html.html_outer_styles.html_px_multiplier
 
-    column_baselines = options["html"]["column_baselines"]
-    html_px = options["html"]["px_size"]
-
-    colspans = get_row_colspans(frame_dict["column_list"], column_baselines)
+    colspans = get_row_colspans(frame_dict.column_list, column_baselines)
 
-    frame_style(frame_dict=frame_dict, frame_styler=frame_styler)
+    style_frame(frame_store=frame_dict, frame_styler=frame_styler)
 
     return_html = html_frame_head_formatter(frame_styler=frame_styler, frame_element=frame_element)
 
-    return_html += html_row_head_formatter()
+    return_html += html_row_head_formatter(frame_styler.row(0))
 
-    for column_index, column_item in enumerate(frame_dict["column_list"]):
+    for column_index, column_item in enumerate(frame_dict.column_list):
 
         column_styler = frame_styler.column(column_index)
 
-        column_style(frame_dict=frame_dict,
-                     column_dict=column_item,
-                     column_styler=column_styler,
-                     column_index=column_index)
+        style_column_dict(column_dict=column_item,
+                          column_styler=column_styler,
+                          html_px_multiplier=frame_dict.html_frame_styles.html_px_multiplier)
 
         return_html += html_column_head_formatter(column_styler=column_styler,
                                                   column_index=column_index,
                                                   colspans=colspans,
                                                   column_element=column_element)
 
         text_styler = column_styler.text
 
-        text_style(text_styler=text_styler,
-                   align=column_item["align"],
-                   padding=column_item["padding"] * html_px,
-                   multiline=frame_dict["multiline"],
-                   max_lines=frame_dict["max_lines"])
-
         return_html += html_text_formatter(text_styler=text_styler, string=column_item["string"])
 
         return_html += html_column_foot_formatter(column_element=column_element)
     return_html += html_row_foot_formatter()
     return_html += html_frame_foot_formatter(frame_element=frame_element)
 
     return return_html
```

### Comparing `tablate-0.0.7/tablate/library/renderers/html/frames/render_html_text.py` & `tablate-0.0.8/tablate/library/renderers/html/frames/render_html_table_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-from tablate.classes.options.html.style.subclasses.ElementStyle import ElementStyle
-from tablate.library.calcs.get_row_colspan import get_row_colspans
+from tablate.classes.options.html.style.subclasses.ElementStyler import ElementStyler
 from tablate.library.formatters.html.element.column import html_column_head_formatter, html_column_foot_formatter
 from tablate.library.formatters.html.element.frame import html_frame_head_formatter, html_frame_foot_formatter
 from tablate.library.formatters.html.element.row import html_row_head_formatter, html_row_foot_formatter
 from tablate.library.formatters.html.element.text import html_text_formatter
-from tablate.library.formatters.html.style.elements.column_style import column_style
-from tablate.library.formatters.html.style.elements.frame_style import frame_style
-from tablate.library.formatters.html.style.elements.text_style import text_style
-from tablate.type.type_frame import TextFrameDict
-from tablate.type.type_options import Options
+from tablate.library.formatters.html.style.elements.style_column import style_column_dict
+from tablate.library.formatters.html.style.elements.style_frame import style_frame
+from tablate.library.formatters.html.style.elements.style_rows import style_row
+from tablate.type.type_global import Options
+
+from tablate.library.calcs.get_row_colspan import get_row_colspans
+from tablate.type.type_store import TableBodyFrameStore
 
 
-def render_html_text(text_frame_dict: TextFrameDict, options: Options, frame_styler: ElementStyle):
+def render_html_table_body(table_body_frame_store: TableBodyFrameStore, options: Options, frame_styler: ElementStyler):
 
-    column_baselines = options["html"]["column_baselines"]
-    html_px = options["html"]["px_size"]
 
-    colspans = get_row_colspans(text_frame_dict["column_list"], column_baselines)
+    column_baselines = options.html.column_baselines
+    html_px = options.html.html_outer_styles.html_px_multiplier
 
-    frame_style(frame_dict=text_frame_dict, frame_styler=frame_styler)
+    colspans = get_row_colspans(table_body_frame_store.column_list, column_baselines)
+
+    style_frame(frame_store=table_body_frame_store, frame_styler=frame_styler)
+    style_row(row_store=table_body_frame_store.html_row_styles, row_styler=frame_styler.row())
 
     return_html = html_frame_head_formatter(frame_styler=frame_styler)
 
-    return_html += html_row_head_formatter()
+    for column_index, column_item in enumerate(table_body_frame_store.column_list):
+        style_column_dict(column_dict=column_item, column_styler=frame_styler.column(column_index=column_index), html_px_multiplier=table_body_frame_store.html_frame_styles.html_px_multiplier)
+
+    for row_index, row_item in enumerate(table_body_frame_store.row_list):
 
-    for column_index, column_item in enumerate(text_frame_dict["column_list"]):
+        row_styler = frame_styler.row(row_index)
 
-        column_styler = frame_styler.column(column_index)
+        return_html += html_row_head_formatter(row_styler=row_styler)
 
-        column_style(frame_dict=text_frame_dict,
-                     column_dict=column_item,
-                     column_styler=column_styler,
-                     column_index=column_index)
+        for row_column_index, row_column_item in enumerate(table_body_frame_store.column_list):
 
-        return_html += html_column_head_formatter(column_styler=column_styler,
-                                                  column_index=column_index,
-                                                  colspans=colspans)
+            column_styler = row_styler.column(row_column_index)
 
-        text_styler = column_styler.text
+            return_html += html_column_head_formatter(column_styler=column_styler,
+                                                      column_index=row_column_index,
+                                                      colspans=colspans)
 
-        text_style(text_styler=text_styler,
-                   align=text_frame_dict["align"],
-                   padding=text_frame_dict["padding"] * html_px,
-                   multiline=text_frame_dict["multiline"],
-                   max_lines=text_frame_dict["max_lines"])
+            text_styler = column_styler.text
 
-        return_html += html_text_formatter(text_styler=text_styler, string=text_frame_dict["string"])
+            return_html += html_text_formatter(text_styler=text_styler,
+                                               string=row_item[row_column_item["key"]])
 
-        return_html += html_column_foot_formatter()
-    return_html += html_row_foot_formatter()
+            return_html += html_column_foot_formatter()
+
+        return_html += html_row_foot_formatter()
     return_html += html_frame_foot_formatter()
 
     return return_html
+
+
+
```

### Comparing `tablate-0.0.7/tablate/library/renderers/html/render_html.py` & `tablate-0.0.8/tablate/library/renderers/html/render_html.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from tablate.classes.options.html.style.StyleCss import StyleCss
+from tablate.classes.options.html.style.CssStyler import CssStyler
 from tablate.library.calcs.calc_column_percent import calc_column_percent
 from tablate.library.renderers.html.render_html_foot import render_html_foot
 from tablate.library.renderers.html.render_html_frames import render_html_frames
 from tablate.library.renderers.html.render_html_head import render_html_head
-from tablate.type.type_frame import FrameDictList
-from tablate.type.type_options import Options
+from tablate.type.type_store import FrameStoreList
+from tablate.type.type_global import Options
 
 
-def render_html(frame_list: FrameDictList, options: Options) -> str:
+def render_html(frame_list: FrameStoreList, options: Options) -> str:
 
-    options["html"]["style"] = StyleCss()
+    options.html.styler = CssStyler()
 
-    options["html"]["style"].inject_css_block(options["html"]["css"])
+    options.html.styler.inject_css_block(options.html.css_injection)
 
     return_html = ""
 
     if len(frame_list) > 0:
         frame_list, column_baselines = calc_column_percent(frame_list=frame_list,
-                                                           frame_width=options["common"]["frame_width"])
-        options["html"]["column_baselines"] = column_baselines
+                                                           outer_width=options.console.outer_styles.outer_width)
+        options.html.column_baselines = column_baselines
         return_html += render_html_head(options=options)
         return_html += render_html_frames(frame_list=frame_list, options=options)
         return_html += render_html_foot()
 
-    css_head = options['html']['style'].return_head_styles()
-    css_foot = options['html']['style'].return_foot_styles()
+    css_head = options.html.styler.return_head_styles()
+    css_foot = options.html.styler.return_foot_styles()
 
     return_html = f"{css_head}{return_html}{css_foot}"
 
     return return_html
```

### Comparing `tablate-0.0.7/tablate/library/renderers/html/render_html_frames.py` & `tablate-0.0.8/tablate/library/renderers/html/render_html_frames.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from tablate.library.renderers.html.frames.render_html_columns import render_html_column
 from tablate.library.renderers.html.frames.render_html_table_body import render_html_table_body
-from tablate.library.renderers.html.frames.render_html_text import render_html_text
-from tablate.type.type_frame import FrameDictList
-from tablate.type.type_options import Options
+from tablate.type.type_store import FrameStoreList
+from tablate.type.type_global import Options
 
 
-def render_html_frames(frame_list: FrameDictList, options: Options) -> str:
+def render_html_frames(frame_list: FrameStoreList, options: Options) -> str:
 
     return_html = ''
 
     for frame_index, frame_item in enumerate(frame_list):
-        frame_styler = options["html"]["style"].frame(frame_index)
-        if frame_item["type"] == "text":
-            return_html += render_html_text(text_frame_dict=frame_item,
-                                            options=options,
-                                            frame_styler=frame_styler)
-        if frame_item["type"] == "grid":
+        frame_item.html_frame_styles.html_px_multiplier = frame_item.html_frame_styles.html_px_multiplier * options.html.html_outer_styles.html_px_multiplier
+        frame_styler = options.html.styler.frame(frame_index)
+        if frame_item.type == "grid":
             return_html += render_html_column(frame_dict=frame_item,
                                               options=options,
                                               frame_styler=frame_styler)
-        if frame_item["type"] == "table-head":
+        if frame_item.type == "table_header":
             return_html += render_html_column(frame_dict=frame_item,
                                               options=options,
                                               frame_styler=frame_styler,
                                               frame_type="head")
-        if frame_item["type"] == "table-body":
-            return_html += render_html_table_body(table_body_frame_dict=frame_item,
+        if frame_item.type == "table_body":
+            return_html += render_html_table_body(table_body_frame_store=frame_item,
                                                   options=options,
                                                   frame_styler=frame_styler)
 
     return return_html
```

### Comparing `tablate-0.0.7/tablate/library/renderers/html/render_html_head.py` & `tablate-0.0.8/tablate/library/renderers/html/render_html_head.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from tablate.library.formatters.html.style.border_style import border_line
-from tablate.type.type_options import Options
+from tablate.library.formatters.html.style.attributes.divider import divider_attr
+from tablate.type.type_global import Options
 
 
 def render_html_head(options: Options) -> str:
 
-    frame_padding = options["common"]["frame_padding"]
-    frame_border = options["common"]["border_style"]
-    html_width = options["html"]["width"]
-    html_px = options["html"]["px_size"]
-    column_baselines = options["html"]["column_baselines"]
+    outer_padding = options.html.html_outer_styles.html_outer_padding
+    frame_border_style = options.html.html_outer_styles.html_outer_border_style
+    frame_border_weight = options.html.html_outer_styles.html_outer_border_weight
 
-    margin_left_px = frame_padding * html_px
+    html_width = options.html.html_outer_styles.html_outer_width
+    column_baselines = options.html.column_baselines
+
+    margin_left_px = outer_padding
     margin_string = f'0 {margin_left_px}px'
 
-    border_string = border_line(frame_border)
+    border_string = divider_attr(divider_style=frame_border_style, divider_weight=frame_border_weight)
+
+    options.html.styler.add_global_style_attribute("font-family", "'Roboto', sans-serif")
+    options.html.styler.add_global_style_attribute("box-sizing", "border-box")
+    options.html.styler.add_global_style_attribute("margin", 0)
+    options.html.styler.add_global_style_attribute("padding", 0)
 
-    options["html"]["style"].add_global_style_attribute("box-sizing", "border-box")
-    options["html"]["style"].add_global_style_attribute("margin", 0)
-    options["html"]["style"].add_global_style_attribute("padding", 0)
+    options.html.styler.wrapper.add_style_attribute("width", f"calc({html_width} - {margin_left_px * 2}px)")
+    options.html.styler.wrapper.add_style_attribute("margin", margin_string)
 
-    options["html"]["style"].wrapper.add_style_attribute("width", f"calc({html_width} - {margin_left_px * 2}px)")
-    options["html"]["style"].wrapper.add_style_attribute("margin", margin_string)
+    options.html.styler.table.add_style_attribute("width", "100%")
+    options.html.styler.table.add_style_attribute("border", border_string)
 
-    options["html"]["style"].table.add_style_attribute("width", "100%")
-    options["html"]["style"].table.add_style_attribute("border", border_string)
+    options.html.styler.table.add_style_attribute("border-collapse", "collapse")
 
-    wrapper_classes = options["html"]["style"].wrapper.generate_class_names()
-    table_classes = options["html"]["style"].table.generate_class_names()
+    wrapper_classes = options.html.styler.wrapper.generate_class_names()
+    table_classes = options.html.styler.table.generate_class_names()
 
     return_string = ''
 
     return_string += f'<div class="{wrapper_classes}">'
     return_string += f'<table class="{table_classes}">'
 
     return_string += f'<colgroup>'
```

### Comparing `tablate-0.0.7/tablate/tests/test_defs.py` & `tablate-0.0.8/tablate/tests/old/test_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tablate as tf
 from tablate.tests.test_objs import column_list1, row_list1, column_list2a, row_list2, column_list2b, column_list2c, \
     column_list3, column_list4, column_list5, really_long_string
 
-# new_frame = tf.Tablate(border_style="thin", frame_padding=6)
+# new_frame = tf.Tablate(outer_border="thin", outer_padding=6)
 new_frame = tf.Tablate()
 
 
 new_frame.add_table_frame(column_list1, row_list1)
 
 new_frame.add_table_frame(column_list1, row_list1, multiline=True)
 new_frame.add_table_frame(column_list1, row_list1, multiline=True, max_lines=3)
@@ -43,23 +43,23 @@
 
 
 
 new_frame.add_text_frame(really_long_string)
 
 new_frame.add_table_frame(column_list2a, row_list2, row_column_divider="blank", row_line_divider="none")
 
-new_frame.add_table_frame(column_list2b, row_list2, row_column_divider="double", row_line_divider="double", frame_base_divider="blank")
+new_frame.add_table_frame(column_list2b, row_list2, row_column_divider="double", row_line_divider="double", frame_divider="blank")
 
-new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="blank", row_line_divider="blank", header_base_divider="thin", header_column_divider="double", frame_base_divider="thin")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="blank", row_line_divider="blank", header_frame_divider="thin", header_column_divider="double", frame_divider="thin")
 
-new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="blank", row_line_divider="none", header_base_divider="none", header_column_divider="double", frame_base_divider="double")
-new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thin", row_line_divider="thin", header_base_divider="thin", header_column_divider="double", frame_base_divider="thick")
-new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thick", row_line_divider="thick", header_base_divider="thick", header_column_divider="double", frame_base_divider="thin")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="blank", row_line_divider="none", header_frame_divider="none", header_column_divider="double", frame_divider="double")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thin", row_line_divider="thin", header_frame_divider="thin", header_column_divider="double", frame_divider="thick")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="thick", row_line_divider="thick", header_frame_divider="thick", header_column_divider="double", frame_divider="thin")
 
-new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="double", row_line_divider="double", header_base_divider="double", header_column_divider="double", frame_base_divider="none")
+new_frame.add_table_frame(column_list2c, row_list2, row_column_divider="double", row_line_divider="double", header_frame_divider="double", header_column_divider="double", frame_divider="none")
 new_frame.add_table_frame(column_list2c, row_list2)
 
 new_frame.add_grid_frame(column_list3, max_lines=1)
 new_frame.add_grid_frame(column_list4, max_lines=6)
 new_frame.add_grid_frame(column_list4, max_lines=100)
 new_frame.add_grid_frame(column_list5)
```

### Comparing `tablate-0.0.7/tablate/tests/test_objs.py` & `tablate-0.0.8/tablate/tests/old/test_objs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,52 +39,52 @@
     {
         "key": "Key One",
         "width": "50%",
         "divider": "thick"
     },
     {
         "key": "Key Two",
-        "align": "right"
+        "text_align": "right"
     },
     {
         "key": "Key Three",
-        "align": "right"
+        "text_align": "right"
     }
 ]
 
 column_list2b = [
     {
         "key": "Key One",
         "width": "20%",
 
     },
     {
         "key": "Key Two",
-        "align": "right"
+        "text_align": "right"
     },
     {
         "key": "Key Three",
-        "align": "right"
+        "text_align": "right"
     }
 ]
 
 column_list2c = [
     {
         "key": "Key One",
         "width": "30%",
         "divider": "thick"
     },
     {
         "key": "Key Two",
-        "align": "right",
+        "text_align": "right",
         "divider": "thin"
     },
     {
         "key": "Key Three",
-        "align": "right"
+        "text_align": "right"
     }
 ]
 
 row_list2 = [
     {
         "Key One": "Some string value",
         "Key Two": 4,
```

### Comparing `tablate-0.0.7/tablate/tests/test_styles.py` & `tablate-0.0.8/tablate/tests/old/test_styles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from tablate.classes.options.html.style.StyleCss import StyleCss
+from tablate.classes.options.html.style.CssStyler import CssStyler
 
-test_style = StyleCss()
+test_style = CssStyler()
 
 test_style.add_global_style_attribute("box-sizing", "border-box")
 test_style.add_global_style_attribute("margin", 0)
 
 print(test_style.table.generate_class_names())
 print(test_style.wrapper.generate_class_names())
```

### Comparing `tablate-0.0.7/tablate/type/type_style.py` & `tablate-0.0.8/tablate/classes/options/html/style/utilities/style_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from typing import TypedDict, NotRequired, Literal, Union
+from typing import TypedDict, NotRequired, Literal, Union, Optional
 
 TablateInstanceKey = Literal["tablate_instance"]
 ElementTypeKey = Literal["element_type"]
 
 BaseSelectorDictKeys = Literal[TablateInstanceKey, ElementTypeKey]
 TableSelectorDictKeys = Literal[BaseSelectorDictKeys, "tablate_container"]
 ElementSelectorDictKeys = Literal[BaseSelectorDictKeys, "tablate_frame", "tablate_column", "tablate_row", "tablate_text"]
 
 SelectorDictKeysUnion = Union[TableSelectorDictKeys, ElementSelectorDictKeys]
 
-# NOTE: Ensure the values of these two types match!!! (this is a hack until Python allows a KeysOf[TypedDict] type...)
+# NOTE: ( ▲ | ▼ ) Ensure the values of these two types match!!! (until Python allows a KeysOf[TypedDict] type...)
+
+class StyleItem(TypedDict):
+    style: str
+    pseudo: Optional[str]
 
 
 class BaseSelectorDict(TypedDict):
     tablate_instance: str
     element_type: str
 
 
@@ -25,8 +29,7 @@
     tablate_frame: NotRequired[str]
     tablate_column: NotRequired[str]
     tablate_row: NotRequired[str]
     tablate_text: NotRequired[str]
 
 
 SelectorDictUnion = Union[TableSelectorDict, ElementSelectorDict]
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tablate-0.0.7/tablate.egg-info/PKG-INFO` & `tablate-0.0.8/tablate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.7
-Summary: A highly customizable and dynamic table renderer for IPython & CLI application.
+Version: 0.0.8
+Summary: A highly customizable and dynamic table renderer for IPython & CLI applications.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/tablate
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/tablate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

