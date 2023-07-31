# Comparing `tmp/mentat-ai-0.1.6.tar.gz` & `tmp/mentat-ai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-ai-0.1.6.tar", last modified: Sat Jul 29 00:41:39 2023, max compression
+gzip compressed data, was "mentat-ai-0.1.7.tar", last modified: Mon Jul 31 14:40:41 2023, max compression
```

## Comparing `mentat-ai-0.1.6.tar` & `mentat-ai-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.362030 mentat-ai-0.1.6/
--rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.6/LICENSE
--rw-r--r--   0 biobootloader   (501) staff       (20)     3324 2023-07-29 00:41:39.361927 mentat-ai-0.1.6/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     3114 2023-07-29 00:20:59.000000 mentat-ai-0.1.6/README.md
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.358661 mentat-ai-0.1.6/mentat/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.6/mentat/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/mentat/__main__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     6025 2023-07-28 22:38:06.000000 mentat-ai-0.1.6/mentat/app.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/change_conflict_resolution.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/code_change.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/code_change_display.py
--rw-r--r--   0 biobootloader   (501) staff       (20)    14002 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/mentat/code_file_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1645 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/mentat/config_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/mentat/conversation.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      359 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/mentat/default_config.json
--rw-r--r--   0 biobootloader   (501) staff       (20)     4821 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/mentat/llm_api.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.6/mentat/logging_config.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.6/mentat/parsing.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.6/mentat/prompts.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/mentat/streaming_printer.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/mentat/user_input_manager.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.359331 mentat-ai-0.1.6/mentat_ai.egg-info/
--rw-r--r--   0 biobootloader   (501) staff       (20)     3324 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/SOURCES.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/dependency_links.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/entry_points.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/requires.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-29 00:41:39.000000 mentat-ai-0.1.6/mentat_ai.egg-info/top_level.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/pyproject.toml
--rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-29 00:41:39.362059 mentat-ai-0.1.6/setup.cfg
--rw-r--r--   0 biobootloader   (501) staff       (20)      853 2023-07-29 00:41:11.000000 mentat-ai-0.1.6/setup.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.359432 mentat-ai-0.1.6/testbed/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.6/testbed/__init__.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.359794 mentat-ai-0.1.6/testbed/multifile_calculator/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.6/testbed/multifile_calculator/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.6/testbed/multifile_calculator/calculator.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.6/testbed/multifile_calculator/operations.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-29 00:41:39.361755 mentat-ai-0.1.6/tests/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.6/tests/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/tests/benchmark_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3872 2023-07-28 23:48:43.000000 mentat-ai-0.1.6/tests/code_file_manager_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-27 16:52:26.000000 mentat-ai-0.1.6/tests/codechange_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      146 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/tests/config_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3805 2023-07-28 22:38:12.000000 mentat-ai-0.1.6/tests/conftest.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.6/tests/measure_api_speed.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.6/tests/record_benchmark.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-27 16:52:26.000000 mentat-ai-0.1.6/tests/system_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.6/tests/ui_test.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.337630 mentat-ai-0.1.7/
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.7/LICENSE
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 14:40:41.337514 mentat-ai-0.1.7/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3898 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/README.md
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.333634 mentat-ai-0.1.7/mentat/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.7/mentat/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.7/mentat/__main__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     6949 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/mentat/app.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/change_conflict_resolution.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/code_change.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/code_change_display.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    10455 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/mentat/code_file_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3422 2023-07-30 05:21:38.000000 mentat-ai-0.1.7/mentat/config_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.7/mentat/conversation.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      293 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/mentat/default_config.json
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2428 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/mentat/git_handler.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4600 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/mentat/llm_api.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/logging_config.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.7/mentat/parsing.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.7/mentat/prompts.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/mentat/streaming_printer.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/mentat/user_input_manager.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.334324 mentat-ai-0.1.7/mentat_ai.egg-info/
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1068 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/entry_points.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)      764 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/requires.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/top_level.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/pyproject.toml
+-rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-31 14:40:41.337661 mentat-ai-0.1.7/setup.cfg
+-rw-r--r--   0 biobootloader   (501) staff       (20)      853 2023-07-31 14:40:26.000000 mentat-ai-0.1.7/setup.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.334441 mentat-ai-0.1.7/testbed/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.7/testbed/__init__.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.334975 mentat-ai-0.1.7/testbed/multifile_calculator/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.7/testbed/multifile_calculator/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.7/testbed/multifile_calculator/calculator.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.7/testbed/multifile_calculator/operations.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.337341 mentat-ai-0.1.7/tests/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.7/tests/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/tests/benchmark_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7024 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/tests/code_file_manager_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7515 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/tests/codechange_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1549 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/config_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3992 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/conftest.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      826 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/git_handler_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1270 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/license_check.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.7/tests/measure_api_speed.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.7/tests/record_benchmark.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-30 14:54:58.000000 mentat-ai-0.1.7/tests/system_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/tests/ui_test.py
```

### Comparing `mentat-ai-0.1.6/LICENSE` & `mentat-ai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/PKG-INFO` & `mentat-ai-0.1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentat-ai
-Version: 0.1.6
+Version: 0.1.7
 Summary: AI coding assistant on your command line
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
@@ -35,14 +35,16 @@
 See more videos on [Twitter](https://twitter.com/bio_bootloader/status/1683906735248125955) or YouTube:
 - [Intro (2 min - same video as above)](https://www.youtube.com/watch?v=lODjaWclwpY)
 - [Explaining and editing Llama2.c (3 min)](https://www.youtube.com/watch?v=qSyTWMFOjPs)
 - [More Mentat features (4 min)](https://www.youtube.com/watch?v=YJLDIqq8k2A)
 
 # ⚙️ Setup
 
+[Installation and Setup Demonstration Video](https://www.youtube.com/watch?v=bVJP8hY8uRM)
+
 ## Install
 
 Before installing, it's suggested that you create a virtual environment to install it in:
 
 ```
 # Python 3.10 or higher is required
 python3 -m venv .venv
@@ -75,12 +77,22 @@
 
 ## Configuration
 
 For custom configuration options see [configuration.md](docs/configuration.md)
 
 
 # 🚀 Usage
-Run Mentat with:
+
+Run Mentat from within your project directory. Mentat uses git, so if your project doesn't already have git set up, run `git init`. Then you can run Mentat with:
 
 `mentat <paths to files or directories>`
 
-If you provide a directory, Mentat will add all non-hidden text files in that directory to it's context. If this exceeds the GPT-4 token context limit, try running Mentat with just the files you need it to see.
+List the files you would like Mentat to read and edit as arguments. Mentat will add each of them to context, so be careful not to exceed the GPT-4 token context limit. To add multiple files at once, you can also provide directories as arguments. When a directory is provided, Mentat will add all the contained files, except for ones ignored in your `.gitignore`. In addition to files and directories, you can use [glob patterns](https://docs.python.org/3/library/glob.html) to add multiple files at once.
+
+## Options
+
+### Exclude Files
+
+Exclude given paths, directories, or [glob patterns](https://docs.python.org/3/library/glob.html) from Mentat's context. Takes precedence over included file paths.
+```
+mentat --exclude exclude_me.py dir1/dir2 **/*.ts
+```
```

### Comparing `mentat-ai-0.1.6/README.md` & `mentat-ai-0.1.7/mentat_ai.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: mentat-ai
+Version: 0.1.7
+Summary: AI coding assistant on your command line
+License: Apache-2.0
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/XbPdxAMJte?style=flat)](https://discord.gg/zbvd9qx9Pb)
 [![Stable Version](https://img.shields.io/pypi/v/mentat-ai?color=blue)](https://pypi.org/project/mentat-ai/)
 [![License](https://img.shields.io/pypi/l/mentat-ai.svg)](https://github.com/biobootloader/mentat/blob/main/LICENSE)
 
 # 🧙‍♂️ Mentat ⚡
 
@@ -26,14 +35,16 @@
 See more videos on [Twitter](https://twitter.com/bio_bootloader/status/1683906735248125955) or YouTube:
 - [Intro (2 min - same video as above)](https://www.youtube.com/watch?v=lODjaWclwpY)
 - [Explaining and editing Llama2.c (3 min)](https://www.youtube.com/watch?v=qSyTWMFOjPs)
 - [More Mentat features (4 min)](https://www.youtube.com/watch?v=YJLDIqq8k2A)
 
 # ⚙️ Setup
 
+[Installation and Setup Demonstration Video](https://www.youtube.com/watch?v=bVJP8hY8uRM)
+
 ## Install
 
 Before installing, it's suggested that you create a virtual environment to install it in:
 
 ```
 # Python 3.10 or higher is required
 python3 -m venv .venv
@@ -66,12 +77,22 @@
 
 ## Configuration
 
 For custom configuration options see [configuration.md](docs/configuration.md)
 
 
 # 🚀 Usage
-Run Mentat with:
+
+Run Mentat from within your project directory. Mentat uses git, so if your project doesn't already have git set up, run `git init`. Then you can run Mentat with:
 
 `mentat <paths to files or directories>`
 
-If you provide a directory, Mentat will add all non-hidden text files in that directory to it's context. If this exceeds the GPT-4 token context limit, try running Mentat with just the files you need it to see.
+List the files you would like Mentat to read and edit as arguments. Mentat will add each of them to context, so be careful not to exceed the GPT-4 token context limit. To add multiple files at once, you can also provide directories as arguments. When a directory is provided, Mentat will add all the contained files, except for ones ignored in your `.gitignore`. In addition to files and directories, you can use [glob patterns](https://docs.python.org/3/library/glob.html) to add multiple files at once.
+
+## Options
+
+### Exclude Files
+
+Exclude given paths, directories, or [glob patterns](https://docs.python.org/3/library/glob.html) from Mentat's context. Takes precedence over included file paths.
+```
+mentat --exclude exclude_me.py dir1/dir2 **/*.ts
+```
```

### Comparing `mentat-ai-0.1.6/mentat/app.py` & `mentat-ai-0.1.7/mentat/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,112 @@
 import argparse
+import glob
 import logging
 import os
-from typing import Iterable
+from typing import Iterable, Optional
 
 from termcolor import cprint
 
 from .code_change import CodeChange, CodeChangeAction
 from .code_change_display import print_change
 from .code_file_manager import CodeFileManager
 from .config_manager import ConfigManager, mentat_dir_path
 from .conversation import Conversation
+from .git_handler import get_shared_git_root_for_paths
 from .llm_api import CostTracker, count_tokens, setup_api_key
 from .logging_config import setup_logging
 from .user_input_manager import UserInputManager
 
 
 def run_cli():
     parser = argparse.ArgumentParser(
         description="Run conversation with command line args"
     )
-    parser.add_argument("paths", nargs="*", help="Paths to directories or files")
-    paths = parser.parse_args().paths
-    run(paths)
+    parser.add_argument(
+        "paths",
+        nargs="*",
+        default=[],
+        help="List of file paths, directory paths, or glob patterns",
+    )
+    parser.add_argument(
+        "--exclude",
+        "-e",
+        nargs="*",
+        default=[],
+        help="List of file paths, directory paths, or glob patterns to exclude",
+    )
+    args = parser.parse_args()
+    paths = args.paths
+    exclude_paths = args.exclude
+    run(expand_paths(paths), expand_paths(exclude_paths))
+
 
+def expand_paths(paths: Iterable[str]) -> Iterable[str]:
+    globbed_paths = set()
+    for path in paths:
+        globbed_paths.update(glob.glob(pathname=path, recursive=True))
+    return globbed_paths
 
-def run(paths: Iterable[str]):
+
+def run(paths: Iterable[str], exclude_paths: Optional[Iterable[str]] = None):
     os.makedirs(mentat_dir_path, exist_ok=True)
     setup_logging()
     setup_api_key()
     logging.debug(f"Paths: {paths}")
 
     cost_tracker = CostTracker()
     try:
-        loop(paths, cost_tracker)
+        loop(paths, exclude_paths, cost_tracker)
     except (EOFError, KeyboardInterrupt) as e:
         print(e)
     finally:
         cost_tracker.display_total_cost()
 
 
-def loop(paths: Iterable[str], cost_tracker: CostTracker) -> None:
-    config = ConfigManager()
+def loop(
+    paths: Iterable[str],
+    exclude_paths: Optional[Iterable[str]],
+    cost_tracker: CostTracker,
+) -> None:
+    git_root = get_shared_git_root_for_paths(paths)
+    config = ConfigManager(git_root)
     conv = Conversation(config, cost_tracker)
     user_input_manager = UserInputManager(config)
-    code_file_manager = CodeFileManager(paths, user_input_manager, config)
+    code_file_manager = CodeFileManager(
+        paths,
+        exclude_paths if exclude_paths is not None else [],
+        user_input_manager,
+        config,
+        git_root,
+    )
 
     tokens = count_tokens(code_file_manager.get_code_message())
     cprint(f"\nFile token count: {tokens}", "cyan")
     cprint("Type 'q' or use Ctrl-C to quit at any time.\n", color="cyan")
     cprint("What can I do for you?", color="light_blue")
     need_user_request = True
     while True:
         if need_user_request:
             user_response = user_input_manager.collect_user_input()
             conv.add_user_message(user_response)
         explanation, code_changes = conv.get_model_response(code_file_manager, config)
-        warn_user_wrong_files(code_file_manager, code_changes)
+        warn_user_wrong_files(code_file_manager, code_changes, git_root)
 
         if code_changes:
             need_user_request = get_user_feedback_on_changes(
                 config, conv, user_input_manager, code_file_manager, code_changes
             )
         else:
             need_user_request = True
 
 
 def warn_user_wrong_files(
-    code_file_manager: CodeFileManager, code_changes: Iterable[CodeChange]
+    code_file_manager: CodeFileManager,
+    code_changes: Iterable[CodeChange],
+    git_root: str,
 ):
     warned = set()
     for change in code_changes:
         if change.action == CodeChangeAction.CreateFile and os.path.exists(change.file):
             logging.info("Model tried to create a file that already exists")
             cprint(
                 f"Error: tried to create {change.file}, but file already existed!",
@@ -84,16 +120,15 @@
             cprint(
                 f"Error: tried to delete {change.file}, but file doesn't exist!",
                 color="red",
             )
             raise KeyboardInterrupt
 
         if (
-            os.path.join(code_file_manager.git_root, change.file)
-            not in code_file_manager.file_paths
+            os.path.join(git_root, change.file) not in code_file_manager.file_paths
             and change.action != CodeChangeAction.CreateFile
             and change.file not in warned
         ):
             warned.add(change.file)
             cprint(
                 f"Change in {change.file} does not match original files!",
                 color="light_yellow",
```

### Comparing `mentat-ai-0.1.6/mentat/change_conflict_resolution.py` & `mentat-ai-0.1.7/mentat/change_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/code_change.py` & `mentat-ai-0.1.7/mentat/code_change.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/code_change_display.py` & `mentat-ai-0.1.7/mentat/code_change_display.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/code_file_manager.py` & `mentat-ai-0.1.7/mentat/code_file_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,271 +1,173 @@
 import glob
 import logging
 import math
-import mimetypes
 import os
-import subprocess
 from collections import defaultdict
 from pathlib import Path
 from typing import Iterable
 
 from termcolor import cprint
 
 from .change_conflict_resolution import (
     resolve_insertion_conflicts,
     resolve_non_insertion_conflicts,
 )
 from .code_change import CodeChange, CodeChangeAction
 from .config_manager import ConfigManager
+from .git_handler import (
+    get_git_diff_for_path,
+    get_non_gitignored_files,
+    get_paths_with_git_diffs,
+)
 from .user_input_manager import UserInputManager
 
-# mimetypes is OS dependent, so it's best to add as many extensions as we can
-# fmt: off
-default_filetype_include_list = [
-    ".py",      # Python
-    ".java",    # Java
-    ".scala",   # Scala
-    ".kt",      # Kotlin
-    ".php",     # PHP
-    ".html",    # HTML
-    ".css",     # CSS
-    ".less",    # Less
-    ".scss",    # SCSS
-    ".js",      # Javascript
-    ".ts",      # Typescript
-    ".c",       # C
-    ".cpp",     # C++
-    ".h",       # C Header
-    ".cs",      # C#
-    ".go",      # Go
-    ".rs",      # Rust
-    ".rb",      # Ruby
-    ".swift",   # Swift
-    ".lua",     # Lua
-    ".pl",      # Perl
-    ".sql",     # SQL
-    ".r",       # R
-    ".m",       # objective-c
-    ".sh",      # shell scripts
-    ".f",       # fortran
-    ".jsx",     # javascript react
-    ".tsx",     # typescript react
-]
-default_filetype_exclude_list = []
-# fmt: on
-
-
-def _get_git_diff_for_path(git_root, path: str) -> str:
-    return subprocess.check_output(["git", "diff", path], cwd=git_root).decode("utf-8")
-
-
-def _get_paths_with_git_diffs(git_root) -> set[str]:
-    changed = subprocess.check_output(
-        ["git", "diff", "--name-only"], cwd=git_root, text=True
-    ).split("\n")
-    return set(
-        map(lambda path: os.path.realpath(os.path.join(git_root, Path(path))), changed)
-    )
-
-
-def _get_git_root_for_path(path) -> str:
-    if os.path.isdir(path):
-        dir_path = path
-    else:
-        dir_path = os.path.dirname(path)
-    try:
-        git_root = (
-            subprocess.check_output(
-                [
-                    "git",
-                    "rev-parse",
-                    "--show-toplevel",
-                ],
-                cwd=os.path.realpath(dir_path),
-                stderr=subprocess.DEVNULL,
-            )
-            .decode("utf-8")
-            .strip()
-        )
-        # call realpath to resolve symlinks, so all paths match
-        return os.path.realpath(git_root)
-    except subprocess.CalledProcessError:
-        logging.error(f"File {path} isn't part of a git project.")
-        exit()
-
-
-def _get_shared_git_root_for_paths(paths) -> str:
-    git_roots = set()
-    for path in paths:
-        git_root = _get_git_root_for_path(path)
-        git_roots.add(git_root)
-    if not paths:
-        git_root = _get_git_root_for_path(os.getcwd())
-        git_roots.add(git_root)
-
-    if len(git_roots) > 1:
-        logging.error(
-            "All paths must be part of the same git project! Projects provided:"
-            f" {git_roots}"
-        )
-        exit()
-    elif len(git_roots) == 0:
-        logging.error("No git projects provided.")
-        exit()
-
-    return git_roots.pop()
-
 
 def _build_path_tree(file_paths, git_root):
     tree = {}
     for path in file_paths:
         path = os.path.relpath(path, git_root)
         parts = Path(path).parts
         current_level = tree
         for part in parts:
             if part not in current_level:
                 current_level[part] = {}
             current_level = current_level[part]
     return tree
 
 
-def _print_path_tree(tree, non_text_files, changed_files, cur_path, prefix=""):
+def _print_path_tree(tree, changed_files, cur_path, prefix=""):
     keys = list(tree.keys())
     for i, key in enumerate(sorted(keys)):
         if i < len(keys) - 1:
             new_prefix = prefix + "│   "
             print(f"{prefix}├── ", end="")
         else:
             new_prefix = prefix + "    "
             print(f"{prefix}└── ", end="")
 
         cur = os.path.join(cur_path, key)
         star = "* " if cur in changed_files else ""
         if tree[key]:
             color = "blue"
-        elif cur in non_text_files:
-            color = "yellow"
         elif star:
             color = "green"
         else:
             color = None
         cprint(f"{star}{key}", color)
         if tree[key]:
-            _print_path_tree(tree[key], non_text_files, changed_files, cur, new_prefix)
+            _print_path_tree(tree[key], changed_files, cur, new_prefix)
+
+
+def _is_file_text_encoded(file_path):
+    try:
+        # The ultimate filetype test
+        with open(file_path) as f:
+            f.read()
+        return True
+    except UnicodeDecodeError:
+        return False
+
 
+def _abs_file_paths_from_list(paths: Iterable[str], check_for_text: bool = True):
+    file_paths_direct = set()
+    file_paths_from_dirs = set()
+    for path in paths:
+        path = Path(path)
+        if path.is_file():
+            if check_for_text and not _is_file_text_encoded(path):
+                logging.info(f"File path {path} is not text encoded.")
+                cprint(
+                    f"Filepath {path} is not text encoded.",
+                    "light_yellow",
+                )
+                raise KeyboardInterrupt
+            file_paths_direct.add(os.path.realpath(path))
+        elif path.is_dir():
+            nonignored_files = set(
+                map(
+                    lambda f: os.path.realpath(os.path.join(path, f)),
+                    get_non_gitignored_files(path),
+                )
+            )
 
-def _is_file_text(file_name):
-    file_type, encoding = mimetypes.guess_type(file_name)
-    return file_type and file_type.split("/")[0] == "text"
+            file_paths_from_dirs.update(
+                filter(
+                    lambda f: (not check_for_text) or _is_file_text_encoded(f),
+                    nonignored_files,
+                )
+            )
+    return file_paths_direct, file_paths_from_dirs
 
 
 class CodeFileManager:
     def __init__(
         self,
         paths: Iterable[str],
+        exclude_paths: Iterable[str],
         user_input_manager: UserInputManager,
         config: ConfigManager,
+        git_root: str,
     ):
-        # Make sure to apply user config last
-        for file_type in default_filetype_include_list:
-            mimetypes.add_type("text/default-include-list", file_type)
-        for file_type in default_filetype_exclude_list:
-            mimetypes.types_map.pop(file_type, None)
-
-        for file_type in config.filetype_include_list():
-            mimetypes.add_type("text/user-include-list", file_type)
-        for file_type in config.filetype_exclude_list():
-            mimetypes.types_map.pop(file_type, None)
-
         self.config = config
-        self.git_root = _get_shared_git_root_for_paths(paths)
-        self._set_file_paths(paths)
+        self.git_root = git_root
+        self._set_file_paths(paths, exclude_paths)
         self.user_input_manager = user_input_manager
 
         if self.file_paths:
             cprint("Files included in context:", "green")
         else:
             cprint("No files included in context.\n", "red")
             cprint("Git project: ", "green", end="")
         cprint(os.path.split(self.git_root)[1], "blue")
         _print_path_tree(
-            _build_path_tree(self.file_paths + self.non_text_file_paths, self.git_root),
-            self.non_text_file_paths,
-            _get_paths_with_git_diffs(self.git_root),
+            _build_path_tree(self.file_paths, self.git_root),
+            get_paths_with_git_diffs(self.git_root),
             self.git_root,
         )
 
-    def _set_file_paths(self, paths: Iterable[str] = None) -> None:
+    def _set_file_paths(
+        self, paths: Iterable[str], exclude_paths: Iterable[str]
+    ) -> None:
         invalid_paths = []
         for path in paths:
             if not os.path.exists(path):
                 invalid_paths.append(path)
         if invalid_paths:
             cprint("Error:", "red", end=" ")
             cprint("The following paths do not exist:")
             print("\n".join(invalid_paths))
             print("Exiting...")
             exit()
 
-        path_set = set()
-        self.non_text_file_paths = []
-        self.file_paths = []
+        excluded_files, excluded_files_from_dir = _abs_file_paths_from_list(
+            exclude_paths, check_for_text=False
+        )
 
-        for path in paths:
-            path = Path(path)
-            if path.is_file():
-                path_set.add(os.path.realpath(path))
-            elif path.is_dir():
-                non_git_ignored_files = set(
-                    # git returns / seperated paths even on windows, convert so we can remove
-                    # glob_excluded_files, which have windows paths on windows
-                    os.path.normpath(path)
-                    for path in filter(
-                        lambda p: p != "",
-                        subprocess.check_output(
-                            # -c shows cached (regular) files, -o shows other (untracked/ new) files
-                            ["git", "ls-files", "-c", "-o", "--exclude-standard"],
-                            cwd=path,
-                            text=True,
-                        ).split("\n"),
-                    )
-                )
-                glob_excluded_files = set(
-                    file
-                    for glob_path in self.config.file_exclude_glob_list()
-                    # If the user puts a / at the beginning, it will try to look in root directory
-                    for file in glob.glob(
-                        pathname=glob_path.lstrip("/"),
-                        root_dir=path,
-                        recursive=True,
-                    )
-                )
-                nonignored_files = non_git_ignored_files - glob_excluded_files
+        glob_excluded_files = set(
+            os.path.join(self.git_root, file)
+            for glob_path in self.config.file_exclude_glob_list()
+            # If the user puts a / at the beginning, it will try to look in root directory
+            for file in glob.glob(
+                pathname=glob_path,
+                root_dir=self.git_root,
+                recursive=True,
+            )
+        )
+        file_paths_direct, file_paths_from_dirs = _abs_file_paths_from_list(
+            paths, check_for_text=True
+        )
 
-                non_text_files = filter(
-                    lambda f: not _is_file_text(
-                        os.path.realpath(os.path.join(path, f))
-                    ),
-                    nonignored_files,
-                )
-                self.non_text_file_paths.extend(
-                    map(
-                        lambda f: os.path.realpath(os.path.join(path, f)),
-                        non_text_files,
-                    )
-                )
-                text_files = filter(
-                    _is_file_text,
-                    map(
-                        lambda f: os.path.realpath(os.path.join(path, f)),
-                        nonignored_files,
-                    ),
-                )
-                path_set.update(text_files)
-        self.file_paths = list(path_set)
+        # config glob excluded files only apply to files added from directories
+        file_paths_from_dirs -= glob_excluded_files
+
+        self.file_paths = list(
+            (file_paths_direct | file_paths_from_dirs)
+            - (excluded_files | excluded_files_from_dir)
+        )
 
     def _read_file(self, abs_path) -> Iterable[str]:
         with open(abs_path, "r") as f:
             lines = f.read().split("\n")
         return lines
 
     def _read_all_file_lines(self) -> None:
@@ -278,24 +180,18 @@
         code_message = ["Code Files:\n"]
         for abs_path in self.file_paths:
             rel_path = os.path.relpath(abs_path, self.git_root)
             code_message.append(rel_path)
             for i, line in enumerate(self.file_lines[abs_path], start=1):
                 code_message.append(f"{i}:{line}")
             code_message.append("")
-            git_diff_output = _get_git_diff_for_path(self.git_root, rel_path)
+            git_diff_output = get_git_diff_for_path(self.git_root, rel_path)
             if git_diff_output:
                 code_message.append("Current git diff for this file:")
                 code_message.append(f"{git_diff_output}")
-        if self.non_text_file_paths:
-            code_message.append("\nOther files:\n")
-            code_message.extend(
-                os.path.relpath(path, self.git_root)
-                for path in self.non_text_file_paths
-            )
         return "\n".join(code_message)
 
     def _handle_delete(self, delete_change):
         file_path = os.path.join(self.git_root, delete_change.file)
         if not os.path.exists(file_path):
             logging.error(f"Path {file_path} non-existent on delete")
             return
@@ -326,18 +222,16 @@
 
         rel_path = changes[0].file
         abs_path = os.path.join(self.git_root, rel_path)
         new_code_lines = self.file_lines[abs_path].copy()
         if new_code_lines != self._read_file(abs_path):
             logging.info(f"File '{rel_path}' changed while generating changes")
             cprint(
-                (
-                    f"File '{rel_path}' changed while generating; current file changes"
-                    " will be erased. Continue?"
-                ),
+                f"File '{rel_path}' changed while generating; current file changes"
+                " will be erased. Continue?",
                 color="light_yellow",
             )
             if not self.user_input_manager.ask_yes_no(default_yes=False):
                 cprint(f"Not applying changes to file {rel_path}.")
                 return None
 
         # Necessary in case the model needs to insert past the end of the file
@@ -370,13 +264,15 @@
         for file_path, changes in file_changes.items():
             new_code_lines = self._get_new_code_lines(changes)
             if new_code_lines:
                 files_to_write[file_path] = new_code_lines
 
         for rel_path, code_lines in files_to_write.items():
             file_path = os.path.join(self.git_root, rel_path)
-            # if changes created a new file and we are now writing to it, add it to context
             if file_path not in self.file_paths:
+                # newly created files added to Mentat's context
                 logging.info(f"Adding new file {file_path} to context")
                 self.file_paths.append(file_path)
+                # create any missing directories in the path
+                os.makedirs(os.path.dirname(file_path), exist_ok=True)
             with open(file_path, "w") as f:
                 f.write("\n".join(code_lines))
```

### Comparing `mentat-ai-0.1.6/mentat/conversation.py` & `mentat-ai-0.1.7/mentat/conversation.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/llm_api.py` & `mentat-ai-0.1.7/mentat/llm_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Generator
 
 import openai
 import tiktoken
 from dotenv import load_dotenv
 from termcolor import cprint
 
-from .config_manager import mentat_dir_path, user_config_file_name
+from .config_manager import mentat_dir_path, user_config_path
 
 package_name = __name__.split(".")[0]
 
 
 # Check for .env file or already exported API key
 # If no api key found, exit and warn user
 def setup_api_key():
@@ -21,18 +21,16 @@
         load_dotenv()
     key = os.getenv("OPENAI_API_KEY")
     try:
         openai.api_key = key
         openai.Model.list()  # Test the API key
     except openai.error.AuthenticationError:
         cprint(
-            (
-                "No valid OpenAI api key detected.\nEither place your key into a .env"
-                " file or export it as an environment variable."
-            ),
+            "No valid OpenAI api key detected.\nEither place your key into a .env"
+            " file or export it as an environment variable.",
             "red",
         )
         sys.exit(0)
 
 
 async def call_llm_api(messages: list[dict[str, str]], model) -> Generator:
     if (
@@ -59,31 +57,27 @@
 
 def check_model_availability(allow_32k: bool) -> bool:
     available_models = [x["id"] for x in openai.Model.list()["data"]]
     if allow_32k:
         # check if user has access to gpt-4-32k
         if "gpt-4-32k-0314" not in available_models:
             cprint(
-                (
-                    "You set ALLOW_32K to true, but your OpenAI API key doesn't"
-                    " have access to gpt-4-32k-0314. To remove this warning, set"
-                    " ALLOW_32K to false until you have access."
-                ),
+                "You set ALLOW_32K to true, but your OpenAI API key doesn't"
+                " have access to gpt-4-32k-0314. To remove this warning, set"
+                " ALLOW_32K to false until you have access.",
                 "yellow",
             )
             allow_32k = False
 
     if not allow_32k:
         # check if user has access to gpt-4
         if "gpt-4-0314" not in available_models:
             cprint(
-                (
-                    "Sorry, but your OpenAI API key doesn't have access to gpt-4-0314,"
-                    " which is currently required to run Mentat."
-                ),
+                "Sorry, but your OpenAI API key doesn't have access to gpt-4-0314,"
+                " which is currently required to run Mentat.",
                 "red",
             )
             raise KeyboardInterrupt
 
     return allow_32k
 
 
@@ -103,20 +97,18 @@
             if prompt_token_count > 32768 - token_buffer:
                 cprint(
                     "Warning: gpt-4-32k-0314 has a token limit of 32768. Attempting"
                     " to run anyway:"
                 )
         else:
             cprint(
-                (
-                    "Warning: gpt-4-0314 has a maximum context length of 8192 tokens."
-                    " If you have access to gpt-4-32k-0314, set allow-32k to `true` in"
-                    f" `{os.path.join(mentat_dir_path, user_config_file_name)}` to use"
-                    " it. Attempting to run with gpt-4-0314:"
-                ),
+                "Warning: gpt-4-0314 has a maximum context length of 8192 tokens."
+                " If you have access to gpt-4-32k-0314, set allow-32k to `true` in"
+                f" `{user_config_path}` to use"
+                " it. Attempting to run with gpt-4-0314:",
                 "yellow",
             )
     return model, prompt_token_count
 
 
 @dataclass
 class CostTracker:
```

### Comparing `mentat-ai-0.1.6/mentat/logging_config.py` & `mentat-ai-0.1.7/mentat/logging_config.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/parsing.py` & `mentat-ai-0.1.7/mentat/parsing.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/prompts.py` & `mentat-ai-0.1.7/mentat/prompts.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/streaming_printer.py` & `mentat-ai-0.1.7/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat/user_input_manager.py` & `mentat-ai-0.1.7/mentat/user_input_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/mentat_ai.egg-info/SOURCES.txt` & `mentat-ai-0.1.7/mentat_ai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 mentat/change_conflict_resolution.py
 mentat/code_change.py
 mentat/code_change_display.py
 mentat/code_file_manager.py
 mentat/config_manager.py
 mentat/conversation.py
 mentat/default_config.json
+mentat/git_handler.py
 mentat/llm_api.py
 mentat/logging_config.py
 mentat/parsing.py
 mentat/prompts.py
 mentat/streaming_printer.py
 mentat/user_input_manager.py
 mentat_ai.egg-info/PKG-INFO
@@ -30,11 +31,13 @@
 testbed/multifile_calculator/operations.py
 tests/__init__.py
 tests/benchmark_test.py
 tests/code_file_manager_test.py
 tests/codechange_test.py
 tests/config_test.py
 tests/conftest.py
+tests/git_handler_test.py
+tests/license_check.py
 tests/measure_api_speed.py
 tests/record_benchmark.py
 tests/system_test.py
 tests/ui_test.py
```

### Comparing `mentat-ai-0.1.6/mentat_ai.egg-info/requires.txt` & `mentat-ai-0.1.7/mentat_ai.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-aiohttp==3.8.4
+aiohttp==3.8.5
 aiosignal==1.3.1
 async-timeout==4.0.2
 attrs==23.1.0
-black==23.3.0
-certifi==2022.12.7
-charset-normalizer==3.1.0
-click==8.1.3
-exceptiongroup==1.1.1
+black==23.7.0
+certifi==2023.7.22
+charset-normalizer==3.2.0
+click==8.1.6
+exceptiongroup==1.1.2
 fire==0.5.0
 flake8==6.0.0
-frozenlist==1.3.3
+frozenlist==1.4.0
 gitdb==4.0.10
 GitPython==3.1.32
 idna==3.4
 iniconfig==2.0.0
 isort==5.12.0
 mccabe==0.7.0
 multidict==6.0.4
 mypy-extensions==1.0.0
-openai==0.27.6
+openai==0.27.8
 packaging==23.1
-pathspec==0.11.1
-platformdirs==3.5.0
-pluggy==1.0.0
+pathspec==0.11.2
+platformdirs==3.10.0
+pluggy==1.2.0
 prompt-toolkit==3.0.39
 pycodestyle==2.10.0
 pyflakes==3.0.1
 Pygments==2.15.1
-pytest==7.3.1
-pytest-mock==3.10.0
+pytest==7.4.0
+pytest-mock==3.11.1
 pytest-repeat==0.9.1
 pytest-reportlog==0.4.0
 python-dotenv==1.0.0
 regex==2023.6.3
-requests==2.29.0
-ruff==0.0.270
+requests==2.31.0
+ruff==0.0.280
 six==1.16.0
 smmap==5.0.0
 termcolor==2.3.0
 tiktoken==0.4.0
 tomli==2.0.1
 tqdm==4.65.0
-urllib3==1.26.15
+urllib3==2.0.4
 wcwidth==0.2.6
 yarl==1.9.2
```

### Comparing `mentat-ai-0.1.6/setup.py` & `mentat-ai-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 readme_path = os.path.join(Path(__file__).parent, "README.md")
 with open(readme_path, "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mentat-ai",
-    version="0.1.6",
+    version="0.1.7",
     python_requires=">=3.10",
     packages=find_packages(),
     install_requires=read_requirements("requirements.txt"),
     package_data={
         "mentat": ["default_config.json"],
     },
     entry_points={
```

### Comparing `mentat-ai-0.1.6/testbed/multifile_calculator/calculator.py` & `mentat-ai-0.1.7/testbed/multifile_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/tests/benchmark_test.py` & `mentat-ai-0.1.7/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/tests/codechange_test.py` & `mentat-ai-0.1.7/tests/codechange_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                         # This is a temporary
                         # lines""")
     assert content == expected_content
 
 
 def test_create_file(mock_call_llm_api, mock_collect_user_input, mock_setup_api_key):
     # Create a temporary file
-    temp_file_name = "temp.py"
+    temp_file_name = "new_dir/temp.py"
     mock_collect_user_input.side_effect = [
         "Create a new file called temp.py",
         "y",
         KeyboardInterrupt,
     ]
 
     mock_call_llm_api.set_generator_values([dedent("""\
```

### Comparing `mentat-ai-0.1.6/tests/conftest.py` & `mentat-ai-0.1.7/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 import stat
 import subprocess
 import tempfile
 
 import pytest
 
+from mentat.config_manager import ConfigManager
 from mentat.streaming_printer import StreamingPrinter
 from mentat.user_input_manager import UserInputManager
 
 pytest_plugins = ("pytest_reportlog",)
 
 
 def filter_mark(items, mark, exists):
@@ -67,14 +68,21 @@
 @pytest.fixture
 def mock_setup_api_key(mocker):
     mocker.patch("mentat.app.setup_api_key")
     mocker.patch("mentat.conversation.check_model_availability")
     return
 
 
+@pytest.fixture
+def mock_config(temp_testbed):
+    config = ConfigManager(temp_testbed)
+    config.project_config = {}
+    return config
+
+
 def add_permissions(func, path, exc_info):
     """
     Error handler for ``shutil.rmtree``.
 
     If the error is due to an access error (read only file)
     it attempts to add write permission and then retries.
```

### Comparing `mentat-ai-0.1.6/tests/measure_api_speed.py` & `mentat-ai-0.1.7/tests/measure_api_speed.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/tests/record_benchmark.py` & `mentat-ai-0.1.7/tests/record_benchmark.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/tests/system_test.py` & `mentat-ai-0.1.7/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.6/tests/ui_test.py` & `mentat-ai-0.1.7/tests/ui_test.py`

 * *Files identical despite different names*

