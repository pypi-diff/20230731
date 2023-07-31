# Comparing `tmp/mentat-ai-0.1.7.tar.gz` & `tmp/mentat-ai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-ai-0.1.7.tar", last modified: Mon Jul 31 14:40:41 2023, max compression
+gzip compressed data, was "mentat-ai-0.1.8.tar", last modified: Mon Jul 31 20:29:29 2023, max compression
```

## Comparing `mentat-ai-0.1.7.tar` & `mentat-ai-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.337630 mentat-ai-0.1.7/
--rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.7/LICENSE
--rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 14:40:41.337514 mentat-ai-0.1.7/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     3898 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/README.md
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.333634 mentat-ai-0.1.7/mentat/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.7/mentat/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.7/mentat/__main__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     6949 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/mentat/app.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/change_conflict_resolution.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/code_change.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/code_change_display.py
--rw-r--r--   0 biobootloader   (501) staff       (20)    10455 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/mentat/code_file_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3422 2023-07-30 05:21:38.000000 mentat-ai-0.1.7/mentat/config_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.7/mentat/conversation.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      293 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/mentat/default_config.json
--rw-r--r--   0 biobootloader   (501) staff       (20)     2428 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/mentat/git_handler.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4600 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/mentat/llm_api.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.7/mentat/logging_config.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.7/mentat/parsing.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.7/mentat/prompts.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/mentat/streaming_printer.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/mentat/user_input_manager.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.334324 mentat-ai-0.1.7/mentat_ai.egg-info/
--rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     1068 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/SOURCES.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/dependency_links.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/entry_points.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)      764 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/requires.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-31 14:40:41.000000 mentat-ai-0.1.7/mentat_ai.egg-info/top_level.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/pyproject.toml
--rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-31 14:40:41.337661 mentat-ai-0.1.7/setup.cfg
--rw-r--r--   0 biobootloader   (501) staff       (20)      853 2023-07-31 14:40:26.000000 mentat-ai-0.1.7/setup.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.334441 mentat-ai-0.1.7/testbed/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.7/testbed/__init__.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.334975 mentat-ai-0.1.7/testbed/multifile_calculator/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.7/testbed/multifile_calculator/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.7/testbed/multifile_calculator/calculator.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.7/testbed/multifile_calculator/operations.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 14:40:41.337341 mentat-ai-0.1.7/tests/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.7/tests/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/tests/benchmark_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7024 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/tests/code_file_manager_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7515 2023-07-31 14:40:12.000000 mentat-ai-0.1.7/tests/codechange_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1549 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/config_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3992 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/conftest.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      826 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/git_handler_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1270 2023-07-30 05:20:49.000000 mentat-ai-0.1.7/tests/license_check.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.7/tests/measure_api_speed.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.7/tests/record_benchmark.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-30 14:54:58.000000 mentat-ai-0.1.7/tests/system_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.7/tests/ui_test.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.150919 mentat-ai-0.1.8/
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.8/LICENSE
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 20:29:29.150785 mentat-ai-0.1.8/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3898 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/README.md
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.140954 mentat-ai-0.1.8/mentat/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.8/mentat/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.8/mentat/__main__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     6949 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/mentat/app.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/change_conflict_resolution.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/code_change.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/code_change_display.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    10455 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/mentat/code_file_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3422 2023-07-30 05:21:38.000000 mentat-ai-0.1.8/mentat/config_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.8/mentat/conversation.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      293 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/mentat/default_config.json
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2603 2023-07-31 20:17:16.000000 mentat-ai-0.1.8/mentat/git_handler.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4547 2023-07-31 20:26:16.000000 mentat-ai-0.1.8/mentat/llm_api.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/logging_config.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.8/mentat/parsing.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.8/mentat/prompts.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/mentat/streaming_printer.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/mentat/user_input_manager.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.141593 mentat-ai-0.1.8/mentat_ai.egg-info/
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1068 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/entry_points.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)      764 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/requires.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/top_level.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/pyproject.toml
+-rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-31 20:29:29.150964 mentat-ai-0.1.8/setup.cfg
+-rw-r--r--   0 biobootloader   (501) staff       (20)      853 2023-07-31 20:29:10.000000 mentat-ai-0.1.8/setup.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.142530 mentat-ai-0.1.8/testbed/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.8/testbed/__init__.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.145171 mentat-ai-0.1.8/testbed/multifile_calculator/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.8/testbed/multifile_calculator/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.8/testbed/multifile_calculator/calculator.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.8/testbed/multifile_calculator/operations.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.150474 mentat-ai-0.1.8/tests/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.8/tests/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/tests/benchmark_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7024 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/tests/code_file_manager_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7515 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/tests/codechange_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1549 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/config_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3992 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/conftest.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      826 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/git_handler_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1270 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/license_check.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.8/tests/measure_api_speed.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.8/tests/record_benchmark.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-30 14:54:58.000000 mentat-ai-0.1.8/tests/system_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/tests/ui_test.py
```

### Comparing `mentat-ai-0.1.7/LICENSE` & `mentat-ai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/PKG-INFO` & `mentat-ai-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentat-ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: AI coding assistant on your command line
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
```

### Comparing `mentat-ai-0.1.7/README.md` & `mentat-ai-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/app.py` & `mentat-ai-0.1.8/mentat/app.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/change_conflict_resolution.py` & `mentat-ai-0.1.8/mentat/change_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/code_change.py` & `mentat-ai-0.1.8/mentat/code_change.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/code_change_display.py` & `mentat-ai-0.1.8/mentat/code_change_display.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/code_file_manager.py` & `mentat-ai-0.1.8/mentat/code_file_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/config_manager.py` & `mentat-ai-0.1.8/mentat/config_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/conversation.py` & `mentat-ai-0.1.8/mentat/conversation.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/git_handler.py` & `mentat-ai-0.1.8/mentat/git_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,22 @@
     )
 
 
 def get_paths_with_git_diffs(git_root) -> set[str]:
     changed = subprocess.check_output(
         ["git", "diff", "--name-only"], cwd=git_root, text=True
     ).split("\n")
+    new = subprocess.check_output(
+        ["git", "ls-files", "-o", "--exclude-standard"], cwd=git_root, text=True
+    ).split("\n")
     return set(
-        map(lambda path: os.path.realpath(os.path.join(git_root, Path(path))), changed)
+        map(
+            lambda path: os.path.realpath(os.path.join(git_root, Path(path))),
+            changed + new,
+        )
     )
 
 
 def _get_git_root_for_path(path) -> str:
     if os.path.isdir(path):
         dir_path = path
     else:
```

### Comparing `mentat-ai-0.1.7/mentat/llm_api.py` & `mentat-ai-0.1.8/mentat/llm_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         stream=True,
     )
 
     return response
 
 
 def count_tokens(message: str) -> int:
-    return len(tiktoken.encoding_for_model("gpt-4").encode(message))
+    return len(
+        tiktoken.encoding_for_model("gpt-4").encode(message, disallowed_special=())
+    )
 
 
 def check_model_availability(allow_32k: bool) -> bool:
     available_models = [x["id"] for x in openai.Model.list()["data"]]
     if allow_32k:
         # check if user has access to gpt-4-32k
         if "gpt-4-32k-0314" not in available_models:
@@ -79,18 +81,16 @@
             raise KeyboardInterrupt
 
     return allow_32k
 
 
 def choose_model(messages: list[dict[str, str]], allow_32k) -> str:
     prompt_token_count = 0
-    tokenizer = tiktoken.encoding_for_model("gpt-4")
     for message in messages:
-        encoding = tokenizer.encode(message["content"])
-        prompt_token_count += len(encoding)
+        prompt_token_count += count_tokens(message["content"])
     cprint(f"\nTotal token count: {prompt_token_count}", "cyan")
 
     model = "gpt-4-0314"
     token_buffer = 500
     if prompt_token_count > 8192 - token_buffer:
         if allow_32k:
             model = "gpt-4-32k-0314"
```

### Comparing `mentat-ai-0.1.7/mentat/logging_config.py` & `mentat-ai-0.1.8/mentat/logging_config.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/parsing.py` & `mentat-ai-0.1.8/mentat/parsing.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/prompts.py` & `mentat-ai-0.1.8/mentat/prompts.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/streaming_printer.py` & `mentat-ai-0.1.8/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat/user_input_manager.py` & `mentat-ai-0.1.8/mentat/user_input_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat_ai.egg-info/PKG-INFO` & `mentat-ai-0.1.8/mentat_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentat-ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: AI coding assistant on your command line
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
```

### Comparing `mentat-ai-0.1.7/mentat_ai.egg-info/SOURCES.txt` & `mentat-ai-0.1.8/mentat_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/mentat_ai.egg-info/requires.txt` & `mentat-ai-0.1.8/mentat_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/setup.py` & `mentat-ai-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 readme_path = os.path.join(Path(__file__).parent, "README.md")
 with open(readme_path, "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mentat-ai",
-    version="0.1.7",
+    version="0.1.8",
     python_requires=">=3.10",
     packages=find_packages(),
     install_requires=read_requirements("requirements.txt"),
     package_data={
         "mentat": ["default_config.json"],
     },
     entry_points={
```

### Comparing `mentat-ai-0.1.7/testbed/multifile_calculator/calculator.py` & `mentat-ai-0.1.8/testbed/multifile_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/benchmark_test.py` & `mentat-ai-0.1.8/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/code_file_manager_test.py` & `mentat-ai-0.1.8/tests/code_file_manager_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/codechange_test.py` & `mentat-ai-0.1.8/tests/codechange_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/config_test.py` & `mentat-ai-0.1.8/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/conftest.py` & `mentat-ai-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/git_handler_test.py` & `mentat-ai-0.1.8/tests/git_handler_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/license_check.py` & `mentat-ai-0.1.8/tests/license_check.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/measure_api_speed.py` & `mentat-ai-0.1.8/tests/measure_api_speed.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/record_benchmark.py` & `mentat-ai-0.1.8/tests/record_benchmark.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/system_test.py` & `mentat-ai-0.1.8/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.7/tests/ui_test.py` & `mentat-ai-0.1.8/tests/ui_test.py`

 * *Files identical despite different names*

