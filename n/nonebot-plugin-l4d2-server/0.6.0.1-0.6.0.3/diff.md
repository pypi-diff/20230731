# Comparing `tmp/nonebot_plugin_l4d2_server-0.6.0.1.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.6.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.6.0.3.tar", last modified: Mon Jul 31 08:18:16 2023, max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.6.0.1.tar` & `nonebot_plugin_l4d2_server-0.6.0.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    35149 2023-07-22 11:39:30.920580 nonebot_plugin_l4d2_server-0.6.0.1/LICENSE
--rw-r--r--   0        0        0     5749 2023-07-22 11:39:30.920580 nonebot_plugin_l4d2_server-0.6.0.1/README.md
--rw-r--r--   0        0        0    18984 2023-07-22 11:39:30.924581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-07-22 11:39:30.924581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     7067 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html
--rw-r--r--   0        0        0     6135 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     9076 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1608 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     2971 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     2054 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      369 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3576 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      449 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3364 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1345 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     3275 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1868 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1831 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     3074 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4179 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4176 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0      665 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9413 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1084 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     4018 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1422 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7526 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     1297 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-22 11:39:30.928581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1294 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py
--rw-r--r--   0        0        0    12635 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     5233 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/utils.py
--rw-r--r--   0        0        0     1588 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1339 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1569 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4067 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1186 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9326 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     5975 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1631 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0     1017 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0     1219 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0      764 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     7291 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     9286 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    15415 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     3492 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py
--rw-r--r--   0        0        0     1648 2023-07-22 11:39:30.932581 nonebot_plugin_l4d2_server-0.6.0.1/pyproject.toml
--rw-r--r--   0        0        0     7614 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.6.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-31 08:17:59.133239 nonebot_plugin_l4d2_server-0.6.0.3/LICENSE
+-rw-r--r--   0        0        0     5749 2023-07-31 08:17:59.133239 nonebot_plugin_l4d2_server-0.6.0.3/README.md
+-rw-r--r--   0        0        0    19681 2023-07-31 08:17:59.137240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-07-31 08:17:59.137240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-07-31 08:17:59.137240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     7067 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html
+-rw-r--r--   0        0        0     6135 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     8647 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     2980 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1887 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      369 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3541 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      449 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3368 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1293 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     3056 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1868 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1976 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     3074 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     3990 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4248 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0      664 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     2801 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/images.py
+-rw-r--r--   0        0        0     1142 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      922 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     2203 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1399 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7543 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     1266 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1177 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/local_ip.py
+-rw-r--r--   0        0        0    12995 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     5273 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/utils.py
+-rw-r--r--   0        0        0     1403 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1321 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1583 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4029 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1186 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2181 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1465 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9074 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     5985 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1631 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0     1007 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0     1230 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0      781 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     7384 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     9778 2023-07-31 08:17:59.141240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    16217 2023-07-31 08:17:59.145240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     3339 2023-07-31 08:17:59.145240 nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py
+-rw-r--r--   0        0        0     2196 2023-07-31 08:18:16.869506 nonebot_plugin_l4d2_server-0.6.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6565 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.6.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/LICENSE` & `nonebot_plugin_l4d2_server-0.6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/README.md` & `nonebot_plugin_l4d2_server-0.6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,45 +10,87 @@
 * but WITHOUT ANY WARRANTY; without even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License
 * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-from nonebot import require
-
-require("nonebot_plugin_apscheduler")
-require("nonebot_plugin_htmlrender")
-require("nonebot_plugin_txt2img")
-import time
-from time import sleep
+from pathlib import Path
 from typing import List, Tuple, Union
 
 from nonebot import get_driver, require
+from nonebot.adapters.onebot.v11 import (
+    Bot,
+    GroupMessageEvent,
+    Message,
+    MessageEvent,
+    MessageSegment,
+    NoticeEvent,
+)
+from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import Arg, ArgPlainText, CommandArg, Keyword, RegexGroup
+from nonebot.plugin import PluginMetadata
 from nonebot.typing import T_State
 
 from .l4d2_anne.server import updata_anne_server
 from .l4d2_data import sq_L4D2
 from .l4d2_file import all_zip_to_one, updown_l4d2_vpk
-from .l4d2_file.input_json import *
+
+# from .l4d2_file.input_json import *
 from .l4d2_image.steam import url_to_byte, url_to_byte_name
 from .l4d2_image.vtfs import img_to_vtf
-from .l4d2_push import *
 from .l4d2_queries.qqgroup import add_ip, del_ip, get_number_url, show_ip
 from .l4d2_queries.utils import queries_server
-from .l4d2_utils.command import *
-from .l4d2_utils.config import *
+from .l4d2_utils.command import (
+    add_queries,
+    anne_bind,
+    anne_player,
+    check_path,
+    del_bind,
+    del_queries,
+    del_vpk,
+    find_vpk,
+    help_,
+    join_server,
+    queries_comm,
+    rcon_to_server,
+    rename_vpk,
+    search_api,
+    show_queries,
+    smx_file,
+    up,
+    up_workshop,
+    updata,
+    vtf_make,
+)
+from .l4d2_utils.config import config_manager, file_format, l4_config, vpk_path
 from .l4d2_utils.txt_to_img import mode_txt_to_img
-from .l4d2_utils.utils import *
-from .l4d2_web import web, webUI
+from .l4d2_utils.utils import (
+    at_to_usrid,
+    bind_steam,
+    command_server,
+    del_map,
+    get_message_at,
+    get_vpk,
+    mes_list,
+    name_exist,
+    rename_map,
+    search_anne,
+    split_maohao,
+    str_to_picstr,
+    upload_file,
+    workshop_msg,
+)
+from .l4d2_web import web, webUI  # noqa: F401
 
+require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_htmlrender")
+require("nonebot_plugin_txt2img")
 scheduler = require("nonebot_plugin_apscheduler").scheduler
-from nonebot.plugin import PluginMetadata
 
 driver = get_driver()
 
 __version__ = "0.6.0"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description="可用于管理求生之路查服和本地管理",
@@ -79,29 +121,28 @@
         await matcher.finish("你填写的路径不存在辣")
     if not Path(map_path).exists():
         await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
     url: str = args["file"]["url"]
     name: str = args["file"]["name"]
     # 如果不符合格式则忽略
     await up.send("已收到文件，开始下载")
-    sleep(1)  # 等待一秒防止因为文件名获取出现BUG
     vpk_files = await updown_l4d2_vpk(map_path, name, url)
     if vpk_files:
         mes = "解压成功，新增以下几个vpk文件"
         await matcher.finish(mes_list(mes, vpk_files))
     else:
         await matcher.finish("你可能上传了相同的文件，或者解压失败了捏")
 
 
 path_list: str = "请选择上传位置（输入阿拉伯数字)"
 times = 0
 for one_path in l4_config.l4_ipall:
     times += 1
     path_msg = one_path["location"]
-    path_list += f"\n {str(times)} | {path_msg}"
+    path_list += f"\n {times!s} | {path_msg}"
 
 
 @up.got("is_sure", prompt=path_list)
 async def _(matcher: Matcher):
     args = matcher.get_arg("txt")
     l4_file = l4_config.l4_ipall
     if not args:
@@ -129,30 +170,29 @@
     url = args["file"]["url"]
     name = args["file"]["name"]
     # 如果不符合格式则忽略
     if not name.endswith(file_format):  # type: ignore
         return
 
     await matcher.send("已收到文件，开始下载")
-    sleep(1)  # 等待一秒防止因为文件名获取出现BUG
     vpk_files = await updown_l4d2_vpk(map_path, name, url)  # type: ignore
 
     if vpk_files:
         logger.info("检查到新增文件")
         mes = "解压成功，新增以下几个vpk文件"
     elif vpk_files is None:
         await matcher.finish("文件错误")
     else:
         mes = "你可能上传了相同的文件，或者解压失败了捏"
 
     await matcher.finish(mes_list(mes, vpk_files))
 
 
 @find_vpk.handle()
-async def _(bot: Bot, event: MessageEvent, matcher: Matcher):
+async def _(matcher: Matcher):
     map_path = Path(l4_config.l4_ipall[l4_config.l4_number]["location"], vpk_path)
     name_vpk = get_vpk(map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
     msg = ""
     msg = mes_list(msg, name_vpk).replace(" ", "")
 
@@ -185,15 +225,15 @@
         rename = rename + ".vpk"
     logger.info("尝试改名")
     try:
         map_name = rename_map(num, rename, map_path)
         if map_name:
             await matcher.finish("改名成功\n原名:" + map_name + "\n新名称:" + rename)
     except ValueError:
-        await matcher.finish("参数错误,请输入格式如【求生地图 5 改名 map.vpk】,或者输入【求生地图】获取全部名称")
+        await matcher.finish("参数错误,输入【求生地图】获取全部名称")
 
 
 @anne_player.handle()
 async def _(matcher: Matcher, event: MessageEvent, args: Message = CommandArg()):
     name = args.extract_plain_text()
     name = name.strip()
     at = await get_message_at(event.json())
@@ -237,33 +277,35 @@
 
 @rcon_to_server.got("command", prompt="请输入向服务器发送的指令")
 async def _(matcher: Matcher, tag: str = ArgPlainText("command")):
     tag = tag.strip()
     msg = await command_server(tag)
     try:
         await matcher.finish(mode_txt_to_img("服务器返回", msg))
-    except:
-        await matcher.finish(msg, reply_message=True)
+    except Exception as E:
+        await matcher.finish(str(E), reply_message=True)
 
 
 @check_path.handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg.startswith("切换"):
         msg_number = int("".join(msg.replace("切换", " ").split()))
         if msg_number > len(l4_config.l4_ipall) or msg_number < 0:
             await matcher.send("没有这个序号的路径呐")
         else:
             l4_config.l4_number = msg_number - 1
             now_path = l4_config.l4_ipall[l4_config.l4_number]["location"]
-            await matcher.send(f"已经切换路径为\n{str(l4_config.l4_number+1)}、{now_path}")
+            await matcher.send(
+                f"已经切换路径为\n{l4_config.l4_number+1!s}、{now_path}",
+            )  # noqa: E501
             config_manager.save()
     else:
         now_path = l4_config.l4_ipall[l4_config.l4_number]["location"]
-        await matcher.send(f"当前的路径为\n{str(l4_config.l4_number+1)}、{now_path}")
+        await matcher.send(f"当前的路径为\n{l4_config.l4_number+1!s}、{now_path}")
 
 
 @queries_comm.handle()
 async def _(matcher: Matcher, event: MessageEvent, keyword: str = Keyword()):
     msg = event.get_plaintext()
 
     if not msg:
@@ -385,14 +427,17 @@
     else:
         await matcher.finish("已取消上传")
 
 
 @updata.handle()
 async def _(matcher: Matcher, args: Message = CommandArg()):
     """更新"""
+    if args:
+        # 占位先，除了电信服还有再加
+        ...
     anne_ip_dict = await updata_anne_server()
     if not anne_ip_dict:
         await matcher.finish("网络开小差了捏")
     server_number = len(anne_ip_dict["云"])
     await matcher.finish(f"更新成功\n一共更新了{server_number}个电信anne服ip")
 
 
@@ -437,15 +482,15 @@
     mes = "当前服务器下有以下smx文件"
     msg = ""
     msg = mes_list(msg, name_smx).replace(" ", "")
     await matcher.finish(mode_txt_to_img(mes, msg))
 
 
 # @search_api.handle()
-# async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
+# async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):  # noqa: E501
 #     msg:str = args.extract_plain_text()
 #     # if msg.startswith('代码'):
 #         # 建图代码返回三方图信息
 #     data = await seach_map(msg,l4_config.l4_master[0],l4_config.l4_key)
 #     # else:
 #     if type(data) == str:
 #         await matcher.finish(data)
@@ -454,15 +499,15 @@
 #         await matcher.send(await map_dict_to_str(data))
 @help_.handle()
 async def _(matcher: Matcher):
     msg = [
         "=====求生机器人帮助=====",
         "1、电信服战绩查询【求生anne[id/steamid/@]】",
         "2、电信服绑定【求生绑定[id/steamid]】",
-        "3、电信服状态查询【云xx】" "4、创意工坊下载【创意工坊下载[物品id/链接]】",
+        "3、电信服状态查询【云xx】4、创意工坊下载【创意工坊下载[物品id/链接]】",
         "5、指定ip查询【求生ip[ip]】(可以是域名)",
         "6、求生喷漆制作【求生喷漆】",
         "6、本地服务器操作(略，详情看项目地址)",
     ]
     messgae = ""
     for i in msg:
         messgae += i + "\n"
@@ -512,8 +557,8 @@
 #     await get_des_ip()
 #     await matcher.finish('已重载ip')
 
 
 @driver.on_shutdown
 async def close_db():
     """关闭数据库"""
-    sq_L4D2._close()
+    sq_L4D2._close()  # noqa: SLF001
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/group_ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,63 @@
 from typing import List
 
+import httpx
 import pandas as pd
+from bs4 import BeautifulSoup
 from nonebot.log import logger
 
 from ..l4d2_data.players import L4D2Player
 from ..l4d2_image import out_png
-from ..l4d2_utils.seach import *
+from ..l4d2_utils.seach import anne_search
 from .analysis import df_to_guoguanlv
 
 # from .anne_telecom import ANNE_API
 
 
 s = L4D2Player()
+headers = {
+    "User-Agent": (
+        "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) "
+        "Gecko/20100101 Firefox/107.0"
+    ),
+}
 
 
 async def anne_html(name: str):
     """搜索里提取玩家信息，返回列表字典"""
     data_title = anne_search(name)
     if not data_title:
-        return
+        return None
     data = data_title[0]
     title = data_title[1]
     if len(data) == 0 or data[0] == "No Player found.":
         return []
     data_list: list = []
     logger.info(data)
     for i in data:
         i: BeautifulSoup
-        try:
-            Rank = i.find("td", {"data-title": "Rank:"}).text.strip()  # type: ignore
-            player = i.find("td", {"data-title": "Player:"}).text.strip()  # type: ignore
-            points = i.find("td", {"data-title": "Points:"}).text.strip()  # type: ignore
-            # country = i.find('img')['alt']
-            playtime = i.find("td", {"data-title": "Playtime:"}).text.strip()  # type: ignore
-            last_online = i.find("td", {"data-title": "Last Online:"}).text.strip()  # type: ignore
-        except AttributeError:
-            Rank = i.find("td", {"data-title": "排名:"}).text.strip()  # type: ignore
-            player = i.find("td", {"data-title": "玩家:"}).text.strip()  # type: ignore
-            points = i.find("td", {"data-title": "分数:"}).text.strip()  # type: ignore
-            playtime = i.find("td", {"data-title": "游玩时间:"}).text.strip()  # type: ignore
-            last_online = i.find("td", {"data-title": "最后上线时间:"}).text.strip()  # type: ignore
+
+        def find_text(soup, attr_en, attr_alt):
+            try:
+                element = soup.find("td", {"data-title": attr_en})
+                if element is None:
+                    element = soup.find("td", {"data-title": attr_alt})
+                return element.text.strip() if element else ""
+            except AttributeError:
+                return ""
+
+        rank = find_text(i, "Rank:", "排名:")
+        player = find_text(i, "Player:", "玩家:")
+        points = find_text(i, "Points:", "分数:")
+        playtime = find_text(i, "Playtime:", "游玩时间:")
+        last_online = find_text(i, "Last Online:", "最后上线时间:")
         onclick = i["onclick"]
         steamid = onclick.split("=")[2].strip("'")  # type: ignore
         play_json = {
-            title[0]: Rank,
+            title[0]: rank,
             title[1]: player,
             title[2]: points,
             # title[3]:country,
             title[3]: playtime,
             title[4]: last_online,
             title[5]: steamid,
         }
@@ -71,67 +81,62 @@
             mes += "\n" + titles[i] + ":" + str(one[titles[i]])
         mes += "\n--------------------"
         if ns > 4:
             break
     return mes
 
 
-async def write_player(id, msg: str, nickname: str):
+async def write_player(id_, msg: str, nickname: str):
     """绑定用户"""
     # 判断是steam
     if msg.startswith("STEAM"):
         # try:
-        data_tuple = s._query_player_qq(id)
-        if data_tuple != None:
+        data_tuple = s.query_player_qq(id_)
+        if data_tuple is not None:
             qq, nicknam, steamid = data_tuple
         else:
             nicknam = None
-        await s._add_player_all(id, nicknam, msg)
+        await s.add_player_all(id_, nicknam, msg)
         # except TypeError:
-        # await s._add_player_steamid(id , msg)
-        mes = "绑定成功喵~\nQQ:" + nickname + "\n" + "steamid:" + msg
-        return mes
+        # await s._add_player_steamid(id_ , msg)
+        return "绑定成功喵~\nQQ:" + nickname + "\n" + "steamid:" + msg
+    # try:
+    data_tuple = s.query_player_qq(id_)
+    if data_tuple is not None:
+        id_, nicknam, steamid = data_tuple
     else:
-        # try:
-        data_tuple = s._query_player_qq(id)
-        if data_tuple != None:
-            id, nicknam, steamid = data_tuple
-        else:
-            steamid = None
-        await s._add_player_all(id, msg, steamid)
-        # except TypeError:
-        #     await s._add_player_nickname(id , msg )
-        mes = "绑定成功喵~\nQQ:" + nickname + "\n" + "steam昵称:" + msg
-        return mes
+        steamid = None
+    await s.add_player_all(id_, msg, steamid)
+    # except TypeError:
+    #     await s._add_player_nickname(id_ , msg )
+    return "绑定成功喵~\nQQ:" + nickname + "\n" + "steam昵称:" + msg
 
 
-def del_player(id: str):
+def del_player(id_: str):
     """删除绑定信息,返回消息"""
-    if not s._query_player_qq(id):
+    if not s.query_player_qq(id_):
         return "你还没有绑定过，请使用[求生绑定+昵称/steamid]"
-    if s._delete_player:
+    if s.delete_player:
         return "删除成功喵~"
+    return None
 
 
 async def id_to_mes(name: str):
     """根据name从数据库,返回steamid、或者空白"""
     data_tuple = await s.search_data(None, name, None)
     if data_tuple:
-        steamid = data_tuple[2]
-        return steamid
+        return data_tuple[2]
     return None
 
 
 def anne_rank_dict(name: str):
     """用steamid,查详情,输出字典"""
     data_dict = {}
     url = f"https://sb.trygek.com/l4d_stats/ranking/player.php?steamid={name}"
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
-    }
+
     data = httpx.get(url=url, headers=headers, timeout=5)
     if data.status_code != 200:
         return [f"查询错误，状态码{data.status_code}"]
     data = data.content.decode("utf-8")
     data = BeautifulSoup(data, "html.parser")
     detail = data.find_all("table")
     n = 0
@@ -148,15 +153,20 @@
         n += 1
     # 获取头像
     element: str = data.find_all(attrs={"style": "cursor:pointer"})[0].get("onclick")
     player_url = element.split("'")[1]
     data_list[0].update({"个人资料": player_url})
     # 获取一言
     message = data.select(
-        "html body div.content.text-center.text-md-left div.container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.justify-content-center.text-center span"
+        (
+            "html body div.content.text-center.text-md-left "
+            "div.container.text-left div.col-md-12.h-100 "
+            "div.card-body.worldmap.d-flex.flex-column.justify-content-center."
+            "text-center span"
+        ),
     )
     msg_list = []
     for i in message:
         msg_list.append(i.text)
     data_list[0].update({"一言": msg_list})
     return data_list
 
@@ -179,15 +189,15 @@
         logger.info("关键词查询" + name)
         if not name.startswith("STEAM"):
             steamid = await id_to_mes(name)
             if not steamid:
                 logger.info("没有找到qq，使用默认头像")
                 message = await anne_html(name)
                 if not message:
-                    return
+                    return None
                 usr_id = "1145149191810"
                 if len(message) == 0:
                     return "没有叫这个名字的...\n"
                 if len(message) > 1:
                     return anne_html_msg(message)
                 name = message[0]["steamid"]
             else:
@@ -196,66 +206,74 @@
         # steamid
         msg = anne_rank_dict(name)[0]
         if isinstance(msg, dict):
             msg.update(await df_to_guoguanlv(await anne_map_msg(name)))
             logger.info("使用图片")
             msg = await out_png(usr_id, msg)
         return msg
-    else:
-        """
-        1、qq>数据>没有数据，返回
-        2、qq>数据>steamid>查询
-        3、qq>数据>昵称>查询
-        """
-        logger.info("qq信息查询")
-        data_tuple = s._query_player_qq(usr_id)
-        logger.info(data_tuple)
-        if not data_tuple:
-            return f"没有绑定信息...请使用【求生绑定 xxx】\n"
-        # 只有名字，先查询数据在判断
-        elif data_tuple[2]:
-            name = data_tuple[2]
-        elif data_tuple[1]:
-            name = await id_to_mes(data_tuple[1])  # type: ignore
-            logger.info(name)
-            if not name:
-                message = await anne_html(data_tuple[1])
-                if not message:
-                    return
-                usr_id = "1145149191810"
-                if len(message) == 0:
-                    return "没有叫这个名字的...\n"
-                if len(message) > 1:
-                    return anne_html_msg(message)
-                name = message[0]["steamid"]
-
-        # name是steamid
-        msg = anne_rank_dict(name)[0]
-        if isinstance(msg, dict):
-            msg.update(await df_to_guoguanlv(await anne_map_msg(name)))
-            logger.info("使用图片")
-            msg = await out_png(usr_id, msg)
-        return msg
+    """
+    1、qq>数据>没有数据，返回
+    2、qq>数据>steamid>查询
+    3、qq>数据>昵称>查询
+    """
+    logger.info("qq信息查询")
+    data_tuple = s.query_player_qq(usr_id)
+    logger.info(data_tuple)
+    if not data_tuple:
+        return "没有绑定信息...请使用【求生绑定 xxx】\n"
+    # 只有名字，先查询数据在判断
+    if data_tuple[2]:
+        name = data_tuple[2]
+    elif data_tuple[1]:
+        name = await id_to_mes(data_tuple[1])  # type: ignore
+        logger.info(name)
+        if not name:
+            message = await anne_html(data_tuple[1])
+            if not message:
+                return None
+            usr_id = "1145149191810"
+            if len(message) == 0:
+                return "没有叫这个名字的...\n"
+            if len(message) > 1:
+                return anne_html_msg(message)
+            name = message[0]["steamid"]
+
+    # name是steamid
+    msg = anne_rank_dict(name)[0]
+    if isinstance(msg, dict):
+        msg.update(await df_to_guoguanlv(await anne_map_msg(name)))
+        logger.info("使用图片")
+        msg = await out_png(usr_id, msg)
+    return msg
 
 
 async def anne_map_msg(steamid: str):
     """steamid->地图信息"""
     url = f"https://sb.trygek.com/l4d_stats/ranking/timedmaps.php?steamid={steamid}"
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
-    }
-    data = httpx.get(url, headers=headers, timeout=5).content.decode("utf-8")
+
+    data = httpx.get(url, headers=headers, timeout=5).content.decode(  # noqa: ASYNC100
+        "utf-8",
+    )
     soup = BeautifulSoup(data, "html.parser")
     data_list = []
     cards = soup.select("div.card.rounded-0")
     for card in cards:
         tbodies = card.select("tbody")
         for tbody in tbodies:
             rows = [td.text.strip() for td in tbody.find_all("td")]
             for i in range(0, len(rows), 9):
                 row = rows[i : i + 9]
                 data_list.append(row)
-    df = pd.DataFrame(
+    return pd.DataFrame(
         data_list,
-        columns=["游戏模式", "地图", "难度", "完成时间", "特感数量", "刷新间隔", "B数使用", "刷特模式", "Anne版本"],
+        columns=[
+            "游戏模式",
+            "地图",
+            "难度",
+            "完成时间",
+            "特感数量",
+            "刷新间隔",
+            "B数使用",
+            "刷特模式",
+            "Anne版本",
+        ],
     )
-    return df
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     try:
         resen += other_map / (all_map + other_map)
         result = {"救援关": str("{:.2%}".format(resen))}
     except (TypeError, KeyError):
         result = {"救援关": "错误"}
     except ZeroDivisionError:
         result = {"救援关": "0.00%"}
-    except:
+    except Exception:
         result = {"救援关": "错误"}
     return result
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,22 @@
 #                 title = i.find('td', {'class': 'w-50'})
 #                 value = title.find_next_sibling('td')
 #                 new_dict = {title.text:value.text}
 #                 data_dict.update(new_dict)
 #             data_list.append(data_dict)
 #             n += 1
 #         # 获取头像
-#         element:str = data_fom.find_all(attrs={"style": "cursor:pointer"})[0].get("onclick")
+#         element:str = data_fom.find_all(attrs={"style": "cursor:pointer"})[0].
+# get("onclick")
 #         player_url = element.split("'")[1]
 #         data_list[0].update({"个人资料":player_url})
 #         # 获取一言
-#         message = data_fom.select("html body div.content.text-center.text-md-left div.container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.justify-content-center.text-center span")
+#         message = data_fom.select("html body div.content.text-center.text-md-left div.
+# container.text-left div.col-md-12.h-100 div.card-body.worldmap.d-flex.flex-column.
+# justify-content-center.text-center span")
 #         msg_list = []
 #         for i in message:
 #             msg_list.append(i.text)
 #         data_list[0].update({"一言":msg_list})
 #         return data_list
 
 #     async def anne_map(self):
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def _check_tables_exist(self) -> None:
         """
         检查表是否存在
         """
         c = self.conn.cursor()
         for table in table_data:
             c.execute(
-                f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table}'"
+                f"SELECT name FROM sqlite_master WHERE type='table' AND name='{table}'",
             )
             if c.fetchone() is None:
                 if table == "L4d2_players":
                     c.execute(f"CREATE TABLE {table} (qq INTEGER PRIMARY KEY)")
                 elif table == "L4D2_server":
                     c.execute(f"CREATE TABLE {table} (number INTEGER PRIMARY KEY)")
                 self.conn.commit()
@@ -53,56 +53,53 @@
         c = self.conn.cursor()
         for table, tag in tables_columns.items():
             for column in tag:
                 c.execute(f"PRAGMA table_info({table})")
                 if not any(col[1] == column for col in c.fetchall()):
                     if column in L4d2_BOOLEAN:
                         c.execute(
-                            f"ALTER TABLE {table} ADD COLUMN {column} BOOLEAN DEFAULT 0"
+                            f"ALTER TABLE {table} ADD COLUMN {column} BOOLEAN DEFAULT 0",
                         )
                     elif column in L4d2_INTEGER:
                         c.execute(
-                            f"ALTER TABLE {table} ADD COLUMN {column} INTEGER DEFAULT NULL"
+                            f"ALTER TABLE {table} ADD COLUMN {column} INTEGER DEFAULT NULL",
                         )
                     else:
                         c.execute(
-                            f"ALTER TABLE {table} ADD COLUMN {column} TEXT DEFAULT NULL"
+                            f"ALTER TABLE {table} ADD COLUMN {column} TEXT DEFAULT NULL",
                         )
         self.conn.commit()
 
     def _check_data_validity(self) -> None:
         """
         检查数据库数据的合法性
         错误数据默认填充NULL或者False
         """
         c = self.conn.cursor()
         columns = None
         table = None
         for table in table_data:
-            if table == "L4d2_players":
-                columns = L4d2_players_tag
-            else:
-                columns = L4d2_server_tag
+            columns = L4d2_players_tag if table == "L4d2_players" else L4d2_server_tag
         if not columns:
             return
         for column in columns:
             if column in L4d2_INTEGER:
                 c.execute(
-                    f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'integer'"
+                    f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'integer'",
                 )
             elif column in L4d2_TEXT:
                 c.execute(
-                    f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'text'"
+                    f"UPDATE {table} SET {column} = NULL WHERE typeof({column}) != 'text'",
                 )
             elif column in L4d2_BOOLEAN:
                 c.execute(
-                    f"UPDATE {table} SET {column} = 'False' WHERE typeof({column}) != 'boolean'"
+                    f"UPDATE {table} SET {column} = 'False' WHERE typeof({column}) != 'boolean'",
                 )
         self.conn.commit()
 
     def _close(self):
         """断开连接到数据库"""
         self.conn.close()
         logger.info("已断开求生数据库")
 
 
-sq_L4D2 = L4D2DataSqlite()
+sq_L4D2 = L4D2DataSqlite()  # noqa: N816
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,50 +29,52 @@
         """绑定steamid"""
         self.c.execute(
             "INSERT INTO L4d2_players (qq, nickname, steamid) VALUES (?,NULL,?)",
             (qq, steamid),
         )
         self.conn.commit()
 
-    async def _add_player_all(self, qq, nickname, steamid):
+    async def add_player_all(self, qq, nickname, steamid):
         """用新数据覆盖旧数据"""
         # try:
         self.c.execute(
-            "INSERT OR REPLACE INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,?)",
+            "INSERT OR REPLACE INTO L4d2_players (qq, nickname, steamid) VALUES (?,?,?)",  # noqa: E501
             (qq, nickname, steamid),
         )
         self.conn.commit()
         return True
         # except sqlite3.IntegrityError:
         #     return False
 
-    def _delete_player(self, qq):
+    def delete_player(self, qq):
         """解除绑定"""
         self.c.execute(f"DELETE FROM L4d2_players WHERE qq = {qq}")
         self.conn.commit()
         return True
 
-    def _query_player_qq(self, qq) -> Union[tuple, None]:
+    def query_player_qq(self, qq) -> Union[tuple, None]:
         """通过qq获取数据"""
         self.c.execute(f"SELECT * FROM L4d2_players WHERE qq = '{qq}'")
         return self.c.fetchone()
 
     async def _query_player_nickname(self, nickname: str) -> Union[tuple, None]:
         """通过nickname获取数据"""
         self.c.execute(f"SELECT * FROM L4d2_players WHERE nickname = '{nickname}'")
         return self.c.fetchone()
 
     async def _query_player_steamid(self, steamid: str):
         """通过steamid获取数据"""
         self.c.execute(f"SELECT * FROM L4d2_players WHERE steamid = '{steamid}'")
-        data_tuple = self.c.fetchone()
-        return data_tuple
+        return self.c.fetchone()
 
     async def search_data(
-        self, qq: Optional[str], nickname: Optional[str], steamid: Optional[str]
+        self,
+        qq: Optional[str],
+        nickname: Optional[str],
+        steamid: Optional[str],
     ) -> Union[tuple, None]:
         """
         输入元组查询，优先qq其次steamid最后nickname，不需要值可以为None
         输出为元组，如果为空输出None
         data = (qq , nickname , steamid )
         """
         if qq:
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,24 +19,22 @@
             (qqgroup, host, port),
         )
         self.conn.commit()
 
     async def query_server_ip(self, qqgroup):
         """输入群号，返回数据库里订阅ip元组列表"""
         self.c.execute(
-            f"SELECT  number, qqgroup ,host ,port FROM L4D2_server WHERE qqgroup = {qqgroup}"
+            f"SELECT  number, qqgroup ,host ,port FROM L4D2_server WHERE qqgroup = {qqgroup}",
         )
-        msg_list = self.c.fetchall()
-        return msg_list
+        return self.c.fetchall()
 
-    async def del_server_ip(self, id: int):
+    async def del_server_ip(self, id_: int):
         """删除指定id的ip"""
-        self.c.execute(f"DELETE FROM L4D2_server WHERE number = {id}")
+        self.c.execute(f"DELETE FROM L4D2_server WHERE number = {id_}")
         self.conn.commit()
 
     async def query_number(self, number: int):
         """通过序号找服务器"""
         self.c.execute(
-            f"SELECT qqgroup , host ,port FROM L4D2_server WHERE number = {number}"
+            f"SELECT qqgroup , host ,port FROM L4D2_server WHERE number = {number}",
         )
-        msg_list = self.c.fetchone()
-        return msg_list
+        return self.c.fetchone()
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,56 @@
 import io
-import os
-import sys
+import zipfile
 from pathlib import Path
-from time import sleep
-from typing import Callable, List
+from typing import Callable, Dict, List
 from zipfile import ZipFile
 
 import rarfile
 from nonebot.log import logger
 from pyunpack import Archive
-from rarfile import RarFile
 
 from ..l4d2_utils.config import systems
 from ..l4d2_utils.utils import get_file, get_vpk
 
 
 async def updown_l4d2_vpk(map_paths: Path, name: str, url: str):
     """从url下载压缩包并解压到位置"""
     original_vpk_files = get_vpk(map_paths)
     down_file = Path(map_paths, name)
-    if await get_file(url, down_file) == None:
+    if await get_file(url, down_file) is None:
         return None
-    sleep(1)
     msg = open_packet(name, down_file)
     logger.info(msg)
 
-    sleep(1)
     extracted_vpk_files = get_vpk(map_paths)
     # 获取新增vpk文件的list
-    vpk_files = list(set(extracted_vpk_files) - set(original_vpk_files))
-    return vpk_files
-
+    return list(set(extracted_vpk_files) - set(original_vpk_files))
 
-import zipfile
-from pathlib import Path
-from typing import Dict
-
-import rarfile
-from pyunpack import Archive
 
 SUPPORTED_EXTENSIONS = (".zip", ".7z", ".rar")
 
 
 def unzip_zipfile(down_file: Path, down_path: Path):
     """解压zip文件"""
     with support_gbk(zipfile.ZipFile(down_file, "r")) as z:
         z.extractall(down_path)
-    os.remove(down_file)
+    down_file.unlink()
 
 
 def unpack_7zfile(down_file: Path, down_path: Path):
     """解压7z文件"""
     Archive(str(down_file)).extractall(str(down_path))
-    os.remove(down_file)
+    down_file.unlink()
 
 
 def unpack_rarfile(down_file: Path, down_path: Path):
     """解压rar文件"""
     with rarfile.RarFile(down_file, "r") as z:
         z.extractall(down_path)
-    os.remove(down_file)
+    down_file.unlink()
 
 
 def open_packet(name: str, down_file: Path) -> str:
     """解压压缩包"""
     down_path = down_file.parent
     logger.info("文件名为：" + name)
     logger.info(f"系统为{systems}")
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import json
 from pathlib import Path
 
-import httpx
+import aiofiles
 from nonebot import on_notice
 from nonebot.adapters.onebot.v11 import NoticeEvent
 
+from ..l4d2_image.steam import url_to_msg
+
 upload = on_notice(priority=1)
 
 
 @upload.handle()
 async def _(event: NoticeEvent):
     try:
         arg = event.dict()
         files: dict = arg["file"]
         name: str = files["name"]
         if arg["notice_type"] == "offline_file" and name.endswith(".json"):
             try:
-                jsons = json.loads(httpx.get(files["url"]).content.decode("utf-8"))
+                msg = await url_to_msg(files["url"])
+                if not msg:
+                    return
+                jsons = json.loads(msg)
             except json.decoder:
                 await upload.finish("求生json格式不正确")
             if not validate_json(jsons):
                 await upload.finish("求生json格式不正确")
             key = await up_date(jsons, name)
             if key:
                 msg = "输入成功\n"
@@ -41,23 +46,23 @@
             if not isinstance(value, list):
                 return False
             for item in value:
                 if not isinstance(item, dict):
                     return False
                 if not all(key in item for key in ["id", "version", "ip"]):
                     return False
-
-        return True
+        if True:
+            return True
 
     except json.JSONDecodeError:
         return False
 
 
 async def up_date(data, name):
     directory = Path("data/L4D2/l4d2")
     directory.mkdir(parents=True, exist_ok=True)
 
     file_path = directory / name
-    with open(file_path, "w") as json_file:
+    async with aiofiles.open(file_path, "w") as json_file:
         json.dump(data, json_file, ensure_ascii=False)
 
     return True
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 from typing import List, Optional
 
 import jinja2
-from bs4 import BeautifulSoup
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic
 
 # from .htmlimg import dict_to_dict_img
 # from ..l4d2_anne.anne_telecom import ANNE_API
 from ..l4d2_utils.config import TEXT_PATH, l4_config
 from .download import get_head_by_user_id_and_save
 from .send_image_tool import convert_img
 
 template_path = TEXT_PATH / "template"
 
 env = jinja2.Environment(
-    loader=jinja2.FileSystemLoader(template_path), enable_async=True
+    loader=jinja2.FileSystemLoader(template_path),
+    enable_async=True,
 )
 
 
 async def out_png(usr_id, data_dict: dict):
     """使用html来生成图片"""
-
-    with open((template_path / "anne.html"), "r", encoding="utf-8") as file:
-        data_html = file.read()
     # content = template.render_async()
-    soup = BeautifulSoup(data_html, "html.parser")
-    msg_dict = await dict_to_html(usr_id, data_dict, soup)
+    msg_dict = await dict_to_html(usr_id, data_dict)
     template = env.get_template("anne.html")
     html = await template.render_async(data=msg_dict)
-    pic = await html_to_pic(
+    return await html_to_pic(
         html,
         wait=0,
         viewport={"width": 1100, "height": 800},
         template_path=f"file://{template_path.absolute()}",
     )
-    return pic
 
 
-async def dict_to_html(usr_id, DETAIL_MAP: dict, soup: BeautifulSoup):
+async def dict_to_html(usr_id, detail_map: dict):
     """输入qq、字典，获取新的msg替换html"""
-    DETAIL_right = {}
-    DETAIL_right["name"] = DETAIL_MAP["Steam 名字:"]
-    DETAIL_right["Steam_ID"] = DETAIL_MAP["Steam ID:"]
-    DETAIL_right["play_time"] = DETAIL_MAP["游玩时间:"]
-    DETAIL_right["last_online"] = DETAIL_MAP["最后上线:"]
-    DETAIL_right["rank"] = DETAIL_MAP["排行:"]
-    DETAIL_right["points"] = DETAIL_MAP["分数:"]
-    DETAIL_right["point_min"] = DETAIL_MAP["每分钟获取分数:"]
-    DETAIL_right["killed"] = DETAIL_MAP["感染者消灭:"]
-    DETAIL_right["shut"] = DETAIL_MAP["爆头:"]
-    DETAIL_right["out"] = DETAIL_MAP["爆头率:"]
-    DETAIL_right["playtimes"] = DETAIL_MAP["游玩地图数量:"]
-    DETAIL_right["url"] = DETAIL_MAP["个人资料"]
-    DETAIL_right["one_msg"] = DETAIL_MAP["一言"]
-    DETAIL_right["last_one"] = DETAIL_MAP["救援关"]
+    detail_right = {}
+    detail_right["name"] = detail_map["Steam 名字:"]
+    detail_right["Steam_ID"] = detail_map["Steam ID:"]
+    detail_right["play_time"] = detail_map["游玩时间:"]
+    detail_right["last_online"] = detail_map["最后上线:"]
+    detail_right["rank"] = detail_map["排行:"]
+    detail_right["points"] = detail_map["分数:"]
+    detail_right["point_min"] = detail_map["每分钟获取分数:"]
+    detail_right["killed"] = detail_map["感染者消灭:"]
+    detail_right["shut"] = detail_map["爆头:"]
+    detail_right["out"] = detail_map["爆头率:"]
+    detail_right["playtimes"] = detail_map["游玩地图数量:"]
+    detail_right["url"] = detail_map["个人资料"]
+    detail_right["one_msg"] = detail_map["一言"]
+    detail_right["last_one"] = detail_map["救援关"]
     # html_text = soup.prettify()
-    # for key, value in DETAIL_right.items():
+    # for key, value in detail_right.items():
     #     html_text = html_text.replace(key,value)
     # 头像
     temp = await get_head_by_user_id_and_save(usr_id)
-    # temp = await get_head_steam_and_save(usr_id,DETAIL_right['url'])
+    # temp = await get_head_steam_and_save(usr_id,detail_right['url'])
     if not temp:
-        return
+        return None
     res = await convert_img(temp, is_base64=True)
-    DETAIL_right["header"] = f"data:image/png;base64,{res}"
-    data_list: List[dict] = [DETAIL_right]
+    detail_right["header"] = f"data:image/png;base64,{res}"
+    data_list: List[dict] = [detail_right]
     return data_list
 
 
 async def server_ip_pic(msg_list: List[dict]):
     """
     输入一个字典列表，输出图片
     msg_dict:folder/name/map_/players/max_players/Players/[Name]
@@ -76,15 +71,17 @@
     for server_info in msg_list:
         server_info[
             "max_players"
         ] = f"{server_info['players']}/{server_info['max_players']}"
         players_list = []
         if "Players" in server_info:
             sorted_players = sorted(
-                server_info["Players"], key=lambda x: x.get("Score", 0), reverse=True
+                server_info["Players"],
+                key=lambda x: x.get("Score", 0),
+                reverse=True,
             )[:4]
             for player_info in sorted_players:
                 player_str = f"{player_info['name']} | {player_info['Duration']}"
                 players_list.append(player_str)
             while len(players_list) < 4:
                 players_list.append("")
             server_info["Players"] = players_list
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 
 async def download_url(url: str) -> bytes:
     async with httpx.AsyncClient() as client:
         for i in range(3):
             try:
                 resp = await client.get(url, timeout=20)
                 resp.raise_for_status()
-                return resp.content
+                if True:
+                    return resp.content
             except Exception as e:
                 logger.warning(f"Error downloading {url}, retry {i}/3: {e}")
                 await asyncio.sleep(3)
+
     raise Exception(f"{url} 下载失败！")
 
 
 async def download_head(user_id: str) -> bytes:
     url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
     data = await download_url(url)
     if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
@@ -37,80 +39,80 @@
 
 
 def square_to_circle(im: ImageS):
     """im是正方形，变圆形"""
     size = im.size
     mask = Image.new("L", size, 0)
     draw = ImageDraw.Draw(mask)
-    draw.ellipse((0, 0) + size, fill=255)
+    draw.ellipse((0, 0, *size), fill=255)
     # 将遮罩层应用到图像上
     im.putalpha(mask)
     return im
 
 
 async def get_head_by_user_id_and_save(user_id):
     """qq转头像"""
     user_id = str(user_id)
 
-    USER_HEAD_PATH = PLAYERSDATA / user_id / "HEAD.png"
-    DEFAULT_HEADER_PATH = TEXT_PATH / "header"
-    DEFAULT_HEAD_PATH = TEXT_PATH / "head"
-    DEFAULT_HEADER = DEFAULT_HEADER_PATH / random.choice(
-        os.listdir(DEFAULT_HEADER_PATH)
+    user_head_path = PLAYERSDATA / user_id / "HEAD.png"
+    default_header_path = TEXT_PATH / "header"
+    default_head_path = TEXT_PATH / "head"
+    default_header = default_header_path / random.choice(
+        os.listdir(default_header_path),
     )
-    DEFAULT_HEAD = DEFAULT_HEAD_PATH / random.choice(os.listdir(DEFAULT_HEAD_PATH))
+    default_head = default_head_path / random.choice(os.listdir(default_head_path))
     ## im头像 im2头像框 im3合成
-    if os.path.exists(USER_HEAD_PATH):
+    if user_head_path.exists():
         logger.info("使用本地头像")
-        im = Image.open(USER_HEAD_PATH).resize((280, 280)).convert("RGBA")
+        im = Image.open(user_head_path).resize((280, 280)).convert("RGBA")
     else:
         if user_id == "1145149191810":
             logger.info("使用默认头像")
-            im = Image.open(DEFAULT_HEADER).resize((280, 280)).convert("RGBA")
+            im = Image.open(default_header).resize((280, 280)).convert("RGBA")
         else:
             try:
                 logger.info("正在下载头像")
                 image_bytes = await download_head(user_id)
                 im = (
                     Image.open(io.BytesIO(image_bytes))
                     .resize((280, 280))
                     .convert("RGBA")
                 )
-                if not os.path.exists(PLAYERSDATA / user_id):  # 用户文件夹不存在
-                    os.makedirs(PLAYERSDATA / user_id)
-                im.save(USER_HEAD_PATH, "PNG")
-            except:
+                if not (PLAYERSDATA / user_id).exists():  # 用户文件夹不存在
+                    (PLAYERSDATA / user_id).mkdir(parents=True, exist_ok=True)
+                im.save(user_head_path, "PNG")
+            except Exception:
                 logger.error("获取失败")
-                return
-    im2 = Image.open(DEFAULT_HEAD).resize((450, 450)).convert("RGBA")
+                return None
+    im2 = Image.open(default_head).resize((450, 450)).convert("RGBA")
     im3 = Image.new("RGBA", im2.size, (255, 255, 255, 0))
     r, g, b, a1 = im.split()
     r, g, b, a2 = im2.split()
     im = square_to_circle(im)
     im3.paste(im, (75, 75), mask=a1)
     im3.paste(im2, mask=a2)
     return im3
 
 
 # async def get_head_steam_and_save(user_id:str,urls):
 #     """保存steam头像"""
-#     USER_HEAD_PATH = PLAYERSDATA / str(user_id) / 'HEAD.png'
-#     # DEFAULT_HEAD_PATH = TEXT_PATH / "template/player.jpg"
+#     user_head_path = PLAYERSDATA / str(user_id) / 'HEAD.png'
+#     # default_head_path = TEXT_PATH / "template/player.jpg"
 #     ## im头像 im2头像框 im3合成
-#     if os.path.exists(USER_HEAD_PATH):
+#     if os.path.exists(user_head_path):
 #         logger.info("使用本地头像")
-#         im = Image.open(USER_HEAD_PATH).resize((280, 280)).convert("RGBA")
+#         im = Image.open(user_head_path).resize((280, 280)).convert("RGBA")
 #     else:
 #         # if user_id == "1145149191810":
 #         #     logger.info("使用默认头像")
-#         #     im = Image.open(DEFAULT_HEAD_PATH).resize((300, 300)).convert("RGBA")
+#         #     im = Image.open(default_head_path).resize((300, 300)).convert("RGBA")
 #         # else:
 #             try:
 #                 logger.info("正在下载头像")
 #                 image_bytes = await web_player(urls)
-#                 im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")
+#                 im = Image.open(io.BytesIO(image_bytes)).resize((280, 280)).convert("RGBA")  # noqa: E501
 #                 if not os.path.exists(PLAYERSDATA / user_id):#用户文件夹不存在
 #                     os.makedirs(PLAYERSDATA / user_id)
-#                 im.save(USER_HEAD_PATH, "PNG")
+#                 im.save(user_head_path, "PNG")
 #             except TimeoutError:
 #                 logger.error("获取失败")
 #     return im
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class DATA_PANDS:
+class DATAPANDS:
     def __init__(self, data_dict: dict) -> None:
         self.new_data = {}
         self.data_dict = data_dict
         for key in data_dict:
             self.dict_pan(key)
 
     def dict_pan(self, key):
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import List
 
-from PIL import Image, ImageDraw, ImageFont
+from PIL import Image
 
 # 半透明素材
 half_whitel_image_path = Path(__file__).parent.parent.joinpath("data/img/white.png")
 half_whitel_image = Image.open(half_whitel_image_path)
 
 
 async def one_server_img(msg: dict):
@@ -19,22 +19,26 @@
     initial_width = 1080
     initial_height = 600
     height_increment = 100
 
     num_players = len(text_list.get("Player", []))
     final_height = initial_height + num_players * height_increment
 
-    image = Image.new("RGBA", (initial_width, final_height), "white")
-    return image
+    return Image.new("RGBA", (initial_width, final_height), "white")
 
 
 async def adjust_server_name(image: Image.Image, name: str):
     """写标题"""
-    pass
+    if image and name:
+        ...
 
 
 async def adjust_ping(image: Image.Image, ping: str):
     """写ping"""
+    if image and ping:
+        ...
 
 
-async def adjust_player(image: Image.Image, Player: List[dict]):
+async def adjust_player(image: Image.Image, player: List[dict]):
     """写玩家"""
+    if image and player:
+        ...
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 from typing import Union
 
 from PIL import Image
 
 
 async def convert_img(
-    img: Union[Image.Image, str, Path, bytes], is_base64: bool = False
+    img: Union[Image.Image, str, Path, bytes],
+    is_base64: bool = False,
 ):
     """
     :说明:
       将PIL.Image对象转换为bytes或者base64格式。
     :参数:
       * img (Image): 图片。
       * is_base64 (bool): 是否转换为base64格式, 不填默认转为bytes。
@@ -22,11 +23,10 @@
         img = img.convert("RGBA")
         result_buffer = BytesIO()
         img.save(result_buffer, format="PNG", quality=80, subsampling=0)
         res = result_buffer.getvalue()
         if is_base64:
             res = b64encode(res).decode()
         return res
-    elif isinstance(img, bytes):
+    if isinstance(img, bytes):
         return b64encode(img).decode()
-    else:
-        return f"[CQ:image,file=file:///{str(img)}]"
+    return f"[CQ:image,file=file:///{img!s}]"
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from io import BytesIO
 
 from nonebot.log import logger
-from PIL import Image
-
-# import sys
-# sys.modules["srctools._cy_vtf_readwrite"] = None
+from PIL import Image as Image
 from srctools.vtf import VTF, ImageFormats
 
 
 async def img_to_vtf(pic_byte: bytes, tag) -> BytesIO:
     pic = BytesIO(pic_byte)
     pic = Image.open(pic).convert("RGBA")
     vtf_io = BytesIO()
     vtf_ = VTF(
-        1024, 1024, fmt=ImageFormats.DXT5, thumb_fmt=ImageFormats.DXT1, version=(7, 2)
+        1024,
+        1024,
+        fmt=ImageFormats.DXT5,
+        thumb_fmt=ImageFormats.DXT1,
+        version=(7, 2),
     )
     if tag == "覆盖":
         logger.info(tag)
         img2 = Image.new("RGBA", (1024, 1024), (255, 255, 255, 0))
         r, g, b, a = pic.split()
         img2.paste(pic, mask=a)
         pic = pic.resize((1024, 1024))
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-import re
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Dict, Optional, Union
 
 import a2s
 
 try:
     import ujson as json
-except:
+except ImportError:
     import json
 
 from nonebot import get_bot, get_driver, on_command, require
 from nonebot.adapters.onebot.v11 import GroupMessageEvent, Message, MessageSegment
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
-require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler
-
-from ..l4d2_queries.utils import json_server_to_tag_dict, queries_dict
+from ..l4d2_queries.utils import json_server_to_tag_dict
 from ..l4d2_utils.command import get_ip_to_mes
 from ..l4d2_utils.config import l4_config
 from ..l4d2_utils.utils import extract_last_digit, split_maohao
 
+require("nonebot_plugin_apscheduler")
+# from nonebot_plugin_apscheduler import scheduler
+
 driver = get_driver()
 sch_json = Path("data/L4D2/scheduler.json")
 if not sch_json.exists():
     with sch_json.open("w") as f:
         json.dump({}, f, ensure_ascii=False)
 
 add_rss = on_command(
@@ -57,15 +56,15 @@
         return
     if push_msg in ["服务器无响应", None]:
         await matcher.finish("无响应的服务器，请检查")
     else:
         return_msg = await add_or_update_data(group_id, msg)
         if isinstance(push_msg, bytes):
             await matcher.finish(MessageSegment.image(push_msg))
-        elif isinstance(push_msg, Message | MessageSegment):
+        elif isinstance(push_msg, Union[Message, MessageSegment]):
             await matcher.finish(push_msg)
         else:
             await matcher.send(push_msg)
         if return_msg == "add":
             await matcher.send(f"已添加群定时任务【{msg}】{l4_config.l4_push_times}次")
         elif return_msg in ["update", "change"]:
             await matcher.send(f"已更新群定时任务【{msg}】{l4_config.l4_push_times}次")
@@ -88,50 +87,47 @@
     sch_json = Path("data/L4D2/scheduler.json")
     if ad_mode == "add":
         if sch_json.exists():
             with sch_json.open(encoding="utf-8") as f:
                 scheduler_data = json.load(f)
             try:
                 msg_dict = scheduler_data[group_id]
-                times = msg_dict["times"]
+                # times = msg_dict["times"]
                 old_msg = msg_dict["msg"]
                 scheduler_data[group_id] = {
                     "times": l4_config.l4_push_times,
                     "msg": some_str,
                 }
-                if old_msg == some_str:
-                    mode = "update"
-                else:
-                    mode = "change"
-            except:
+                mode = "update" if old_msg == some_str else "change"
+            except Exception:
                 scheduler_data[group_id] = {
                     "times": l4_config.l4_push_times,
                     "msg": some_str,
                 }
                 mode = "new"
 
         else:
             scheduler_data = {
-                group_id: {"times": l4_config.l4_push_times, "msg": some_str}
+                group_id: {"times": l4_config.l4_push_times, "msg": some_str},
             }
             mode = "new"
 
         with sch_json.open("w", encoding="utf-8") as f:
             json.dump(scheduler_data, f, ensure_ascii=False)
 
     else:
         if sch_json.exists():
             with sch_json.open() as f:
                 scheduler_data: Dict[str, Dict[str, Union[str, int]]] = json.load(f)
             try:
                 msg_dict = scheduler_data[group_id]
-                times = msg_dict["times"]
+                # times = msg_dict["times"]
                 old_msg = msg_dict["msg"]
                 scheduler_data[group_id] = {"times": 0, "msg": old_msg}
-            except:
+            except Exception:
                 scheduler_data[group_id] = {"times": 0, "msg": some_str}
         else:
             scheduler_data = {group_id: {"times": 0, "msg": some_str}}
         mode = "del"
 
         with sch_json.open("w", encoding="utf-8") as f:
             json.dump(scheduler_data, f, ensure_ascii=False)
@@ -165,33 +161,37 @@
                     continue
 
         with sch_json.open(mode="w", encoding="utf-8") as f:
             json.dump(scheduler_data, f, ensure_ascii=False)
 
 
 async def send_message(
-    recipient_id: int, msg: str, value: Optional[Dict[str, Union[int, str]]] = None
+    recipient_id: int,
+    msg: str,
+    value: Optional[Dict[str, Union[int, str]]] = None,
 ):
     # 执行发送消息的操作，参数可以根据需要进行传递和使用
     command, message = await extract_last_digit(msg)
     push_msg = await get_ip_to_mes(msg=message, command=command)
     if isinstance(push_msg, bytes):
         await get_bot().send_group_msg(
-            group_id=recipient_id, message=MessageSegment.image(push_msg)
+            group_id=recipient_id,
+            message=MessageSegment.image(push_msg),
         )
-    elif msg and isinstance(push_msg, str):
+        return None
+    if msg and isinstance(push_msg, str):
         # 单服务器
         message = await json_server_to_tag_dict(msg, command)
         if len(message) == 0 or not value:
             # 关键词不匹配，忽略
-            return
+            return None
         try:
             old_msg = value.get("ip_detail", {})
             if not isinstance(old_msg, dict):
-                return
+                return None
             ip = str(message["ip"])
             host, port = split_maohao(ip)
             msg_: a2s.SourceInfo = await a2s.ainfo((host, port))
             value["map_"] = msg_.map_name
             value["rank_players"] = f"{msg_.player_count}/{msg_.max_players}"
             if (
                 old_msg["map_"] == value["map_"]
@@ -200,14 +200,15 @@
                 logger.info(f"{msg}{command}人数和地图未发生变化")
             else:
                 await get_bot().send_group_msg(group_id=recipient_id, message=push_msg)
         except Exception as e:
             logger.warning(e)
 
         return value
+    return None
 
 
 async def server_is_change():
     """检测服务器是否发生变化"""
 
 
 # @driver.on_bot_connect
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Tuple
 
 from ..l4d2_utils.utils import split_maohao
-from .localIP import ALL_HOST, Group_All_HOST
+from .local_ip import ALL_HOST, Group_All_HOST
 from .qqgroup import qq_ip_querie
 
 
 async def get_group_ip_to_msg(command: str, text: str = ""):
     """输出群组ip"""
     if not text:
         group_tag_list: List[str] = Group_All_HOST[command]
@@ -15,19 +15,20 @@
                 group_ip_dict.update({tag: one_group})
                 ip_tuple_list: List[Tuple[str, str, int]] = []
                 for one_server in one_group:
                     number = one_server["id"]
                     host, port = split_maohao(one_server["ip"])
                     ip_tuple_list.append((number, host, int(port)))
                 msg_group_server = await qq_ip_querie(ip_tuple_list)
-                send_dict = await check_group_msg(msg_group_server)
-            else:
-                continue
-            # 还没写完
-        #     host, port = split_maohao(one_ip["ip"])
-        #     msg_tuple = (one_ip["id"], host, port)
-        #     ip_list.append(msg_tuple)
-        # img = await qq_ip_queries_pic(ip_list, igr)
+                return await check_group_msg(msg_group_server)
+    return None
+    # 还没写完
+    #     host, port = split_maohao(one_ip["ip"])
+    #     msg_tuple = (one_ip["id"], host, port)
+    #     ip_list.append(msg_tuple)
+    # img = await qq_ip_queries_pic(ip_list, igr)
 
 
 async def check_group_msg(msg: Dict[str, List[Dict[str, str]]]):
+    if msg:
+        ...
     ...
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/localIP.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/local_ip.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,38 @@
-try:
-    import ujson as json
-except:
-    import json
+import json
 from pathlib import Path
 from typing import Dict, List
-import os
 
-BOT_DIR = os.path.dirname(os.path.abspath(__file__))
-filename = "data/L4D2/l4d2.json"
+filename = Path("data/L4D2/l4d2.json")
 global_file = Path(Path(__file__).parent.parent, filename)
 
 
 def load_ip_json():
     # 本地模块
-    LOCAL_HOST: Dict[str, List[Dict[str, str]]] = {}
+    local_host: Dict[str, List[Dict[str, str]]] = {}
     try:
         # 获取所有json文件的路径
         json_files = Path("data/L4D2/l4d2").glob("*.json")
 
         # 将所有json文件中的字典对象合并为一个字典
         for file_path in json_files:
-            with open(file_path, "r", encoding="utf-8") as f:
-                LOCAL_HOST.update(json.load(f))
-    except:
+            with file_path.open("r", encoding="utf-8") as f:
+                local_host.update(json.load(f))
+    except Exception:
         pass
-    return LOCAL_HOST
+    return local_host
 
 
 def load_group_json():
     try:
-        GROUP_HOST: Dict[str, List[str]] = json.load(
-            open(filename, "r", encoding="utf8")
-        )
-    except IOError or FileNotFoundError:
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
+        group_host: Dict[str, List[str]] = json.load(filename.open("r", encoding="utf8"))
+    except (IOError, FileNotFoundError):
+        filename.parent.mkdir(parents=True, exist_ok=True)
         data: Dict[str, List[str]] = {"anne": ["云"]}
-        with open(filename, "w") as f:
+        with filename.open("w") as f:
             json.dump(data, f)
-        GROUP_HOST: Dict[str, List[str]] = {}
-    return GROUP_HOST
+        group_host: Dict[str, List[str]] = {}
+    return group_host
 
 
 ALL_HOST: Dict[str, List[Dict[str, str]]] = load_ip_json()
 Group_All_HOST: Dict[str, List[str]] = load_group_json()
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import asyncio
 import random
-from typing import Any, Dict, List, Tuple, Union
+from pathlib import Path
+from typing import Any, Dict, List, Tuple
 
+import a2s
+import aiofiles
 from nonebot.log import logger
 
-from ..l4d2_data.serverip import L4D2Server
-from ..l4d2_image import server_ip_pic
-from ..l4d2_utils.message import KAILAO, PRISON, QUEREN
-from ..l4d2_utils.utils import split_maohao
-from .localIP import ALL_HOST
-from .utils import (
+from nonebot_plugin_l4d2_server.l4d2_data.serverip import L4D2Server
+from nonebot_plugin_l4d2_server.l4d2_image import server_ip_pic
+from nonebot_plugin_l4d2_server.l4d2_queries.local_ip import ALL_HOST
+from nonebot_plugin_l4d2_server.l4d2_queries.utils import (
     msg_ip_to_list,
     player_queries,
     player_queries_anne_dict,
     queries,
     queries_dict,
 )
+from nonebot_plugin_l4d2_server.l4d2_utils.message import KAILAO, PRISON, QUEREN
+from nonebot_plugin_l4d2_server.l4d2_utils.utils import split_maohao
 
 try:
     import ujson as json
-except:
+except ImportError:
     import json
 si = L4D2Server()
 errors = (
     ConnectionRefusedError,
     ConnectionResetError,
     asyncio.exceptions.TimeoutError,
     OSError,
 )
 # errors = (TypeError,KeyError,ValueError,ConnectionResetError,TimeoutError)
 
 
 async def get_qqgroup_ip_msg(qqgroup):
     """首先，获取qq群订阅数据，再依次queries返回ip原标"""
-    ip_list = await si.query_server_ip(qqgroup)
-    return ip_list
+    return await si.query_server_ip(qqgroup)
 
 
 async def bind_group_ip(group: int, host: str, port: int):
     ip_list = await si.query_server_ip(group)
     if (host, port) in ip_list:
         return "本群已添加过该ip辣"
     await si.bind_server_ip(group, host, port)
@@ -62,15 +64,15 @@
     """输入一个ip的二元元组组成的列表，返回一个输出消息的列表
     未来作图这里重置"""
     messsage = ""
     for i in msg:
         number, qqgroup, host, port = i
         msg2 = await player_queries(host, port)
         msg1 = await queries(host, port)
-        messsage += "序号、" + str(number) + "\n" + msg1 + msg2 + "--------------------\n"
+        messsage += f"序号、{number!s} \n{msg1}{msg2}--------------------\n"
     return messsage
 
 
 async def qq_ip_querie(msg: List[Tuple[str, str, int]], igr: bool = True):
     msg_list: List[Dict[str, Any]] = []
     tasks = []  # 用来保存异步任务
     if msg != []:
@@ -90,16 +92,16 @@
                         process_message(
                             number,
                             host,
                             port,
                             msg_list,
                             igr,
                             qqgroup,
-                        )
-                    )
+                        ),
+                    ),
                 )
             except ValueError:
                 continue  # 处理异常情况
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
         # msg_list.sort(key=lambda x: x["number"])
@@ -132,15 +134,15 @@
         msg2 = await player_queries_anne_dict(host, port)
         msg1 = await queries_dict(host, port)
         msg3 = await server_rule_dict(host, port)
         msg1.update(
             {
                 "Players": msg2,
                 "number": number,
-            }
+            },
         )
         msg1.update(msg3)
         if qqgroup:
             msg1.update({"tag": qqgroup})
         msg_list.append(msg1)
     except errors:
         if igr:
@@ -154,15 +156,15 @@
                     "map_",
                     "players",
                     "max_players",
                     "rank_players",
                     "ping",
                 ]
             }
-            null_dict.update({"number": number, "ip": f"{host}:{port}", "Players": []})  # type: ignore
+            null_dict.update({"number": number, "ip": f"{host}:{port}", "Players": []})  # type: ignore  # noqa: E501
             msg_list.append(null_dict)
 
 
 async def get_tan_jian(msg: List[tuple], mode: int):
     """获取anne列表抽一个"""
     msg_list = []
     random.shuffle(msg)
@@ -184,41 +186,41 @@
                 points = point / 4
                 if points / sps < 10:
                     continue
                 if "HT" in msg1["name"]:
                     continue
                 msg1.update({"Players": msg2})
                 msg1.update({"ranks": point})
-                ips = f"{host}:{str(port)}"
+                ips = f"{host}:{port!s}"
                 msg1.update({"ips": ips})
                 # msg1是一行数据完整的字典
                 msg_list.append(msg1)
             if mode == 2:
                 # 坐牢
                 # try:
                 msg1 = await queries_dict(host, port)
                 if "普通药役" in msg1["name"]:
                     if "缺人" in msg1["name"]:
                         msg2 = await player_queries_anne_dict(host, port)
                         msg1.update({"Players": msg2})
-                        ips = f"{host}:{str(port)}"
+                        ips = f"{host}:{port!s}"
                         msg1.update({"ips": ips})
                         # msg1是一行数据完整的字典
                     else:
                         continue
                 else:
                     continue
                 msg_list.append(msg1)
             if mode == 3:
                 # 开牢
                 msg1 = await queries_dict(host, port)
                 if "[" not in msg1["name"]:
                     msg2 = await player_queries_anne_dict(host, port)
                     msg1.update({"Players": msg2})
-                    ips = f"{host}:{str(port)}"
+                    ips = f"{host}:{port!s}"
                     msg1.update({"ips": ips})
                     # msg1是一行数据完整的字典
                     msg_list.append(msg1)
         except errors:
             continue
         if msg_list != []:
             break
@@ -245,15 +247,15 @@
             message = random.choice(QUEREN[2])
         elif player_point == "3":
             message = random.choice(QUEREN[3])
         else:
             message = random.choice(QUEREN[4])
     if mode == 3:
         message = random.choice(KAILAO)
-    message += "\n" + "名称：" + mse["name"] + "\n"
+    message += f"\n名称：{mse['name']}\n"
     message += "地图：" + mse["map_"] + "\n"
     message += f"玩家：{mse['players']} / {mse['max_players']}\n"
     try:
         message += await msg_ip_to_list(mse["Players"])
     except KeyError:
         message += "服务器里，是空空的呢\n"
     return message
@@ -287,51 +289,60 @@
                 ids = [server["id"] for server in value]
                 # 序号
                 if len(data_list) == 4:
                     data_num = int(max(ids, default=0)) + 1
                     add_server.update({"id": data_num})
                 elif len(data_list) == 5:
                     if not data_list[4].isdigit():
-                        return "序号应该为大于0的正整数，请输入【求生更新 添加 腐竹 ip 模式 序号】"
+                        return "请输入【求生更新 添加 腐竹 ip 模式 序号】"
                     data_num = int(data_list[4])
                     if data_num in ids:
-                        return "该序号已存在，请尝试删除原序号【求生更新 删除 腐竹 序号】"
+                        return "该序号已存在，请删除原序号【求生更新 删除 腐竹 序号】"
                     add_server.update({"id": data_num})
                 else:
-                    return "输入参数错误，请输入【求生更新 添加 腐竹 ip 模式 序号】或【求生更新 添加 腐竹 ip 模式】"
+                    return "请输入【求生更新 添加 腐竹 ip 模式 序号】"
                 # 模式，ip
                 try:
                     host, port = split_maohao(data_list[2])
                     add_server.update({"host": host, "port": port})
                 except KeyError:
                     return "ip格式不正确【114.11.4.514:9191】"
                 add_server.update({"version": data_list[3]})
                 value.append(add_server)
                 ALL_HOST[key] = value
-                with open("data/L4D2/l4d2.json", "w", encoding="utf8") as f_new:
+                with Path("data/L4D2/l4d2.json").open("w", encoding="utf8") as f_new:
                     json.dump(ALL_HOST, f_new, ensure_ascii=False, indent=4)
                 return f"添加成功，指令为{key}{data_num}"
+        return None
 
-    elif data_list[0] == "删除":
+    if data_list[0] == "删除":
         for key, value in ALL_HOST.items():
             if data_list[1] == key:
                 try:
                     data_num = int(data_list[2])
                 except ValueError:
                     return "序号应该为大于0的正整数，请输入【求生更新 删除 腐竹 序号】"
                 for i, server in enumerate(value):
                     if data_num == server["id"]:
                         value.pop(i)
                         if not value:
                             ALL_HOST.pop(key)
-                        with open("data/L4D2/l4d2.json", "w", encoding="utf8") as f_new:
-                            json.dump(ALL_HOST, f_new, ensure_ascii=False, indent=4)
+                        async with aiofiles.open(
+                            "data/L4D2/l4d2.json",
+                            "w",
+                            encoding="utf8",
+                        ) as f_new:
+                            await f_new.write(
+                                json.dumps(ALL_HOST, ensure_ascii=False, indent=4),
+                            )
+                            await f_new.flush()
                         return "删除成功喵"
                 return "序号不正确，请输入【求生更新 删除 腐竹 序号】"
         return "腐竹名不存在，请输入【求生更新 删除 腐竹 序号】"
+    return None
 
 
 async def add_ip(group_id, host, port):
     """先查找是否存在，如果不存在则创建"""
     return await bind_group_ip(group_id, host, port)
 
 
@@ -342,30 +353,28 @@
 
 async def show_ip(group_id):
     """先查找群ip，再根据群ip返回"""
     data_list = await get_qqgroup_ip_msg(group_id)
     logger.info(data_list)
     if len(data_list) == 0:
         return "本群没有订阅"
-    msg = await qq_ip_queries_pic(data_list)
-    return msg
+    return await qq_ip_queries_pic(data_list)
 
 
 async def get_number_url(number):
     ip = await get_server_ip(number)
     if not ip:
         return "该序号不存在"
-    url = f"connect {ip}"
-    return url
+    return f"connect {ip}"
 
 
 async def server_rule_dict(ip: str, port: int):
     port = int(port)
     ip = str(ip)
     msg_dict = {}
     # message_dict = await l4d(ip,port)
     try:
         msg: dict = await a2s.arules((ip, port))  # type: ignore
         msg_dict["tick"] = msg["l4d2_tickrate_enabler"] + "tick"
-    except:
+    except Exception:
         msg_dict["tick"] = ""
     return msg_dict
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_queries/utils.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_queries/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import a2s
 from nonebot.log import logger
 from pydantic import BaseModel
 
 from ..l4d2_utils.config import l4_config
 from ..l4d2_utils.txt_to_img import mode_txt_to_img
 from ..l4d2_utils.utils import split_maohao
-from .localIP import ALL_HOST
+from .local_ip import ALL_HOST
 
 
-class GROUP_MSG(BaseModel):
+class GROUPMSG(BaseModel):
     tag: str
     online_server: int
     empty_server: int
     full_server: int
     max_server: int
 
     online_player: int
@@ -44,20 +44,23 @@
     # msgs = '有无法识别的用户名'
     # return msgs
     return msgs
 
 
 async def get_anne_server_ip(ip, ismsg: bool = False):
     """输出查询ip和ping"""
+    if ismsg:
+        ...
     host, port = split_maohao(ip)
     data = await queries_server([host, port])
 
     if l4_config.l4_image:
         data = mode_txt_to_img(
-            data.split("\n")[0], data.replace(data.split("\n")[0], f"\nconnect {ip}")
+            data.split("\n")[0],
+            data.replace(data.split("\n")[0], f"\nconnect {ip}"),
         )
     else:
         data += f"\nconnect {ip}"
     return data
 
 
 async def json_server_to_tag_dict(key: str, msg: str):
@@ -95,15 +98,15 @@
     if message_list != []:
         for i in message_list:
             msg_list.append(
                 {
                     "name": i.name,
                     "Score": i.score,
                     "Duration": await convert_duration(i.duration),
-                }
+                },
             )
     return msg_list
 
 
 async def player_queries(ip: str, port: int):
     port = int(port)
     message_list = await player_queries_anne_dict(ip, port)
@@ -117,20 +120,20 @@
         message += "服务器里，是空空的呢\n"
     else:
         max_duration_len = max([len(str(i["Duration"])) for i in message_list])
         max_score_len = max([len(str(i["Score"])) for i in message_list])
         for i in message_list:
             n += 1
             name = i["name"]
-            Score = i["Score"]
-            if Score == "0":
-                Score = "摸"
-            Duration = i["Duration"]
-            soc = "[{:>{}}]".format(Score, max_score_len)
-            dur = "{:^{}}".format(Duration, max_duration_len)
+            score = i["Score"]
+            if score == "0":
+                score = "摸"
+            duration = i["Duration"]
+            soc = "[{:>{}}]".format(score, max_score_len)
+            dur = "{:^{}}".format(duration, max_duration_len)
             message += f"{soc} | {dur} | {name} \n"
     return message
 
 
 async def convert_duration(duration: float) -> str:
     minutes, seconds = divmod(duration, 60)
     hours, minutes = divmod(minutes, 60)
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
     # 等待 SERVERDATA_AUTH_RESPONSE 数据包
     while response.type != Type.SERVERDATA_AUTH_RESPONSE:
         response = await Packet.aread(reader)
 
     if response.id == -1:
         await close(writer)
-        raise WrongPassword()
 
     # 循环接收用户输入并发送指令
     while True:
         try:
             command = input("请输入指令：")
 
         except EOFError:
@@ -51,15 +50,7 @@
         # if response.id != request.id:
         #     raise SessionTimeout()
 
         print(response.payload.decode(encoding, errors="ignore"))
 
     # 断开连接
     await close(writer)
-
-
-class WrongPassword(Exception):
-    """Indicates a wrong password."""
-
-
-class SessionTimeout(Exception):
-    """Indicates that the session timed out."""
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import asyncio
 from pathlib import Path
 
+import aiofiles
 from rcon.source import rcon
 
 from ..l4d2_utils.config import CHECK_FILE, l4_config
 
 
-async def rcon_server(PASSWORD: str, msg: str):
-    # response = await rcon(command=msg, host=l4_host, port=l4_port, passwd=PASSWORD,encoding='utf-8')
+async def rcon_server(password: str, msg: str):
+    # response = await rcon(command=msg, host=l4_host, port=l4_port, passwd=password,encoding='utf-8')
     # return response
     try:
-        response = await asyncio.wait_for(
+        return await asyncio.wait_for(
             rcon(
                 command=msg,
                 host=l4_config.l4_ipall[CHECK_FILE]["host"],
                 port=l4_config.l4_ipall[CHECK_FILE]["port"],
-                passwd=PASSWORD,
+                passwd=password,
             ),
             timeout=30,
         )
-        return response
     except asyncio.TimeoutError:
         return "超时"
 
 
 async def read_server_cfg_rcon():
     """如果没有输入rcon，尝试自动获取"""
     if not l4_config.l4_ipall[CHECK_FILE]["rcon"]:
         cfg_server = Path(
-            l4_config.l4_ipall[CHECK_FILE]["location"], "left4dead2/cfg/server.cfg"
+            l4_config.l4_ipall[CHECK_FILE]["location"],
+            "left4dead2/cfg/server.cfg",
         )
-        with open(cfg_server, "r") as cfg:
-            content: str = cfg.read()
+        async with aiofiles.open(cfg_server, "r") as cfg:
+            content: str = await cfg.read()
             lines = content.split("\n")
             for line in lines:
                 if line.startswith("rcon_password"):
                     password = line.split(" ")[-1]
-                    password = password.strip('"')
-                    return password
+                    return password.strip('"')
     return l4_config.l4_ipall[CHECK_FILE]["rcon"]
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 from typing import Dict, List, Union
 
 import httpx
-from nonebot.log import logger
 
 try:
     import ujson as json
-except:
+except ImportError:
     import json
 
 
 async def workshop_to_dict(msg: str):
     """把创意工坊的id，转化为信息字典"""
     i = await api_get_json(msg)
 
     # 处理是否是多地图文件
     if i["file_url"] == i["preview_url"]:
-        return await primary_map(i)
-    else:
-        return await only_map(i)
+        return await primary_map(i)  # type: ignore
+    return await only_map(i)
 
 
-async def api_get_json(msg: str):
+async def api_get_json(msg: str) -> Dict[str, str]:
     url_serach = "https://db.steamworkshopdownloader.io/prod/api/details/file"
     data: Dict[str, str] = {msg: ""}
     headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0",
     }
-    data_msg = httpx.post(url=url_serach, headers=headers, data=data).content.decode(
-        "utf-8"
-    )
-    logger.info(data_msg)
-    out = {}
-    data_msg = data_msg[1:-1]
-    datas: Dict[str, str] = json.loads(data_msg)
-    return datas
+    async with httpx.AsyncClient() as client:
+        response = await client.post(url_serach, headers=headers, data=data)
+        data_msg = response.content.decode("utf-8")
+        datas: Dict[str, str] = json.loads(data_msg[1:-1])
+        return datas
 
 
 async def only_map(i: Dict[str, str]):
     """单地图下载"""
     out: Dict[str, str] = {}
     out["名字"] = i["title"]
     out["游戏"] = i["app_name"]
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,15 @@
 
 
 @get_update_log.handle()
 @register_menu(
     "更新记录",
     "更新记录",
     "查看插件最近的更新记录",
-    detail_des=(
-        "介绍：\n" "查看插件最近的有效Git更新记录\n" " \n" "指令：\n" "- <ft color=(238,120,0)>更新记录</ft>"
-    ),
+    detail_des=("介绍：\n查看插件最近的有效Git更新记录\n \n指令：\n- <ft color=(238,120,0)>更新记录</ft>"),
 )
 async def send_updatelog_msg(
     matcher: Matcher,
 ):
     im = await draw_update_log_img(is_update=False)
     logger.info("正在执行[更新记录]...")
     if isinstance(im, str):
@@ -69,15 +67,15 @@
 
 @l4d_restart.handle()
 @register_menu(
     "重启Bot",
     "l4重启",
     "重启Bot框架",
     trigger_method="超级用户指令",
-    detail_des=("介绍：\n" "重启Bot框架\n" " \n" "指令：\n" "- <ft color=(238,120,0)>l4重启</ft>"),
+    detail_des=("介绍：\n重启Bot框架\n \n指令：\n- <ft color=(238,120,0)>l4重启</ft>"),
 )
 async def send_restart_msg(
     bot: Bot,
     event: MessageEvent,
     matcher: Matcher,
 ):
     if not await SUPERUSER(bot, event):
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,66 +2,68 @@
 import os
 import platform
 import subprocess
 import sys
 import time
 from pathlib import Path
 
+import aiofiles
+
 # from ..utils.db_operation.db_operation import config_check
 
 bot_start = Path().cwd() / "bot.py"
 restart_sh_path = Path().cwd() / "gs_restart.sh"
 update_log_path = Path(__file__).parent / "update_log.json"
 
 _restart_sh = """#!/bin/bash
 kill -9 {}
 {} &"""
 
 
 async def get_restart_sh(extra: str) -> str:
-    args = f"{extra} {str(bot_start.absolute())}"
+    args = f"{extra} {bot_start.absolute()!s}"
     return _restart_sh.format(str(bot_start.absolute()), args)
 
 
 async def restart_genshinuid(send_type: str, send_id: str) -> None:
     # extra = ''
     # if await config_check('UsePoetry'):
     #     extra = 'poetry run '
     extra = sys.executable
     restart_sh = await get_restart_sh(extra)
     if not restart_sh_path.exists():
-        with open(restart_sh_path, "w", encoding="utf8") as f:
-            f.write(restart_sh)
+        async with aiofiles.open(restart_sh_path, "w", encoding="utf8") as f:
+            await f.write(restart_sh)
         if platform.system() == "Linux":
-            os.system(f"chmod +x {str(restart_sh_path)}")
-            os.system(f"chmod +x {str(bot_start)}")
+            os.system(f"chmod +x {restart_sh_path!s}")  # noqa: ASYNC102
+            os.system(f"chmod +x {bot_start!s}")  # noqa: ASYNC102
     now_time = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(time.time()))
     update_log = {
         "type": "restart",
         "msg": "重启完成!",
         "send_type": send_type,
         "send_to": send_id,
         "time": now_time,
     }
-    with open(str(update_log_path), "w", encoding="utf-8") as f:
-        json.dump(update_log, f)
+    async with aiofiles.open(str(update_log_path), mode="w", encoding="utf-8") as f:
+        await f.write(json.dumps(update_log))
     if platform.system() == "Linux":
         os.execl(str(restart_sh_path), " ")
     else:
         pid = os.getpid()
-        subprocess.Popen(
+        subprocess.Popen(  # noqa: ASYNC101
             f"taskkill /F /PID {pid} & {extra} {bot_start}",
             shell=True,
         )
 
 
 async def restart_message() -> dict:
     if update_log_path.exists():
-        with open(update_log_path, "r", encoding="utf-8") as f:
-            update_log = json.load(f)
+        async with aiofiles.open(update_log_path, "r", encoding="utf-8") as f:
+            content = await f.read()
+            update_log = json.loads(content)
         msg = f'{update_log["msg"]}\n重启时间:{update_log["time"]}'
         update_log["msg"] = msg
-        os.remove(update_log_path)
-        os.remove(restart_sh_path)
+        update_log_path.unlink()
+        restart_sh_path.unlink()
         return update_log
-    else:
-        return {}
+    return {}
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from pathlib import Path
 from typing import List, Union
 
 import git
 from git.exc import GitCommandError
 from nonebot.log import logger
 
+log_config = (
+    {
+        "key": "✨🐛🎨⚡🍱♻️",
+        "num": 7,
+    },
+)
+
 
 async def update_from_git(
     level: int = 0,
     repo_path: Union[str, Path, None] = None,
-    log_config: dict = {
-        "key": "✨🐛🎨⚡🍱♻️",
-        "num": 7,
-    },
+    log_config=log_config,
     is_update: bool = True,
 ) -> List[str]:
     if repo_path is None:
         repo_path = Path(__file__).parents[2]
     repo = git.Repo(repo_path)  # type: ignore
     o = repo.remotes.origin
 
@@ -40,10 +44,10 @@
     commits = list(repo.iter_commits(max_count=40))
     log_list = []
     for commit in commits:
         if isinstance(commit.message, str):
             for key in log_config["key"]:
                 if key in commit.message:
                     log_list.append(commit.message.replace("\n", ""))
-                    if len(log_list) >= log_config["num"]:
+                    if len(log_list) >= int(log_config["num"]):
                         break
     return log_list
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,102 +1,139 @@
 import asyncio
 import re
 from time import sleep
-from typing import List, Tuple, Type
+from typing import Dict, List, Tuple, Type
 
 from nonebot import on_command, on_keyword, on_notice, on_regex
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment
+from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, CommandStart, RawCommand
 
-from ..l4d2_anne.server import ANNE_IP, group_key, server_key
-from ..l4d2_image.one import one_server_img
+from ..l4d2_anne.server import group_key, server_key
 from ..l4d2_queries import get_group_ip_to_msg
-from ..l4d2_queries.localIP import ALL_HOST, Group_All_HOST
+from ..l4d2_queries.local_ip import ALL_HOST
 from ..l4d2_queries.qqgroup import get_tan_jian, qq_ip_queries_pic, split_maohao
 from ..l4d2_queries.utils import get_anne_server_ip, json_server_to_tag_dict
-from .config import *
-from .rule import *
-from .txt_to_img import mode_txt_to_img
-
-# from .utils import qq_ip_queries_pic,json_server_to_tag_dict,get_anne_server_ip,get_tan_jian
-from .utils import *
+from .config import MASTER, driver, l4_config
+from .rule import wenjian
+from .utils import str_to_picstr
 
 help_ = on_command("l4_help", aliases={"求生帮助"}, priority=20, block=True)
 
-# 服务器
-# last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
-
 
 up = on_notice(rule=wenjian)
 
 
 rename_vpk = on_regex(
     r"^求生地图\s*(\S+.*?)\s*(改|改名)?\s*(\S+.*?)\s*$",
     flags=re.S,
     block=True,
     priority=20,
-    permission=Master,
+    permission=MASTER,
 )
 
-find_vpk = on_command("l4_map", aliases={"求生地图", "查看求生地图"}, priority=25, block=True)
+find_vpk = on_command("l4_map", aliases={"求生地图"}, priority=25, block=True)
 del_vpk = on_command(
-    "l4_del_map", aliases={"求生地图删除", "地图删除"}, priority=20, block=True, permission=Master
+    "l4_del_map",
+    aliases={"求生地图删除", "地图删除"},
+    priority=20,
+    permission=MASTER,
 )
 rcon_to_server = on_command(
-    "rcon", aliases={"求生服务器指令", "服务器指令", "求生服务器控制台"}, block=True, permission=Master
-)
+    "rcon",
+    aliases={"求生服务器指令", "服务器指令"},
+    permission=MASTER,
+)  # noqa: E501
 check_path = on_command(
-    "l4_check", aliases={"求生路径"}, priority=20, block=True, permission=Master
+    "l4_check",
+    aliases={"求生路径"},
+    priority=20,
+    block=True,
+    permission=MASTER,
 )
 smx_file = on_command(
-    "l4_smx", aliases={"求生插件"}, priority=20, block=True, permission=Master
+    "l4_smx",
+    aliases={"求生插件"},
+    priority=20,
+    block=True,
+    permission=MASTER,
 )
 
 # anne
 anne_player = on_command("Ranne", aliases={"求生anne"}, priority=25, block=True)
 anne_bind = on_command(
-    "Rbind", aliases={"steam绑定", "求生绑定", "anne绑定"}, priority=20, block=True
+    "Rbind",
+    aliases={"steam绑定", "求生绑定", "anne绑定"},
+    priority=20,
+    block=True,
 )
 del_bind = on_command(
-    "del_bind", aliases={"steam解绑", "求生解绑", "anne解绑"}, priority=20, block=True
+    "del_bind",
+    aliases={"steam解绑", "求生解绑", "anne解绑"},
+    priority=20,
+    block=True,
 )
 prison = on_command("zl", aliases={"坐牢"}, priority=20, block=True)
 open_prison = on_command("kl", aliases={"开牢"}, priority=20, block=True)
 
 updata = on_command(
-    "updata_anne", aliases={"求生更新anne"}, priority=20, block=True, permission=Master
+    "updata_anne",
+    aliases={"求生更新anne"},
+    priority=20,
+    block=True,
+    permission=MASTER,
 )
 tan_jian = on_command("tj", aliases={"探监"}, priority=20, block=True)
 
 # 查询
 queries_comm = on_keyword(
-    keywords={"queries", "求生ip", "求生IP", "connect"}, priority=20, block=True
+    keywords={"queries", "求生ip", "求生IP", "connect"},
+    priority=20,
+    block=True,
 )
 add_queries = on_command(
-    "addq", aliases={"求生添加订阅"}, priority=20, block=True, permission=Master
+    "addq",
+    aliases={"求生添加订阅"},
+    priority=20,
+    block=True,
+    permission=MASTER,
 )
 del_queries = on_command(
-    "delq", aliases={"求生取消订阅"}, priority=20, block=True, permission=Master
+    "delq",
+    aliases={"求生取消订阅"},
+    priority=20,
+    block=True,
+    permission=MASTER,
 )
 show_queries = on_command("showq", aliases={"求生订阅"}, priority=20, block=True)
 join_server = on_command("ld_jr", aliases={"求生加入"}, priority=20, block=True)
 connect_rcon = on_command(
-    "Rrcon", aliases={"求生连接", "求生链接", "求生rcon"}, priority=50, block=False
+    "Rrcon",
+    aliases={"求生连接", "求生链接", "求生rcon"},
+    priority=50,
+    block=False,
 )
 end_connect = ["stop", "结束", "连接结束", "结束连接"]
 search_api = on_command(
-    "search", aliases={"求生三方"}, priority=20, block=True, permission=Master
+    "search",
+    aliases={"求生三方"},
+    priority=20,
+    block=True,
+    permission=MASTER,
 )
 # which_map = on_keyword("是什么图"), priority=20, block=False)
-reload_ip = on_command("l4_reload", aliases={"重载ip"}, priority=30, permission=Master)
+reload_ip = on_command("l4_reload", aliases={"重载ip"}, priority=30, permission=MASTER)
 
 # 下载内容
 up_workshop = on_command(
-    "workshop", aliases={"创意工坊下载", "求生创意工坊"}, priority=20, block=True
+    "workshop",
+    aliases={"创意工坊下载", "求生创意工坊"},
+    priority=20,
+    block=True,
 )
 vtf_make = on_command("vtf_make", aliases={"求生喷漆"}, priority=20, block=True)
 
 
 matchers: Dict[str, List[Type[Matcher]]] = {}
 
 
@@ -130,36 +167,37 @@
                 host, port = split_maohao(one_ip["ip"])
                 ip_anne_list.append((one_ip["id"], host, port))
     except (KeyError, TypeError):
         pass
     await get_read_ip(ip_anne_list)
 
     @tan_jian.handle()
-    async def _(matcher: Matcher, event: MessageEvent):
+    async def _(matcher: Matcher):
         msg = await get_tan_jian(ip_anne_list, 1)
         await str_to_picstr(push_msg=msg, matcher=matcher)
 
     @prison.handle()
-    async def _(matcher: Matcher, event: MessageEvent):
+    async def _(matcher: Matcher):
         msg = await get_tan_jian(ip_anne_list, 2)
         await str_to_picstr(push_msg=msg, matcher=matcher)
 
     @open_prison.handle()
-    async def _(matcher: Matcher, event: MessageEvent):
+    async def _(matcher: Matcher):
         msg = await get_tan_jian(ip_anne_list, 3)
         await str_to_picstr(push_msg=msg, matcher=matcher)
 
 
 async def get_read_ip(ip_anne_list: List[Tuple[str, str, str]]):
     get_ip = on_command("云", aliases=server_key(), priority=50, block=True)
+    if not ip_anne_list:
+        ...
 
     @get_ip.handle()
     async def _(
         matcher: Matcher,
-        event: MessageEvent,
         start: str = CommandStart(),
         command: str = RawCommand(),
         args: Message = CommandArg(),
     ):
         if start:
             command = command.replace(start, "")
         if command == "anne":
@@ -205,39 +243,37 @@
         this_ips = ALL_HOST[command]
         ip_list: List[Tuple[str, str, str]] = []
         for one_ip in this_ips:
             host, port = split_maohao(one_ip["ip"])
             msg_tuple = (one_ip["id"], host, port)
             ip_list.append(msg_tuple)
         img = await qq_ip_queries_pic(ip_list, igr)
-        if img:
-            return img
-        else:
-            return "服务器无响应"
-    else:
-        if not msg[0].isdigit():
-            # if any(mode in msg for mode in gamemode_list):
-            #     pass
-            # else:
-            return
-        message = await json_server_to_tag_dict(command, msg)
-        if len(message) == 0:
-            # 关键词不匹配，忽略
-            return
-        ip = str(message["ip"])
-        logger.info(ip)
 
-        try:
-            msgs = await get_anne_server_ip(ip)
-            return msgs
-        except (OSError, asyncio.exceptions.TimeoutError):
-            return "服务器无响应"
+        return img if img else "服务器无响应"
+
+    if not msg[0].isdigit():
+        # if any(mode in msg for mode in gamemode_list):
+        #     pass
+        # else:
+        return None
+    message = await json_server_to_tag_dict(command, msg)
+    if len(message) == 0:
+        # 关键词不匹配，忽略
+        return None
+    ip = str(message["ip"])
+    logger.info(ip)
+
+    try:
+        return await get_anne_server_ip(ip)
+    except (OSError, asyncio.exceptions.TimeoutError):
+        return "服务器无响应"
 
 
 async def get_read_group_ip():
+    """输出群组服务器"""
     get_grou_ip = on_command("anne", aliases=group_key(), priority=80, block=True)
 
     @get_grou_ip.handle()
     async def _(
         matcher: Matcher,
         start: str = CommandStart(),
         command: str = RawCommand(),
@@ -249,28 +285,31 @@
         push_msg = await get_group_ip_to_msg(msg, command)
         if isinstance(push_msg, bytes):
             send_msg = MessageSegment.image(push_msg)
         elif msg and type(push_msg) == list:
             send_msg = Message(MessageSegment.image(push_msg[0]) + push_msg[-1])
         elif msg and isinstance(push_msg, str):
             await str_to_picstr(push_msg, matcher)
+            return
+        else:
+            return
+        await matcher.finish(send_msg)
 
 
 # tests = on_command("测试1")
 
 # @tests.handle()
 # async def _(event: Event,arg:Message=CommandArg()):
 #     logger.info(event)
 #     logger.info(arg.extract_plain_text())
 
 
 async def init():
     global matchers
     # print('启动辣')
-    from ..l4d2_update import driver, get_update_log, l4d_restart, l4d_update
 
     await get_des_ip()
 
 
 @driver.on_startup
 async def _():
     await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,38 +4,37 @@
 
 from nonebot import get_driver
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
     PRIVATE_FRIEND,
 )
-from nonebot.log import logger
 from nonebot.permission import SUPERUSER
 from pydantic import BaseModel, Field
 from ruamel import yaml
 
 file_format = (".vpk", ".zip", ".7z", "rar")
 # 权限
 
 driver = get_driver()
 COMMAND_START = list(driver.config.command_start)
 
 headers = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0",  # noqa: E501
 }
 
 try:
-    NICKNAME: str = list(driver.config.nickname)[0]
+    NICKNAME: str = next(iter(driver.config.nickname))
 except Exception:
     NICKNAME = "bot"
 CHECK_FILE: int = 0
 
 
-reMaster = SUPERUSER | GROUP_OWNER
-Master = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
+re_master = SUPERUSER | GROUP_OWNER
+MASTER = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
 ADMINISTRATOR = SUPERUSER | GROUP_ADMIN | GROUP_OWNER | PRIVATE_FRIEND
 # file 填写求生服务器所在路径
 
 
 CONFIG_PATH = Path() / "data" / "L4D2" / "l4d2.yml"
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
@@ -104,16 +103,17 @@
 
 class L4d2ConfigManager:
     def __init__(self):
         self.file_path = CONFIG_PATH
         if self.file_path.exists():
             self.config = L4d2Config.parse_obj(
                 yaml.load(
-                    self.file_path.read_text(encoding="utf-8"), Loader=yaml.Loader
-                )
+                    self.file_path.read_text(encoding="utf-8"),
+                    Loader=yaml.Loader,
+                ),
             )
         else:
             self.config = L4d2Config()  # type: ignore
         self.save()
 
     def get_group_config(self, group_id: int) -> L4d2GroupConfig:
         if group_id not in self.config.group_config:
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 from .config import file_format, l4_config
 
 
 async def full_command(arg: Message = CommandArg()) -> bool:
     return not bool(str(arg))
 
 
-def FullCommand() -> Rule:
+def FullCommand() -> Rule:  # noqa: N802
     return Rule(full_command)
 
 
-def FullCommandDepend():
+def FullCommandDepend():  # noqa: N802
     return Depends(full_command)
 
 
 def wenjian(event: NoticeEvent):
     args = event.dict()
     try:
         name: str = args["file"]["name"]
         usr_id = str(args["user_id"])
     except KeyError:
         return False
     if args["notice_type"] == "offline_file":
         if l4_config.l4_master:
             return name.endswith(file_format) and usr_id in l4_config.l4_master
-        else:
-            return name.endswith(file_format)
-    elif args["notice_type"] == "group_upload":
+        return name.endswith(file_format)
+    if args["notice_type"] == "group_upload":
         if l4_config.l4_master:
             return usr_id in l4_config.l4_master and name.endswith(file_format)
-        else:
-            return False
+        return False
     return False
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 
 def anne_search(name: str):
     """输入名字返回列表["""
     url = "https://sb.trygek.com/l4d_stats/ranking/search.php"
     data = {"search": name}
     headers = {"Content-Type": "application/x-www-form-urlencoded"}
     data = httpx.post(url, data=data, headers=headers, timeout=60).content.decode(
-        "utf-8"
+        "utf-8",
     )
     soup = BeautifulSoup(data, "html.parser")
     # 获取标题
     title = []
     thead = soup.find("thead")
     if not thead:
-        return
+        return None
     for i in thead.find_all("td"):  # type: ignore
         tag = i.text.strip()
         title.append(tag)
     title.append("steamid")
     # 角色信息
     datas_table = soup.find("table")
     if not datas_table:
-        return
+        return None
     datas_tbody = datas_table.find("tbody")
     if not datas_tbody:
-        return
+        return None
     datas = datas_tbody.find_all("tr")  # type: ignore
     return [datas, title]
 
 
 def name_steamid_html(name):
     """您称通过网页来返回求生steamid"""
     data_title = anne_search(name)
     if not data_title:
-        return
+        return None
     data = data_title[0]
     for i in data:
         onclick: str = i["onclick"]
-        steamid = onclick.split("=")[2].strip("'")
-        return steamid
+        return onclick.split("=")[2].strip("'")
+    return None
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import base64
-import io
 from typing import Optional
 
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot_plugin_txt2img import Txt2Img
 
 from .config import l4_config
 
@@ -19,14 +18,15 @@
     ex_msg: Optional[str] = None,
 ):
     """文字转图片，如果有额外的信息则构造图文"""
     txt2img = Txt2Img()
     txt2img.set_font_size(font_size)
     pic = txt2img.draw(title, text)
     pic = base64.b64decode(pic)
-
+    if ex_text:
+        ...
     if not ex_msg:
         msg = MessageSegment.image(pic)
     else:
         msg = Message(MessageSegment.image(pic) + MessageSegment.text(ex_msg))
 
     return msg
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import json
-import os
 import tempfile
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
+import aiofiles
 import httpx
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 
 from ..l4d2_anne import anne_message, del_player, write_player
 from ..l4d2_image.steam import url_to_byte
 from ..l4d2_server.rcon import rcon_server, read_server_cfg_rcon
 from ..l4d2_server.workshop import workshop_to_dict
-from .config import *
-from .rule import *
+from .config import l4_config, systems
+
+# from .rule import
 from .txt_to_img import mode_txt_to_img
 
 
 async def get_file(url: str, down_file: Path):
     """
     下载指定Url到指定位置
     """
     try:
         if l4_config.l4_only:
             maps = await url_to_byte(url)
         else:
-            maps = httpx.get(url).content
+            maps = httpx.get(url).content  # noqa: ASYNC100
         logger.info("已获取文件，尝试新建文件并写入")
         if maps:
-            with open(down_file, "wb") as mfile:
-                mfile.write(maps)
+            async with aiofiles.open(down_file, "wb") as mfile:
+                await mfile.write(maps)
             logger.info("下载成功")
             return "文件已下载，正在解压"
     except Exception as e:
         logger.info(f"文件获取不到/已损坏:原因是{e}")
         return None
 
 
@@ -53,30 +54,30 @@
     return mes
 
 
 def del_map(num: int, map_path: Path) -> str:
     """
     删除指定的地图
     """
-    map = get_vpk(map_path)
-    map_name = map[num - 1]
+    map_ = get_vpk(map_path)
+    map_name = map_[num - 1]
     del_file = map_path / map_name
-    os.remove(del_file)
+    del_file.unlink()
     return map_name
 
 
 def rename_map(num: int, rename: str, map_path: Path) -> str:
     """
     改名指定的地图
     """
-    map = get_vpk(map_path)
-    map_name = map[num - 1]
+    map_ = get_vpk(map_path)
+    map_name = map_[num - 1]
     old_file = map_path / map_name
     new_file = map_path / rename
-    os.rename(old_file, new_file)
+    old_file.rename(new_file)
     logger.info("改名成功")
     return map_name
 
 
 def solve(msg: str):
     """删除str最后一行"""
     lines = msg.splitlines()
@@ -85,22 +86,22 @@
 
 
 async def search_anne(name: str, usr_id: str):
     """获取anne成绩"""
     return await anne_message(name, usr_id)
 
 
-async def bind_steam(id: str, msg: str, nickname: str):
+async def bind_steam(id_: str, msg: str, nickname: str):
     """绑定qq-steam"""
-    return await write_player(id, msg, nickname)
+    return await write_player(id_, msg, nickname)
 
 
-def name_exist(id: str):
+def name_exist(id_: str):
     """删除绑定信息"""
-    return del_player(id)
+    return del_player(id_)
 
 
 async def get_message_at(datas: str) -> List[int]:
     data: Dict[str, Any] = json.loads(datas)
     return [int(msg["data"]["qq"]) for msg in data["message"] if msg["type"] == "at"]
 
 
@@ -121,53 +122,52 @@
         msg = "无效指令：" + msg.replace("Unknown command", "").strip()
     return msg.strip().replace("\n", "")
 
 
 async def workshop_msg(msg: str):
     """url变成id，拼接post请求"""
     if msg.startswith("https://steamcommunity.com/sharedfiles/filedetails/?id"):
-        try:
+        if "&" in msg:
             msg = msg.split("&")[0]
-        except:
+        else:
             pass
         msg = msg.replace("https://steamcommunity.com/sharedfiles/filedetails/?id=", "")
     if msg.isdigit():
         data: Union[dict, List[dict]] = await workshop_to_dict(msg)
         return data
-    else:
-        return None
+    return None
 
 
 async def save_file(file: bytes, path_name):
     """保存文件"""
-    with open(path_name, "wb") as files:
-        files.write(file)
+    async with aiofiles.open(path_name, "wb") as files:
+        await files.write(file)
 
 
 async def upload_file(bot: Bot, event: MessageEvent, file_data: bytes, filename: str):
     """上传临时文件"""
-    if systems == "win" or "other":
+    if systems in ["win", "other"]:
         with tempfile.TemporaryDirectory() as temp_dir:
-            with open(Path(temp_dir) / filename, "wb") as f:
-                f.write(file_data)
+            async with aiofiles.open(Path(temp_dir) / filename, "wb") as f:
+                await f.write(file_data)
             if isinstance(event, GroupMessageEvent):
                 await bot.call_api(
                     "upload_group_file",
                     group_id=event.group_id,
                     file=f.name,
                     name=filename,
                 )
             else:
                 await bot.call_api(
                     "upload_private_file",
                     user_id=event.user_id,
                     file=f.name,
                     name=filename,
                 )
-        os.remove(Path().joinpath(filename))
+        (Path().joinpath(filename)).unlink()
     elif systems == "linux":
         with tempfile.NamedTemporaryFile("wb+") as f:
             f.write(file_data)
             if isinstance(event, GroupMessageEvent):
                 await bot.call_api(
                     "upload_group_file",
                     group_id=event.group_id,
@@ -196,15 +196,15 @@
     sub_menus.append(
         {
             "func": func,
             "trigger_method": trigger_method,
             "trigger_condition": trigger_condition,
             "brief_des": brief_des,
             "detail_des": detail_des or brief_des,
-        }
+        },
     )
 
 
 def register_menu(*args, **kwargs):
     def decorator(f):
         register_menu_func(*args, **kwargs)
         return f
@@ -246,9 +246,8 @@
         msgs: List[str] = msg.split(":")
     elif "：" in msg:
         msgs: List[str] = msg.split("：")
     elif msg.replace(".", "").isdigit():
         msgs: List[str] = [msg, "20715"]
     else:
         msgs = []
-    mse = [msgs[0], msgs[-1]]
-    return mse
+    return [msgs[0], msgs[-1]]
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,60 +6,71 @@
 from fastapi.responses import HTMLResponse, JSONResponse, RedirectResponse
 from jose import jwt
 from jose.exceptions import ExpiredSignatureError, JWTError
 from nonebot import get_adapter, get_app, get_driver, logger
 from nonebot.adapters.onebot.v11 import Adapter
 
 from ..l4d2_queries.qqgroup import qq_ip_querie
-from ..l4d2_utils.config import *
+from ..l4d2_utils.config import UserModel, config_manager
 from ..l4d2_utils.utils import split_maohao
+from .webUI import admin_app, login_page
+from .webUI_s import user_app
 
 CONFIG_PATH = Path() / "data" / "L4D2" / "l4d2.yml"
 
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
 driver = get_driver()
 
-from .webUI import admin_app, login_page
-from .webUI_s import user_app
 
 requestAdaptor = """
 requestAdaptor(api) {
     api.headers["token"] = localStorage.getItem("token");
     return api;
 },
-"""
+"""  # noqa: N816
 responseAdaptor = """
 responseAdaptor(api, payload, query, request, response) {
     if (response.data.detail == '登录验证失败或已失效，请重新登录') {
         window.location.href = '/l4d2/login'
         window.localStorage.clear()
         window.sessionStorage.clear()
         window.alert('登录验证失败或已失效，请重新登录')
     }
     return payload
 },
-"""
+"""  # noqa: N816
 
 
 def authentication():
     def inner(token: Optional[str] = Header(...)):
         try:
             if not token:
-                raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
+                raise HTTPException(
+                    status_code=400,
+                    detail="登录验证失败或已失效，请重新登录",
+                )  # noqa: E501
             payload = jwt.decode(
-                token, config_manager.config.web_secret_key, algorithms="HS256"
+                token,
+                config_manager.config.web_secret_key,
+                algorithms="HS256",
             )
             if (
                 not (username := payload.get("username"))
                 or username != config_manager.config.web_username
             ):
-                raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
+                raise HTTPException(
+                    status_code=400,
+                    detail="登录验证失败或已失效，请重新登录",
+                )  # noqa: E501
         except (JWTError, ExpiredSignatureError, AttributeError):
-            raise HTTPException(status_code=400, detail="登录验证失败或已失效，请重新登录")
+            raise HTTPException(  # noqa: B904, TRY200
+                status_code=400,
+                detail="登录验证失败或已失效，请重新登录",
+            )
 
     return Depends(inner)
 
 
 COMMAND_START = driver.config.command_start.copy()
 if "" in COMMAND_START:
     COMMAND_START.remove("")
@@ -96,24 +107,25 @@
         dependencies=[authentication()],
     )
     async def get_group_list_api():
         try:
             bots = get_adapter(Adapter).bots
             if len(bots) == 0:
                 return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
-            bot = list(bots.values())[0]
+            bot = next(iter(bots.values()))
             group_list = await bot.get_group_list()
             group_list = [
                 {
                     "label": f'{group["group_name"]}({group["group_id"]})',
                     "value": group["group_id"],
                 }
                 for group in group_list
             ]
-            return {"status": 0, "msg": "ok", "data": {"group_list": group_list}}
+            if True:
+                return {"status": 0, "msg": "ok", "data": {"group_list": group_list}}
         except ValueError:
             return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
 
     @app.post(
         "/l4d2/api/l4d2_global_config",
         response_class=JSONResponse,
         dependencies=[authentication()],
@@ -129,33 +141,33 @@
         dependencies=[authentication()],
     )
     async def get_l4d2_global_config():
         try:
             bots = get_adapter(Adapter).bots
             if len(bots) == 0:
                 return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
-            bot = list(bots.values())[0]
+            bot = next(iter(bots.values()))
             groups = await bot.get_group_list()
             member_list = []
             for group in groups:
                 members = await bot.get_group_member_list(group_id=group["group_id"])
                 member_list.extend(
                     [
                         {
-                            "label": f'{member["nickname"] or member["card"]}({member["user_id"]})',
+                            "label": f'{member["nickname"] or member["card"]}({member["user_id"]})',  # noqa: E501
                             "value": member["user_id"],
                         }
                         for member in members
-                    ]
+                    ],
                 )
             config = config_manager.config.dict(exclude={"group_config"})
             config["member_list"] = member_list
             config["l4_styles"] = ["standard", "black"]
-
-            return config
+            if True:
+                return config
         except ValueError:
             return {"status": -100, "msg": "获取群和好友列表失败，请确认已连接GOCQ"}
 
     @app.get("/l4d2/api/user/get_query_contexts", response_class=JSONResponse)
     @app.get(
         "/l4d2/api/get_query_contexts",
         response_class=JSONResponse,
@@ -191,37 +203,44 @@
         "/l4d2/api/get_l4d2_messages",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_l4d2_messages():
         try:
             l4_ipall = config_manager.config.l4_ipall
-            config = [
-                {"label": item["server_id"], "value": item["id_rank"]}
-                for item in l4_ipall
-            ]
-            return {"status": 0, "msg": "ok", "data": {"server_list": config}}
+
+            return {
+                "status": 0,
+                "msg": "ok",
+                "data": {
+                    "server_list": [
+                        {"label": item["server_id"], "value": item["id_rank"]}
+                        for item in l4_ipall
+                    ],
+                },
+            }
         except ValueError:
             return {"status": -100, "msg": "返回失败，请确保网络连接正常"}
 
     @app.get(
         "/l4d2/api/l4d2_server_config",
         response_class=JSONResponse,
         dependencies=[authentication()],
     )
     async def get_l4d2_server_config(id_rank: str):
         try:
             l4_ipall = config_manager.config.l4_ipall
             config = {}
             for item in l4_ipall:
                 if item["id_rank"] == id_rank:
-                    item["place"] = item["place"] == "True" or item["place"] == True
+                    item["place"] = item["place"] is True or item["place"] is True
                     config = item
                     break
-            return {"status": 0, "msg": "ok", "data": config}
+            if True:
+                return {"status": 0, "msg": "ok", "data": config}
         except ValueError:
             return {"status": -100, "msg": "返回失败，请确保网络连接正常"}
 
     @app.post(
         "/l4d2/api/l4d2_server_config",
         response_class=JSONResponse,
         dependencies=[authentication()],
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 <h1 align="center">Nonebot-Plugin-L4d2-Server 控制台</h1>
 <div align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/" target="_blank">
     Github仓库</a>
 </div>
 <br>
 <br>
-"""
+""",
 )
 login_api = AmisAPI(
     url="/l4d2/api/login",
     method="post",
     adaptor="""
         if (payload.status == 0) {
             localStorage.setItem("token", payload.data.token);
@@ -85,110 +85,137 @@
     body=[
         Switch(
             label="控制总开关（摆设）",
             name="total_enable",
             value="${total_enable}",
             onText="开启",
             offText="关闭",
-            labelRemark=Remark(shape="circle", content="关闭后，禁用网页控制台，请参考文档启动方法"),
+            labelRemark=Remark(
+                shape="circle",
+                content="关闭后，禁用网页控制台，请参考文档启动方法",
+            ),  # noqa: E501
         ),
         InputText(
             label="后台管理用户名",
             name="web_username",
             value="${web_username}",
-            labelRemark=Remark(shape="circle", content="登录本后台管理所需要的用户名。"),
+            labelRemark=Remark(shape="circle", content="登录本后台管理所需要的用户名。"),  # noqa: E501
         ),
         InputPassword(
             label="后台管理密码",
             name="web_password",
             value="${web_password}",
             labelRemark=Remark(shape="circle", content="登录本后台管理所需要的密码。"),
         ),
         InputText(
             label="后台管理token密钥",
             name="web_secret_key",
             value="${web_secret_key}",
-            labelRemark=Remark(shape="circle", content="用于本后台管理加密验证token的密钥。"),
+            labelRemark=Remark(
+                shape="circle",
+                content="用于本后台管理加密验证token的密钥。",
+            ),  # noqa: E501
         ),
         InputText(
             label="字体",
             name="l4_font",
             value="${l4_font}",
-            labelRemark=Remark(shape="circle", content="机器人返回图片中文字的字体。"),
+            labelRemark=Remark(shape="circle", content="机器人返回图片中文字的字体。"),  # noqa: E501
         ),
         Switch(
             label="是否图片发送单服务器查询",
             name="l4_image",
             value="${l4_image}",
             onText="开启",
             offText="关闭",
-            labelRemark=Remark(shape="circle", content="开启时，会查询单服务器会使用图片，避免长信息风控"),
+            labelRemark=Remark(
+                shape="circle",
+                content="开启时，会查询单服务器会使用图片，避免长信息风控",  # noqa: E501
+            ),  # noqa: E501
         ),
         Select(
             label="图片风格",
             name="l4_style",
             value="${l4_style}",
             source="${l4_styles}",
             labelRemark=Remark(shape="circle", content="仅仅是批量查询的风格"),
         ),
         Switch(
             label="是否优先上传地图",
             name="l4_only",
             value="${l4_only}",
             onText="开启",
             offText="关闭",
-            labelRemark=Remark(shape="circle", content="开启时，上传地图会保证优先级，从而阻碍其他指令"),
+            labelRemark=Remark(
+                shape="circle",
+                content="开启时，上传地图会保证优先级，从而阻碍其他指令",
+            ),  # noqa: E501
         ),
         Switch(
             label="是否显示connect",
             name="l4_connect",
             value="${l4_connect}",
             onText="开启",
             offText="关闭",
-            labelRemark=Remark(shape="circle", content="关闭后，查询服务器将不再显示connect和ip地址"),
+            labelRemark=Remark(
+                shape="circle",
+                content="关闭后，查询服务器将不再显示connect和ip地址",
+            ),  # noqa: E501
         ),
         InputNumber(
             label="定时推送间隔（min）",
             name="l4_push_interval",
             value="${l4_push_interval}",
-            labelRemark=Remark(shape="circle", content="设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次"),
+            labelRemark=Remark(
+                shape="circle",
+                content="设置好后，使用推送服务器定时指令，将以x分钟为间隔推送一次",  # noqa: E501
+            ),
         ),
         InputNumber(
             label="定时推次数",
             name="l4_push_times",
             value="${l4_push_times}",
-            labelRemark=Remark(shape="circle", content="设置好后，将按照推送间隔时间推送x此"),
+            labelRemark=Remark(
+                shape="circle",
+                content="设置好后，将按照推送间隔时间推送x此",
+            ),  # noqa: E501
         ),
         InputNumber(
             label="当前路径序号",
             name="l4_number",
             value="${l4_number}",
-            labelRemark=Remark(shape="circle", content="如果选定了路径，则上传地图优先传这个路径"),
+            labelRemark=Remark(
+                shape="circle",
+                content="如果选定了路径，则上传地图优先传这个路径",
+            ),  # noqa: E501
         ),
         InputTag(
             label="求生上传地图用户",
             name="l4_master",
             value="${l4_master}",
             enableBatchAdd=True,
             placeholder="添加qq号",
             visibleOn="${total_enable}",
             joinValues=False,
             extractValue=True,
-            labelRemark=Remark(shape="circle", content="在这里加入的用户，才能上传地图"),
+            labelRemark=Remark(shape="circle", content="在这里加入的用户，才能上传地图"),  # noqa: E501
         ),
         InputTag(
             label="坐牢三指令tag",
             name="l4_zl_tag",
             value="${l4_zl_tag}",
             enableBatchAdd=True,
             placeholder="添加qq号",
             visibleOn="${total_enable}",
             joinValues=False,
             extractValue=True,
-            labelRemark=Remark(shape="circle", content="在这里的指令，可以响应坐牢三指令"),
+            labelRemark=Remark(
+                shape="circle",
+                content="在这里的指令，可以响应坐牢三指令",  # noqa: E501
+            ),
         ),
     ],
     actions=[
         Action(label="保存", level=LevelEnum.success, type="submit"),
         Action(label="重置", level=LevelEnum.warning, type="reset"),
     ],
 )
@@ -210,15 +237,18 @@
             value="${web_password}",
             labelRemark=Remark(shape="circle", content="登录本后台管理所需要的密码。"),
         ),
         InputText(
             label="后台管理token密钥",
             name="web_secret_key",
             value="${web_secret_key}",
-            labelRemark=Remark(shape="circle", content="用于本后台管理加密验证token的密钥。"),
+            labelRemark=Remark(
+                shape="circle",
+                content="用于本后台管理加密验证token的密钥。",
+            ),  # noqa: E501
         ),
         InputText(
             label="查询key",
             name="l4_key",
             value="${l4_key}",
             labelRemark=Remark(shape="circle", content="用于获取拓展功能的key。"),
         ),
@@ -227,29 +257,32 @@
         Action(label="保存", level=LevelEnum.success, type="submit"),
         Action(label="重置", level=LevelEnum.warning, type="reset"),
     ],
 )
 
 
 group_select = Select(
-    label="分群配置（暂未完成）", name="group_id", source="${group_list}", placeholder="选择群"
+    label="分群配置（暂未完成）",
+    name="group_id",
+    source="${group_list}",
+    placeholder="选择群",  # noqa: E501
 )
 group_config_form = Form(
     title="分群配置（暂未完成）",
     visibleOn="group_id != null",
     initApi="/l4d2/api/l4d2_group_config?group_id=${group_id}",
     api="post:/l4d2/api/l4d2_group_config?group_id=${group_id}",
     body=[
         Switch(
             label="分群开关",
             name="enable",
             value="${enable}",
             onText="开启",
             offText="关闭",
-            labelRemark=Remark(shape="circle", content="针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。"),
+            labelRemark=Remark(shape="circle", content=""),
         ),
         InputNumber(
             label="占位符",
             name="answer_threshold",
             value="${answer_threshold}",
             visibleOn="${enable}",
             min=2,
@@ -276,15 +309,18 @@
             api="post:/l4d2/api/l4d2_group_config?group_id=all",
         ),
         Action(label="重置", level=LevelEnum.warning, type="reset"),
     ],
 )
 
 server_control = Select(
-    label="服务器设置", name="id_rank", source="${server_list}", placeholder="选择服务器"
+    label="服务器设置",
+    name="id_rank",
+    source="${server_list}",
+    placeholder="选择服务器",  # noqa: E501
 )
 
 server_ditail = Form(
     title="",
     api="post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}",
     initApi="/l4d2/api/l4d2_server_config?id_rank=${id_rank}",
     visibleOn="id_rank != null",
@@ -321,15 +357,18 @@
             value="${rcon}",
             labelRemark=Remark(shape="circle", content="服务端rcon密码"),
         ),
         InputText(
             label="服务器本地文件位置",
             name="location",
             value="${location}",
-            labelRemark=Remark(shape="circle", content="求生服务器所在路径,该路径下有文件srcds_run"),
+            labelRemark=Remark(
+                shape="circle",
+                content="求生服务器所在路径,该路径下有文件srcds_run",
+            ),  # noqa: E501
         ),
         InputText(
             label="远程账户",
             name="account",
             value="${account}",
             visibleOn="${place}",
             labelRemark=Remark(shape="circle", content="远程服务器的登录账户名"),
@@ -354,16 +393,16 @@
     syncLocation=False,
     api="/l4d2/api/get_query_contexts",
     interval=60000,
     itemActions=[
         ActionType.Url(
             tooltip="加入游戏",
             icon="fa fa-gamepad",
-            confirmText="加入steam://connect/" + "${ip}",
-            url="steam://connect/" + "${ip}",
+            confirmText="加入steam://connect/" + "${ip}",  # noqa: ISC003
+            url="steam://connect/" + "${ip}",  # noqa: ISC003
             # url= "http://"+'${ip}',
             blank=True,
         ),
     ],
     columns=[
         TableColumn(label="服主", name="tag", searchable=True),
         TableColumn(label="序号", name="number", searchable=True),
@@ -383,15 +422,15 @@
         title="本地服务器管理",
         interval=120000,
         initApi="/l4d2/api/get_l4d2_messages",
         body=[
             Alert(
                 level=LevelEnum.info,
                 className="white-space-pre-wrap",
-                body=(f"此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n" f"· 功能暂未完善"),
+                body=(f"此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n· 功能暂未完善"),  # noqa: E501
             ),
             server_control,
             server_ditail,
         ],
     ),
 )
 query_page = PageSchema(
@@ -413,40 +452,47 @@
             ),
             query_table,
         ],
     ),
 )
 
 database_page = PageSchema(
-    label="数据库", icon="fa fa-database", children=[server_page, query_page]
+    label="数据库",
+    icon="fa fa-database",
+    children=[server_page, query_page],
 )  # type: ignore
 
 config_page = PageSchema(
     url="/configs",
     isDefaultPage=True,
     icon="fa fa-wrench",
     label="配置",
     schema=Page(
         title="配置",
         initApi="/l4d2/api/get_group_list",
         body=[global_config_form, group_select, group_config_form],
     ),
 )
 l4d2_page = PageSchema(
-    label="求生之路", icon="fa fa-wechat (alias)", children=[config_page, database_page]
+    label="求生之路",
+    icon="fa fa-wechat (alias)",
+    children=[config_page, database_page],
 )  # type: ignore
 
 github_logo = Tpl(
     className="w-full",
-    tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>',
+    tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>',  # noqa: E501
 )
 header = Flex(
-    className="w-full", justify="flex-end", alignItems="flex-end", items=[github_logo]
+    className="w-full",
+    justify="flex-end",
+    alignItems="flex-end",
+    items=[github_logo],
 )
 
 admin_app = App(
     brandName="L4d2-Server",
     logo="https://ghproxy.com/https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png",
     header=header,
     pages=[{"children": [config_page, database_page]}],
-    footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>',
+    footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>',  # noqa: E501
 )
```

#### html2text {}

```diff
@@ -3,163 +3,167 @@
 LevelEnum, Page, PageSchema, Remark, Select, Switch, TableColumn, TableCRUD,
 Tpl, Wrapper, ) from ..l4d2_utils.config import NICKNAME logo = Html( html="""
                                  [l4d2-server]
               ****** Nonebot-Plugin-L4d2-Server æ§å¶å° ******
                                  Githubä»åº
 
 
-""" ) login_api = AmisAPI( url="/l4d2/api/login", method="post", adaptor=""" if
-(payload.status == 0) { localStorage.setItem("token", payload.data.token); }
+""", ) login_api = AmisAPI( url="/l4d2/api/login", method="post", adaptor="""
+if (payload.status == 0) { localStorage.setItem("token", payload.data.token); }
 return payload; """, ) login_form = Form( api=login_api, title="", body=
 [ InputText( name="username", label="ç¨æ·å", labelRemark=Remark
 (shape="circle", content="åå°ç®¡çç¨æ·åï¼é»è®¤ä¸ºl4d2"), ),
 InputPassword( name="password", label="å¯ç ", labelRemark=Remark
 (shape="circle", content="åå°ç®¡çå¯ç ï¼é»è®¤ä¸ºadmin"), ), ],
 mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9,
 offset=5), redirect="/l4d2/admin", ) body = Wrapper(className="w-2/5 mx-auto
 my-0 m:w-full", body=login_form) login_page = Page(title="", body=[logo, body])
 global_config_form = Form( title="å¨å±éç½®", name="global_config",
 initApi="/l4d2/api/l4d2_global_config", api="post:/l4d2/api/
 l4d2_global_config", body=[ Switch( label="æ§å¶æ»å¼å³ï¼æè®¾ï¼",
 name="total_enable", value="${total_enable}", onText="å¼å¯",
-offText="å³é­", labelRemark=Remark(shape="circle",
-content="å³é­åï¼ç¦ç¨ç½é¡µæ§å¶å°ï¼è¯·åèææ¡£å¯å¨æ¹æ³"), ),
-InputText( label="åå°ç®¡çç¨æ·å", name="web_username", value="$
-{web_username}", labelRemark=Remark(shape="circle",
-content="ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã"), ), InputPassword
-( label="åå°ç®¡çå¯ç ", name="web_password", value="${web_password}",
-labelRemark=Remark(shape="circle",
+offText="å³é­", labelRemark=Remark( shape="circle",
+content="å³é­åï¼ç¦ç¨ç½é¡µæ§å¶å°ï¼è¯·åèææ¡£å¯å¨æ¹æ³", ), #
+noqa: E501 ), InputText( label="åå°ç®¡çç¨æ·å", name="web_username",
+value="${web_username}", labelRemark=Remark(shape="circle",
+content="ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã"), # noqa: E501 ),
+InputPassword( label="åå°ç®¡çå¯ç ", name="web_password", value="$
+{web_password}", labelRemark=Remark(shape="circle",
 content="ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã"), ), InputText
 ( label="åå°ç®¡çtokenå¯é¥", name="web_secret_key", value="$
-{web_secret_key}", labelRemark=Remark(shape="circle",
-content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã"), ), InputText
-( label="å­ä½", name="l4_font", value="${l4_font}", labelRemark=Remark
-(shape="circle", content="æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã"), ),
-Switch( label="æ¯å¦å¾çåéåæå¡å¨æ¥è¯¢", name="l4_image", value="$
+{web_secret_key}", labelRemark=Remark( shape="circle",
+content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã", ), # noqa: E501
+), InputText( label="å­ä½", name="l4_font", value="${l4_font}",
+labelRemark=Remark(shape="circle",
+content="æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã"), # noqa: E501 ), Switch
+( label="æ¯å¦å¾çåéåæå¡å¨æ¥è¯¢", name="l4_image", value="$
 {l4_image}", onText="å¼å¯", offText="å³é­", labelRemark=Remark
-(shape="circle",
-content="å¼å¯æ¶ï¼ä¼æ¥è¯¢åæå¡å¨ä¼ä½¿ç¨å¾çï¼é¿åé¿ä¿¡æ¯é£æ§"),
-), Select( label="å¾çé£æ ¼", name="l4_style", value="${l4_style}",
-source="${l4_styles}", labelRemark=Remark(shape="circle",
+( shape="circle",
+content="å¼å¯æ¶ï¼ä¼æ¥è¯¢åæå¡å¨ä¼ä½¿ç¨å¾çï¼é¿åé¿ä¿¡æ¯é£æ§",
+# noqa: E501 ), # noqa: E501 ), Select( label="å¾çé£æ ¼", name="l4_style",
+value="${l4_style}", source="${l4_styles}", labelRemark=Remark(shape="circle",
 content="ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼"), ), Switch
 ( label="æ¯å¦ä¼åä¸ä¼ å°å¾", name="l4_only", value="${l4_only}",
-onText="å¼å¯", offText="å³é­", labelRemark=Remark(shape="circle",
-content="å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤"),
-), Switch( label="æ¯å¦æ¾ç¤ºconnect", name="l4_connect", value="$
-{l4_connect}", onText="å¼å¯", offText="å³é­", labelRemark=Remark
-(shape="circle",
-content="å³é­åï¼æ¥è¯¢æå¡å¨å°ä¸åæ¾ç¤ºconnectåipå°å"), ),
-InputNumber( label="å®æ¶æ¨éé´éï¼minï¼", name="l4_push_interval",
-value="${l4_push_interval}", labelRemark=Remark(shape="circle",
-content="è®¾ç½®å¥½åï¼ä½¿ç¨æ¨éæå¡å¨å®æ¶æä»¤ï¼å°ä»¥xåéä¸ºé´éæ¨éä¸æ¬¡"),
-), InputNumber( label="å®æ¶æ¨æ¬¡æ°", name="l4_push_times", value="$
-{l4_push_times}", labelRemark=Remark(shape="circle",
-content="è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤"), ), InputNumber
-( label="å½åè·¯å¾åºå·", name="l4_number", value="${l4_number}",
+onText="å¼å¯", offText="å³é­", labelRemark=Remark( shape="circle",
+content="å¼å¯æ¶ï¼ä¸ä¼ å°å¾ä¼ä¿è¯ä¼åçº§ï¼ä»èé»ç¢å¶ä»æä»¤",
+), # noqa: E501 ), Switch( label="æ¯å¦æ¾ç¤ºconnect", name="l4_connect",
+value="${l4_connect}", onText="å¼å¯", offText="å³é­", labelRemark=Remark
+( shape="circle",
+content="å³é­åï¼æ¥è¯¢æå¡å¨å°ä¸åæ¾ç¤ºconnectåipå°å", ), #
+noqa: E501 ), InputNumber( label="å®æ¶æ¨éé´éï¼minï¼",
+name="l4_push_interval", value="${l4_push_interval}", labelRemark=Remark
+( shape="circle",
+content="è®¾ç½®å¥½åï¼ä½¿ç¨æ¨éæå¡å¨å®æ¶æä»¤ï¼å°ä»¥xåéä¸ºé´éæ¨éä¸æ¬¡",
+# noqa: E501 ), ), InputNumber( label="å®æ¶æ¨æ¬¡æ°", name="l4_push_times",
+value="${l4_push_times}", labelRemark=Remark( shape="circle",
+content="è®¾ç½®å¥½åï¼å°æç§æ¨éé´éæ¶é´æ¨éxæ­¤", ), # noqa: E501
+), InputNumber( label="å½åè·¯å¾åºå·", name="l4_number", value="$
+{l4_number}", labelRemark=Remark( shape="circle",
+content="å¦æéå®äºè·¯å¾ï¼åä¸ä¼ å°å¾ä¼åä¼ è¿ä¸ªè·¯å¾", ), #
+noqa: E501 ), InputTag( label="æ±çä¸ä¼ å°å¾ç¨æ·", name="l4_master",
+value="${l4_master}", enableBatchAdd=True, placeholder="æ·»å qqå·",
+visibleOn="${total_enable}", joinValues=False, extractValue=True,
 labelRemark=Remark(shape="circle",
-content="å¦æéå®äºè·¯å¾ï¼åä¸ä¼ å°å¾ä¼åä¼ è¿ä¸ªè·¯å¾"), ),
-InputTag( label="æ±çä¸ä¼ å°å¾ç¨æ·", name="l4_master", value="$
-{l4_master}", enableBatchAdd=True, placeholder="æ·»å qqå·", visibleOn="$
-{total_enable}", joinValues=False, extractValue=True, labelRemark=Remark
-(shape="circle", content="å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾"), ),
+content="å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾"), # noqa: E501 ),
 InputTag( label="åç¢ä¸æä»¤tag", name="l4_zl_tag", value="${l4_zl_tag}",
 enableBatchAdd=True, placeholder="æ·»å qqå·", visibleOn="${total_enable}",
-joinValues=False, extractValue=True, labelRemark=Remark(shape="circle",
-content="å¨è¿éçæä»¤ï¼å¯ä»¥ååºåç¢ä¸æä»¤"), ), ], actions=
-[ Action(label="ä¿å­", level=LevelEnum.success, type="submit"), Action
-(label="éç½®", level=LevelEnum.warning, type="reset"), ], ) upload_map_form =
-Form( title="å¨å±éç½®", name="global_config", api="post:/l4d2/api/
-l4d2_map_config", body=[ InputText( label="æå¡å¨host", name="web_username",
-value="${web_username}", labelRemark=Remark(shape="circle",
-content="127.0.0.1"), ), InputPassword( label="æå¡å¨", name="web_password",
-value="${web_password}", labelRemark=Remark(shape="circle",
-content="ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã"), ), InputText
-( label="åå°ç®¡çtokenå¯é¥", name="web_secret_key", value="$
-{web_secret_key}", labelRemark=Remark(shape="circle",
-content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã"), ), InputText
-( label="æ¥è¯¢key", name="l4_key", value="${l4_key}", labelRemark=Remark
-(shape="circle", content="ç¨äºè·åæå±åè½çkeyã"), ), ], actions=
-[ Action(label="ä¿å­", level=LevelEnum.success, type="submit"), Action
+joinValues=False, extractValue=True, labelRemark=Remark( shape="circle",
+content="å¨è¿éçæä»¤ï¼å¯ä»¥ååºåç¢ä¸æä»¤", # noqa: E501 ), ),
+], actions=[ Action(label="ä¿å­", level=LevelEnum.success, type="submit"),
+Action(label="éç½®", level=LevelEnum.warning, type="reset"), ], )
+upload_map_form = Form( title="å¨å±éç½®", name="global_config", api="post:/
+l4d2/api/l4d2_map_config", body=[ InputText( label="æå¡å¨host",
+name="web_username", value="${web_username}", labelRemark=Remark
+(shape="circle", content="127.0.0.1"), ), InputPassword( label="æå¡å¨",
+name="web_password", value="${web_password}", labelRemark=Remark
+(shape="circle", content="ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã"), ),
+InputText( label="åå°ç®¡çtokenå¯é¥", name="web_secret_key", value="$
+{web_secret_key}", labelRemark=Remark( shape="circle",
+content="ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã", ), # noqa: E501
+), InputText( label="æ¥è¯¢key", name="l4_key", value="${l4_key}",
+labelRemark=Remark(shape="circle",
+content="ç¨äºè·åæå±åè½çkeyã"), ), ], actions=[ Action
+(label="ä¿å­", level=LevelEnum.success, type="submit"), Action
 (label="éç½®", level=LevelEnum.warning, type="reset"), ], ) group_select =
 Select( label="åç¾¤éç½®ï¼ææªå®æï¼", name="group_id", source="$
-{group_list}", placeholder="éæ©ç¾¤" ) group_config_form = Form
+{group_list}", placeholder="éæ©ç¾¤", # noqa: E501 ) group_config_form = Form
 ( title="åç¾¤éç½®ï¼ææªå®æï¼", visibleOn="group_id != null",
 initApi="/l4d2/api/l4d2_group_config?group_id=${group_id}", api="post:/l4d2/
 api/l4d2_group_config?group_id=${group_id}", body=[ Switch
 ( label="åç¾¤å¼å³", name="enable", value="${enable}", onText="å¼å¯",
-offText="å³é­", labelRemark=Remark(shape="circle",
-content="éå¯¹è¯¥ç¾¤çç¾¤èå­¦ä¹ å¼å³ï¼å³é­åï¼ä»è¯¥ç¾¤ä¸ä¼å­¦ä¹ ååå¤ã"),
-), InputNumber( label="å ä½ç¬¦", name="answer_threshold", value="$
+offText="å³é­", labelRemark=Remark(shape="circle", content=""), ),
+InputNumber( label="å ä½ç¬¦", name="answer_threshold", value="$
 {answer_threshold}", visibleOn="${enable}", min=2, labelRemark=Remark
 (shape="circle", content="åææ¬"), ), InputTag( label="å ä½ç¬¦",
 name="ban_words", value="${ban_words}", enableBatchAdd=True,
 placeholder="å ä½ç¬¦ï¼è¯æ¡", visibleOn="${enable}", joinValues=False,
 extractValue=True, labelRemark=Remark(shape="circle",
 content="å ä½ç¬¦è¯æ¡"), ), ], actions=[ Action(label="ä¿å­",
 level=LevelEnum.success, type="submit"), ActionType.Ajax
 ( label="ä¿å­è³ææç¾¤", level=LevelEnum.primary,
 confirmText="ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼", api="post:/l4d2/api/
 l4d2_group_config?group_id=all", ), Action(label="éç½®",
 level=LevelEnum.warning, type="reset"), ], ) server_control = Select
 ( label="æå¡å¨è®¾ç½®", name="id_rank", source="${server_list}",
-placeholder="éæ©æå¡å¨" ) server_ditail = Form( title="", api="post:/
-l4d2/api/l4d2_server_config?id_rank=${id_rank}", initApi="/l4d2/api/
+placeholder="éæ©æå¡å¨", # noqa: E501 ) server_ditail = Form( title="",
+api="post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}", initApi="/l4d2/api/
 l4d2_server_config?id_rank=${id_rank}", visibleOn="id_rank != null", body=
 [ Switch( label="æ¯å¦æ¯è¿ç¨æå¡å¨", name="place", value="${place}",
 onText="æ¯ç", offText="ä¸æ¯", labelRemark=Remark(shape="circle",
 content="å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨"), ), InputText
 ( label="æå¡å¨åç§°", name="server_id", value="${server_id}",
 labelRemark=Remark(shape="circle", content="æå¡å¨åå­"), ), InputText
 ( label="æå¡å¨ipå°å", name="host", value="${host}", labelRemark=Remark
 (shape="circle", content="æå¡ç«¯æå¨ipå°å,ä¹å¯ä»¥æ¯åå"), ),
 InputText( label="æå¨ç«¯å£", name="port", value="${port}",
 labelRemark=Remark(shape="circle", content="æå¡ç«¯æå¨ç«¯å£"), ),
 InputPassword( label="rconæ§å¶å°å¯ç ", name="rcon", value="${rcon}",
 labelRemark=Remark(shape="circle", content="æå¡ç«¯rconå¯ç "), ), InputText
 ( label="æå¡å¨æ¬å°æä»¶ä½ç½®", name="location", value="${location}",
-labelRemark=Remark(shape="circle",
-content="æ±çæå¡å¨æå¨è·¯å¾,è¯¥è·¯å¾ä¸ææä»¶srcds_run"), ),
-InputText( label="è¿ç¨è´¦æ·", name="account", value="${account}",
-visibleOn="${place}", labelRemark=Remark(shape="circle",
+labelRemark=Remark( shape="circle",
+content="æ±çæå¡å¨æå¨è·¯å¾,è¯¥è·¯å¾ä¸ææä»¶srcds_run", ), #
+noqa: E501 ), InputText( label="è¿ç¨è´¦æ·", name="account", value="$
+{account}", visibleOn="${place}", labelRemark=Remark(shape="circle",
 content="è¿ç¨æå¡å¨çç»å½è´¦æ·å"), ), InputPassword
 ( label="è¿ç¨å¯ç ", name="password", value="${password}", visibleOn="$
 {place}", labelRemark=Remark(shape="circle",
 content="è¿ç¨æå¡å¨çç»å½å¯ç "), ), ], actions=[ Action
 (label="ä¿å­", level=LevelEnum.success, type="submit"), Action
 (label="éç½®", level=LevelEnum.warning, type="reset"), ], ) query_table =
 TableCRUD( mode="table", title="", syncLocation=False, api="/l4d2/api/
 get_query_contexts", interval=60000, itemActions=[ ActionType.Url
 ( tooltip="å å¥æ¸¸æ", icon="fa fa-gamepad", confirmText="å å¥steam://
-connect/" + "${ip}", url="steam://connect/" + "${ip}", # url= "http://"+'$
-{ip}', blank=True, ), ], columns=[ TableColumn(label="æä¸»", name="tag",
-searchable=True), TableColumn(label="åºå·", name="number", searchable=True),
-TableColumn(label="åç§°", name="name", searchable=True), TableColumn
-(label="å°å¾", name="map_", searchable=True), TableColumn(label="ç©å®¶",
-name="rank_players", searchable=True), TableColumn(label="å»¶è¿", name="ping",
-searchable=True), TableColumn(label="IP å°å", name="ip", searchable=True),
-], ) server_page = PageSchema( url="/messages", icon="fa fa-comment",
-label="æ¬å°æå¡å¨ç®¡ç", schema=Page( title="æ¬å°æå¡å¨ç®¡ç",
-interval=120000, initApi="/l4d2/api/get_l4d2_messages", body=[ Alert
-( level=LevelEnum.info, className="white-space-pre-wrap", body=
-(f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n"
-f"Â· åè½ææªå®å"), ), server_control, server_ditail, ], ), ) query_page
-= PageSchema( url="/contexts", icon="fa fa-comments",
-label="è¿ç¨æå¡å¨æ¥è¯¢", schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢",
-body=[ Alert( level=LevelEnum.info, className="white-space-pre-wrap", body=
-( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
+connect/" + "${ip}", # noqa: ISC003 url="steam://connect/" + "${ip}", # noqa:
+ISC003 # url= "http://"+'${ip}', blank=True, ), ], columns=[ TableColumn
+(label="æä¸»", name="tag", searchable=True), TableColumn(label="åºå·",
+name="number", searchable=True), TableColumn(label="åç§°", name="name",
+searchable=True), TableColumn(label="å°å¾", name="map_", searchable=True),
+TableColumn(label="ç©å®¶", name="rank_players", searchable=True), TableColumn
+(label="å»¶è¿", name="ping", searchable=True), TableColumn(label="IP å°å",
+name="ip", searchable=True), ], ) server_page = PageSchema( url="/messages",
+icon="fa fa-comment", label="æ¬å°æå¡å¨ç®¡ç", schema=Page
+( title="æ¬å°æå¡å¨ç®¡ç", interval=120000, initApi="/l4d2/api/
+get_l4d2_messages", body=[ Alert( level=LevelEnum.info, className="white-space-
+pre-wrap", body=(f"æ­¤æ°æ®åºè®°å½äº
+{NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\nÂ· åè½ææªå®å"), #
+noqa: E501 ), server_control, server_ditail, ], ), ) query_page = PageSchema
+( url="/contexts", icon="fa fa-comments", label="è¿ç¨æå¡å¨æ¥è¯¢",
+schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢", body=[ Alert( level=LevelEnum.info,
+className="white-space-pre-wrap", body=( f"æ­¤æ°æ®åºè®°å½äº
+{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
 f"Â· åè½ææªå®å" ), ), query_table, ], ), ) database_page = PageSchema
-( label="æ°æ®åº", icon="fa fa-database", children=[server_page, query_page]
+( label="æ°æ®åº", icon="fa fa-database", children=[server_page, query_page],
 ) # type: ignore config_page = PageSchema( url="/configs", isDefaultPage=True,
 icon="fa fa-wrench", label="éç½®", schema=Page( title="éç½®", initApi="/
 l4d2/api/get_group_list", body=[global_config_form, group_select,
 group_config_form], ), ) l4d2_page = PageSchema( label="æ±çä¹è·¯", icon="fa
-fa-wechat (alias)", children=[config_page, database_page] ) # type: ignore
+fa-wechat (alias)", children=[config_page, database_page], ) # type: ignore
 github_logo = Tpl( className="w-full", tpl='
-', ) header = Flex( className="w-full", justify="flex-end", alignItems="flex-
-end", items=[github_logo] ) admin_app = App( brandName="L4d2-Server",
-logo="https://ghproxy.com/https://raw.githubusercontent.com/Agnes4m/
+', # noqa: E501 ) header = Flex( className="w-full", justify="flex-end",
+alignItems="flex-end", items=[github_logo], ) admin_app = App( brandName="L4d2-
+Server", logo="https://ghproxy.com/https://raw.githubusercontent.com/Agnes4m/
 nonebot_plugin_l4d2_server/main/image/logo.png", header=header, pages=[
 {"children": [config_page, database_page]}], footer='
 Copyright Â© 2022 - 2023 AGNES_DIGIAL Xamis_v2.2.0
-', )
+', # noqa: E501 )
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py` & `nonebot_plugin_l4d2_server-0.6.0.3/nonebot_plugin_l4d2_server/l4d2_web/webUI_s.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 from amis import (
-    Action,
     ActionType,
     Alert,
-    AmisAPI,
     App,
-    DisplayModeEnum,
-    Flex,
-    Form,
-    Horizontal,
-    Html,
-    InputNumber,
-    InputPassword,
-    InputTag,
-    InputText,
     LevelEnum,
     Page,
     PageSchema,
-    Remark,
-    Select,
-    Switch,
     TableColumn,
     TableCRUD,
-    Tpl,
-    Wrapper,
 )
 
 from ..l4d2_utils.config import NICKNAME
 from .webUI import header
 
 query_table = TableCRUD(
     mode="table",
@@ -34,30 +18,30 @@
     syncLocation=False,
     api="/l4d2/api/user/get_query_contexts",
     interval=60000,
     itemActions=[
         ActionType.Url(
             tooltip="加入游戏",
             icon="fa fa-gamepad",
-            confirmText="加入steam://connect/" + "${ip}",
-            url="steam://connect/" + "${ip}",
+            confirmText="加入steam://connect/" + "${ip}",  # noqa: ISC003
+            url="steam://connect/" + "${ip}",  # noqa: ISC003
             # url= "http://"+'${ip}',
             blank=True,
         ),
     ],
     columns=[
         TableColumn(label="服主", name="tag", searchable=True, sortable=True),
         TableColumn(label="序号", name="number", sortable=True, searchable=True),
         TableColumn(label="名称", name="name", sortable=True, searchable=True),
         TableColumn(label="地图", name="map_", sortable=True, searchable=True),
         TableColumn(label="玩家", name="rank_players", sortable=True, searchable=True),
         TableColumn(label="延迟", name="ping", sortable=True, searchable=True),
         TableColumn(label="IP 地址", name="ip", sortable=True, searchable=True),
     ],
-)
+)  # type: ignore
 
 
 query_page = PageSchema(
     url="/contexts",
     icon="fa fa-comments",
     label="远程服务器查询",
     schema=Page(
@@ -102,9 +86,9 @@
 )
 
 user_app = App(
     brandName="L4d2-Server",
     logo="https://ghproxy.com/https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png",
     header=header,
     pages=[{"children": [database_page]}],
-    footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>',
+    footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>',  # noqa: E501
 )
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
-from amis import ( Action, ActionType, Alert, AmisAPI, App, DisplayModeEnum,
-Flex, Form, Horizontal, Html, InputNumber, InputPassword, InputTag, InputText,
-LevelEnum, Page, PageSchema, Remark, Select, Switch, TableColumn, TableCRUD,
-Tpl, Wrapper, ) from ..l4d2_utils.config import NICKNAME from .webUI import
-header query_table = TableCRUD( mode="table", title="", syncLocation=False,
-api="/l4d2/api/user/get_query_contexts", interval=60000, itemActions=
-[ ActionType.Url( tooltip="å å¥æ¸¸æ", icon="fa fa-gamepad",
-confirmText="å å¥steam://connect/" + "${ip}", url="steam://connect/" + "$
-{ip}", # url= "http://"+'${ip}', blank=True, ), ], columns=[ TableColumn
-(label="æä¸»", name="tag", searchable=True, sortable=True), TableColumn
-(label="åºå·", name="number", sortable=True, searchable=True), TableColumn
-(label="åç§°", name="name", sortable=True, searchable=True), TableColumn
-(label="å°å¾", name="map_", sortable=True, searchable=True), TableColumn
-(label="ç©å®¶", name="rank_players", sortable=True, searchable=True),
-TableColumn(label="å»¶è¿", name="ping", sortable=True, searchable=True),
-TableColumn(label="IP å°å", name="ip", sortable=True, searchable=True), ], )
-query_page = PageSchema( url="/contexts", icon="fa fa-comments",
-label="è¿ç¨æå¡å¨æ¥è¯¢", schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢",
-body=[ Alert( level=LevelEnum.info, className="white-space-pre-wrap", body=
-( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
+from amis import ( ActionType, Alert, App, LevelEnum, Page, PageSchema,
+TableColumn, TableCRUD, ) from ..l4d2_utils.config import NICKNAME from .webUI
+import header query_table = TableCRUD( mode="table", title="",
+syncLocation=False, api="/l4d2/api/user/get_query_contexts", interval=60000,
+itemActions=[ ActionType.Url( tooltip="å å¥æ¸¸æ", icon="fa fa-gamepad",
+confirmText="å å¥steam://connect/" + "${ip}", # noqa: ISC003 url="steam://
+connect/" + "${ip}", # noqa: ISC003 # url= "http://"+'${ip}', blank=True, ), ],
+columns=[ TableColumn(label="æä¸»", name="tag", searchable=True,
+sortable=True), TableColumn(label="åºå·", name="number", sortable=True,
+searchable=True), TableColumn(label="åç§°", name="name", sortable=True,
+searchable=True), TableColumn(label="å°å¾", name="map_", sortable=True,
+searchable=True), TableColumn(label="ç©å®¶", name="rank_players",
+sortable=True, searchable=True), TableColumn(label="å»¶è¿", name="ping",
+sortable=True, searchable=True), TableColumn(label="IP å°å", name="ip",
+sortable=True, searchable=True), ], ) # type: ignore query_page = PageSchema
+( url="/contexts", icon="fa fa-comments", label="è¿ç¨æå¡å¨æ¥è¯¢",
+schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢", body=[ Alert( level=LevelEnum.info,
+className="white-space-pre-wrap", body=( f"æ­¤æ°æ®åºè®°å½äº
+{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
 f"Â· åè½ææªå®å" ), ), query_table, ], ), ) database_page = PageSchema
 ( label="æ°æ®åº", icon="fa fa-database", url="/contexts",
 isDefaultPage=True, schema=Page( title="è¿ç¨æå¡å¨æ¥è¯¢", body=[ Alert
 ( level=LevelEnum.info, className="white-space-pre-wrap", body=
 ( f"æ­¤æ°æ®åºè®°å½äº{NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n" # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
 f"Â· åè½ææªå®å" ), ), query_table, ], ), ) user_app = App
 ( brandName="L4d2-Server", logo="https://ghproxy.com/https://
 raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/
 logo.png", header=header, pages=[{"children": [database_page]}], footer='
 Copyright Â© 2022 - 2023 AGNES_DIGIAL Xamis_v2.2.0
-', )
+', # noqa: E501 )
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/pyproject.toml` & `nonebot_plugin_l4d2_server-0.6.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-[tool.poetry]
+[project]
 name = "nonebot-plugin-l4d2-server"
-version = "0.6.0.1"
+version = "0.6.0.3"
 description = "L4D2 server related operations plugin for NoneBot2"
-authors = ["Agnes_Digital <Z735803792@163.com>"]
-license = "GPLv3"
-readme = "README.md"
-homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
-repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
-keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
+authors = [
+    { name = "Agnes_Digital", email = "Z735803792@163.com" },
+]
+requires-python = ">=3.9,<4.0"
+keywords = [
+    "steam",
+    "game",
+    "l4d2",
+    "nonebot2",
+    "plugin",
+]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-include = [
-    "LICENSE","README.md"
-]
+readme = "README.md"
+
+[project.license]
+text = "GPLv3"
 
-[tool.poetry.dependencies]
-python = "^3.8"
+[project.urls]
+homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
+
+[tool.pdm.dependencies]
 nonebot2 = "^2.0.0"
 nonebot-plugin-htmlrender = "^0.2.0.3"
 nonebot_plugin_txt2img = ">=0.3.0"
 nonebot_plugin_apscheduler = "^0.2.0"
 nonebot-adapter-onebot = "^2.2.3"
 asyncio = ">=3.4.3"
 aiohttp = "^3.8.4"
 jinja2 = ">=3.0.0"
-srctools="^2.3.9"
+srctools = "^2.3.9"
 bs4 = "0.0.1"
 httpx = ">=0.22.0"
 rcon = "^2.1.0"
 pillow = "^9.4.0"
 pyunpack = "^0.3.0"
 "ruamel.yaml" = "^0.17.21"
 rarfile = "^4.0"
@@ -43,20 +51,78 @@
 python-a2s = "^1.3.0"
 amis-python = "^1.0.6"
 pandas = ">=1.5.2"
 python-jose = ">=3.3.0"
 gitpython = ">=3.1.27"
 attrs = "^23.1.0"
 
-[tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
-pycln = "^2.1.2"
-
-[[tool.poetry.source]]
-name = "aliyun"
-url = "https://mirrors.aliyun.com/pypi/simple/"
-priority = "default"
+[tool.pdm.build]
+includes = []
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.pyright]
+pythonVersion = "3.9"
 
+[tool.black]
+line-length = 89
+target-version = [
+    "py39",
+    "py310",
+    "py311",
+]
+include = "\\.pyi?$"
+
+[tool.ruff]
+ignore = [
+    "B008",
+    "B905",
+    "E501",
+    "FBT001",
+    "FBT002",
+    "FBT003",
+    "PGH003",
+    "RUF001",
+    "RUF002",
+    "RUF003",
+    "RUF006",
+    "RUF100",
+    "SIM117",
+    "TRY002",
+    "TRY003",
+]
+select = [
+    "A",
+    "ARG",
+    "ASYNC",
+    "B",
+    "C4",
+    "COM",
+    "E",
+    "F",
+    "FBT",
+    "FLY",
+    "I",
+    "ISC",
+    "N",
+    "PIE",
+    "PGH",
+    "PTH",
+    "PYI",
+    "Q",
+    "RET",
+    "RSE",
+    "RUF",
+    "SIM",
+    "SLF",
+    "SLOT",
+    "TRY",
+]
+
+[tool.ruff.isort]
+extra-standard-library = [
+    "typing_extensions",
+]
+
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
```

### Comparing `nonebot_plugin_l4d2_server-0.6.0.1/PKG-INFO` & `nonebot_plugin_l4d2_server-0.6.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.6.0.1
+Version: 0.6.0.3
 Summary: L4D2 server related operations plugin for NoneBot2
+Keywords: steam game l4d2 nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+Author-Email: Agnes_Digital <Z735803792@163.com>
 License: GPLv3
-Keywords: steam,game,l4d2,nonebot2,plugin
-Author: Agnes_Digital
-Author-email: Z735803792@163.com
-Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: amis-python (>=1.0.6,<2.0.0)
-Requires-Dist: asyncio (>=3.4.3)
-Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: bs4 (==0.0.1)
-Requires-Dist: gitpython (>=3.1.27)
-Requires-Dist: httpx (>=0.22.0)
-Requires-Dist: jinja2 (>=3.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
-Requires-Dist: pandas (>=1.5.2)
-Requires-Dist: patool (>=1.12,<2.0)
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
-Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
-Requires-Dist: python-jose (>=3.3.0)
-Requires-Dist: pyunpack (>=0.3.0,<0.4.0)
-Requires-Dist: rarfile (>=4.0,<5.0)
-Requires-Dist: rcon (>=2.1.0,<3.0.0)
-Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: srctools (>=2.3.9,<3.0.0)
-Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+Classifier: Operating System :: OS Independent
+Project-URL: Homepage, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+Requires-Python: <4.0,>=3.9
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -189,8 +163,7 @@
 - [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
   - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
 - [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
 - [日向麻麻](https://github.com/Special-Week)- 配置优化参考
 - [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考，以及3.1版本的更新和重启
 - 呆呆- 提供三方地图的详细数据
 - ArcPav -积极反馈bug，提供改进思路
-
```

#### html2text {}

```diff
@@ -1,32 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.6.0.1
-Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
-github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
-steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
-Z735803792@163.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
-Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
-Proprietary License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.6.0.3
+Summary: L4D2 server related operations plugin for NoneBot2 Keywords: steam
+game l4d2 nonebot2 plugin Home-page: https://github.com/Agnes4m/
+nonebot_plugin_l4d2_server Author-Email: Agnes_Digital
+163.com> License: GPLv3 Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
-(>=3.8.4,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
-asyncio (>=3.4.3) Requires-Dist: attrs (>=23.1.0,<24.0.0) Requires-Dist: bs4
-(==0.0.1) Requires-Dist: gitpython (>=3.1.27) Requires-Dist: httpx (>=0.22.0)
-Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
-nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
-nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
-patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.4.0,<10.0.0) Requires-Dist:
-python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0) Requires-Dist:
-pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0) Requires-Dist:
-rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-
-Dist: srctools (>=2.3.9,<3.0.0) Project-URL: Repository, https://github.com/
-Agnes4m/nonebot_plugin_l4d2_server Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Operating System
+:: OS Independent Project-URL: Homepage, https://github.com/Agnes4m/
+nonebot_plugin_l4d2_server Requires-Python: <4.0,>=3.9 Description-Content-
+Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
  # nonebot_plugin_l4d2_server 0.6 _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
```

