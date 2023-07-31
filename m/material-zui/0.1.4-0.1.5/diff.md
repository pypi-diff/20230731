# Comparing `tmp/material_zui-0.1.4.tar.gz` & `tmp/material_zui-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.1.4.tar", max compression
+gzip compressed data, was "material_zui-0.1.5.tar", max compression
```

## Comparing `material_zui-0.1.4.tar` & `material_zui-0.1.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1268 2023-07-31 06:13:19.959889 material_zui-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.4/src/material_zui/.pypirc
--rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.4/src/material_zui/ResizeImage.py
--rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.4/src/material_zui/bard/__init__.py
--rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.4/src/material_zui/bard/google_bard.py
--rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.4/src/material_zui/bard/index.py
--rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.4/src/material_zui/bing_ai/__init__.py
--rw-r--r--   0        0        0     3531 2023-06-27 03:27:48.335228 material_zui-0.1.4/src/material_zui/bing_ai/bing_ai.py
--rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.4/src/material_zui/bing_ai/index.py
--rw-r--r--   0        0        0      955 2023-06-24 04:25:16.261811 material_zui-0.1.4/src/material_zui/bing_ai/result.py
--rw-r--r--   0        0        0      132 2023-06-24 05:06:49.316509 material_zui-0.1.4/src/material_zui/bing_ai/type.py
--rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.4/src/material_zui/compress/__init__.py
--rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.4/src/material_zui/compress/index.py
--rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.4/src/material_zui/compress/text.py
--rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.4/src/material_zui/crawl/__init__.py
--rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.4/src/material_zui/crawl/image.py
--rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.4/src/material_zui/crawl/index.py
--rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.4/src/material_zui/crontab/__init__.py
--rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.4/src/material_zui/crontab/index.py
--rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.4/src/material_zui/date_time/__init__.py
--rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.4/src/material_zui/date_time/__init__.pyc
--rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.4/src/material_zui/date_time/date_time.py
--rw-r--r--   0        0        0      123 2023-07-16 12:10:14.125544 material_zui-0.1.4/src/material_zui/date_time/index.py
--rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.4/src/material_zui/date_time/index.pyc
--rw-r--r--   0        0        0     2211 2023-07-16 13:22:45.935630 material_zui-0.1.4/src/material_zui/date_time/time.py
--rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.4/src/material_zui/dict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.4/src/material_zui/dict/common.py
--rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.4/src/material_zui/dict/index.py
--rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.4/src/material_zui/env/__init__.py
--rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.4/src/material_zui/env/env.py
--rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.4/src/material_zui/env/index.py
--rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.4/src/material_zui/fake/__init__.py
--rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.4/src/material_zui/fake/index.py
--rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.4/src/material_zui/fake/number.py
--rw-r--r--   0        0        0       21 2023-06-24 01:47:34.605558 material_zui-0.1.4/src/material_zui/file/__init__.py
--rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.4/src/material_zui/file/check.py
--rw-r--r--   0        0        0     2115 2023-07-02 11:49:59.755643 material_zui-0.1.4/src/material_zui/file/common.py
--rw-r--r--   0        0        0      912 2023-07-29 05:10:16.021864 material_zui-0.1.4/src/material_zui/file/download.py
--rw-r--r--   0        0        0     2051 2023-06-24 03:27:30.253159 material_zui-0.1.4/src/material_zui/file/excel.py
--rw-r--r--   0        0        0      410 2023-07-29 04:56:18.852441 material_zui-0.1.4/src/material_zui/file/index.py
--rw-r--r--   0        0        0     1757 2023-07-02 11:37:34.980074 material_zui-0.1.4/src/material_zui/file/read.py
--rw-r--r--   0        0        0      430 2023-06-24 05:09:30.541040 material_zui-0.1.4/src/material_zui/file/type.py
--rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.4/src/material_zui/file/write.py
--rw-r--r--   0        0        0       21 2023-06-27 03:03:29.674154 material_zui-0.1.4/src/material_zui/generate/__init__.py
--rw-r--r--   0        0        0     2002 2023-06-27 07:49:36.922442 material_zui-0.1.4/src/material_zui/generate/common.py
--rw-r--r--   0        0        0       22 2023-06-27 03:05:13.513527 material_zui-0.1.4/src/material_zui/generate/index.py
--rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.4/src/material_zui/gpt/__init__.py
--rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.4/src/material_zui/gpt/gpt_vietnam.py
--rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.4/src/material_zui/gpt/index.py
--rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.4/src/material_zui/image/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.4/src/material_zui/image/colorization.py
--rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.4/src/material_zui/image/combine.py
--rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.4/src/material_zui/image/common.py
--rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.4/src/material_zui/image/convert.py
--rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.4/src/material_zui/image/data.py
--rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.4/src/material_zui/image/index.py
--rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.4/src/material_zui/image/model/colorization_deploy_v2.prototxt
--rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.4/src/material_zui/image/model/pts_in_hull.npy
--rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.4/src/material_zui/image/remove_background.py
--rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.4/src/material_zui/image/to_svg.py
--rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.4/src/material_zui/image/transparent_background.py
--rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.4/src/material_zui/image/type.py
--rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.4/src/material_zui/image/upscale.py
--rw-r--r--   0        0        0       21 2023-07-30 11:44:27.414884 material_zui-0.1.4/src/material_zui/list/__init__.py
--rw-r--r--   0        0        0     4415 2023-07-30 13:24:18.913364 material_zui-0.1.4/src/material_zui/list/common.py
--rw-r--r--   0        0        0      154 2023-07-30 13:24:35.996722 material_zui-0.1.4/src/material_zui/list/index.py
--rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.4/src/material_zui/log/__init__.py
--rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.4/src/material_zui/log/index.py
--rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.4/src/material_zui/log/log.py
--rw-r--r--   0        0        0       21 2023-07-29 03:49:37.553797 material_zui-0.1.4/src/material_zui/network/__init__.py
--rw-r--r--   0        0        0     2606 2023-07-31 06:13:07.060055 material_zui-0.1.4/src/material_zui/network/common.py
--rw-r--r--   0        0        0       70 2023-07-29 11:25:06.057119 material_zui-0.1.4/src/material_zui/network/index.py
--rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.4/src/material_zui/number/__init__.py
--rw-r--r--   0        0        0      380 2023-07-29 05:39:04.869919 material_zui-0.1.4/src/material_zui/number/common.py
--rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.4/src/material_zui/number/index.py
--rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.4/src/material_zui/os/__init__.py
--rw-r--r--   0        0        0      840 2023-07-12 02:26:10.443342 material_zui-0.1.4/src/material_zui/os/common.py
--rw-r--r--   0        0        0      125 2023-07-12 02:29:41.294270 material_zui-0.1.4/src/material_zui/os/index.py
--rw-r--r--   0        0        0      330 2023-07-12 02:54:51.769004 material_zui-0.1.4/src/material_zui/os/terminal.py
--rw-r--r--   0        0        0     1250 2023-07-29 05:39:04.697919 material_zui-0.1.4/src/material_zui/readme.md
--rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.4/src/material_zui/regex/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.4/src/material_zui/regex/index.py
--rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.4/src/material_zui/replicate/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.4/src/material_zui/replicate/index.py
--rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.4/src/material_zui/selenium/__init__.py
--rw-r--r--   0        0        0     4155 2023-07-31 01:53:50.526065 material_zui-0.1.4/src/material_zui/selenium/chrome.py
--rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.4/src/material_zui/selenium/common.py
--rw-r--r--   0        0        0     2836 2023-07-30 03:31:40.599764 material_zui-0.1.4/src/material_zui/selenium/firefox.py
--rw-r--r--   0        0        0      150 2023-07-16 03:36:28.421675 material_zui-0.1.4/src/material_zui/selenium/index.py
--rw-r--r--   0        0        0     9288 2023-07-30 03:32:09.290158 material_zui-0.1.4/src/material_zui/selenium/selenium.py
--rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.4/src/material_zui/setup.py
--rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.4/src/material_zui/string/__init__.py
--rw-r--r--   0        0        0     3403 2023-07-29 11:24:14.277396 material_zui-0.1.4/src/material_zui/string/common.py
--rw-r--r--   0        0        0      345 2023-07-29 11:24:14.137397 material_zui-0.1.4/src/material_zui/string/index.py
--rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.4/src/material_zui/telegram_bot/__init__.py
--rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.4/src/material_zui/telegram_bot/index.py
--rw-r--r--   0        0        0       21 2023-07-29 05:45:31.405279 material_zui-0.1.4/src/material_zui/thread/__init__.py
--rw-r--r--   0        0        0      455 2023-07-30 14:11:11.539245 material_zui-0.1.4/src/material_zui/thread/common.py
--rw-r--r--   0        0        0       37 2023-07-29 05:53:44.309345 material_zui-0.1.4/src/material_zui/thread/index.py
--rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.4/src/material_zui/tmp/__init__.py
--rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.4/src/material_zui/tmp/index.py
--rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.4/src/material_zui/utility/__init__.py
--rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.4/src/material_zui/utility/common.py
--rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.4/src/material_zui/utility/index.py
--rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.4/src/material_zui/validate/__init__.py
--rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.4/src/material_zui/validate/common.py
--rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.4/src/material_zui/validate/index.py
--rw-r--r--   0        0        0     2944 1970-01-01 00:00:00.000000 material_zui-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1268 2023-07-31 06:57:57.592257 material_zui-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.5/src/material_zui/.pypirc
+-rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.5/src/material_zui/ResizeImage.py
+-rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.5/src/material_zui/bard/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.5/src/material_zui/bard/google_bard.py
+-rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.5/src/material_zui/bard/index.py
+-rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.5/src/material_zui/bing_ai/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 03:27:48.335228 material_zui-0.1.5/src/material_zui/bing_ai/bing_ai.py
+-rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.5/src/material_zui/bing_ai/index.py
+-rw-r--r--   0        0        0      955 2023-06-24 04:25:16.261811 material_zui-0.1.5/src/material_zui/bing_ai/result.py
+-rw-r--r--   0        0        0      132 2023-06-24 05:06:49.316509 material_zui-0.1.5/src/material_zui/bing_ai/type.py
+-rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.5/src/material_zui/compress/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.5/src/material_zui/compress/index.py
+-rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.5/src/material_zui/compress/text.py
+-rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.5/src/material_zui/crawl/__init__.py
+-rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.5/src/material_zui/crawl/image.py
+-rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.5/src/material_zui/crawl/index.py
+-rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.5/src/material_zui/crontab/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.5/src/material_zui/crontab/index.py
+-rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.5/src/material_zui/date_time/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.5/src/material_zui/date_time/__init__.pyc
+-rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.5/src/material_zui/date_time/date_time.py
+-rw-r--r--   0        0        0      123 2023-07-16 12:10:14.125544 material_zui-0.1.5/src/material_zui/date_time/index.py
+-rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.5/src/material_zui/date_time/index.pyc
+-rw-r--r--   0        0        0     2211 2023-07-16 13:22:45.935630 material_zui-0.1.5/src/material_zui/date_time/time.py
+-rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.5/src/material_zui/dict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.5/src/material_zui/dict/common.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.5/src/material_zui/dict/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.5/src/material_zui/env/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.5/src/material_zui/env/env.py
+-rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.5/src/material_zui/env/index.py
+-rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.5/src/material_zui/fake/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.5/src/material_zui/fake/index.py
+-rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.5/src/material_zui/fake/number.py
+-rw-r--r--   0        0        0       21 2023-06-24 01:47:34.605558 material_zui-0.1.5/src/material_zui/file/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.5/src/material_zui/file/check.py
+-rw-r--r--   0        0        0     2115 2023-07-02 11:49:59.755643 material_zui-0.1.5/src/material_zui/file/common.py
+-rw-r--r--   0        0        0      912 2023-07-29 05:10:16.021864 material_zui-0.1.5/src/material_zui/file/download.py
+-rw-r--r--   0        0        0     2051 2023-06-24 03:27:30.253159 material_zui-0.1.5/src/material_zui/file/excel.py
+-rw-r--r--   0        0        0      410 2023-07-29 04:56:18.852441 material_zui-0.1.5/src/material_zui/file/index.py
+-rw-r--r--   0        0        0     1757 2023-07-02 11:37:34.980074 material_zui-0.1.5/src/material_zui/file/read.py
+-rw-r--r--   0        0        0      430 2023-06-24 05:09:30.541040 material_zui-0.1.5/src/material_zui/file/type.py
+-rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.5/src/material_zui/file/write.py
+-rw-r--r--   0        0        0       21 2023-06-27 03:03:29.674154 material_zui-0.1.5/src/material_zui/generate/__init__.py
+-rw-r--r--   0        0        0     2002 2023-06-27 07:49:36.922442 material_zui-0.1.5/src/material_zui/generate/common.py
+-rw-r--r--   0        0        0       22 2023-06-27 03:05:13.513527 material_zui-0.1.5/src/material_zui/generate/index.py
+-rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.5/src/material_zui/gpt/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.5/src/material_zui/gpt/gpt_vietnam.py
+-rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.5/src/material_zui/gpt/index.py
+-rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.5/src/material_zui/image/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.5/src/material_zui/image/colorization.py
+-rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.5/src/material_zui/image/combine.py
+-rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.5/src/material_zui/image/common.py
+-rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.5/src/material_zui/image/convert.py
+-rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.5/src/material_zui/image/data.py
+-rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.5/src/material_zui/image/index.py
+-rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.5/src/material_zui/image/model/colorization_deploy_v2.prototxt
+-rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.5/src/material_zui/image/model/pts_in_hull.npy
+-rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.5/src/material_zui/image/remove_background.py
+-rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.5/src/material_zui/image/to_svg.py
+-rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.5/src/material_zui/image/transparent_background.py
+-rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.5/src/material_zui/image/type.py
+-rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.5/src/material_zui/image/upscale.py
+-rw-r--r--   0        0        0       21 2023-07-30 11:44:27.414884 material_zui-0.1.5/src/material_zui/list/__init__.py
+-rw-r--r--   0        0        0     4415 2023-07-30 13:24:18.913364 material_zui-0.1.5/src/material_zui/list/common.py
+-rw-r--r--   0        0        0      154 2023-07-30 13:24:35.996722 material_zui-0.1.5/src/material_zui/list/index.py
+-rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.5/src/material_zui/log/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.5/src/material_zui/log/index.py
+-rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.5/src/material_zui/log/log.py
+-rw-r--r--   0        0        0       21 2023-07-29 03:49:37.553797 material_zui-0.1.5/src/material_zui/network/__init__.py
+-rw-r--r--   0        0        0     2606 2023-07-31 06:13:07.060055 material_zui-0.1.5/src/material_zui/network/common.py
+-rw-r--r--   0        0        0       70 2023-07-29 11:25:06.057119 material_zui-0.1.5/src/material_zui/network/index.py
+-rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.5/src/material_zui/number/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-29 05:39:04.869919 material_zui-0.1.5/src/material_zui/number/common.py
+-rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.5/src/material_zui/number/index.py
+-rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.5/src/material_zui/os/__init__.py
+-rw-r--r--   0        0        0      840 2023-07-12 02:26:10.443342 material_zui-0.1.5/src/material_zui/os/common.py
+-rw-r--r--   0        0        0      125 2023-07-12 02:29:41.294270 material_zui-0.1.5/src/material_zui/os/index.py
+-rw-r--r--   0        0        0      330 2023-07-12 02:54:51.769004 material_zui-0.1.5/src/material_zui/os/terminal.py
+-rw-r--r--   0        0        0     1480 2023-07-31 06:43:38.844082 material_zui-0.1.5/src/material_zui/readme.md
+-rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.5/src/material_zui/regex/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.5/src/material_zui/regex/index.py
+-rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.5/src/material_zui/replicate/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.5/src/material_zui/replicate/index.py
+-rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.5/src/material_zui/selenium/__init__.py
+-rw-r--r--   0        0        0     4155 2023-07-31 01:53:50.526065 material_zui-0.1.5/src/material_zui/selenium/chrome.py
+-rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.5/src/material_zui/selenium/common.py
+-rw-r--r--   0        0        0     2836 2023-07-30 03:31:40.599764 material_zui-0.1.5/src/material_zui/selenium/firefox.py
+-rw-r--r--   0        0        0      150 2023-07-16 03:36:28.421675 material_zui-0.1.5/src/material_zui/selenium/index.py
+-rw-r--r--   0        0        0     9288 2023-07-30 03:32:09.290158 material_zui-0.1.5/src/material_zui/selenium/selenium.py
+-rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.5/src/material_zui/setup.py
+-rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.5/src/material_zui/string/__init__.py
+-rw-r--r--   0        0        0     3403 2023-07-29 11:24:14.277396 material_zui-0.1.5/src/material_zui/string/common.py
+-rw-r--r--   0        0        0      345 2023-07-29 11:24:14.137397 material_zui-0.1.5/src/material_zui/string/index.py
+-rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.5/src/material_zui/telegram_bot/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.5/src/material_zui/telegram_bot/index.py
+-rw-r--r--   0        0        0       21 2023-07-29 05:45:31.405279 material_zui-0.1.5/src/material_zui/thread/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-30 14:11:11.539245 material_zui-0.1.5/src/material_zui/thread/common.py
+-rw-r--r--   0        0        0       37 2023-07-29 05:53:44.309345 material_zui-0.1.5/src/material_zui/thread/index.py
+-rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.5/src/material_zui/tmp/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.5/src/material_zui/tmp/index.py
+-rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.5/src/material_zui/utility/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.5/src/material_zui/utility/common.py
+-rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.5/src/material_zui/utility/index.py
+-rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.5/src/material_zui/validate/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.5/src/material_zui/validate/common.py
+-rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.5/src/material_zui/validate/index.py
+-rw-r--r--   0        0        0     3174 1970-01-01 00:00:00.000000 material_zui-0.1.5/PKG-INFO
```

### Comparing `material_zui-0.1.4/pyproject.toml` & `material_zui-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "material_zui"
-version = "0.1.4"
+version = "0.1.5"
 description = "Material Zui"
 authors = ["chauhmnguyen <chauhoangminhnguyen@gmail.com>"]
 readme = "src/material_zui/readme.md"
 keywords = [
 	"material",
 	"zui",
 	"material zui",
```

### Comparing `material_zui-0.1.4/src/material_zui/ResizeImage.py` & `material_zui-0.1.5/src/material_zui/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/bard/google_bard.py` & `material_zui-0.1.5/src/material_zui/bard/google_bard.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/bing_ai/bing_ai.py` & `material_zui-0.1.5/src/material_zui/bing_ai/bing_ai.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/bing_ai/result.py` & `material_zui-0.1.5/src/material_zui/bing_ai/result.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/compress/text.py` & `material_zui-0.1.5/src/material_zui/compress/text.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/crawl/image.py` & `material_zui-0.1.5/src/material_zui/crawl/image.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/crontab/index.py` & `material_zui-0.1.5/src/material_zui/crontab/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/date_time/time.py` & `material_zui-0.1.5/src/material_zui/date_time/time.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/file/check.py` & `material_zui-0.1.5/src/material_zui/file/check.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/file/common.py` & `material_zui-0.1.5/src/material_zui/file/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/file/download.py` & `material_zui-0.1.5/src/material_zui/file/download.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/file/excel.py` & `material_zui-0.1.5/src/material_zui/file/excel.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/file/read.py` & `material_zui-0.1.5/src/material_zui/file/read.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/file/write.py` & `material_zui-0.1.5/src/material_zui/file/write.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/generate/common.py` & `material_zui-0.1.5/src/material_zui/generate/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/gpt/gpt_vietnam.py` & `material_zui-0.1.5/src/material_zui/gpt/gpt_vietnam.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/colorization.py` & `material_zui-0.1.5/src/material_zui/image/colorization.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/combine.py` & `material_zui-0.1.5/src/material_zui/image/combine.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/common.py` & `material_zui-0.1.5/src/material_zui/image/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/convert.py` & `material_zui-0.1.5/src/material_zui/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/model/colorization_deploy_v2.prototxt` & `material_zui-0.1.5/src/material_zui/image/model/colorization_deploy_v2.prototxt`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/model/pts_in_hull.npy` & `material_zui-0.1.5/src/material_zui/image/model/pts_in_hull.npy`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/remove_background.py` & `material_zui-0.1.5/src/material_zui/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/to_svg.py` & `material_zui-0.1.5/src/material_zui/image/to_svg.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/transparent_background.py` & `material_zui-0.1.5/src/material_zui/image/transparent_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/image/upscale.py` & `material_zui-0.1.5/src/material_zui/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/list/common.py` & `material_zui-0.1.5/src/material_zui/list/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/log/log.py` & `material_zui-0.1.5/src/material_zui/log/log.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/network/common.py` & `material_zui-0.1.5/src/material_zui/network/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/os/common.py` & `material_zui-0.1.5/src/material_zui/os/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/readme.md` & `material_zui-0.1.5/src/material_zui/readme.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Installation
+
+## Prerequisites
+
+- Python >= `v3.10`
+
+## Install package
+
+1. `pip install poetry`
+2. Setup and active virtual enviroment with `poetry`
+3. `poetry add material-zui` to install all dependencies
+4. Done!! &#128513;
+
 # Modules
 
 <ol>
   <!-- <li>automation</li> -->
   <li>bard</li>
   <li>bing_ai</li>
   <li>compress</li>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
-# Modules
+# Installation ## Prerequisites - Python >= `v3.10` ## Install package 1. `pip
+install poetry` 2. Setup and active virtual enviroment with `poetry` 3. `poetry
+add material-zui` to install all dependencies 4. Done!!  # Modules
    1. bard
    2. bing_ai
    3. compress
    4. crawl
    5. crontab
    6. date_time
    7. env
```

### Comparing `material_zui-0.1.4/src/material_zui/regex/index.py` & `material_zui-0.1.5/src/material_zui/regex/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/replicate/index.py` & `material_zui-0.1.5/src/material_zui/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/selenium/chrome.py` & `material_zui-0.1.5/src/material_zui/selenium/chrome.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/selenium/firefox.py` & `material_zui-0.1.5/src/material_zui/selenium/firefox.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/selenium/selenium.py` & `material_zui-0.1.5/src/material_zui/selenium/selenium.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/setup.py` & `material_zui-0.1.5/src/material_zui/setup.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/string/common.py` & `material_zui-0.1.5/src/material_zui/string/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/src/material_zui/utility/common.py` & `material_zui-0.1.5/src/material_zui/utility/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.4/PKG-INFO` & `material_zui-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.1.4
+Version: 0.1.5
 Summary: Material Zui
 Keywords: material,zui,material zui,zui material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -36,14 +36,27 @@
 Requires-Dist: streamlit (>=1.24.1,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Requires-Dist: xlsxwriter (>=3.1.2,<4.0.0)
 Requires-Dist: youtube-dl (>=2021.12.17,<2022.0.0)
 Description-Content-Type: text/markdown
 
+# Installation
+
+## Prerequisites
+
+- Python >= `v3.10`
+
+## Install package
+
+1. `pip install poetry`
+2. Setup and active virtual enviroment with `poetry`
+3. `poetry add material-zui` to install all dependencies
+4. Done!! &#128513;
+
 # Modules
 
 <ol>
   <!-- <li>automation</li> -->
   <li>bard</li>
   <li>bing_ai</li>
   <li>compress</li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: material-zui Version: 0.1.4 Summary: Material Zui
+Metadata-Version: 2.1 Name: material-zui Version: 0.1.5 Summary: Material Zui
 Keywords: material,zui,material zui,zui material Author: chauhmnguyen Author-
 email: chauhoangminhnguyen@gmail.com Requires-Python: >=3.10,<3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Requires-Dist: bardapi (>=0.1.2,<0.2.0) Requires-Dist: beautifulsoup4
 (>=4.12.2,<5.0.0) Requires-Dist: edgegpt (>=0.11.6,<0.12.0) Requires-Dist:
 flask (>=2.3.2,<3.0.0) Requires-Dist: free-proxy (>=1.1.1,<2.0.0) Requires-
 Dist: huggingface-hub (>=0.15.1,<0.16.0) Requires-Dist: langchain
@@ -16,15 +16,18 @@
 pytube (>=15.0.0,<16.0.0) Requires-Dist: rembg (>=2.0.36,<3.0.0) Requires-Dist:
 replicate (>=0.8.1,<0.9.0) Requires-Dist: requests (>=2.30.0,<3.0.0) Requires-
 Dist: selenium (>=4.9.1,<5.0.0) Requires-Dist: selenium-browser
 (>=0.0.15,<0.0.16) Requires-Dist: setuptools (>=67.8.0,<68.0.0) Requires-Dist:
 streamlit (>=1.24.1,<2.0.0) Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0) Requires-Dist: xlsxwriter
 (>=3.1.2,<4.0.0) Requires-Dist: youtube-dl (>=2021.12.17,<2022.0.0)
-Description-Content-Type: text/markdown # Modules
+Description-Content-Type: text/markdown # Installation ## Prerequisites -
+Python >= `v3.10` ## Install package 1. `pip install poetry` 2. Setup and
+active virtual enviroment with `poetry` 3. `poetry add material-zui` to install
+all dependencies 4. Done!!  # Modules
    1. bard
    2. bing_ai
    3. compress
    4. crawl
    5. crontab
    6. date_time
    7. env
```

