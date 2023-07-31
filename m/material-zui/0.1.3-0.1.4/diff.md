# Comparing `tmp/material_zui-0.1.3.tar.gz` & `tmp/material_zui-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.1.3.tar", max compression
+gzip compressed data, was "material_zui-0.1.4.tar", max compression
```

## Comparing `material_zui-0.1.3.tar` & `material_zui-0.1.4.tar`

### file list

```diff
@@ -1,99 +1,108 @@
--rw-r--r--   0        0        0     1224 2023-06-27 07:46:19.598737 material_zui-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.3/src/material_zui/.pypirc
--rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.3/src/material_zui/ResizeImage.py
--rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.3/src/material_zui/bard/__init__.py
--rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.3/src/material_zui/bard/google_bard.py
--rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.3/src/material_zui/bard/index.py
--rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.3/src/material_zui/bing_ai/__init__.py
--rw-r--r--   0        0        0     3531 2023-06-27 03:27:48.335228 material_zui-0.1.3/src/material_zui/bing_ai/bing_ai.py
--rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.3/src/material_zui/bing_ai/index.py
--rw-r--r--   0        0        0      955 2023-06-24 04:25:16.261811 material_zui-0.1.3/src/material_zui/bing_ai/result.py
--rw-r--r--   0        0        0      132 2023-06-24 05:06:49.316509 material_zui-0.1.3/src/material_zui/bing_ai/type.py
--rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.3/src/material_zui/compress/__init__.py
--rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.3/src/material_zui/compress/index.py
--rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.3/src/material_zui/compress/text.py
--rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.3/src/material_zui/crawl/__init__.py
--rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.3/src/material_zui/crawl/image.py
--rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.3/src/material_zui/crawl/index.py
--rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.3/src/material_zui/crontab/__init__.py
--rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.3/src/material_zui/crontab/index.py
--rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.3/src/material_zui/date_time/__init__.py
--rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.3/src/material_zui/date_time/__init__.pyc
--rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.3/src/material_zui/date_time/date_time.py
--rw-r--r--   0        0        0       73 2023-06-13 08:55:03.914876 material_zui-0.1.3/src/material_zui/date_time/index.py
--rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.3/src/material_zui/date_time/index.pyc
--rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.3/src/material_zui/date_time/time.py
--rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.3/src/material_zui/dict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.3/src/material_zui/dict/common.py
--rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.3/src/material_zui/dict/index.py
--rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.3/src/material_zui/env/__init__.py
--rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.3/src/material_zui/env/env.py
--rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.3/src/material_zui/env/index.py
--rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.3/src/material_zui/fake/__init__.py
--rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.3/src/material_zui/fake/index.py
--rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.3/src/material_zui/fake/number.py
--rw-r--r--   0        0        0       21 2023-06-24 01:47:34.605558 material_zui-0.1.3/src/material_zui/file/__init__.py
--rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.3/src/material_zui/file/check.py
--rw-r--r--   0        0        0     2115 2023-06-15 03:25:12.103320 material_zui-0.1.3/src/material_zui/file/common.py
--rw-r--r--   0        0        0      304 2023-06-15 03:25:12.271318 material_zui-0.1.3/src/material_zui/file/download.py
--rw-r--r--   0        0        0     2051 2023-06-24 03:27:30.253159 material_zui-0.1.3/src/material_zui/file/excel.py
--rw-r--r--   0        0        0      353 2023-06-25 14:02:51.225505 material_zui-0.1.3/src/material_zui/file/index.py
--rw-r--r--   0        0        0     1757 2023-06-27 02:48:30.793448 material_zui-0.1.3/src/material_zui/file/read.py
--rw-r--r--   0        0        0      430 2023-06-24 05:09:30.541040 material_zui-0.1.3/src/material_zui/file/type.py
--rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.3/src/material_zui/file/write.py
--rw-r--r--   0        0        0       21 2023-06-27 03:03:29.674154 material_zui-0.1.3/src/material_zui/generate/__init__.py
--rw-r--r--   0        0        0     2103 2023-06-27 07:23:41.480905 material_zui-0.1.3/src/material_zui/generate/common.py
--rw-r--r--   0        0        0       22 2023-06-27 03:05:13.513527 material_zui-0.1.3/src/material_zui/generate/index.py
--rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.3/src/material_zui/gpt/__init__.py
--rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.3/src/material_zui/gpt/gpt_vietnam.py
--rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.3/src/material_zui/gpt/index.py
--rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.3/src/material_zui/image/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.3/src/material_zui/image/colorization.py
--rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.3/src/material_zui/image/combine.py
--rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.3/src/material_zui/image/common.py
--rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.3/src/material_zui/image/convert.py
--rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.3/src/material_zui/image/data.py
--rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.3/src/material_zui/image/index.py
--rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.3/src/material_zui/image/model/colorization_deploy_v2.prototxt
--rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.3/src/material_zui/image/model/pts_in_hull.npy
--rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.3/src/material_zui/image/remove_background.py
--rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.3/src/material_zui/image/to_svg.py
--rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.3/src/material_zui/image/transparent_background.py
--rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.3/src/material_zui/image/type.py
--rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.3/src/material_zui/image/upscale.py
--rw-r--r--   0        0        0       38 2023-05-22 04:09:03.922071 material_zui-0.1.3/src/material_zui/list/__init__.py
--rw-r--r--   0        0        0     2916 2023-06-18 14:13:03.127264 material_zui-0.1.3/src/material_zui/list/common.py
--rw-r--r--   0        0        0       92 2023-06-13 09:15:39.330734 material_zui-0.1.3/src/material_zui/list/index.py
--rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.3/src/material_zui/log/__init__.py
--rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.3/src/material_zui/log/index.py
--rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.3/src/material_zui/log/log.py
--rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.3/src/material_zui/number/__init__.py
--rw-r--r--   0        0        0      364 2023-06-13 10:11:32.006838 material_zui-0.1.3/src/material_zui/number/common.py
--rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.3/src/material_zui/number/index.py
--rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.3/src/material_zui/os/__init__.py
--rw-r--r--   0        0        0       83 2023-06-16 02:02:57.672095 material_zui-0.1.3/src/material_zui/os/index.py
--rw-r--r--   0        0        0      840 2023-06-15 03:40:00.119319 material_zui-0.1.3/src/material_zui/os/os.py
--rw-r--r--   0        0        0     1213 2023-06-23 08:04:27.953396 material_zui-0.1.3/src/material_zui/readme.md
--rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.3/src/material_zui/regex/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.3/src/material_zui/regex/index.py
--rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.3/src/material_zui/replicate/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.3/src/material_zui/replicate/index.py
--rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.3/src/material_zui/selenium/__init__.py
--rw-r--r--   0        0        0     6709 2023-06-25 13:43:29.275206 material_zui-0.1.3/src/material_zui/selenium/chrome.py
--rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.3/src/material_zui/selenium/common.py
--rw-r--r--   0        0        0      120 2023-05-22 02:03:54.393486 material_zui-0.1.3/src/material_zui/selenium/index.py
--rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.3/src/material_zui/setup.py
--rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.3/src/material_zui/string/__init__.py
--rw-r--r--   0        0        0     2802 2023-06-18 14:03:40.774857 material_zui-0.1.3/src/material_zui/string/common.py
--rw-r--r--   0        0        0      135 2023-06-14 08:12:20.153192 material_zui-0.1.3/src/material_zui/string/index.py
--rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.3/src/material_zui/telegram_bot/__init__.py
--rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.3/src/material_zui/telegram_bot/index.py
--rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.3/src/material_zui/tmp/__init__.py
--rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.3/src/material_zui/tmp/index.py
--rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.3/src/material_zui/utility/__init__.py
--rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.3/src/material_zui/utility/common.py
--rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.3/src/material_zui/utility/index.py
--rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.3/src/material_zui/validate/__init__.py
--rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.3/src/material_zui/validate/common.py
--rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.3/src/material_zui/validate/index.py
--rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 material_zui-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1268 2023-07-31 06:13:19.959889 material_zui-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.4/src/material_zui/.pypirc
+-rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.4/src/material_zui/ResizeImage.py
+-rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.4/src/material_zui/bard/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.4/src/material_zui/bard/google_bard.py
+-rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.4/src/material_zui/bard/index.py
+-rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.4/src/material_zui/bing_ai/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 03:27:48.335228 material_zui-0.1.4/src/material_zui/bing_ai/bing_ai.py
+-rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.4/src/material_zui/bing_ai/index.py
+-rw-r--r--   0        0        0      955 2023-06-24 04:25:16.261811 material_zui-0.1.4/src/material_zui/bing_ai/result.py
+-rw-r--r--   0        0        0      132 2023-06-24 05:06:49.316509 material_zui-0.1.4/src/material_zui/bing_ai/type.py
+-rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.4/src/material_zui/compress/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.4/src/material_zui/compress/index.py
+-rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.4/src/material_zui/compress/text.py
+-rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.4/src/material_zui/crawl/__init__.py
+-rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.4/src/material_zui/crawl/image.py
+-rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.4/src/material_zui/crawl/index.py
+-rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.4/src/material_zui/crontab/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.4/src/material_zui/crontab/index.py
+-rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.4/src/material_zui/date_time/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.4/src/material_zui/date_time/__init__.pyc
+-rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.4/src/material_zui/date_time/date_time.py
+-rw-r--r--   0        0        0      123 2023-07-16 12:10:14.125544 material_zui-0.1.4/src/material_zui/date_time/index.py
+-rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.4/src/material_zui/date_time/index.pyc
+-rw-r--r--   0        0        0     2211 2023-07-16 13:22:45.935630 material_zui-0.1.4/src/material_zui/date_time/time.py
+-rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.4/src/material_zui/dict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.4/src/material_zui/dict/common.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.4/src/material_zui/dict/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.4/src/material_zui/env/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.4/src/material_zui/env/env.py
+-rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.4/src/material_zui/env/index.py
+-rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.4/src/material_zui/fake/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.4/src/material_zui/fake/index.py
+-rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.4/src/material_zui/fake/number.py
+-rw-r--r--   0        0        0       21 2023-06-24 01:47:34.605558 material_zui-0.1.4/src/material_zui/file/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.4/src/material_zui/file/check.py
+-rw-r--r--   0        0        0     2115 2023-07-02 11:49:59.755643 material_zui-0.1.4/src/material_zui/file/common.py
+-rw-r--r--   0        0        0      912 2023-07-29 05:10:16.021864 material_zui-0.1.4/src/material_zui/file/download.py
+-rw-r--r--   0        0        0     2051 2023-06-24 03:27:30.253159 material_zui-0.1.4/src/material_zui/file/excel.py
+-rw-r--r--   0        0        0      410 2023-07-29 04:56:18.852441 material_zui-0.1.4/src/material_zui/file/index.py
+-rw-r--r--   0        0        0     1757 2023-07-02 11:37:34.980074 material_zui-0.1.4/src/material_zui/file/read.py
+-rw-r--r--   0        0        0      430 2023-06-24 05:09:30.541040 material_zui-0.1.4/src/material_zui/file/type.py
+-rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.4/src/material_zui/file/write.py
+-rw-r--r--   0        0        0       21 2023-06-27 03:03:29.674154 material_zui-0.1.4/src/material_zui/generate/__init__.py
+-rw-r--r--   0        0        0     2002 2023-06-27 07:49:36.922442 material_zui-0.1.4/src/material_zui/generate/common.py
+-rw-r--r--   0        0        0       22 2023-06-27 03:05:13.513527 material_zui-0.1.4/src/material_zui/generate/index.py
+-rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.4/src/material_zui/gpt/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.4/src/material_zui/gpt/gpt_vietnam.py
+-rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.4/src/material_zui/gpt/index.py
+-rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.4/src/material_zui/image/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.4/src/material_zui/image/colorization.py
+-rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.4/src/material_zui/image/combine.py
+-rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.4/src/material_zui/image/common.py
+-rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.4/src/material_zui/image/convert.py
+-rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.4/src/material_zui/image/data.py
+-rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.4/src/material_zui/image/index.py
+-rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.4/src/material_zui/image/model/colorization_deploy_v2.prototxt
+-rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.4/src/material_zui/image/model/pts_in_hull.npy
+-rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.4/src/material_zui/image/remove_background.py
+-rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.4/src/material_zui/image/to_svg.py
+-rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.4/src/material_zui/image/transparent_background.py
+-rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.4/src/material_zui/image/type.py
+-rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.4/src/material_zui/image/upscale.py
+-rw-r--r--   0        0        0       21 2023-07-30 11:44:27.414884 material_zui-0.1.4/src/material_zui/list/__init__.py
+-rw-r--r--   0        0        0     4415 2023-07-30 13:24:18.913364 material_zui-0.1.4/src/material_zui/list/common.py
+-rw-r--r--   0        0        0      154 2023-07-30 13:24:35.996722 material_zui-0.1.4/src/material_zui/list/index.py
+-rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.4/src/material_zui/log/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.4/src/material_zui/log/index.py
+-rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.4/src/material_zui/log/log.py
+-rw-r--r--   0        0        0       21 2023-07-29 03:49:37.553797 material_zui-0.1.4/src/material_zui/network/__init__.py
+-rw-r--r--   0        0        0     2606 2023-07-31 06:13:07.060055 material_zui-0.1.4/src/material_zui/network/common.py
+-rw-r--r--   0        0        0       70 2023-07-29 11:25:06.057119 material_zui-0.1.4/src/material_zui/network/index.py
+-rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.4/src/material_zui/number/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-29 05:39:04.869919 material_zui-0.1.4/src/material_zui/number/common.py
+-rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.4/src/material_zui/number/index.py
+-rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.4/src/material_zui/os/__init__.py
+-rw-r--r--   0        0        0      840 2023-07-12 02:26:10.443342 material_zui-0.1.4/src/material_zui/os/common.py
+-rw-r--r--   0        0        0      125 2023-07-12 02:29:41.294270 material_zui-0.1.4/src/material_zui/os/index.py
+-rw-r--r--   0        0        0      330 2023-07-12 02:54:51.769004 material_zui-0.1.4/src/material_zui/os/terminal.py
+-rw-r--r--   0        0        0     1250 2023-07-29 05:39:04.697919 material_zui-0.1.4/src/material_zui/readme.md
+-rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.4/src/material_zui/regex/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.4/src/material_zui/regex/index.py
+-rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.4/src/material_zui/replicate/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.4/src/material_zui/replicate/index.py
+-rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.4/src/material_zui/selenium/__init__.py
+-rw-r--r--   0        0        0     4155 2023-07-31 01:53:50.526065 material_zui-0.1.4/src/material_zui/selenium/chrome.py
+-rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.4/src/material_zui/selenium/common.py
+-rw-r--r--   0        0        0     2836 2023-07-30 03:31:40.599764 material_zui-0.1.4/src/material_zui/selenium/firefox.py
+-rw-r--r--   0        0        0      150 2023-07-16 03:36:28.421675 material_zui-0.1.4/src/material_zui/selenium/index.py
+-rw-r--r--   0        0        0     9288 2023-07-30 03:32:09.290158 material_zui-0.1.4/src/material_zui/selenium/selenium.py
+-rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.4/src/material_zui/setup.py
+-rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.4/src/material_zui/string/__init__.py
+-rw-r--r--   0        0        0     3403 2023-07-29 11:24:14.277396 material_zui-0.1.4/src/material_zui/string/common.py
+-rw-r--r--   0        0        0      345 2023-07-29 11:24:14.137397 material_zui-0.1.4/src/material_zui/string/index.py
+-rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.4/src/material_zui/telegram_bot/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.4/src/material_zui/telegram_bot/index.py
+-rw-r--r--   0        0        0       21 2023-07-29 05:45:31.405279 material_zui-0.1.4/src/material_zui/thread/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-30 14:11:11.539245 material_zui-0.1.4/src/material_zui/thread/common.py
+-rw-r--r--   0        0        0       37 2023-07-29 05:53:44.309345 material_zui-0.1.4/src/material_zui/thread/index.py
+-rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.4/src/material_zui/tmp/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.4/src/material_zui/tmp/index.py
+-rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.4/src/material_zui/utility/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.4/src/material_zui/utility/common.py
+-rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.4/src/material_zui/utility/index.py
+-rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.4/src/material_zui/validate/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.4/src/material_zui/validate/common.py
+-rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.4/src/material_zui/validate/index.py
+-rw-r--r--   0        0        0     2944 1970-01-01 00:00:00.000000 material_zui-0.1.4/PKG-INFO
```

### Comparing `material_zui-0.1.3/pyproject.toml` & `material_zui-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "material_zui"
-version = "0.1.3"
+version = "0.1.4"
 description = "Material Zui"
 authors = ["chauhmnguyen <chauhoangminhnguyen@gmail.com>"]
 readme = "src/material_zui/readme.md"
 keywords = [
 	"material",
 	"zui",
 	"material zui",
@@ -39,14 +39,16 @@
 validators = "^0.20.0"
 edgegpt = "^0.11.6"
 setuptools = "^67.8.0"
 xlsxwriter = "^3.1.2"
 youtube-dl = "^2021.12.17"
 langchain = "^0.0.216"
 huggingface-hub = "^0.15.1"
+streamlit = "^1.24.1"
+free-proxy = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `material_zui-0.1.3/src/material_zui/ResizeImage.py` & `material_zui-0.1.4/src/material_zui/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/bard/google_bard.py` & `material_zui-0.1.4/src/material_zui/bard/google_bard.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/bing_ai/bing_ai.py` & `material_zui-0.1.4/src/material_zui/bing_ai/bing_ai.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/bing_ai/result.py` & `material_zui-0.1.4/src/material_zui/bing_ai/result.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/compress/text.py` & `material_zui-0.1.4/src/material_zui/compress/text.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/crawl/image.py` & `material_zui-0.1.4/src/material_zui/crawl/image.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/crontab/index.py` & `material_zui-0.1.4/src/material_zui/crontab/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/file/check.py` & `material_zui-0.1.4/src/material_zui/file/check.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/file/common.py` & `material_zui-0.1.4/src/material_zui/file/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/file/excel.py` & `material_zui-0.1.4/src/material_zui/file/excel.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/file/read.py` & `material_zui-0.1.4/src/material_zui/file/read.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/file/write.py` & `material_zui-0.1.4/src/material_zui/file/write.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/generate/common.py` & `material_zui-0.1.4/src/material_zui/generate/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,10 +53,8 @@
     def ask(self, ask: str) -> str:
         template = """Question: {query}
         Answer: Let's think step by step."""
         prompt = PromptTemplate(template=template, input_variables=["query"])
         llm = HuggingFaceHub(repo_id="google/flan-t5-xxl",
                              model_kwargs={"temperature": 0.1})  # type: ignore
         llm_chain = LLMChain(prompt=prompt, llm=llm)
-        # query = "When was America discovered?"
-        # query = "What the nodejs latest version?"
         return llm_chain.run(ask)
```

### Comparing `material_zui-0.1.3/src/material_zui/gpt/gpt_vietnam.py` & `material_zui-0.1.4/src/material_zui/gpt/gpt_vietnam.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/colorization.py` & `material_zui-0.1.4/src/material_zui/image/colorization.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/combine.py` & `material_zui-0.1.4/src/material_zui/image/combine.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/common.py` & `material_zui-0.1.4/src/material_zui/image/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/convert.py` & `material_zui-0.1.4/src/material_zui/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/model/colorization_deploy_v2.prototxt` & `material_zui-0.1.4/src/material_zui/image/model/colorization_deploy_v2.prototxt`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/model/pts_in_hull.npy` & `material_zui-0.1.4/src/material_zui/image/model/pts_in_hull.npy`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/remove_background.py` & `material_zui-0.1.4/src/material_zui/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/to_svg.py` & `material_zui-0.1.4/src/material_zui/image/to_svg.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/transparent_background.py` & `material_zui-0.1.4/src/material_zui/image/transparent_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/image/upscale.py` & `material_zui-0.1.4/src/material_zui/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/log/log.py` & `material_zui-0.1.4/src/material_zui/log/log.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/os/os.py` & `material_zui-0.1.4/src/material_zui/os/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/readme.md` & `material_zui-0.1.4/src/material_zui/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
       <li>upscale</li>
       <li>convert to jpg/png</li>
     </ul>
   </li>
   <li>list</li>
   <!-- <li><a href="#log">Log</a></li> -->
   <li>log</li>
+  <li>network</li>
+  <li>number</li>
   <li>os</li>
   <li>regex</li>
   <li>replicate: AI Platform API</li>
   <li>selenium</li>
   <li>string</li>
   <li>telegram_bot</li>
   <li>utility</li>
```

#### html2text {}

```diff
@@ -14,16 +14,18 @@
           o colorization
           o sketch
           o transparent background
           o upscale
           o convert to jpg/png
   12. list
   13. log
-  14. os
-  15. regex
-  16. replicate: AI Platform API
-  17. selenium
-  18. string
-  19. telegram_bot
-  20. utility
-  21. validate
+  14. network
+  15. number
+  16. os
+  17. regex
+  18. replicate: AI Platform API
+  19. selenium
+  20. string
+  21. telegram_bot
+  22. utility
+  23. validate
   # Package - https://pypi.org/project/material-zui
```

### Comparing `material_zui-0.1.3/src/material_zui/regex/index.py` & `material_zui-0.1.4/src/material_zui/regex/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/replicate/index.py` & `material_zui-0.1.4/src/material_zui/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/selenium/chrome.py` & `material_zui-0.1.4/src/material_zui/selenium/selenium.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 import os
 import platform
 from typing import Any
+
 from bs4 import BeautifulSoup
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.support.wait import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.remote.webelement import WebElement
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.wait import WebDriverWait
 
-from material_zui.selenium.common import safe_find_element
 from material_zui.fake import random_sleep
-from material_zui.list import map_to
+from material_zui.list import filter_to, map_to
+from material_zui.string import (list_match, remove_bmp_characters,
+                                 remove_special_characters, trim_space)
+from material_zui.string.common import remove_all
+from material_zui.utility import pipe, pipe_list
+
+from .common import safe_find_element
+
+# from selenium.webdriver.chrome.webdriver import WebDriver
 
 
-class Zui_Selenium_Chrome:
-    def __init__(self) -> None:
+class ZuiSelenium:
+    # driver: WebDriver
+    driver: Any
+
+    def __init__(self, driver: Any = None) -> None:
         self.is_mac = False
         if not any(os_name in platform.platform() for os_name in ["Windows", "Linux"]):
             self.is_mac = True
+        if driver:
+            self.driver = driver
+
+    # def __init__(self) -> None:
+    #     self.is_mac = False
+    #     if not any(os_name in platform.platform() for os_name in ["Windows", "Linux"]):
+    #         self.is_mac = True
 
     @property
     def screen_height(self) -> int:
         return self.driver.execute_script("return window.screen.height;")
 
     @property
     def scroll_height(self) -> int:
@@ -32,34 +48,22 @@
     @property
     def page_source(self) -> str: return self.driver.page_source
 
     @property
     def document(self) -> BeautifulSoup:
         return BeautifulSoup(self.driver.page_source, "html.parser")
 
-    def connect(self):
-        self.driver = webdriver.Chrome()
-        return self.driver
-
-    def connect_debug(self, port: int = 9000, debug_address: str = ''):
-        '''
-        @port: port number, default `9000`
-        @debug_address: format `127.0.0.1:9000`, default `localhost:{port}`
-        - Use for case need authorization, you just need to start `chrome beta` -> login account -> close browswer then
-            - start `chrome` on debug mode -> call this method to connect to browser opened
-        1. Install `chrome beta` for better automation: https://www.google.com/chrome/beta
-        2. Start `chrome` by command: `google-chrome-beta --remote-debugging-port={port}`
-                - `port` must the same with input parameter of this method
-        '''
-        debug_address = debug_address or f"localhost:{port}"
-        self.options = Options()
-        self.options.add_experimental_option(
-            "debuggerAddress", debug_address)
-        self.driver = webdriver.Chrome(options=self.options)
-        return self.driver
+    @property
+    def current_url(self) -> str: return self.driver.current_url
+
+    def get(self, url: str) -> None:
+        self.driver.get(url)
+
+    def close(self) -> None:
+        self.driver.close()
 
     def delay(self, sec: float = 0) -> None:
         random_sleep(1, 5, sec)
 
     def safe_find_element(
             self, by: str = By.ID,
             value: str | None = None,
@@ -69,21 +73,25 @@
         @return `None` in case not found
         '''
         return safe_find_element(parent if parent else self.driver, by, value)
 
     def safe_find_element_by_xpath(self, xpath_value: str) -> WebElement | None:
         return self.safe_find_element(By.XPATH, xpath_value)
 
-    def find_element_by_xpath(self, xpath_value: str): return self.driver.find_element(
+    def safe_get_text(self, xpath_value: str) -> str:
+        element = self.safe_find_element_by_xpath(xpath_value)
+        return element.text if element else ''
+
+    def find_element_by_xpath(self, xpath_value: str) -> WebElement: return self.driver.find_element(
         By.XPATH, xpath_value)
 
-    def find_elements_by_xpath(self, xpath_value: str): return self.driver.find_elements(
+    def find_elements_by_xpath(self, xpath_value: str) -> list[WebElement]: return self.driver.find_elements(
         By.XPATH, xpath_value)
 
-    def find_elements_by_class(self, class_value: str): return self.driver.find_elements(
+    def find_elements_by_class(self, class_value: str) -> list[WebElement]: return self.driver.find_elements(
         By.CLASS_NAME, class_value)
 
     def scroll_to_end(self) -> None:
         self.driver.execute_script("window.scrollTo(0, {scroll_height});".format(
             scroll_height=self.scroll_height))
 
     def scroll(self, step_scroll: int) -> None:
@@ -120,52 +128,121 @@
         '''
         Click then return that element
         '''
         element = self.find_element_by_xpath(xpath_value)
         element.click()
         return element
 
+    def wait_click(self, xpath_value: str, delay_time: int = 10, time_to_try: int = 10):
+        element = self.wait_get(xpath_value, delay_time, time_to_try)
+        element.click()
+        return element
+
     def safe_click(self, xpath_value: str):
         '''
         Safe click element
         '''
         try:
             element = self.safe_find_element_by_xpath(xpath_value)
             if element:
                 element.click()
             return element
         except:
             return None
 
-    def send_keys(self, xpath_value: str, key_value: str, clear_before_send_keys: bool = True, delay_time: int = 10):
+    def send_keys(self, xpath_value: str, key_value: str, clear_before_send_keys: bool = True, delay_time: int = 10, time_to_try: int = 10) -> WebElement | None:
         '''
         Send keys then return that element
         @xpath_value: only valid with element selector can input value
         @clear_before_send_keys:
         - True: clear input before send keys
         - False: value will input after existed value
         '''
-        # element = self.find_element_by_xpath(xpath_value)
-        element = self.wait_get(xpath_value, delay_time)
-        element.click()
-        if clear_before_send_keys:
-            element.send_keys(Keys.CONTROL + 'a')
-            element.send_keys(Keys.BACKSPACE)
-        element.send_keys(key_value)
-        return element
+        try:
+            element = self.wait_get(xpath_value, delay_time, time_to_try)
+            # element = self.find_element_by_xpath(xpath_value)
+            element.click()
+            self.delay(10)
+            if clear_before_send_keys:
+                element.send_keys(Keys.CONTROL + 'a')
+                self.delay()
+                element.send_keys(Keys.BACKSPACE)
+            self.delay()
+            element.send_keys(key_value)
+            return element
+        except:
+            if time_to_try:
+                time_to_try -= 1
+                return self.send_keys(xpath_value, key_value,
+                                      clear_before_send_keys, delay_time, time_to_try)
+            return None
 
-    # def wait_get(self, xpath_value: str, delay_time: int = 10) -> WebElement:
-    #     element: Any = WebDriverWait(self.driver, delay_time).until(  # using explicit wait for 10 seconds
-    #         EC.presence_of_element_located(
-    #             (By.XPATH, xpath_value))  # finding the element
-    #     )
+    # def send_keys(self, xpath_value: str, key_value: str, clear_before_send_keys: bool = True, delay_time: int = 10, time_to_try: int = 10):
+    #     '''
+    #     Send keys then return that element
+    #     @xpath_value: only valid with element selector can input value
+    #     @clear_before_send_keys:
+    #     - True: clear input before send keys
+    #     - False: value will input after existed value
+    #     '''
+    #     element = self.wait_get(xpath_value, delay_time, time_to_try)
+    #     # element = self.find_element_by_xpath(xpath_value)
+    #     element.click()
+    #     self.delay(10)
+    #     if clear_before_send_keys:
+    #         element.send_keys(Keys.CONTROL + 'a')
+    #         self.delay()
+    #         element.send_keys(Keys.BACKSPACE)
+    #     self.delay()
+    #     element.send_keys(key_value)
     #     return element
+
     def wait_get(self, xpath_value: str, delay_time: int = 10, time_to_try: int = 10) -> WebElement:
+        '''
+        - Total wait time of this function is `delay_time x time_to_try`, default is `10x10 = 100 seconds`
+        - @delay_time: delay time for each `time_to_try`
+        - @time_to_try: how many time to try
+        '''
         for _ in range(time_to_try):
             element = self.safe_find_element_by_xpath(xpath_value)
             if element:
                 return element
             self.delay(delay_time)
         return WebDriverWait(self.driver, delay_time).until(  # using explicit wait for 10 seconds
             EC.presence_of_element_located(
                 (By.XPATH, xpath_value))  # finding the element
         )
+
+    def input_tags(self, tags: list[str], title_element: WebElement | None = None, xpath_value: str = '') -> None:
+        title_element = title_element or self.wait_get(xpath_value)
+        if tags and len(tags):
+            title_element.send_keys(Keys.SPACE)
+            for tag in tags:
+                title_element.send_keys(tag)
+                self.delay()
+                title_element.send_keys(Keys.SPACE)
+
+    def split_title(self, title: str) -> dict[{'title': str, 'caption': str, 'yt_description': str, 'tags': list[str], 'hash_tags': list[str]}]:
+        '''
+        '''
+        valid_title = pipe(
+            remove_bmp_characters,
+            trim_space
+        )(title)
+        caption = pipe(
+            remove_all(r' \#.+'),
+            trim_space
+        )(valid_title)
+        yt_description = remove_all(r'>')(caption)
+
+        raw_tags = pipe_list(remove_special_characters, trim_space)(
+            list_match('(#)([^ ]+)', 2)(valid_title.strip('#')))
+        tags = filter_to(raw_tags, lambda tag, _: len(tag) > 1)
+        hash_tags = map_to(tags, lambda tag, _: f'#{tag}')
+
+        return {
+            'title': valid_title,
+            'caption': caption,
+            'yt_description': yt_description,
+            'tags': tags,
+            'hash_tags': hash_tags,
+        }
```

### Comparing `material_zui-0.1.3/src/material_zui/setup.py` & `material_zui-0.1.4/src/material_zui/setup.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/src/material_zui/string/common.py` & `material_zui-0.1.4/src/material_zui/string/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,56 @@
-from re import finditer, compile
+from re import compile, finditer
 from typing import Any, Callable
 
-from material_zui.list import map_to, filter_to
-
-
-# def list_match(value: str, regex: str, group: int = 0) -> list[str]:
-#     pattern = compile(regex)
-#     items = map_to(list(finditer(pattern, value)),
-#                    lambda match, _: match.group(group))
-#     return filter_to(items, lambda item, _: len(item) > 0)
+from material_zui.list import filter_to, map_to
 
 
 def list_match(regex: str, group: int = 0) -> Callable[[str], list[str]]:
+    '''
+    - ex:
+
+    ```py
+    list_match('(#)([^ ]+)', 2)("title #tag1 #tag2 #tag3") => ['tag', 'tag2', 'tag3']
+    ```
+    '''
     pattern = compile(regex)
 
     def matcher(value: str) -> list[str]:
         items = map_to(list(finditer(pattern, value)),
                        lambda match, _: match.group(group))
         return filter_to(items, lambda item, _: len(item) > 0)
     return matcher
 
-# def remove_all(text: str, regex_pattern_to_remove: str) -> str:
-#     pattern = compile(regex_pattern_to_remove)
-#     return pattern.sub('', text)
-
-# def remove_all(regex_pattern_to_remove: str) -> Callable[[str], str]:
-#     pattern = compile(regex_pattern_to_remove)
-#     def remove_all_impl(text: str) -> str:
-#         return pattern.sub('', text)
-#     return remove_all_impl
+
+def is_exist(regex: str) -> Callable[[str], bool]:
+    pattern = compile(regex)
+    return lambda value: bool(pattern.search(value))
+
+# def is_exist(value: str, regex: str) -> bool:
+#     pattern = compile(regex)
+#     return bool(pattern.search(value))
+
+# def check_substring(string, substring):
+#     regex = re.compile(substring)
+#     if regex.search(string):
+#         return True
+#     else:
+#         return False
 
 
 def remove_all(regex_pattern_to_remove: str) -> Callable[[str], str]:
     pattern = compile(regex_pattern_to_remove)
     return lambda text: pattern.sub('', text)
 
 
+def replace_all(regex_pattern: str, replace_value: str) -> Callable[[str], str]:
+    pattern = compile(regex_pattern)
+    return lambda text: pattern.sub(replace_value, text)
+
+
 def remove_special_characters(text: str) -> str:
     """
     The function removes all special characters from a given string.
 
     @param text: The input text string that may contain special characters
     @type text: str
     @return: The function `remove_special_characters` takes a string `text` as input and removes all
@@ -65,13 +76,30 @@
     consecutive spaces within the string with a single space.
 
     :param text: A string that may contain extra spaces that need to be trimmed down to a single space
     :type text: str
     :return: The function `trim_space` takes a string `text` as input and returns a new string with all
     consecutive spaces replaced by a single space, and leading/trailing spaces removed.
     """
-    pattern = compile('  ')
-    return pattern.sub(' ', text.strip())
+    return replace_all(r' +', ' ')(text)
 
 
 def not_empty(value: Any) -> bool:
     return value != None and len(value) > 0
+
+
+def limit_by_byte(byte_limit: int = 256) -> Callable[[str], str]:
+    """Limits the length of a string by byte count.
+    Args:
+      byte_limit: The maximum number of bytes allowed.
+    Returns:
+      A function that takes a string and returns the limited string.
+    """
+    def inner_function(value: str) -> str:
+        return value.encode()[:byte_limit].decode() if len(value.encode()) > byte_limit else value
+    return inner_function
+
+
+def count_byte(value: str) -> int: return len(value.encode())
+
+
+def to_string(value: Any) -> str: return str(value)
```

### Comparing `material_zui-0.1.3/src/material_zui/utility/common.py` & `material_zui-0.1.4/src/material_zui/utility/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.3/PKG-INFO` & `material_zui-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.1.3
+Version: 0.1.4
 Summary: Material Zui
 Keywords: material,zui,material zui,zui material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bardapi (>=0.1.2,<0.2.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: edgegpt (>=0.11.6,<0.12.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: free-proxy (>=1.1.1,<2.0.0)
 Requires-Dist: huggingface-hub (>=0.15.1,<0.16.0)
 Requires-Dist: langchain (>=0.0.216,<0.0.217)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: multipledispatch (>=0.6.0,<0.7.0)
 Requires-Dist: newspaper3k (>=0.2.8,<0.3.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
@@ -28,14 +29,15 @@
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: rembg (>=2.0.36,<3.0.0)
 Requires-Dist: replicate (>=0.8.1,<0.9.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: selenium (>=4.9.1,<5.0.0)
 Requires-Dist: selenium-browser (>=0.0.15,<0.0.16)
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
+Requires-Dist: streamlit (>=1.24.1,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Requires-Dist: xlsxwriter (>=3.1.2,<4.0.0)
 Requires-Dist: youtube-dl (>=2021.12.17,<2022.0.0)
 Description-Content-Type: text/markdown
 
 # Modules
@@ -62,14 +64,16 @@
       <li>upscale</li>
       <li>convert to jpg/png</li>
     </ul>
   </li>
   <li>list</li>
   <!-- <li><a href="#log">Log</a></li> -->
   <li>log</li>
+  <li>network</li>
+  <li>number</li>
   <li>os</li>
   <li>regex</li>
   <li>replicate: AI Platform API</li>
   <li>selenium</li>
   <li>string</li>
   <li>telegram_bot</li>
   <li>utility</li>
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: material-zui Version: 0.1.3 Summary: Material Zui
+Metadata-Version: 2.1 Name: material-zui Version: 0.1.4 Summary: Material Zui
 Keywords: material,zui,material zui,zui material Author: chauhmnguyen Author-
 email: chauhoangminhnguyen@gmail.com Requires-Python: >=3.10,<3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Requires-Dist: bardapi (>=0.1.2,<0.2.0) Requires-Dist: beautifulsoup4
 (>=4.12.2,<5.0.0) Requires-Dist: edgegpt (>=0.11.6,<0.12.0) Requires-Dist:
-flask (>=2.3.2,<3.0.0) Requires-Dist: huggingface-hub (>=0.15.1,<0.16.0)
-Requires-Dist: langchain (>=0.0.216,<0.0.217) Requires-Dist: matplotlib
-(>=3.7.1,<4.0.0) Requires-Dist: multipledispatch (>=0.6.0,<0.7.0) Requires-
-Dist: newspaper3k (>=0.2.8,<0.3.0) Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0) Requires-Dist: pandas
-(>=2.0.1,<3.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
-pytelegrambotapi (>=4.11.0,<5.0.0) Requires-Dist: python-crontab
-(>=2.7.1,<3.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist:
-pythonlangutil (>=0.1,<0.2) Requires-Dist: pytube (>=15.0.0,<16.0.0) Requires-
-Dist: rembg (>=2.0.36,<3.0.0) Requires-Dist: replicate (>=0.8.1,<0.9.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0) Requires-Dist: selenium
-(>=4.9.1,<5.0.0) Requires-Dist: selenium-browser (>=0.0.15,<0.0.16) Requires-
-Dist: setuptools (>=67.8.0,<68.0.0) Requires-Dist: validators
-(>=0.20.0,<0.21.0) Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0) Requires-
-Dist: xlsxwriter (>=3.1.2,<4.0.0) Requires-Dist: youtube-dl
-(>=2021.12.17,<2022.0.0) Description-Content-Type: text/markdown # Modules
+flask (>=2.3.2,<3.0.0) Requires-Dist: free-proxy (>=1.1.1,<2.0.0) Requires-
+Dist: huggingface-hub (>=0.15.1,<0.16.0) Requires-Dist: langchain
+(>=0.0.216,<0.0.217) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist:
+multipledispatch (>=0.6.0,<0.7.0) Requires-Dist: newspaper3k (>=0.2.8,<0.3.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0) Requires-Dist: opencv-python
+(>=4.7.0.72,<5.0.0.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist:
+pillow (>=9.5.0,<10.0.0) Requires-Dist: pytelegrambotapi (>=4.11.0,<5.0.0)
+Requires-Dist: python-crontab (>=2.7.1,<3.0.0) Requires-Dist: python-dotenv
+(>=1.0.0,<2.0.0) Requires-Dist: pythonlangutil (>=0.1,<0.2) Requires-Dist:
+pytube (>=15.0.0,<16.0.0) Requires-Dist: rembg (>=2.0.36,<3.0.0) Requires-Dist:
+replicate (>=0.8.1,<0.9.0) Requires-Dist: requests (>=2.30.0,<3.0.0) Requires-
+Dist: selenium (>=4.9.1,<5.0.0) Requires-Dist: selenium-browser
+(>=0.0.15,<0.0.16) Requires-Dist: setuptools (>=67.8.0,<68.0.0) Requires-Dist:
+streamlit (>=1.24.1,<2.0.0) Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0) Requires-Dist: xlsxwriter
+(>=3.1.2,<4.0.0) Requires-Dist: youtube-dl (>=2021.12.17,<2022.0.0)
+Description-Content-Type: text/markdown # Modules
    1. bard
    2. bing_ai
    3. compress
    4. crawl
    5. crontab
    6. date_time
    7. env
@@ -35,16 +36,18 @@
           o colorization
           o sketch
           o transparent background
           o upscale
           o convert to jpg/png
   12. list
   13. log
-  14. os
-  15. regex
-  16. replicate: AI Platform API
-  17. selenium
-  18. string
-  19. telegram_bot
-  20. utility
-  21. validate
+  14. network
+  15. number
+  16. os
+  17. regex
+  18. replicate: AI Platform API
+  19. selenium
+  20. string
+  21. telegram_bot
+  22. utility
+  23. validate
   # Package - https://pypi.org/project/material-zui
```

