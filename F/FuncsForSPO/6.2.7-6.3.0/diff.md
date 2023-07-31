# Comparing `tmp/FuncsForSPO-6.2.7.tar.gz` & `tmp/FuncsForSPO-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-6.2.7.tar", last modified: Tue Jul  4 20:16:04 2023, max compression
+gzip compressed data, was "FuncsForSPO-6.3.0.tar", last modified: Mon Jul 31 12:53:04 2023, max compression
```

## Comparing `FuncsForSPO-6.2.7.tar` & `FuncsForSPO-6.3.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:04.019993 FuncsForSPO-6.2.7/
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.504599 FuncsForSPO-6.2.7/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.588350 FuncsForSPO-6.2.7/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.2.7/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.2.7/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.599235 FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.608266 FuncsForSPO-6.2.7/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.2.7/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.628019 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/
--rw-rw-rw-   0        0        0      886 2023-06-24 20:49:12.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/__fgpt.py
--rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/__init__.py
--rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/base.py
--rw-rw-rw-   0        0        0    14672 2023-06-26 14:09:10.000000 FuncsForSPO-6.2.7/FuncsForSPO/fgpt/fgpt.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.634030 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.658398 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/__translator.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/base.py
--rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.668397 FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.675579 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.720393 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0    11162 2023-06-28 17:53:11.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3579 2023-06-28 17:15:41.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
--rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
--rw-rw-rw-   0        0        0     1340 2023-06-28 13:21:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
--rw-rw-rw-   0        0        0      616 2023-06-29 19:53:08.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.738697 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.756227 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.760223 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.790744 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
--rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/base.py
--rw-rw-rw-   0        0        0     9951 2023-06-30 12:26:15.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.801751 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.812751 FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.824274 FuncsForSPO-6.2.7/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    55610 2023-06-26 14:09:24.000000 FuncsForSPO-6.2.7/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.897161 FuncsForSPO-6.2.7/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.2.7/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.917198 FuncsForSPO-6.2.7/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38845 2023-07-04 20:15:36.000000 FuncsForSPO-6.2.7/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.933110 FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.943282 FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.951277 FuncsForSPO-6.2.7/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.2.7/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 20:16:03.577374 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8023 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2127 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      475 2023-07-04 20:16:03.000000 FuncsForSPO-6.2.7/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.2.7/LICENSE
--rw-rw-rw-   0        0        0     8023 2023-07-04 20:16:04.014471 FuncsForSPO-6.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 20:16:04.019993 FuncsForSPO-6.2.7/setup.cfg
--rw-rw-rw-   0        0        0     2663 2023-07-04 20:15:51.000000 FuncsForSPO-6.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.430457 FuncsForSPO-6.3.0/
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.858463 FuncsForSPO-6.3.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.933522 FuncsForSPO-6.3.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-6.3.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-6.3.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.946044 FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.958043 FuncsForSPO-6.3.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-6.3.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.982107 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/
+-rw-rw-rw-   0        0        0     2127 2023-07-08 15:03:37.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/__fgpt.py
+-rw-rw-rw-   0        0        0        0 2023-06-24 21:16:46.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/__init__.py
+-rw-rw-rw-   0        0        0     2419 2023-06-09 19:08:44.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/base.py
+-rw-rw-rw-   0        0        0    14957 2023-07-08 15:04:45.000000 FuncsForSPO-6.3.0/FuncsForSPO/fgpt/fgpt.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.989436 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.012457 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0     4400 2023-06-20 16:22:20.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/__translator.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/base.py
+-rw-rw-rw-   0        0        0      829 2023-06-20 16:21:06.000000 FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.024956 FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.032239 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.105939 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0    13836 2023-07-21 12:08:34.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3602 2023-07-20 21:51:33.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1138 2023-06-09 17:41:46.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2024 2023-07-21 11:40:46.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+-rw-rw-rw-   0        0        0     1173 2023-07-21 11:45:44.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py
+-rw-rw-rw-   0        0        0      616 2023-06-29 19:53:08.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.124682 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.142408 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.151045 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.185177 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     8709 2023-06-18 14:37:35.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     1034 2023-06-18 14:17:07.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py
+-rw-rw-rw-   0        0        0     2482 2023-06-18 01:12:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/base.py
+-rw-rw-rw-   0        0        0    10234 2023-07-31 12:52:24.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.203973 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-06-18 14:25:59.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.224274 FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4696 2023-06-24 21:08:38.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.238057 FuncsForSPO-6.3.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    56235 2023-07-18 20:57:07.000000 FuncsForSPO-6.3.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.254740 FuncsForSPO-6.3.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10378 2023-06-24 21:07:45.000000 FuncsForSPO-6.3.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.269942 FuncsForSPO-6.3.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    38845 2023-07-04 20:15:36.000000 FuncsForSPO-6.3.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.288144 FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.300831 FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:04.306859 FuncsForSPO-6.3.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   122169 2023-06-24 20:59:57.000000 FuncsForSPO-6.3.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:53:03.922815 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8023 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2127 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      475 2023-07-31 12:53:03.000000 FuncsForSPO-6.3.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-6.3.0/LICENSE
+-rw-rw-rw-   0        0        0     8023 2023-07-31 12:53:04.426752 FuncsForSPO-6.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7604 2023-06-20 16:05:40.000000 FuncsForSPO-6.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:53:04.430457 FuncsForSPO-6.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2663 2023-07-31 12:52:49.000000 FuncsForSPO-6.3.0/setup.py
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/femails/femails.py` & `FuncsForSPO-6.3.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fgpt/__fgpt.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fgpt/__fgpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,43 @@
     def __init__(self, prompt, headless):
         self.PROMPT = prompt
         self.HEADLESS = headless
         super().__init__(headless)
         
     def run(self):
         self.DRIVER.get('https://chat.chatgptdemo.net/')
-        espera_elemento_e_envia_send_keys(self.WDW, 'coloque no final "GPT_RESPOSTA" '+self.PROMPT, (By.CSS_SELECTOR, '#input-chat'))
-        espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'div.send-button'))
-        tentativas = 20
-        while tentativas != 0:
-            text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'pre[class="chat-content chat-response"]'))
-            if 'GPT_RESPOSTA' in text:
+        if isinstance(self.PROMPT, str):
+            espera_elemento_e_envia_send_keys(self.WDW, 'coloque no final "GPT_RESPOSTA" '+self.PROMPT, (By.CSS_SELECTOR, '#input-chat'))
+            espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'div.send-button'))
+            tentativas = 20
+            while tentativas != 0:
+                text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'pre[class="chat-content chat-response"]'))
+                if 'GPT_RESPOSTA' in text:
+                    return text
+                else:
+                    sleep(1)
+                    tentativas -= 1
+            else:
                 return text
+        if isinstance(self.PROMPT, dict):
+            response = {}
+            for chave, valor in self.PROMPT.items():
+                faz_log(f'Fazendo pergunta {chave}: {valor}')
+                espera_elemento_e_envia_send_keys(self.WDW, 'Adicione "GPT_RESPOSTA" apenas no final da sua resposta! '+valor, (By.CSS_SELECTOR, '#input-chat'))
+                espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'div.send-button'))
+                tentativas = 20
+                while tentativas != 0:
+                    try:
+                        text = espera_e_retorna_lista_de_elementos(self.WDW, (By.CSS_SELECTOR, 'pre[class="chat-content chat-response"]'))[-1].text
+                    except:
+                        sleep(1)
+                        tentativas -= 1
+                    if 'GPT_RESPOSTA' in text:
+                        response[chave] = text
+                        break
+                    else:
+                        sleep(1)
+                        tentativas -= 1
+                else:
+                    response[chave] = text
             else:
-                sleep(1)
-                tentativas -= 1
-        else:
-            return text
+                return response
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fgpt/base.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fgpt/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fgpt/fgpt.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fgpt/fgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,25 @@
     :param prompt: A string representing the prompt to generate text from.
     :type prompt: str
     :param headless: A boolean flag indicating whether to run the bot in headless mode. Defaults to False.
     :type headless: bool
     :return: A string representing the generated text.
     :rtype: str
     """
-    prompt = re.sub(r'[\n\t\r\f\v\\]', '', prompt)
-    app = GPTBot(prompt, headless)
-    return app.run().replace("GPT_RESPOSTA", '').strip()
+    if isinstance(prompt, str):
+        prompt = re.sub(r'[\n\t\r\f\v\\]', '', prompt)
+        app = GPTBot(prompt, headless)
+        return app.run().replace("GPT_RESPOSTA", '').strip()
+    else:
+        prompt_to_gpt = {}
+        for chave, valor in prompt.items():
+            prompt_to_gpt[chave] = re.sub(r'[\n\t\r\f\v\\]', '', valor)
+        app = GPTBot(prompt_to_gpt, headless)
+        return app.run()
+        
 
 
 def cria_diretorios_para_novo_projeto_python(with_draft=False, create_base_dir:bool=True, packages:str='FuncsForSPO'):
     """# ATENÇÃO, UTILIZAR SOMENTE UMA VEZ NO MOMENTO DA CRIAÇÃO DO NOVO PROJETO!
     
     create_base_dir: cria o diretorio para o user colocar a base
     packages: instala pacotes necessários
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/__translator.py` & `FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/__translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/base.py` & `FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-6.3.0/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,61 +98,106 @@
             self.DRIVER.quit()
             raise ErroPDFAIException
 
 class GPTPDFV2(BotMain):    
     def __init__(self, content_txt: str, prompt:str, headless: bool=True) -> str:
         cria_dir_no_dir_de_trabalho_atual('tempdir')
         self.CONTEXT = content_txt
+        self.PROMPT = prompt
         faz_log('Criando arquivo em uma pasta temporária')
         self.TXT_CONTENT = arquivo_com_caminho_absoluto('tempdir', 'temp.txt')
         with open(self.TXT_CONTENT, 'w', encoding='utf-8') as f:
             f.write(self.CONTEXT.replace('\n', '').replace('\\n', '').replace('\t', '').replace('\\t', ''))
         
-        
-        self.PROMPT = prompt.replace('\n', ' ').replace('\\n', ' ').replace('\t', '').replace('\\t', '')
+        # self.PROMPT = prompt.replace('\n', ' ').replace('\\n', ' ').replace('\t', '').replace('\\t', '')
         self.HEADLESS = headless
         super().__init__(self.HEADLESS)
     
     def run(self):
         try:
             faz_log('Indo para askyourpdf')
             self.DRIVER.get('https://askyourpdf.com/')
             espera_elemento(self.WDW, (By.CSS_SELECTOR, 'input[type="file"]'), in_dom=True)
             self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.TXT_CONTENT)
             
-            faz_log('Documento enviado, aguardando entrada para o prompt')
-            espera_input_limpa_e_envia_send_keys(self.WDW130, self.PROMPT+' Adicione "AI RESPONSE" apenas no final da sua resposta (isso é de suma importância) e deve ser tudo em português!', (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
-            espera_elemento_disponivel_e_clica(self.WDW130, (By.CSS_SELECTOR, 'button[class*="ant-btn-default"]'))
-            faz_log('Esperando a resposta')
-            start_time = time.time()
-            timeout = 180  # Tempo limite em segundos
-
-            while True:
-                try:
-                    text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
-                    faz_log(f'Resposta até agora: [green]{text}[/green]')
-                    time.sleep(7)
-                except:
-                    # Lidar com exceções, se necessário
-                    pass
-
-                if 'AI RES' in text:
-                    break
-                if 'try again.' in text.lower():
-                    text = text + '  Não foi possível ter uma interpretação adequada. Tente outro prompt'
-                    break
-
-                elapsed_time = time.time() - start_time
-                if elapsed_time >= timeout:
-                    # Tempo limite atingido, interromper o loop
-                    break
-            faz_log('Recuperando o id do documento')
-            self.apaga_arquivo_da_base_do_site()
-            self.DRIVER.close()
-            return text
+            if isinstance(self.PROMPT, str):
+                faz_log('Documento enviado, aguardando entrada para o prompt')
+                espera_input_limpa_e_envia_send_keys(self.WDW130, self.PROMPT+' Adicione "GPT_RESPOSTA" apenas no final da sua resposta (isso é de suma importância) e deve ser tudo em português!', (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
+                espera_elemento_disponivel_e_clica(self.WDW130, (By.CSS_SELECTOR, 'button[class*="ant-btn-default"]'))
+                faz_log('Esperando a resposta')
+                start_time = time.time()
+                timeout = 180  # Tempo limite em segundos
+
+                while True:
+                    try:
+                        text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
+                        faz_log(f'Resposta até agora: [green]{text}[/green]')
+                        time.sleep(2)
+                    except:
+                        # Lidar com exceções, se necessário
+                        pass
+
+                    if 'AI RES' in text:
+                        break
+                    if 'try again.' in text.lower():
+                        text = text + '  Não foi possível ter uma interpretação adequada. Tente outro prompt'
+                        break
+
+                    elapsed_time = time.time() - start_time
+                    if elapsed_time >= timeout:
+                        # Tempo limite atingido, interromper o loop
+                        break
+                faz_log('Recuperando o id do documento')
+                self.apaga_arquivo_da_base_do_site()
+                self.DRIVER.close()
+                return text
+            elif isinstance(self.PROMPT, dict):
+                response = {}
+                for chave, valor in self.PROMPT.items():
+                    valor = re.sub(r'[\n\t\r\f\v\\]', '', valor)
+                    
+                    espera_elemento(self.WDW, (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'), in_dom=True)
+                    sleep(2)
+                    self.DRIVER.refresh()
+                    espera_elemento(self.WDW, (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'), in_dom=True)
+                    sleep(5)
+                    
+                    if len(response) == 0:
+                        espera_input_limpa_e_envia_send_keys(self.WDW130, valor+' Adicione "GPT_RESPOSTA" no final da sua resposta para eu saber quando acaba a sua resposta', (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
+                    else:
+                        espera_input_limpa_e_envia_send_keys(self.WDW130, valor+' .Lembre-se de adicionar "GPT_RESPOSTA" no final', (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
+                    espera_elemento_disponivel_e_clica(self.WDW130, (By.CSS_SELECTOR, 'button[class*="ant-btn-default"]'))
+                    faz_log('Esperando a resposta')
+
+
+                    tentativas = 10
+                    while True:
+                        try:
+                            text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
+                            faz_log(f'Resposta até agora: [green]{text}[/green]')
+                            time.sleep(7)
+                        except:
+                            pass
+                        
+                        if 'GPT_RESPOSTA' in text:
+                            response[chave] = text
+                            break
+                        elif tentativas == 1:
+                            response[chave] = text
+                            break
+                        elif 'try again' in text.lower():
+                            response[chave] = text
+                            break
+                        else:
+                            tentativas -= 1
+                            continue
+                faz_log('Recuperando o id do documento')
+                self.apaga_arquivo_da_base_do_site()
+                self.DRIVER.close()
+                return response
         except Exception as e:
             faz_log(repr(e), 'c*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
             self.DRIVER.quit()
             raise ErroPDFAIException
         
     def apaga_arquivo_da_base_do_site(self):
@@ -178,15 +223,15 @@
         try:
             faz_log('Indo para chatpdf')
             self.DRIVER.get('https://www.chatpdf.com/')
             espera_elemento(self.WDW, (By.CSS_SELECTOR, 'input[type="file"]'), in_dom=True)
             self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.FILE_PATH)
             
             faz_log('Documento enviado, aguardando entrada para o prompt')
-            espera_input_limpa_e_envia_send_keys(self.WDW130, self.PROMPT+' Adicione "AI RESPONSE" apenas no final da sua resposta (isso é de suma importância) e deve ser tudo em português!', (By.CSS_SELECTOR, 'textarea[placeholder="Ask any question…"]'))
+            espera_input_limpa_e_envia_send_keys(self.WDW130, self.PROMPT+' Adicione "GPT_RESPOSTA" apenas no final da sua resposta (isso é de suma importância) e deve ser tudo em português!', (By.CSS_SELECTOR, 'textarea[placeholder="Ask any question…"]'))
             espera_elemento_disponivel_e_clica(self.WDW130, (By.CSS_SELECTOR, 'button[type="button"]'))
             faz_log('Esperando a resposta')
             start_time = time.time()
             timeout = 180  # Tempo limite em segundos
 
             while True:
                 try:
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             self._options.add_argument('--disable-gpu')
             self._options.add_argument('--disable-software-rasterizer')
             self._options.add_argument('--incognito')
             self._options.add_argument("--window-size=1920,1080")
             self._options.add_argument('--kiosk-printing')
 
         
-        self.__service = Service(ChromeDriverManager().install())
+        self.__service = Service(ChromeDriverManager(version='114.0.5735.90').install())
         
         # create DRIVER
         self.DRIVER = Chrome(service=self.__service, options=self._options)
 
         self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
         self.WDW5 = WebDriverWait(self.DRIVER, timeout=5)
         self.WDW7 = WebDriverWait(self.DRIVER, timeout=7)
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from FuncsForSPO.fpdf.fanalyser.__pdfanalyser import *
 
-def analyse_pdf_with_gpt(file_pdf:str, prompt:str, headless=True) -> str:
+def analyse_pdf_with_gpt(file_pdf:str, prompt:str, headless=True) -> str|dict:
     """
     DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
 
     https://pdf.ai/
 
     Esse robô envia o PDF para o site e recupera o texto com a resposta do GPT
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from FuncsForSPO.fpdf.fanalyser.__pdfanalyser import *
 
-def analyse_pdf_with_gpt(content_txt:str, prompt:str, headless=True) -> str:
+def analyse_pdf_with_gpt(content_txt:str, prompt:str|dict, headless=True) -> str:
     """
     DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
 
     https://askyourpdf.com/
     
 	Takes in a string of PDF content, a prompt for the GPT model, and a boolean flag indicating whether to run the 
 	model in headless mode or not. Returns a string with the result of running the GPT model on the provided PDF 
@@ -21,8 +21,10 @@
 	
 	:return: A string with the result of running the GPT model on the provided PDF content
 	:rtype: str
 	"""
     # CREDENTIALS EXEMPLE -> (username, password)
     app = GPTPDFV2(content_txt=content_txt, prompt=prompt, headless=headless)
     text = app.run()
-    return text.replace('Olá, eu sou uma assistente de documentos multilíngue e estou aqui para ajudá-lo com qualquer dúvida que você possa ter sobre o documento que você enviou. ', '')
+    return text
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v4.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/__ocr_online_v2.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/__ocr_online_v2.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/base.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/focr/orc.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,24 +160,25 @@
                 raise ErroAPI('ErroAPI')
             if response_json.get('status') == 'finalizado':
                 return response_json.get('result')
             else:
                 print(response_json.get('status'))
 
 
-def ocr_tesseract(pdf, dpi=300, file_output=uuid.uuid4(), return_text=True, config_tesseract=''):
+def ocr_tesseract(pdf, dpi=300, file_output=uuid.uuid4(), return_text=True, config_tesseract='', limit_pages=None):
     """
     Perform optical character recognition (OCR) on a PDF using Tesseract.
 
     Args:
         pdf (str): The path to the input PDF file.
         dpi (int, optional): The resolution in dots per inch (DPI) for the OCR process. Defaults to 300.
         file_output (str, optional): The output file name for the OCR result. Defaults to a randomly generated UUID.
         return_text (bool, optional): Specifies whether to return the OCR result as a string directly in the code or as the path to the output file. Defaults to True.
         config_tesseract (str, optional): Additional configuration options for Tesseract. Defaults to an empty string.
+        limit_pages (int, optional): Maximum number of pages to process. If None, all pages are processed. Defaults to None.
 
     Returns:
         str: The OCR result as a string if `return_text` is True, otherwise the path to the output file.
     """
 
     # se for return_text, retornará o texto no diretamente no código, se for false, retornará o caminho do arquivo com a resposta do OCR
 
@@ -200,21 +201,23 @@
             for file_info in zip_ref.infolist():
                 if file_info.filename.startswith(f"{folder_name}/"):
                     file_info.filename = file_info.filename.replace(f"{folder_name}/", "", 1)
                     zip_ref.extract(file_info, path_tesseract_extract)
         deleta_diretorio('temp_tess')
     pytesseract.pytesseract.tesseract_cmd = path_tesseract
 
-    pdf_fitz = fitz.open(pdf)
     with fitz.open(pdf) as pdf_fitz:
         cria_dir_no_dir_de_trabalho_atual('pages')
         limpa_diretorio('pages')
         faz_log(f'Convertendo PDF para páginas...')
-        with tqdm(total=len(pdf_fitz), desc='EXTRACT PAGES') as bar:
+        number_of_pages = len(pdf_fitz) if limit_pages is None else min(limit_pages, len(pdf_fitz))
+        with tqdm(total=number_of_pages, desc='EXTRACT PAGES') as bar:
             for i, page in enumerate(pdf_fitz):
+                if i >= number_of_pages:
+                    break
                 page = pdf_fitz.load_page(i)
                 mat = fitz.Matrix(dpi/72, dpi/72)  # Matriz de transformação usando DPI
                 pix = page.get_pixmap(matrix=mat)
                 image = Image.frombytes("RGB", [pix.width, pix.height], pix.samples)
                 image.save(f'pages/{i}.png')
                 bar.update(1)
         
@@ -231,8 +234,8 @@
                 if return_text:
                     text_all = ''
                     with open(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'), 'r', encoding='utf-8') as f:
                         text_all = f.read()
                     os.remove(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'))
                     return text_all
                 else:
-                    return os.path.abspath(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'))
+                    return os.path.abspath(arquivo_com_caminho_absoluto('tempdir', f'{file_output}.txt'))
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpdf/pdfutils/pdfutils.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files 0% similar despite different names*

```diff
@@ -1573,7 +1573,29 @@
             if palavra_chave in file:
                 os.remove(file)
 
 
 def tipo_objeto(objeto):
     """Apenas printa o tipo de objeto""" 
     return print(type(objeto))
+
+
+def verifica_se_existe_arquivo_repetido_no_diretorio(dir:str):
+    """
+    Verifica se existem arquivos com o mesmo nome no diretório especificado.
+
+    Args:
+        dir (str): O caminho do diretório a ser verificado.
+
+    Returns:
+        bool: Retorna True se existem arquivos com o mesmo nome no diretório, False caso contrário.
+    """
+    path = os.path.abspath(dir)
+    files = arquivos_com_caminho_absoluto_do_arquivo(path)
+    exists = []
+    for file in files:
+        if file in exists:
+            return True
+        else:
+            exists.append(file)
+    else:
+        return False
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-6.3.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO/utils/utils.py` & `FuncsForSPO-6.3.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-6.3.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.2.7
+Version: 6.3.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.2.7/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-6.3.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/LICENSE` & `FuncsForSPO-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/PKG-INFO` & `FuncsForSPO-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 6.2.7
+Version: 6.3.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-6.2.7/README.md` & `FuncsForSPO-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-6.2.7/setup.py` & `FuncsForSPO-6.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '6.2.7'
+version = '6.3.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

