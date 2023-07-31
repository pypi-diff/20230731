# Comparing `tmp/aunly-bbot-1.5.1.tar.gz` & `tmp/aunly-bbot-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aunly-bbot-1.5.1.tar", last modified: Tue Jun 27 10:49:34 2023, max compression
+gzip compressed data, was "aunly-bbot-1.6.0.tar", last modified: Mon Jul 31 12:47:20 2023, max compression
```

## Comparing `aunly-bbot-1.5.1.tar` & `aunly-bbot-1.6.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rwxr-xr-x   0        0        0    34523 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/LICENSE
--rw-r--r--   0        0        0       61 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/__main__.py
--rw-r--r--   0        0        0     3361 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/bot.py
--rw-r--r--   0        0        0     1753 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/__init__.py
--rw-r--r--   0        0        0     2302 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/api.py
--rw-r--r--   0        0        0    23358 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/config.py
--rw-r--r--   0        0        0      401 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/cli/run.py
--rw-r--r--   0        0        0     1981 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/__init__.py
--rw-r--r--   0        0        0     3054 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/announcement.py
--rw-r--r--   0        0        0      944 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/bot_config.py
--rw-r--r--   0        0        0      162 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/context.py
--rw-r--r--   0        0        0     5470 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/control.py
--rw-r--r--   0        0        0    10888 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/data.py
--rw-r--r--   0        0        0     1796 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/group_config.py
--rw-r--r--   0        0        0     2620 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/log.py
--rw-r--r--   0        0        0     2957 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/core/subgroup_config.py
--rw-r--r--   0        0        0     1996 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/__init__.py
--rw-r--r--   0        0        0      322 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/add_talk.py
--rw-r--r--   0        0        0     1526 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/admin/add.py
--rw-r--r--   0        0        0     1523 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/admin/remove.py
--rw-r--r--   0        0        0     1088 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/announcement.py
--rw-r--r--   0        0        0     2264 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/configure/atall.py
--rw-r--r--   0        0        0     2316 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/configure/nick.py
--rwxr-xr-x   0        0        0    13806 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/content_resolve.py
--rw-r--r--   0        0        0     1415 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/init.py
--rw-r--r--   0        0        0     2480 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/menu/__init__.py
--rw-r--r--   0        0        0     2491 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/quit_group.py
--rw-r--r--   0        0        0     1068 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/status.py
--rw-r--r--   0        0        0     1456 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add.py
--rw-r--r--   0        0        0     2455 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add_up.py
--rw-r--r--   0        0        0     1336 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/get_subgroup.py
--rw-r--r--   0        0        0     1355 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove.py
--rw-r--r--   0        0        0     2259 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove_up.py
--rw-r--r--   0        0        0     1666 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/up/get_subscribe.py
--rw-r--r--   0        0        0     2547 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/up/subscribe.py
--rw-r--r--   0        0        0     2101 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/up/unsubscribe.py
--rw-r--r--   0        0        0     1447 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/vip/add.py
--rw-r--r--   0        0        0     1446 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/vip/remove.py
--rw-r--r--   0        0        0     3017 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/vive_dynamic.py
--rw-r--r--   0        0        0     1554 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/web_auth.py
--rw-r--r--   0        0        0     1454 2023-06-27 10:49:17.105930 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/add.py
--rw-r--r--   0        0        0     1015 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/close.py
--rw-r--r--   0        0        0     1014 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/open.py
--rw-r--r--   0        0        0     1566 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/remove.py
--rw-r--r--   0        0        0     4026 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/bot_launch.py
--rw-r--r--   0        0        0     1432 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/exception.py
--rw-r--r--   0        0        0     1940 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/invited_join_group.py
--rw-r--r--   0        0        0     1762 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/join_group.py
--rw-r--r--   0        0        0     1923 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/leave_group.py
--rw-r--r--   0        0        0     1291 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/mute.py
--rw-r--r--   0        0        0     1475 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/new_friend.py
--rw-r--r--   0        0        0      919 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/offline.py
--rw-r--r--   0        0        0     1183 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/event/prem_change.py
--rw-r--r--   0        0        0    16966 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/pusher/dynamic.py
--rw-r--r--   0        0        0    15163 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/pusher/init.py
--rw-r--r--   0        0        0    10666 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/pusher/live.py
--rw-r--r--   0        0        0     2102 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/scheduler/refresh_token.py
--rw-r--r--   0        0        0      946 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/function/scheduler/version_update.py
--rw-r--r--   0        0        0     2856 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/bcut_asr.py
--rw-r--r--   0        0        0      315 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/captcha.py
--rw-r--r--   0        0        0     8284 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/config.py
--rw-r--r--   0        0        0       93 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/exception.py
--rw-r--r--   0        0        0     1742 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/fastapi.py
--rw-r--r--   0        0        0      322 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/model/openai.py
--rw-r--r--   0        0        0     4174 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/bot_config.exp.yaml
--rw-r--r--   0        0        0     9159 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/mobile_style.js
--rw-r--r--   0        0        0      684 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/mobile_style_bak.js
--rw-r--r--   0        0        0     1187 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7534 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/style_blue/video-details.html
--rw-r--r--   0        0        0     2098 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/index.html
--rw-r--r--   0        0        0    47433 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/marked.min.js
--rw-r--r--   0        0        0    27644 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/newbing.png
--rw-r--r--   0        0        0    59199 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/static/summary/openai.png
--rw-r--r--   0        0        0      850 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/test.py
--rw-r--r--   0        0        0      675 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/b23_extract.py
--rw-r--r--   0        0        0     6220 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/bcut_asr.py
--rw-r--r--   0        0        0      780 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_parse.py
--rw-r--r--   0        0        0     4760 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_request.py
--rw-r--r--   0        0        0    11463 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/browser_shot.py
--rw-r--r--   0        0        0     1160 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/column_resolve.py
--rw-r--r--   0        0        0      735 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/content_summarise.py
--rw-r--r--   0        0        0     2165 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/detect_package.py
--rw-r--r--   0        0        0    16749 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/draw_bili_image.py
--rw-r--r--   0        0        0      551 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/dynamic_shot.py
--rw-r--r--   0        0        0      310 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/fastapi.py
--rw-r--r--   0        0        0     4384 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/fonts_provider.py
--rw-r--r--   0        0        0     6183 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/openai.py
--rw-r--r--   0        0        0     1103 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/pil_shot.py
--rw-r--r--   0        0        0     5069 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/send_action.py
--rw-r--r--   0        0        0     1867 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/strings.py
--rw-r--r--   0        0        0     3545 2023-06-27 10:49:17.109931 aunly-bbot-1.5.1/aunly_bbot/utils/text2image.py
--rw-r--r--   0        0        0      516 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/time_tools.py
--rw-r--r--   0        0        0     2474 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/uid_extract.py
--rw-r--r--   0        0        0     5876 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/up_operation.py
--rw-r--r--   0        0        0     1089 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/update_version.py
--rw-r--r--   0        0        0     1666 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/verify_mah.py
--rw-r--r--   0        0        0     3803 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/video_subtitle.py
--rw-r--r--   0        0        0      713 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/utils/wordcloud.py
--rw-r--r--   0        0        0     1509 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/__init__.py
--rw-r--r--   0        0        0      415 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/__init__.py
--rw-r--r--   0        0        0     4953 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/auth.py
--rw-r--r--   0        0        0     1266 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/config.py
--rw-r--r--   0        0        0     2730 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/follow.py
--rw-r--r--   0        0        0     1664 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/home.py
--rw-r--r--   0        0        0     1459 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/user.py
--rw-r--r--   0        0        0     4009 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/api/router/ws.py
--rw-r--r--   0        0        0    87542 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/static/html/favicon.ico
--rw-r--r--   0        0        0      306 2023-06-27 10:49:17.113931 aunly-bbot-1.5.1/aunly_bbot/website/static/html/index.html
--rw-r--r--   0        0        0     1735 2023-06-27 10:49:17.121931 aunly-bbot-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     5120 2023-06-27 10:49:17.121931 aunly-bbot-1.5.1/readme.md
--rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 aunly-bbot-1.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0    34523 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/LICENSE
+-rw-r--r--   0        0        0       61 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/__main__.py
+-rw-r--r--   0        0        0     3362 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/bot.py
+-rw-r--r--   0        0        0     1754 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/cli/__init__.py
+-rw-r--r--   0        0        0     2312 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/cli/api.py
+-rw-r--r--   0        0        0    23358 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/cli/config.py
+-rw-r--r--   0        0        0      401 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/cli/run.py
+-rw-r--r--   0        0        0     1981 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/__init__.py
+-rw-r--r--   0        0        0     3054 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/announcement.py
+-rw-r--r--   0        0        0      944 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/bot_config.py
+-rw-r--r--   0        0        0      162 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/context.py
+-rw-r--r--   0        0        0     5470 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/control.py
+-rw-r--r--   0        0        0    10888 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/data.py
+-rw-r--r--   0        0        0     1796 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/group_config.py
+-rw-r--r--   0        0        0     2620 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/log.py
+-rw-r--r--   0        0        0     2957 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/core/subgroup_config.py
+-rw-r--r--   0        0        0     1996 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/add_talk.py
+-rw-r--r--   0        0        0     1526 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/admin/add.py
+-rw-r--r--   0        0        0     1523 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/admin/remove.py
+-rw-r--r--   0        0        0     1088 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/announcement.py
+-rw-r--r--   0        0        0     2264 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/configure/atall.py
+-rw-r--r--   0        0        0     2316 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/configure/nick.py
+-rwxr-xr-x   0        0        0    13806 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/content_resolve.py
+-rw-r--r--   0        0        0     1415 2023-07-31 12:47:09.218442 aunly-bbot-1.6.0/aunly_bbot/function/command/init.py
+-rw-r--r--   0        0        0     2480 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/menu/__init__.py
+-rw-r--r--   0        0        0     2491 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/quit_group.py
+-rw-r--r--   0        0        0     1068 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/status.py
+-rw-r--r--   0        0        0     1456 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/add.py
+-rw-r--r--   0        0        0     2455 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/add_up.py
+-rw-r--r--   0        0        0     1336 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/get_subgroup.py
+-rw-r--r--   0        0        0     1355 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/remove.py
+-rw-r--r--   0        0        0     2259 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/remove_up.py
+-rw-r--r--   0        0        0     2040 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/up/get_subscribe.py
+-rw-r--r--   0        0        0     2589 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/up/subscribe.py
+-rw-r--r--   0        0        0     2101 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/up/unsubscribe.py
+-rw-r--r--   0        0        0     1447 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/vip/add.py
+-rw-r--r--   0        0        0     1446 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/vip/remove.py
+-rw-r--r--   0        0        0     3079 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/vive_dynamic.py
+-rw-r--r--   0        0        0     1554 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/web_auth.py
+-rw-r--r--   0        0        0     1454 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/add.py
+-rw-r--r--   0        0        0     1015 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/close.py
+-rw-r--r--   0        0        0     1014 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/open.py
+-rw-r--r--   0        0        0     1566 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/remove.py
+-rw-r--r--   0        0        0     4026 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/bot_launch.py
+-rw-r--r--   0        0        0     1432 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/exception.py
+-rw-r--r--   0        0        0     1940 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/invited_join_group.py
+-rw-r--r--   0        0        0     1762 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/join_group.py
+-rw-r--r--   0        0        0     1923 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/leave_group.py
+-rw-r--r--   0        0        0     1291 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/mute.py
+-rw-r--r--   0        0        0     1475 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/new_friend.py
+-rw-r--r--   0        0        0      919 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/offline.py
+-rw-r--r--   0        0        0     1183 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/event/prem_change.py
+-rw-r--r--   0        0        0    16998 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/pusher/dynamic.py
+-rw-r--r--   0        0        0    15163 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/pusher/init.py
+-rw-r--r--   0        0        0    10700 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/pusher/live.py
+-rw-r--r--   0        0        0     2102 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/scheduler/refresh_token.py
+-rw-r--r--   0        0        0      946 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/function/scheduler/version_update.py
+-rw-r--r--   0        0        0     2856 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/model/bcut_asr.py
+-rw-r--r--   0        0        0      315 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/model/captcha.py
+-rw-r--r--   0        0        0     8312 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/model/config.py
+-rw-r--r--   0        0        0       93 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/model/exception.py
+-rw-r--r--   0        0        0     1742 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/model/fastapi.py
+-rw-r--r--   0        0        0      322 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/model/openai.py
+-rw-r--r--   0        0        0     4174 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/bot_config.exp.yaml
+-rw-r--r--   0        0        0     9200 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/mobile_style.js
+-rw-r--r--   0        0        0      684 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/mobile_style_bak.js
+-rw-r--r--   0        0        0     1187 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7534 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     2098 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/summary/marked.min.js
+-rw-r--r--   0        0        0    27644 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/summary/newbing.png
+-rw-r--r--   0        0        0    59199 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/static/summary/openai.png
+-rw-r--r--   0        0        0      850 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/test.py
+-rw-r--r--   0        0        0      675 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/b23_extract.py
+-rw-r--r--   0        0        0     6220 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/bcut_asr.py
+-rw-r--r--   0        0        0      780 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/bilibili_parse.py
+-rw-r--r--   0        0        0     4744 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/bilibili_request.py
+-rw-r--r--   0        0        0    12609 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/browser_shot.py
+-rw-r--r--   0        0        0     1160 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/column_resolve.py
+-rw-r--r--   0        0        0      735 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/content_summarise.py
+-rw-r--r--   0        0        0     2165 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/detect_package.py
+-rw-r--r--   0        0        0    16749 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/draw_bili_image.py
+-rw-r--r--   0        0        0      551 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/dynamic_shot.py
+-rw-r--r--   0        0        0      310 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/fastapi.py
+-rw-r--r--   0        0        0     4384 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/fonts_provider.py
+-rw-r--r--   0        0        0     6183 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/openai.py
+-rw-r--r--   0        0        0     1103 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/pil_shot.py
+-rw-r--r--   0        0        0     5069 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/send_action.py
+-rw-r--r--   0        0        0     1867 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/strings.py
+-rw-r--r--   0        0        0     3545 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/text2image.py
+-rw-r--r--   0        0        0      516 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/time_tools.py
+-rw-r--r--   0        0        0     3116 2023-07-31 12:47:09.222442 aunly-bbot-1.6.0/aunly_bbot/utils/uid_extract.py
+-rw-r--r--   0        0        0     5876 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/utils/up_operation.py
+-rw-r--r--   0        0        0     1089 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/utils/update_version.py
+-rw-r--r--   0        0        0     1666 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/utils/verify_mah.py
+-rw-r--r--   0        0        0     3803 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/utils/video_subtitle.py
+-rw-r--r--   0        0        0      713 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/utils/wordcloud.py
+-rw-r--r--   0        0        0     1509 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/api/router/__init__.py
+-rw-r--r--   0        0        0     4953 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/api/router/auth.py
+-rw-r--r--   0        0        0     1266 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/api/router/config.py
+-rw-r--r--   0        0        0     2730 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/api/router/follow.py
+-rw-r--r--   0        0        0     1664 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/api/router/home.py
+-rw-r--r--   0        0        0     1459 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/api/router/user.py
+-rw-r--r--   0        0        0     4009 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/api/router/ws.py
+-rw-r--r--   0        0        0    87542 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/static/html/favicon.ico
+-rw-r--r--   0        0        0      306 2023-07-31 12:47:09.226442 aunly-bbot-1.6.0/aunly_bbot/website/static/html/index.html
+-rw-r--r--   0        0        0     1711 2023-07-31 12:47:09.230442 aunly-bbot-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5120 2023-07-31 12:47:09.230442 aunly-bbot-1.6.0/readme.md
+-rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 aunly-bbot-1.6.0/PKG-INFO
```

### Comparing `aunly-bbot-1.5.1/LICENSE` & `aunly-bbot-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/bot.py` & `aunly-bbot-1.6.0/aunly_bbot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 app.config(install_log=True)
 
 if BotConfig.Bilibili.use_browser:
     from graiax.playwright.service import PlaywrightService  # type: ignore # noqa
 
     app.launch_manager.add_service(
         PlaywrightService(
-            browser_type="firefox",
+            browser_type="chromium",
             user_data_dir=Path("data").joinpath("browser"),
             device_scale_factor=1.5 if BotConfig.Bilibili.mobile_style else 1.25,
             user_agent=(
                 "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
                 "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
             )
             if BotConfig.Bilibili.mobile_style
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/cli/__init__.py` & `aunly-bbot-1.6.0/aunly_bbot/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 @click.command(name="install-deps", help="安装 Playwright 所需依赖")
 @click.help_option("-h", "--help", help="显示帮助信息")
 def install_deps():
     import sys
     from playwright.__main__ import main as pw_main
 
-    sys.argv.append("firefox")
+    sys.argv.append("chromium")
     pw_main()
 
 
 @click.command(help="BBot 配置向导")
 def config():
     from .config import click_config
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/cli/api.py` & `aunly-bbot-1.6.0/aunly_bbot/cli/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,26 +26,26 @@
 @app.on_event("startup")
 async def init_playwright():
     global PLAYWRIGIT
     logger.info("正在下载字体...")
     font_init()
     logger.success("字体下载完成！")
 
-    await install_playwright(browser_type="firefox")
+    await install_playwright(browser_type="chromium")
     pw = await async_playwright().start()
-    ff = await pw.firefox.launch_persistent_context(
+    chrome = await pw.chromium.launch_persistent_context(
         Path("data").joinpath("browser"),
         device_scale_factor=1.5,
         user_agent=(
             "Mozilla/5.0 (Linux; Android 10; RMX1911) AppleWebKit/537.36 "
             "(KHTML, like Gecko) Chrome/100.0.4896.127 Mobile Safari/537.36"
         ),
         # headless=False,
     )
-    PLAYWRIGIT = ff
+    PLAYWRIGIT = chrome
     logger.info("[Playwright] 正在获取浏览器版本")
     if len(PLAYWRIGIT.pages) > 0:
         page = PLAYWRIGIT.pages[0]
     else:
         page = await PLAYWRIGIT.new_page()
     version = await page.evaluate("navigator.appVersion")
     logger.info(f"[BiliBili推送] 浏览器启动完成，当前版本 {version}")
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/cli/config.py` & `aunly-bbot-1.6.0/aunly_bbot/cli/config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/__init__.py` & `aunly-bbot-1.6.0/aunly_bbot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/announcement.py` & `aunly-bbot-1.6.0/aunly_bbot/core/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/bot_config.py` & `aunly-bbot-1.6.0/aunly_bbot/core/bot_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/control.py` & `aunly-bbot-1.6.0/aunly_bbot/core/control.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/data.py` & `aunly-bbot-1.6.0/aunly_bbot/core/data.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/group_config.py` & `aunly-bbot-1.6.0/aunly_bbot/core/group_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/log.py` & `aunly-bbot-1.6.0/aunly_bbot/core/log.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/core/subgroup_config.py` & `aunly-bbot-1.6.0/aunly_bbot/core/subgroup_config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/__init__.py` & `aunly-bbot-1.6.0/aunly_bbot/function/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/admin/add.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/admin/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/admin/remove.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/admin/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/announcement.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/announcement.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/configure/atall.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/configure/atall.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/configure/nick.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/configure/nick.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/content_resolve.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/content_resolve.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/init.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/menu/__init__.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/quit_group.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/quit_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/status.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/status.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/add_up.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/add_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/get_subgroup.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/get_subgroup.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/subgroup/remove_up.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/subgroup/remove_up.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/up/get_subscribe.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/up/unsubscribe.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,44 +4,61 @@
 from graia.ariadne.message.element import At
 from graia.ariadne.event.message import GroupMessage
 from graia.ariadne.message.chain import MessageChain
 from graia.saya.builtins.broadcast.schema import ListenerSchema
 from graia.ariadne.message.parser.twilight import (
     Twilight,
     RegexMatch,
+    RegexResult,
     ElementMatch,
     ElementResult,
+    WildcardMatch,
 )
 
+
+from ....utils.up_operation import unsubscribe_uid
 from ....core.bot_config import BotConfig
-from ....core.data import get_sub_by_group
+from ....utils.uid_extract import uid_extract
 from ....core.control import Interval, Permission
 
 channel = Channel.current()
 
 
 @channel.use(
     ListenerSchema(
         listening_events=[GroupMessage],
         inline_dispatchers=[
-            Twilight(["at" @ ElementMatch(At, optional=True), RegexMatch(r"查看(本群)?(订阅|关注)列表")])
+            Twilight(
+                [
+                    "at" @ ElementMatch(At),
+                    RegexMatch(r"(退订|取消?关注?)\s?(主播|[uU][pP])?"),
+                    "anything" @ WildcardMatch(optional=True),
+                ]
+            )
         ],
-        decorators=[Permission.require(), Interval.require()],
-    ),
+        decorators=[Permission.require(Permission.GROUP_ADMIN), Interval.require()],
+    )
 )
-async def sub_list(app: Ariadne, group: Group, at: ElementResult):
-    if at.result:
-        at_element: At = at.result  # type: ignore
-        if at_element.target != BotConfig.Mirai.account:
-            return
-    sublist = get_sub_by_group(group.id)
-    sublist_count = len(sublist)
-    if sublist_count == 0:
-        await app.send_group_message(group, MessageChain("本群未订阅任何 UP"))
-    else:
-        msg = [f"本群共订阅 {sublist_count} 个 UP\n注：带*号的表示该 UP 已被设定自定义昵称"]
-        msg.extend(
-            f"\n{i}. {f'*{data.nick}' if data.nick else data.uname}（{data.uid}）"
-            for i, data in enumerate(sublist, 1)
-        )
+async def main(app: Ariadne, group: Group, at: ElementResult, anything: RegexResult):
+
+    at_result: At = at.result  # type: ignore
+    if at_result.target == app.account:
+        message = anything.result.display  # type: ignore
+
+        uid = await uid_extract(message, group.id)
 
-        await app.send_group_message(group, MessageChain(msg))
+        if uid:
+            msg = await unsubscribe_uid(uid, group.id)
+            await app.send_friend_message(
+                BotConfig.master,
+                MessageChain(f"群 {group.name}（{group.id}）正在退订 UP：{uid}\n{msg}"),
+            )
+            if BotConfig.Event.subscribe:
+                await app.send_group_message(
+                    group,
+                    MessageChain(msg),
+                )
+        else:
+            await app.send_group_message(
+                group,
+                MessageChain("未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接"),
+            )
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/up/subscribe.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/up/subscribe.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     if at_result.target == app.account:
         if not BOT_Status.check_status(Status.INITIALIZED):
             return await app.send_group_message(
                 group,
                 MessageChain("正在初始化，请稍后..."),
             )
         message = anything.result.display  # type: ignore
-        uid = await uid_extract(message)
-        if uid:
+        uid = await uid_extract(message, show_error=True)
+        if uid and uid.isdigit():
             if not BOT_Status.check_status(Status.DYNAMIC_IDLE):
                 await app.send_group_message(
                     group,
                     MessageChain("正在订阅，请稍后..."),
                 )
             msg = await subscribe_uid(uid, group.id)
             await app.send_group_message(
@@ -63,9 +63,9 @@
                 await app.send_friend_message(
                     BotConfig.master,
                     MessageChain(f"群：{group.name}（{group.id}）\n正在订阅 UP：{uid}\n{msg}"),
                 )
         else:
             await app.send_group_message(
                 group,
-                MessageChain("未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接"),
+                MessageChain(uid or "未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接"),
             )
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/up/unsubscribe.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/up/get_subscribe.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,55 @@
-from graia.saya import Channel
 from graia.ariadne.app import Ariadne
-from graia.ariadne.model import Group
-from graia.ariadne.message.element import At
 from graia.ariadne.event.message import GroupMessage
 from graia.ariadne.message.chain import MessageChain
-from graia.saya.builtins.broadcast.schema import ListenerSchema
+from graia.ariadne.message.element import At
 from graia.ariadne.message.parser.twilight import (
-    Twilight,
-    RegexMatch,
-    RegexResult,
     ElementMatch,
     ElementResult,
-    WildcardMatch,
+    RegexMatch,
+    Twilight,
 )
-
-
-from ....utils.up_operation import unsubscribe_uid
+from graia.ariadne.model import Group
+from graia.saya import Channel
+from graia.saya.builtins.broadcast.schema import ListenerSchema
+import time
+from ....core import BOT_Status
 from ....core.bot_config import BotConfig
-from ....utils.uid_extract import uid_extract
 from ....core.control import Interval, Permission
+from ....core.data import get_sub_by_group
+from ....utils.time_tools import calc_time_total
 
 channel = Channel.current()
 
 
 @channel.use(
     ListenerSchema(
         listening_events=[GroupMessage],
         inline_dispatchers=[
-            Twilight(
-                [
-                    "at" @ ElementMatch(At),
-                    RegexMatch(r"(退订|取消?关注?)\s?(主播|[uU][pP])?"),
-                    "anything" @ WildcardMatch(optional=True),
-                ]
-            )
+            Twilight(["at" @ ElementMatch(At, optional=True), RegexMatch(r"查看(本群)?(订阅|关注)列表")])
         ],
-        decorators=[Permission.require(Permission.GROUP_ADMIN), Interval.require()],
-    )
+        decorators=[Permission.require(), Interval.require()],
+    ),
 )
-async def main(app: Ariadne, group: Group, at: ElementResult, anything: RegexResult):
-
-    at_result: At = at.result  # type: ignore
-    if at_result.target == app.account:
-        message = anything.result.display  # type: ignore
-
-        uid = await uid_extract(message, group.id)
+async def sub_list(app: Ariadne, group: Group, at: ElementResult):
+    if at.result:
+        at_element: At = at.result  # type: ignore
+        if at_element.target != BotConfig.Mirai.account:
+            return
+    sublist = get_sub_by_group(group.id)
+
+    sublist_count = len(sublist)
+    if sublist_count == 0:
+        await app.send_group_message(group, MessageChain("本群未订阅任何 UP"))
+    else:
+        msg = [f"本群共订阅 {sublist_count} 个 UP\n注：带*号的表示该 UP 已被设定自定义昵称"]
+        for i, sub in enumerate(sublist, 1):
+            live_time = BOT_Status.living.get(str(sub.uid), -1)
+            if live_time > 100000:
+                live = f" 🔴直播中: {calc_time_total(time.time() - live_time)}"
+            elif live_time >= 0:
+                live = " 🔴直播中"
+            else:
+                live = ""
+            msg.append(f"\n{i}. {f'*{sub.nick}' if sub.nick else sub.uname}（{sub.uid}）{live}")
 
-        if uid:
-            msg = await unsubscribe_uid(uid, group.id)
-            await app.send_friend_message(
-                BotConfig.master,
-                MessageChain(f"群 {group.name}（{group.id}）正在退订 UP：{uid}\n{msg}"),
-            )
-            if BotConfig.Event.subscribe:
-                await app.send_group_message(
-                    group,
-                    MessageChain(msg),
-                )
-        else:
-            await app.send_group_message(
-                group,
-                MessageChain("未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接"),
-            )
+        await app.send_group_message(group, MessageChain(msg))
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/vip/add.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/vip/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/vip/remove.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/vip/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/vive_dynamic.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/vive_dynamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 async def main(
     app: Ariadne,
     group: Group,
     source: Source,
     up: RegexResult,
     offset: RegexResult,
 ):
-
-    if not (uid := await uid_extract(up.result.display, group.id)):
+    uid = await uid_extract(text=up.result.display, groupid=group.id, show_error=True)
+    if not uid or not uid.isdigit():
         return await app.send_group_message(
             group,
-            MessageChain("未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接"),
+            MessageChain(uid or "未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接"),
             quote=source,
         )
 
     if int(uid) == 0:
         return await app.send_group_message(group, MessageChain("UP 主不存在"), quote=source)
 
     try:
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/web_auth.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/web_auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/add.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/add.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/close.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/close.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/open.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/open.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/command/whitelist/remove.py` & `aunly-bbot-1.6.0/aunly_bbot/function/command/whitelist/remove.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/bot_launch.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/bot_launch.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/exception.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/exception.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/invited_join_group.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/invited_join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/join_group.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/join_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/leave_group.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/leave_group.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/mute.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/mute.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/new_friend.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/new_friend.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/offline.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/offline.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/event/prem_change.py` & `aunly-bbot-1.6.0/aunly_bbot/function/event/prem_change.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/pusher/dynamic.py` & `aunly-bbot-1.6.0/aunly_bbot/function/pusher/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     is_dyn_pushed_in_group,
     insert_dyn_push_to_group,
 )
 
 channel = Channel.current()
 
 
-@channel.use(SchedulerSchema(every_custom_seconds(3)))
+@channel.use(SchedulerSchema(every_custom_seconds(BotConfig.Bilibili.dynamic_interval)))
 async def main(app: Ariadne):
     logger.debug("[Dynamic Pusher] Dynamic Pusher running now...")
     subid_list = get_all_uid()
     sub_sum = len(subid_list)
 
     if not BOT_Status.is_all_statuses_true(
         Status.INITIALIZED, Status.ACCOUNT_CONNECTED, Status.STARTED, Status.SUBSCRIBE_IDLE
@@ -136,15 +136,15 @@
             await asyncio.gather(
                 *[check_uid(app, uid) for uid in subid_group], return_exceptions=True
             )
 
     BOT_Status.last_finish = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     BOT_Status.set_status(Status.DYNAMIC_IDLE, True)
     logger.debug("[Dynamic] Updating finished")
-    await asyncio.sleep(0.5)
+    await asyncio.sleep(3)
 
 
 async def push(app: Ariadne, dyn: DynamicItem):
     """推送动态"""
 
     up_id = str(dyn.modules[0].module_author.author.mid)
     up_name = dyn.modules[0].module_author.author.name
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/pusher/init.py` & `aunly-bbot-1.6.0/aunly_bbot/function/pusher/init.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/pusher/live.py` & `aunly-bbot-1.6.0/aunly_bbot/function/pusher/live.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ...utils.bilibili_request import get_b23_url
 from ...utils.up_operation import delete_group, delete_uid, set_name
 from ...core.data import insert_live_push, get_all_uid, get_sub_by_uid, update_cover_by_id
 
 channel = Channel.current()
 
 
-@channel.use(SchedulerSchema(every_custom_seconds(3)))
+@channel.use(SchedulerSchema(every_custom_seconds(BotConfig.Bilibili.dynamic_interval)))
 async def main(app: Ariadne):
     if (
         not BOT_Status.is_all_statuses_true(
             Status.INITIALIZED, Status.ACCOUNT_CONNECTED, Status.STARTED, Status.SUBSCRIBE_IDLE
         )
         or BOT_Status.is_all_statuses_true(
             Status.INITIALIZED, Status.ACCOUNT_CONNECTED, Status.STARTED, Status.SUBSCRIBE_IDLE
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/scheduler/refresh_token.py` & `aunly-bbot-1.6.0/aunly_bbot/function/scheduler/refresh_token.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/function/scheduler/version_update.py` & `aunly-bbot-1.6.0/aunly_bbot/function/scheduler/version_update.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/model/bcut_asr.py` & `aunly-bbot-1.6.0/aunly_bbot/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/model/config.py` & `aunly-bbot-1.6.0/aunly_bbot/model/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     username: Optional[str]
     password: Optional[str]
     use_login: bool = False
     use_browser: bool = True
     allow_fallback: bool = True
     mobile_style: bool = True
     render_style: Literal["bbot_default", "style_blue"] = "bbot_default"
-    concurrency: int = 5
+    concurrency: int = 1
+    dynamic_interval: int = 30
     dynamic_font: str = "HarmonyOS_Sans_SC_Medium.ttf"
     dynamic_font_source: Literal["local", "remote"] = "local"
     openai_summarization: bool = False
     openai_api_token: Optional[str] = None
     openai_model: str = "gpt-3.5-turbo-0301"
     openai_proxy: Optional[AnyHttpUrl] = None
     openai_cooldown: int = 60
@@ -117,16 +118,16 @@
             return openai_promot_version
         click.secho("openai_promot_version 只能为 1 或 2", fg="bright_yellow")
         sys.exit()
 
     # 验证 Bilibili gRPC 并发数
     @validator("concurrency")
     def limit_concurrency(cls, concurrency):
-        if concurrency > 50:
-            click.secho("gRPC 并发数超过 50，已自动调整为 50", fg="bright_yellow")
+        if concurrency > 5:
+            click.secho("gRPC 并发数超过 5，已自动调整为 5", fg="bright_yellow")
             return 50
         elif concurrency < 1:
             click.secho("gRPC 并发数小于 1，已自动调整为 1", fg="bright_yellow")
             return 1
         else:
             return concurrency
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/model/fastapi.py` & `aunly-bbot-1.6.0/aunly_bbot/model/fastapi.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/bot_config.exp.yaml` & `aunly-bbot-1.6.0/aunly_bbot/static/bot_config.exp.yaml`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/mobile_style.js` & `aunly-bbot-1.6.0/aunly_bbot/static/mobile_style.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 /*
  * @Author: KBD
  * @Date: 2022-12-26 13:45:30
  * @LastEditors: KBD
- * @LastEditTime: 2023-01-13 01:35:34
+ * @LastEditTime: 2023-06-28 10:55:31
  * @Description: 用于初始化手机动态页面的样式以及图片大小
  */
-async function getMobileStyle() {
+async function getMobileStyle(useImageBig = true) {
     // 删除 dom 的对象, 可以自行添加 ( className 需要增加 '.' 为前缀, id 需要增加 '#' 为前缀)
     const deleteDoms = {
         // 关注 dom
         followDoms: [".dyn-header__following", ".easy-follow-btn", ".dyn-orig-author__right"],
         // 分享 dom
         shareDoms: [".dyn-share"],
         // 打开程序 dom
@@ -81,15 +81,15 @@
         // 获取图片的宽高比
         ratioList.push(await getImageRatio(item.firstChild.src));
     })).then(() => {
         // 判断 ratioList 中超过 1 的个数为 3 的倍数 且 ratioList 的长度大于 3
         const isAllOneLength = ratioList.filter(item => item >= 0.9 && item <= 1.1).length;
         const isAllOne = ratioList.length === 9 ? isAllOneLength > ratioList.length / 2 : isAllOneLength > 0 && isAllOneLength % 3 === 0 && ratioList.length > 3;
         // 说明可能为组装的拼图, 如果不是则放大为大图
-        if (!isAllOne) {
+        if (!isAllOne && useImageBig) {
             // 找到图标容器dom
             const containerDom = document.querySelector(".bm-pics-block__container");
             if (containerDom) {
                 // 先把默认 padding-left 置为0
                 containerDom.style.paddingLeft = "0";
                 // 先把默认 padding-right 置为0
                 containerDom.style.paddingRight = "0";
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/mobile_style_bak.js` & `aunly-bbot-1.6.0/aunly_bbot/static/mobile_style_bak.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/business.png` & `aunly-bbot-1.6.0/aunly_bbot/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/personal.png` & `aunly-bbot-1.6.0/aunly_bbot/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/style_blue/assets/video_bottom.png` & `aunly-bbot-1.6.0/aunly_bbot/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/style_blue/video-details.html` & `aunly-bbot-1.6.0/aunly_bbot/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/summary/index.html` & `aunly-bbot-1.6.0/aunly_bbot/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/summary/marked.min.js` & `aunly-bbot-1.6.0/aunly_bbot/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/summary/newbing.png` & `aunly-bbot-1.6.0/aunly_bbot/static/summary/newbing.png`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/static/summary/openai.png` & `aunly-bbot-1.6.0/aunly_bbot/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/test.py` & `aunly-bbot-1.6.0/aunly_bbot/test.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/b23_extract.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/b23_extract.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/bcut_asr.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_parse.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/bilibili_parse.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/bilibili_request.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/bilibili_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,19 +88,20 @@
     return resp["content"]
 
 
 async def search_user(keyword: str):
     """
     搜索用户
     """
-    url = "https://api.bilibili.com/x/web-interface/search/type"
-    data = {"keyword": keyword, "search_type": "bili_user"}
-    resp = (await hc.get(url, params=data)).json()
+    url = "https://app.bilibili.com/x/v2/search/type"
+    data = {"build": "6840300", "keyword": keyword, "type": "2", "ps": 5}
+
+    resp = await get(url, params=data)
     logger.debug(resp)
-    return resp["data"]
+    return resp
 
 
 async def get_user_space_info(uid: int):
     """
     获取用户空间信息
     """
     url = "https://app.bilibili.com/x/v2/space"
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/browser_shot.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/browser_shot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,29 @@
-import re
-import time
-import httpx
 import asyncio
 import contextlib
-
-from yarl import URL
+import re
+import time
 from pathlib import Path
-from loguru import logger
+import json
+
+import httpx
 from graia.ariadne import Ariadne
-from sentry_sdk import capture_exception
-from playwright._impl._api_types import TimeoutError
 from graiax.playwright.interface import PlaywrightContext
+from loguru import logger
 from playwright._impl._api_structures import Position
-from playwright.async_api._generated import (
-    Page,
-    Route,
-    Request,
-    Response,
-    BrowserContext,
-)
+from playwright._impl._api_types import TimeoutError
+from playwright.async_api._generated import BrowserContext, Page, Request, Response, Route
+from sentry_sdk import capture_exception
+from yarl import URL
 
 from ..core.bot_config import BotConfig
 from ..model.captcha import CaptchaResponse
-
 from .fonts_provider import get_font
 
-
+browser_cookies_file = Path("data").joinpath("browser_cookies.json")
 error_path = Path("data").joinpath("error")
 error_path.mkdir(parents=True, exist_ok=True)
 captcha_path = Path("data").joinpath("captcha")
 captcha_path.mkdir(parents=True, exist_ok=True)
 mobile_style_js = Path(__file__).parent.parent.joinpath("static", "mobile_style.js")
 font_mime_map = {
     "collection": "font/collection",
@@ -60,17 +54,38 @@
 async def resolve_select_captcha(page: Page):
     pass
 
 
 async def browser_dynamic(dynid: str):
     app = Ariadne.current()
     browser_context = app.launch_manager.get_interface(PlaywrightContext).context
+    # add cookies
+    if browser_cookies_file.exists() and browser_cookies_file.is_file():
+        if browser_cookies := json.loads(browser_cookies_file.read_bytes()):
+            logger.debug(f"正在为浏览器添加cookies")
+            await browser_context.add_cookies(
+                [
+                    {
+                        "domain": cookie["domain"],
+                        "name": cookie["name"],
+                        "path": cookie["path"],
+                        "value": cookie["value"],
+                    }
+                    for cookie in browser_cookies
+                ]
+            )
     return await screenshot(dynid, browser_context)
 
 
+async def refresh_cookies(browser_context: BrowserContext):
+    storage_state = await browser_context.storage_state()
+    if cookies := storage_state.get("cookies"):
+        browser_cookies_file.write_text(json.dumps(cookies))
+
+
 async def screenshot(dynid: str, browser_context: BrowserContext, log=True):
     logger.info(f"正在截图动态：{dynid}")
     st = int(time.time())
     for i in range(3):
         page = await browser_context.new_page()
         await page.route(re.compile("^https://fonts.bbot/(.+)$"), fill_font)
         try:
@@ -78,30 +93,36 @@
                 page.on("requestfinished", network_request)
             page.on("requestfailed", network_requestfailed)
             if BotConfig.Bilibili.mobile_style:
                 page, clip = await get_mobile_screenshot(page, dynid)
             else:
                 page, clip = await get_pc_screenshot(page, dynid)
             clip["height"] = min(clip["height"], 32766)  # 限制高度
-            return await page.screenshot(clip=clip, full_page=True, type="jpeg", quality=98)
+            if picture := await page.screenshot(
+                clip=clip, full_page=True, type="jpeg", quality=98
+            ):
+                await refresh_cookies(browser_context)
+                return picture
         except TimeoutError:
             logger.error(f"[BiliBili推送] {dynid} 动态截图超时，正在重试：")
         except Notfound:
-            logger.error(f"[Bilibili推送] {dynid} 动态不存在")
+            logger.error(f"[Bilibili推送] {dynid} 动态不存在，等待 3 秒后重试...")
+            await asyncio.sleep(3)
         except AssertionError:
             logger.exception(f"[BiliBili推送] {dynid} 动态截图失败，正在重试：")
             await page.screenshot(
                 path=f"{error_path}/{dynid}_{i}_{st}.jpg",
                 full_page=True,
                 type="jpeg",
                 quality=80,
             )
         except Exception as e:  # noqa
             if "bilibili.com/404" in page.url:
                 logger.error(f"[Bilibili推送] {dynid} 动态不存在")
+                await refresh_cookies(browser_context)
                 break
             elif "waiting until" in str(e):
                 logger.error(f"[BiliBili推送] {dynid} 动态截图超时，正在重试：")
             else:
                 capture_exception()
                 logger.exception(f"[BiliBili推送] {dynid} 动态截图失败，正在重试：")
                 try:
@@ -216,26 +237,26 @@
                 for point in click_points:
                     real_click_points = {
                         "x": point[0] * captcha_size["width"] / origin_image_size[0],
                         "y": point[1] * captcha_size["height"] / origin_image_size[1],
                     }
                     await captcha_image.click(position=Position(**real_click_points))
                     await page.wait_for_timeout(800)
-                captcha_image_body = ""
                 await page.click("text=确认")
                 geetest_up = await page.wait_for_selector(".geetest_up", state="visible")
                 await page.screenshot(path=captcha_path.joinpath(f"{last_captcha_id}.jpg"))
                 if not geetest_up:
                     logger.warning("[Captcha] 未检测到验证码验证结果，正在重试")
                     continue
                 geetest_result = await geetest_up.text_content()
                 assert geetest_result
                 logger.debug(f"[Captcha] Geetest result: {geetest_result}")
                 if "验证成功" in geetest_result:
                     logger.success("[Captcha] 极验网页 Tip 验证成功")
+                    captcha_image_body = ""
                 else:
                     logger.warning("[Captcha] 极验验证失败，正在重试")
 
                 with contextlib.suppress(TimeoutError):
                     await page.wait_for_load_state(state="domcontentloaded", timeout=20000)
 
     if "bilibili.com/404" in page.url:
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/column_resolve.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/column_resolve.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/content_summarise.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/content_summarise.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/detect_package.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/detect_package.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/draw_bili_image.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/dynamic_shot.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/dynamic_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/fonts_provider.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/openai.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/openai.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/pil_shot.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/pil_shot.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/send_action.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/send_action.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/strings.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/strings.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/text2image.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/text2image.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/time_tools.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/uid_extract.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/uid_extract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import re
+from typing import Optional, Union
 
 from loguru import logger
-from typing import Union, Optional
+from pydantic import BaseModel, Extra
 
-
-from .b23_extract import b23_extract
 from ..core.data import get_sub_by_group
+from .b23_extract import b23_extract
 from .bilibili_request import search_user
 
 
-async def uid_extract(text: str, groupid: Optional[Union[int, str]] = None):
+class SearchUp(BaseModel, extra=Extra.ignore):
+    title: str
+    mid: int
+
+    def __str__(self) -> str:
+        return f"{self.title}({self.mid})"
+
+
+class SearchResult(BaseModel, extra=Extra.ignore):
+    items: list[SearchUp] = []
+
+
+async def uid_extract(
+    text: str, groupid: Optional[Union[int, str]] = None, show_error: bool = False
+):
     logger.debug(f"[UID Extract] Original Text: {text}")
     if up_list := get_sub_by_group(groupid or 0):
         logger.debug(f"[UID Extract] Group {groupid} has {len(up_list)} Subscribers")
         if text.isdigit():
             logger.debug("[UID Extract] Text is a Number")
         for data in up_list:
             if text.isdigit():
@@ -46,13 +60,20 @@
     else:
         text_u = text.strip(""""'“”‘’""")
         if text_u != text:
             logger.debug(f"[UID Extract] Text is a Quoted Digit: {text_u}")
         logger.debug(f"[UID Extract] Searching UID in BiliBili: {text_u}")
         resp = await search_user(text_u)
         logger.debug(f"[UID Extract] Search result: {resp}")
-        if resp and resp["numResults"]:
-            for result in resp["result"]:
-                if result["uname"] == text_u:
-                    logger.debug(f"[UID Extract] Found User: {result}")
-                    return str(result["mid"])
+        result = SearchResult(**resp)
+        if result.items:
+            for up in result.items:
+                if up.title == text_u:
+                    return str(up.mid)
+                logger.debug("[UID Extract] No User found")
+                return (
+                    ("未找到该 UP，你可能在找：\n" + "\n".join([str(up) for up in result.items]))
+                    if show_error
+                    else None
+                )
         logger.debug("[UID Extract] No User found")
+        return "未找到该 UP，请输入正确的 UP 群内昵称、UP 名、UP UID或 UP 首页链接" if show_error else None
```

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/up_operation.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/up_operation.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/update_version.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/update_version.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/verify_mah.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/verify_mah.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/video_subtitle.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/utils/wordcloud.py` & `aunly-bbot-1.6.0/aunly_bbot/utils/wordcloud.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/__init__.py` & `aunly-bbot-1.6.0/aunly_bbot/website/__init__.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/api/router/auth.py` & `aunly-bbot-1.6.0/aunly_bbot/website/api/router/auth.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/api/router/config.py` & `aunly-bbot-1.6.0/aunly_bbot/website/api/router/config.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/api/router/follow.py` & `aunly-bbot-1.6.0/aunly_bbot/website/api/router/follow.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/api/router/home.py` & `aunly-bbot-1.6.0/aunly_bbot/website/api/router/home.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/api/router/user.py` & `aunly-bbot-1.6.0/aunly_bbot/website/api/router/user.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/api/router/ws.py` & `aunly-bbot-1.6.0/aunly_bbot/website/api/router/ws.py`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/aunly_bbot/website/static/html/favicon.ico` & `aunly-bbot-1.6.0/aunly_bbot/website/static/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/pyproject.toml` & `aunly-bbot-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aunly-bbot"
-version = "1.5.1"
+version = "1.6.0"
 description = "一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人"
 readme = "readme.md"
 keywords = [
     "graia",
     "graiax",
     "bilibili",
     "qqbot",
@@ -50,15 +50,14 @@
 
 [project.optional-dependencies]
 full = [
     "graiax-playwright>=0.2.4",
     "graiax-text2img-playwright>=0.4.0",
     "wordcloud>=1.9.2",
     "jieba>=0.42.1",
-    "edgegpt>=0.10.13",
     "jinja2>=3.1.2",
 ]
 
 [project.scripts]
 bbot = "aunly_bbot.__main__:main"
 
 [tool.pdm.build]
```

### Comparing `aunly-bbot-1.5.1/readme.md` & `aunly-bbot-1.6.0/readme.md`

 * *Files identical despite different names*

### Comparing `aunly-bbot-1.5.1/PKG-INFO` & `aunly-bbot-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aunly-bbot
-Version: 1.5.1
+Version: 1.6.0
 Summary: 一个用于 QQ 群内高效推送哔哩哔哩 UP 动态及直播的机器人
 License: AGPL3.0
 Keywords: graia,graiax,bilibili,qqbot,grpc,playwright,fastapi,bot,openai,chatgpt
 Author-email: djkcyl <cyl@cyllive.cn>
 Requires-Python: >=3.9,<4.0
 Provides-Extra: full
 Project-URL: documentation, https://github.com/djkcyl/BBot-Graia/blob/master/readme.md
```

