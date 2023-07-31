# Comparing `tmp/nonebot_plugin_nagabus-0.2.7.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.2.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.8.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.2.7.tar` & `nonebot_plugin_nagabus-0.2.8.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.7/LICENSE
--rw-r--r--   0        0        0     1485 2023-06-27 03:08:54.351266 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1364 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      715 2023-06-19 13:39:23.143434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-27 03:05:14.174566 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4650 2023-06-19 13:39:23.144435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2840 2023-06-27 03:07:21.048380 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1617 2023-06-19 13:39:23.145434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0      998 2023-07-28 15:04:21.945700 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      178 2023-06-19 13:39:23.146434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     4617 2023-07-30 16:24:05.300757 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0      436 2023-06-19 13:39:23.147435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/errors.py
--rw-r--r--   0        0        0     3669 2023-06-27 03:05:14.166569 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1248 2023-06-19 13:39:23.148435 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    21282 2023-06-27 03:05:14.157193 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0      347 2023-06-19 13:39:23.149434 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      996 2023-07-30 16:24:28.982337 nonebot_plugin_nagabus-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.7/README.md
--rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1485 2023-06-27 03:08:54.351266 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1530 2023-07-31 14:41:13.608117 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-19 13:39:23.142435 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      715 2023-06-19 13:39:23.143434 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     3379 2023-07-31 14:42:34.654316 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0      942 2023-07-31 14:42:34.659835 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/interceptors/send_waiting_prompt.py
+-rw-r--r--   0        0        0     4741 2023-07-31 14:38:39.085252 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2840 2023-06-27 03:07:21.048380 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1617 2023-06-19 13:39:23.145434 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0      998 2023-07-28 15:04:21.945700 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      178 2023-06-19 13:39:23.146434 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     4617 2023-07-30 16:24:05.300757 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0      436 2023-06-19 13:39:23.147435 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/errors.py
+-rw-r--r--   0        0        0     3669 2023-06-27 03:05:14.166569 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1248 2023-06-19 13:39:23.148435 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    21313 2023-07-31 14:36:01.152113 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0      347 2023-06-19 13:39:23.149434 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      996 2023-07-31 14:43:15.534698 nonebot_plugin_nagabus-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.8/README.md
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.8/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.2.7/LICENSE` & `nonebot_plugin_nagabus-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from typing import Dict
+from typing import Dict, Optional
 from urllib.parse import urlparse
 
 from nonebot import get_driver
 from pydantic import BaseSettings, root_validator, ValidationError
 
 from .errors import ConfigError
 
 
 class Config(BaseSettings):
     naga_cookies: Dict[str, str]
     naga_fake_api: bool = False
+    naga_timeout: float = 60 * 10
+
+    access_control_reply_on_permission_denied: Optional[str]
+    access_control_reply_on_rate_limited: Optional[str]
 
     datastore_database_dialect: str
 
     @root_validator(pre=True, allow_reuse=True)
     def detect_sql_dialect(cls, values):
         if "datastore_database_url" in values:
             url = urlparse(values["datastore_database_url"])
```

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import asyncio
 from functools import wraps
 
 from httpx import HTTPError
 from nonebot import logger
 from nonebot.exception import MatcherException, ActionFailed
 from nonebot.internal.matcher import current_matcher
-from nonebot_plugin_access_control.errors import RateLimitedError
+from nonebot_plugin_access_control.errors import RateLimitedError, PermissionDeniedError
 from nonebot_plugin_saa import MessageFactory
 
 from ..errors import BadRequestError
+from ...config import conf
 from ...naga.errors import OrderError, InvalidGameError, UnsupportedGameError
 
 
 def handle_error(silently: bool = False):
     def decorator(func):
         @wraps(func)
-        async def wrapped_func(*args, **kwargs):
+        async def wrapper(*args, **kwargs):
             matcher = current_matcher.get()
 
             try:
                 return await func(*args, **kwargs)
             except MatcherException as e:
                 raise e
             except ActionFailed as e:
@@ -27,20 +28,26 @@
                 logger.exception(e)
             except BadRequestError as e:
                 if not silently:
                     await MessageFactory(e.message).send(reply=True)
                     await matcher.finish()
             except RateLimitedError as e:
                 if not silently:
-                    await MessageFactory("已达到使用次数上限").send(reply=True)
+                    if conf().access_control_reply_on_rate_limited:
+                        await MessageFactory(conf().access_control_reply_on_rate_limited).send(reply=True)
+                    await matcher.finish()
+            except PermissionDeniedError as e:
+                if not silently:
+                    if conf().access_control_reply_on_permission_denied:
+                        await MessageFactory(conf().access_control_reply_on_permission_denied).send(reply=True)
                     await matcher.finish()
             except OrderError as e:
                 logger.exception(e)
                 if not silently:
-                    await MessageFactory("不知道为什么总之解析错误，请在NAGA网页端检查是否已成功解析").send(reply=True)
+                    await MessageFactory(f"不知道为什么总之解析错误，请在NAGA网页端检查是否已成功解析（{str(e)}）").send(reply=True)
                     await matcher.finish()
             except InvalidGameError as e:
                 logger.warning(e)
                 if not silently:
                     await MessageFactory("牌谱链接不正确").send(reply=True)
                     await matcher.finish()
             except UnsupportedGameError as e:
@@ -52,18 +59,18 @@
                 logger.exception(e)
                 if not silently:
                     await MessageFactory(f"网络错误").send(reply=True)
                     await matcher.finish()
             except asyncio.TimeoutError as e:
                 logger.warning(e)
                 if not silently:
-                    await MessageFactory(f"查询超时").send(reply=True)
+                    await MessageFactory(f"查询超时，请在NAGA网页端检查是否已成功解析").send(reply=True)
                     await matcher.finish()
             except Exception as e:
                 logger.exception(e)
                 if not silently:
                     await MessageFactory(f"内部错误：{type(e)}{str(e)}").send(reply=True)
                     await matcher.finish()
 
-        return wrapped_func
+        return wrapper
 
     return decorator
```

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from nonebot.internal.params import Depends
 from nonebot.params import CommandArg
 from nonebot_plugin_saa import MessageFactory
 from nonebot_plugin_session import extract_session, Session
 
 from .errors import BadRequestError
 from .interceptors.handle_error import handle_error
+from .interceptors.send_waiting_prompt import send_waiting_prompt
 from ..ac import ac
 from ..naga import naga
 from ..naga.errors import InvalidKyokuHonbaError
 from ..utils.integer import decode_integer
 from ..utils.nonebot import default_cmd_start
 
 analyze_srv = ac.create_subservice("analyze")
@@ -61,14 +62,15 @@
 
 kyoku_honba_reg = re.compile(r"([东南西])([一二三四1234])局(([0123456789零一两二三四五六七八九十百千万亿]+)本场)?")
 
 
 @naga_analyze_matcher.handle()
 @handle_error()
 @analyze_srv.patch_handler(retire_on_throw=True)
+@send_waiting_prompt()
 async def naga_analyze(matcher: Matcher, cmd_args=CommandArg(),
                        session: Session = Depends(extract_session)):
     args = cmd_args.extract_plain_text().split(' ')
     if "maj-soul" in args[0]:
         mat = uuid_reg.search(args[0])
         if not mat:
             raise BadRequestError("不正确的雀魂牌谱")
```

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/naga/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,32 +71,35 @@
         if self._refresh_worker is None:
             self._refresh_worker = asyncio.create_task(self._refresh())
 
 
 class NagaService:
     _tenhou_haihu_id_reg = re.compile(r"^20\d{8}gm-[a-f\d]{4}-[a-z\d]{4,5}-[a-zA-Z\d]{8}$")
 
-    def __init__(self, cookies: Dict[str, str], timeout: float = 90.0):
+    def __init__(self, cookies: Dict[str, str]):
         if conf().naga_fake_api:
             self.api = FakeNagaApi()
             logger.warning("using fake naga api")
         else:
             self.api = NagaApi(cookies)
 
         self._majsoul_order_mutex = Lock()
         self._tenhou_order_mutex = Lock()
 
         self._last_custom_haihu_id = None
 
         self._order_report = ObservableOrderReport(self.api)
-        self.timeout = timeout
 
     async def close(self):
         await self.api.close()
 
+    @property
+    def timeout(self) -> float:
+        return conf().naga_timeout
+
     async def _get_report(self, haihu_id: str) -> NagaReport:
         report = asyncio.get_running_loop().create_future()
         cancel_flag = False
 
         def _make_callback():
             async def callback(order_report: OrderReportList):
                 try:
```

### Comparing `nonebot_plugin_nagabus-0.2.7/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.8/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/pyproject.toml` & `nonebot_plugin_nagabus-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.2.7/README.md` & `nonebot_plugin_nagabus-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.7/PKG-INFO` & `nonebot_plugin_nagabus-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

