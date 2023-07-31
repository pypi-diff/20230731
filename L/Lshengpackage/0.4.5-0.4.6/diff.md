# Comparing `tmp/Lshengpackage-0.4.5.tar.gz` & `tmp/Lshengpackage-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.4.5.tar", last modified: Fri May 19 06:23:13 2023, max compression
+gzip compressed data, was "Lshengpackage-0.4.6.tar", last modified: Mon Jul 31 09:28:40 2023, max compression
```

## Comparing `Lshengpackage-0.4.5.tar` & `Lshengpackage-0.4.6.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.264726 Lshengpackage-0.4.5/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.5/License.md
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.206652 Lshengpackage-0.4.5/Lshengpackage/
--rw-rw-rw-   0        0        0      550 2023-05-18 16:33:59.000000 Lshengpackage-0.4.5/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.216244 Lshengpackage-0.4.5/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.221179 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/
--rw-rw-rw-   0        0        0      162 2023-05-19 03:15:17.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      428 2023-05-19 03:15:17.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/mock_findFr.cpython-39.pyc
--rw-rw-rw-   0        0        0     1717 2023-05-19 03:26:52.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.223689 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     3313 2023-05-19 03:03:37.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       49 2023-05-18 15:10:46.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.227234 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0     3855 2023-05-19 03:15:18.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
--rw-rw-rw-   0        0        0      166 2023-05-19 03:15:18.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2290 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.231221 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.234221 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__pycache__/
--rw-rw-rw-   0        0        0      175 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     6503 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc
--rw-rw-rw-   0        0        0     8853 2023-05-19 05:56:20.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
--rw-rw-rw-   0        0        0     3059 2023-05-19 03:37:17.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/adb/re_Pic.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.238533 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4683 2023-05-18 16:25:46.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.244057 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4828 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      160 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2554 2023-05-19 03:34:10.000000 Lshengpackage-0.4.5/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.257730 Lshengpackage-0.4.5/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.5/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      757 2023-05-18 15:10:46.000000 Lshengpackage-0.4.5/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0     2019 2023-05-19 03:47:29.000000 Lshengpackage-0.4.5/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3311 2023-05-18 14:57:22.000000 Lshengpackage-0.4.5/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.5/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       49 2023-05-18 16:20:17.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.264726 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/
--rw-rw-rw-   0        0        0     1982 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc
--rw-rw-rw-   0        0        0     1167 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/General.cpython-39.pyc
--rw-rw-rw-   0        0        0     1431 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc
--rw-rw-rw-   0        0        0     2530 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc
--rw-rw-rw-   0        0        0     1282 2023-05-19 03:16:36.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc
--rw-rw-rw-   0        0        0      159 2023-05-19 03:16:35.000000 Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-19 06:23:13.212662 Lshengpackage-0.4.5/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      858 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2058 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-19 06:23:13.000000 Lshengpackage-0.4.5/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      299 2023-05-17 15:14:59.000000 Lshengpackage-0.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-05-19 06:23:13.264726 Lshengpackage-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.5/README.md
--rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.4.5/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-19 06:23:13.267246 Lshengpackage-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1987 2023-05-19 05:56:20.000000 Lshengpackage-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.042842 Lshengpackage-0.4.6/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.4.6/License.md
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.928592 Lshengpackage-0.4.6/Lshengpackage/
+-rw-rw-rw-   0        0        0      550 2023-05-18 16:33:59.000000 Lshengpackage-0.4.6/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.940081 Lshengpackage-0.4.6/Lshengpackage/network/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:41:45.000000 Lshengpackage-0.4.6/Lshengpackage/network/__init__.py
+-rw-rw-rw-   0        0        0     2495 2023-07-31 09:22:35.000000 Lshengpackage-0.4.6/Lshengpackage/network/scan.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.945082 Lshengpackage-0.4.6/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2023-05-18 15:10:46.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.950080 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/
+-rw-rw-rw-   0        0        0      162 2023-05-19 03:15:17.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      428 2023-05-19 03:15:17.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/mock_findFr.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1717 2023-05-19 03:26:52.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.972629 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     3313 2023-05-19 03:03:37.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       49 2023-05-18 15:10:46.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.990141 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0     3855 2023-05-19 03:15:18.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc
+-rw-rw-rw-   0        0        0      166 2023-05-19 03:15:18.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2290 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.001640 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.004680 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/
+-rw-rw-rw-   0        0        0      175 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6503 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8853 2023-05-19 05:56:20.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
+-rw-rw-rw-   0        0        0     3059 2023-05-19 03:37:17.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/adb/re_Pic.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.011681 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4683 2023-05-18 16:25:46.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.019688 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4828 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      160 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2023-05-18 05:41:23.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2554 2023-05-19 03:34:10.000000 Lshengpackage-0.4.6/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.029650 Lshengpackage-0.4.6/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.4.6/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      757 2023-05-18 15:10:46.000000 Lshengpackage-0.4.6/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0     2019 2023-05-19 03:47:29.000000 Lshengpackage-0.4.6/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3311 2023-05-18 14:57:22.000000 Lshengpackage-0.4.6/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2055 2023-05-18 05:41:23.000000 Lshengpackage-0.4.6/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       49 2023-05-18 16:20:17.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:40.040853 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/
+-rw-rw-rw-   0        0        0     1982 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1167 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/General.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1431 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2530 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1282 2023-05-19 03:16:36.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc
+-rw-rw-rw-   0        0        0      159 2023-05-19 03:16:35.000000 Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-07-31 09:28:39.936560 Lshengpackage-0.4.6/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      969 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2122 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 09:28:39.000000 Lshengpackage-0.4.6/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      342 2023-07-31 07:42:41.000000 Lshengpackage-0.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      969 2023-07-31 09:28:40.042842 Lshengpackage-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.4.6/README.md
+-rw-rw-rw-   0        0        0      422 2023-07-31 08:17:55.000000 Lshengpackage-0.4.6/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-31 09:28:40.043842 Lshengpackage-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     2098 2023-07-31 09:24:09.000000 Lshengpackage-0.4.6/setup.py
```

### Comparing `Lshengpackage-0.4.5/LICENSE` & `Lshengpackage-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/License.md` & `Lshengpackage-0.4.6/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/__init__.py` & `Lshengpackage-0.4.6/Lshengpackage/__init__.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/Command_adb.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/__pycache__/re_Pic.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/__pycache__/dingtalk_api.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py` & `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/adb/re_Pic.py` & `Lshengpackage-0.4.6/Lshengpackage/simulate/adb/re_Pic.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.4.6/Lshengpackage/simulate/mock_findPic.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.4.6/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/General.py` & `Lshengpackage-0.4.6/Lshengpackage/tools/General.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/Loading.py` & `Lshengpackage-0.4.6/Lshengpackage/tools/Loading.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.4.6/Lshengpackage/tools/OperateFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.4.6/Lshengpackage/tools/SearchFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/ChaoJiYing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/General.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/General.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/Loading.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/OperateFile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc` & `Lshengpackage-0.4.6/Lshengpackage/tools/__pycache__/SearchFile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.4.6/Lshengpackage.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.5
+Version: 0.4.6
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
-Keywords: 游戏,办公,自动化,爬虫
+Keywords: 游戏,办公,自动化,爬虫,网络
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: License.md
```

### Comparing `Lshengpackage-0.4.5/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.4.6/Lshengpackage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 setup.py
 Lshengpackage/__init__.py
 Lshengpackage.egg-info/PKG-INFO
 Lshengpackage.egg-info/SOURCES.txt
 Lshengpackage.egg-info/dependency_links.txt
 Lshengpackage.egg-info/requires.txt
 Lshengpackage.egg-info/top_level.txt
+Lshengpackage/network/__init__.py
+Lshengpackage/network/scan.py
 Lshengpackage/simulate/__init__.py
 Lshengpackage/simulate/mock_findFr.py
 Lshengpackage/simulate/mock_findPic.py
 Lshengpackage/simulate/__pycache__/__init__.cpython-39.pyc
 Lshengpackage/simulate/__pycache__/mock_findFr.cpython-39.pyc
 Lshengpackage/simulate/__pycache__/mock_findPic.cpython-39.pyc
 Lshengpackage/simulate/adb/Command_adb.py
```

### Comparing `Lshengpackage-0.4.5/PKG-INFO` & `Lshengpackage-0.4.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.4.5
+Version: 0.4.6
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
-Keywords: 游戏,办公,自动化,爬虫
+Keywords: 游戏,办公,自动化,爬虫,网络
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: License.md
```

### Comparing `Lshengpackage-0.4.5/README.md` & `Lshengpackage-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.4.5/setup.py` & `Lshengpackage-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.4.5',  # Start with a small number and increase it with every change you make
+    version='0.4.6',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
@@ -19,21 +19,23 @@
         'pyperclip',
         'opencv-python',
         'Pillow',
         'aircv',
         'numpy',
         'requests'
     ],
-    keywords=['游戏', '办公', '自动化', '爬虫'],  # Keywords that define your package best
+    keywords=['游戏', '办公', '自动化', '爬虫','网络'],  # Keywords that define your package best
     classifiers=[
         'Development Status :: 3 - Alpha',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  # Again, pick a license
         'Programming Language :: Python :: 3',  # Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ], )
```

