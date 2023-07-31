# Comparing `tmp/pyxk-0.6.4.tar.gz` & `tmp/pyxk-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.4.tar", last modified: Fri Jun  9 06:26:03 2023, max compression
+gzip compressed data, was "pyxk-0.6.5.tar", last modified: Mon Jul 31 13:21:47 2023, max compression
```

## Comparing `pyxk-0.6.4.tar` & `pyxk-0.6.5.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.679999 pyxk-0.6.4/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.4/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-09 06:26:03.679999 pyxk-0.6.4/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1530 2023-06-08 05:36:28.000000 pyxk-0.6.4/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.659999 pyxk-0.6.4/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-08 05:49:20.000000 pyxk-0.6.4/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.659999 pyxk-0.6.4/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.4/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    19762 2023-06-09 05:18:06.000000 pyxk-0.6.4/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      606 2023-06-08 10:10:07.000000 pyxk-0.6.4/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.669999 pyxk-0.6.4/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.4/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3401 2023-06-08 05:42:28.000000 pyxk-0.6.4/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4873 2023-06-07 02:30:14.000000 pyxk-0.6.4/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.669999 pyxk-0.6.4/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.4/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.4/pyxk/m3u8/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4690 2023-06-07 02:27:20.000000 pyxk-0.6.4/pyxk/m3u8/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2946 2023-06-07 02:27:50.000000 pyxk-0.6.4/pyxk/m3u8/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    12434 2023-06-08 05:49:20.000000 pyxk-0.6.4/pyxk/m3u8/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.669999 pyxk-0.6.4/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.4/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7476 2023-06-08 05:49:20.000000 pyxk-0.6.4/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.4/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    16522 2023-06-07 02:31:20.000000 pyxk-0.6.4/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    18885 2023-06-07 02:31:52.000000 pyxk-0.6.4/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-09 06:26:03.659999 pyxk-0.6.4/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       62 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-09 06:26:03.000000 pyxk-0.6.4/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-09 06:26:03.679999 pyxk-0.6.4/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      898 2023-06-09 06:25:59.000000 pyxk-0.6.4/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.579178 pyxk-0.6.5/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.5/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:21:47.579178 pyxk-0.6.5/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.5/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.5/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.5/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    22508 2023-07-31 13:16:20.000000 pyxk-0.6.5/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.5/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.5/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.5/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.579178 pyxk-0.6.5/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.5/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8840 2023-07-31 12:53:28.000000 pyxk-0.6.5/pyxk/m3u8/_initial.py
+-rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.5/pyxk/m3u8/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.5/pyxk/m3u8/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    10222 2023-07-31 13:12:02.000000 pyxk-0.6.5/pyxk/m3u8/m3u8parse.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.579178 pyxk-0.6.5/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.5/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.5/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.5/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.5/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.5/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      558 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       62 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-31 13:21:47.579178 pyxk-0.6.5/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      898 2023-07-31 13:17:30.000000 pyxk-0.6.5/setup.py
```

### Comparing `pyxk-0.6.4/LICENSE` & `pyxk-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.4/PKG-INFO` & `pyxk-0.6.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.4
+Version: 0.6.5
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,22 +23,24 @@
 ```python
 from pprint import pprint
 from pyxk import Client, Response
 
 class Downloader(Client):
     start_urls = ['https://pypi.org' for _ in range(2)]
 
-    async def parse(self, response: Response):
+    async def parse(self, response: Response, **kwargs):
         title = await response.xpath('//title/text()')
         return title.get()
 
     async def completed(self, result: list):
         pprint(result)
 
-Downloader.run()
+
+if __name__ == '__main__':
+    Downloader.run()
 
 >> ['PyPI · The Python Package Index', 'PyPI · The Python Package Index']
 ```
 
 ### pyxk.m3u8
 ```python
 from pyxk.m3u8 import load_url, load_content
```

### Comparing `pyxk-0.6.4/README.md` & `pyxk-0.6.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 ```python
 from pprint import pprint
 from pyxk import Client, Response
 
 class Downloader(Client):
     start_urls = ['https://pypi.org' for _ in range(2)]
 
-    async def parse(self, response: Response):
+    async def parse(self, response: Response, **kwargs):
         title = await response.xpath('//title/text()')
         return title.get()
 
     async def completed(self, result: list):
         pprint(result)
 
-Downloader.run()
+
+if __name__ == '__main__':
+    Downloader.run()
 
 >> ['PyPI · The Python Package Index', 'PyPI · The Python Package Index']
 ```
 
 ### pyxk.m3u8
 ```python
 from pyxk.m3u8 import load_url, load_content
```

### Comparing `pyxk-0.6.4/pyxk/aclient/client.py` & `pyxk-0.6.5/pyxk/aclient/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,31 @@
 import asyncio
-import warnings
+from types import MethodType
 from typing import (
-    Any,
-    List,
-    Tuple,
-    Union,
-    Optional,
-    Mapping,
-    Pattern,
-    Callable
+    Any, List, Tuple, Union, Optional, Mapping, Callable
 )
-from types import MethodType
-from itertools import zip_longest
-from multidict import CIMultiDict
 
-from pyxk.utils import (
-    chardet,
-    LazyLoader,
-    get_user_agent,
-    default_headers,
-)
+from multidict import CIMultiDict
 from pyxk.aclient.typedef import (
-    StrOrURL,
-    Session,
-    Response,
-    EventLoop,
-    CIMDict,
-    Timeout,
-    URLS
+    URL, Session, Response, EventLoop, CIMDict, Timeout, URLS
+)
+from pyxk.utils import (
+    LazyLoader, get_user_agent, default_headers
 )
 
-_copy = LazyLoader("_copy", globals(), "copy")
-_yarl = LazyLoader("_yarl", globals(), "yarl")
-aiohttp = LazyLoader("aiohttp", globals(), "aiohttp")
-_selector = LazyLoader("_selector", globals(), "parsel.selector")
-aiohttp_client_exceptions = LazyLoader("aiohttp_client_exceptions", globals(), "aiohttp.client_exceptions")
+copy = LazyLoader('copy', globals(), 'copy')
+yarl = LazyLoader('yarl', globals(), 'yarl')
+urllib = LazyLoader('urllib', globals(), 'urllib.parse')
+aiohttp = LazyLoader('aiohttp', globals(), 'aiohttp')
+logging = LazyLoader('logging', globals(), 'logging')
+selector = LazyLoader('selector', globals(), 'parsel.selector')
+aiohttp_exceptions = LazyLoader('aiohttp_exceptions', globals(), 'aiohttp.client_exceptions')
+
 
-__all__ = ["Client", "Response"]
+__all__ = ['Client', 'Response']
 
 
 class Client:
     """异步下载器
 
     explain:
     from pyxk import Client, Response
@@ -49,494 +34,613 @@
         start_urls = ['http://www.baidu.com' for _ in range(10)]
 
         async def parse(self, response: Response, **kwargs):
             print(response.url)
 
     Download.run()
     """
-    limit: Optional[int] = None
+
+    limit: int = 100
     timeout: Timeout = None
-    req_kwargs: Optional[Union[dict, List[dict]]] = None
-    async_sleep: Optional[int] = None
-    maximum_retry: Optional[int] = None
-    headers: Optional[Union[dict, CIMDict]] = None
-    semaphore: Union[Optional[int], asyncio.Semaphore] = None
-    verify: Optional[bool] = None
-    start_urls: Union[List[str], List[Tuple[str, dict]]] = []
+    verify: bool = True
+    warning: bool = False
+    headers: Union[dict, CIMDict] = CIMultiDict(default_headers())
+    semaphore: Union[int, asyncio.Semaphore] = 32
     user_agent: Optional[str] = None
-    aiohttp_kwargs: Optional[dict] = None
-    retry_status_code: Optional[list] = None
-    error_status_code: Optional[list] = None
-    until_request_succeed: Optional[Union[bool, List[int]]] = None
-
-    ATTR = (
-        ("limit", 100),
-        ("timeout", 7),
-        ("headers", CIMultiDict(default_headers())),
-        ("semaphore", 16),
-        ("verify", True),
-        ("async_sleep", 1),
-        ("maximum_retry", 20),
-        ("user_agent", get_user_agent()),
-        ("aiohttp_kwargs", {}),
-        ("until_request_succeed", False),
-    )
+    req_kwargs: dict = {}
+    start_urls: Union[List[str], List[Tuple[str, dict]]] = []
+    async_sleep: Union[int, float] = 0
+    max_retries: int = 15
+    aiohttp_kwargs: dict = {}
+    status_retry_list: List[int] = []
+    status_error_list: List[int] = []
+    until_request_succeed: Union[bool, List[int]] = True
+    ATTRS = {
+        'timeout': 10,
+        'semaphore': 16,
+        'user_agent': get_user_agent(),
+    }
 
-    def __init__(self, *, base_url: StrOrURL = None, **kwargs):
-        """异步下载器 init
+    def __init__(self, *, base_url: URL = None, **kwargs):
+        """异步下载器
 
         :param limit: aiohttp 并发控制
         :param timeout: 请求超时时间
-        :param req_kwargs: start_request请求参数
-        :param async_sleep: 异步休眠时间
-        :param maximum_retry: 异步请求最大重试次数
+        :param verify: ssl验证
+        :param warning: 警告信息
         :param headers: 请求头
         :param semaphore: asyncio并发控制
-        :param verify: ssl验证
-        :param start_urls: 请求入口urls
         :param user_agent: User-Agent
+        :param req_kwargs: start_request请求参数
+        :param start_urls: 请求入口urls
+        :param async_sleep: 异步休眠时间
+        :param max_retries: 异步请求最大重试次数
         :param aiohttp_kwargs: aiohttp.ClientSession 实例化参数
-        :param retry_status_code: 请求状态码，包含在列表中的进行重新发送
-        :param error_status_code: 请求状态码，包含在列表中直接抛出错误
+        :param status_retry_list: 请求状态码，包含在列表中的进行重新发送
+        :param status_error_list: 请求状态码，包含在列表中直接抛出错误
         :param until_request_succeed: 请求状态码，直到请求响应成功(可自定义响应状态码)
         :param base_url: base_url 每个请求URL进行拼接
-        :param kwargs: **kwargs 关键字参数进行实例化
         """
+        # 动态生成实例变量
         for key, val in kwargs.items():
             setattr(self, key, val)
+
         # event loop
         self._loop: EventLoop = None
+
         # aiohttp session
         self._session: Session = None
+
         # base_url
-        self._base_url: StrOrURL = self.set_base_url(base_url)
+        self._base_url: URL = self.set_base_url(base_url)
 
     @classmethod
     def run(cls, **kwargs):
-        """程序运行入口 - 应该调用该方法运行
-
-        :params: **kwargs: 类实例化关键字参数
-        """
+        """程序运行入口 - 应该调用该方法运行"""
         self = cls(**kwargs)
+
         # 创建新的 event loop
-        try:
-            self._loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(self._loop)
-            # 运行
-            self._loop.run_until_complete(self.async_start())
-        finally:
+        self._loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(self.loop)
+
+        # 运行
+        self.loop.run_until_complete(self.async_start())
+
+        # 关闭 EventLoop
+        if self.loop:
+            self.loop.close()
             asyncio.set_event_loop(None)
-            if self._loop:
-                # 关闭 event loop
-                self._loop.close()
-        return self
 
-    @property
-    def attr(self):
-        """默认变量ATTR"""
-        return dict(self.ATTR)
+        return self
 
-    async def async_start(self) -> None:
+    async def async_start(self):
         """开启异步下载器"""
-        try:
-            # event loop
-            if (
-                not self._loop
-                or not isinstance(self._loop, asyncio.AbstractEventLoop)
-                or self._loop.is_closed()
-            ):
-                self._loop = asyncio.get_event_loop()
-                asyncio.set_event_loop(self._loop)
-            # semaphore
-            if not isinstance(self.semaphore, (int, float)) or self.semaphore < 0:
-                self.semaphore = self.attr["semaphore"]
+        await self.open()
+
+        # 无效 event loop
+        if not isinstance(self.loop, asyncio.AbstractEventLoop):
+            raise TypeError(f'Event loop must be an instance of AbstractEventLoop, not {type(self.loop).__name__!r}')
+
+        # event loop 已经关闭
+        if self.loop.is_closed():
+            raise ValueError('Event loop is not closed')
+
+        # 配置 asyncio semaphore
+        if isinstance(self.semaphore, int) and self.semaphore > 0:
             self.semaphore = asyncio.Semaphore(self.semaphore)
-            # aiohttp kwargs
-            aiohttp_kwargs = self.aiohttp_kwargs \
-                if isinstance(self.aiohttp_kwargs, dict) \
-                else self.attr["aiohttp_kwargs"]
-            aiohttp_kwargs = _copy.deepcopy(aiohttp_kwargs)
-            # timeout
-            if not aiohttp_kwargs.__contains__("timeout"):
-                if not isinstance(self.timeout, aiohttp.ClientTimeout):
-                    timeout = aiohttp.ClientTimeout(
-                        total=self.timeout
-                        if isinstance(self.timeout, (int, float)) and self.timeout > 0
-                        else self.attr["timeout"]
-                    )
-                else:
-                    timeout = self.timeout
-                aiohttp_kwargs["timeout"] = timeout
-            # connector
-            if not aiohttp_kwargs.__contains__("connector"):
-                aiohttp_kwargs["connector"] = aiohttp.TCPConnector(
-                    loop=self._loop,
-                    limit=self.limit
-                    if isinstance(self.limit, int) and self.limit > 0
-                    else self.attr["limit"],
-                    ssl=bool(self.verify)
-                    if self.verify is not None
-                    else self.attr["verify"],
-                )
-            # headers
-            if aiohttp_kwargs.__contains__("headers"):
-                headers = self.headers \
-                    if self.headers \
-                    else aiohttp_kwargs.pop("headers")
-                if not isinstance(headers, (dict, CIMultiDict)):
-                    headers = {}
-            else:
-                headers = self.headers \
-                    if isinstance(self.headers, (dict, CIMultiDict)) \
-                    else self.attr["headers"]
-            headers = CIMultiDict(_copy.deepcopy(headers))
-            # User Agent
-            if self.user_agent and isinstance(self.user_agent, str):
-                headers["User-Agent"] = self.user_agent
-            else:
-                headers.setdefault("User-Agent", self.attr["user_agent"])
-            aiohttp_kwargs["headers"] = headers
-            # 创建 aiohttp client_session
-            self._session = aiohttp.ClientSession(loop=self._loop, **aiohttp_kwargs)
-            # 开始运行
+        elif not isinstance(self.semaphore, asyncio.Semaphore):
+            self.semaphore = asyncio.Semaphore(self.__class__.ATTRS['semaphore'])
+
+        # aiohttp.Session 实例化参数
+        aiohttp_kwargs = copy.deepcopy(dict(self.aiohttp_kwargs))
+
+        # 为 aiohttp.Session 设置超时时间
+        if isinstance(self.timeout, int) and self.timeout >= 0:
+            aiohttp_kwargs['timeout'] = aiohttp.ClientTimeout(total=self.timeout)
+        elif not aiohttp_kwargs.__contains__('timeout'):
+            aiohttp_kwargs['timeout'] = aiohttp.ClientTimeout(total=self.__class__.ATTRS['timeout'])
+        self.timeout = aiohttp_kwargs['timeout'].total
+
+        # 为 aiohttp.Session 设置连接器
+        if not aiohttp_kwargs.__contains__('connector'):
+            if not isinstance(self.limit, int) or self.limit <= 0:
+                raise ValueError(f'Limit must be a positive integer(正整数), got {self.limit!r}')
+
+            aiohttp_kwargs['connector'] = aiohttp.TCPConnector(
+                limit=self.limit, ssl=bool(self.verify), loop=self.loop
+            )
+
+        # 为 aiohttp.Session 设置 headers(user_agent)
+        self.headers = CIMultiDict(self.headers)
+        # user_agent
+        if self.user_agent and isinstance(self.user_agent, str):
+            self.headers['User-Agent'] = self.user_agent
+        elif not self.headers.__contains__('User-Agent'):
+            self.headers['User-Agent'] = self.__class__.ATTRS['user_agent']
+        self.user_agent = self.headers.get('User-Agent')
+        aiohttp_kwargs['headers'] = self.headers
+
+        # 创建 aiohttp.ClientSession
+        self._session = aiohttp.ClientSession(loop=self.loop, **aiohttp_kwargs)
+
+        # 初始化变量
+        self._init_attrs()
+
+        # 开启请求
+        try:
             await self.start()
-            result = await self.start_request()
-            await self.completed(result)
+            ret = await self.start_request()
+            await self.completed(ret)
         finally:
             await self.async_close()
 
     async def async_close(self):
         """关闭异步下载器"""
+        await self.stop()
+        # 关闭 aiohttp session
+        if self.session:
+            await self.session.close()
+        # 关闭 aiohttp session 之后调用
         await self.close()
-        # 关闭 aiohttp client session
-        if isinstance(self._session, aiohttp.ClientSession) and self._session.closed is False:
-            await self._session.close()
 
     async def start_request(self):
         """start_urls 默认运行方法"""
         if not self.start_urls or not isinstance(self.start_urls, (list, tuple)):
-            raise NotImplementedError(f"{self.__class__.__name__}.start_urls is not available!")
-        # req_kwargs
-        req_kwargs = self.req_kwargs
-        if not req_kwargs or not isinstance(req_kwargs, dict):
-            req_kwargs = {}
-        return await self.gather(
-            self.start_urls,
-            self.parse,
-            cb_kwargs_list=req_kwargs,
-            automatic_base_url=True
-        )
+            raise NotImplementedError(f'Invalid start_urls, got {self.start_urls!r}')
+
+        return await self.gather(self.start_urls, self.parse, set_base_url=True, **dict(self.req_kwargs))
 
     async def request(
         self,
-        url: StrOrURL,
+        url: URL,
         callback: Optional[Callable] = None,
         *,
         method: str = "GET",
         cb_kwargs: Optional[dict] = None,
-        **req_kwargs
+        **kwargs
     ) -> Union[Response, Any]:
         """异步请求发送以及回调
 
+        :return:
         :param url: URL
         :param callback: 响应response 回调函数(函数是异步的)
         :param method: 请求方法(default: GET)
         :param cb_kwargs: 传递给回调函数的关键字参数
-        :param req_kwargs: 异步请求 request参数
+        :param kwargs: 异步请求 request参数
+            params
+            data
+            json
+            cookies
+            headers
+            skip_auto_headers
+            auth
+            allow_redirects
+            max_redirects
+            compress
+            chunked
+            expect100
+            raise_for_status
+            read_until_eof
+            proxy
+            proxy_auth
+            timeout
+            verify_ssl
+            fingerprint
+            ssl_context
+            ssl
+            proxy_headers
+            trace_request_ctx
+            read_bufsize
         :return: Response, Any
         """
-        retry, exc_count, ret, response = 0, 0, None, None
-        maximum_retry = self.maximum_retry \
-            if isinstance(self.maximum_retry, int) and self.maximum_retry > 0 \
-            else self.attr["maximum_retry"]
+        status_retry_list, status_error_list = self.status_retry_list.copy(), self.status_error_list.copy()
+        url, response, result, exc_from_request = self.build_url(url), None, None, None
+        warning = {
+            'status_retry_list': True,
+            'status_error_list': True,
+            'until_request_succeed': True,
+            'timeout': True,
+            'client': True,
+            'server_disconnected': True
+        }
+
         async with self.semaphore:
-            url = self.build_url(url)
-            while True:
+            for _ in range(1, self.max_retries+1):
                 try:
-                    response = await self._session.request(method=method, url=url, **req_kwargs)
-                    # 抛出 error status_code
-                    if isinstance(self.error_status_code, (list, tuple)) and response.status in self.error_status_code:
-                        raise aiohttp.InvalidURL(f"<Response[{response.status}] {url}>")
-                    # 重试 retry status_code
-                    if isinstance(self.retry_status_code, (list, tuple)) and response.status in self.retry_status_code:
-                        response.close()
-                        retry += 1
-                        if retry % 10 == 0:
-                            warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
-                        await self.sleep()
-                        continue
-                    # 直到请求状态码200才返回 until_request_succeed
-                    as_succeed = self.until_request_succeed \
-                        if self.until_request_succeed is not None else self.attr["until_request_succeed"]
-                    if not isinstance(as_succeed, (list, tuple)):
-                        as_succeed = [200] if as_succeed else []
-                    if as_succeed and response.status not in as_succeed:
-                        response.close()
-                        retry += 1
-                        if retry % 10 == 0:
-                            warnings.warn(f"<Response[{response.status}] {url}>, Retry: {retry}", stacklevel=4)
-                        await self.sleep()
+                    response = result = await self.session.request(method=method, url=url, **kwargs)
+
+                    # 直到请求成功
+                    if self.until_request_succeed:
+                        if response.status in self.until_request_succeed:
+                            status_retry_list, status_error_list = [], []
+                        else:
+                            # 提示信息
+                            await self._warning('until_request_succeed', url, warning, response)
+                            continue
+
+                    # 状态码错误
+                    if response.status in status_error_list:
+                        raise aiohttp_exceptions.ClientError(f'<Response[{response.status}] {url}>')
+
+                    # 状态码重试
+                    if response.status in status_retry_list:
+                        # 提示信息
+                        await self._warning('status_retry_list', url, warning, response)
                         continue
-                    # 添加自定义方法
-                    add_method_to_response(response)
+
+                    # 添加 aiohttp.ClientResponse 实例方法
+                    add_instance_method(response)
+
                     # 开启回调函数
                     if callable(callback):
                         cb_kwargs = dict(cb_kwargs or {})
-                        ret = await callback(response, **cb_kwargs)
-                        response.close()
-                    else:
-                        ret = response
+                        result = await callback(response, **dict(cb_kwargs or {}))
                     break
+
                 # 请求超时 重试
-                except asyncio.exceptions.TimeoutError:
-                    if response:
-                        response.close()
-                    exc_count += 1
-                    if exc_count >= maximum_retry:
-                        raise
-                    # warnings.warn(f"<{url}> Timeout", stacklevel=4)
-                    await self.sleep()
+                except asyncio.exceptions.TimeoutError as exc:
+                    # 提示信息
+                    await self._warning('timeout', url, warning, response)
+                    exc_from_request = exc
+
                 # 连接错误 重试
                 except (
-                    aiohttp_client_exceptions.ClientOSError,
-                    aiohttp_client_exceptions.ClientPayloadError,
-                    aiohttp_client_exceptions.ClientConnectorError,
-                ):
-                    if response:
-                        response.close()
-                    exc_count += 1
-                    if exc_count >= maximum_retry:
-                        raise
-                    # warnings.warn(f"<{url}> ConnectorError", stacklevel=4)
-                    await self.sleep()
+                    aiohttp_exceptions.ClientOSError,
+                    aiohttp_exceptions.ClientPayloadError,
+                    aiohttp_exceptions.ClientConnectorError,
+                ) as exc:
+                    # 提示信息
+                    await self._warning('client', url, warning, response)
+                    exc_from_request = exc
+
                 # 服务器拒绝连接
-                except aiohttp_client_exceptions.ServerDisconnectedError:
+                except aiohttp_exceptions.ServerDisconnectedError as exc:
+                    # 提示信息
+                    await self._warning('server_disconnected', url, warning, response)
+                    exc_from_request = exc
+
+                finally:
+                    # 关闭连接
                     if response:
                         response.close()
-                    exc_count += 1
-                    if exc_count >= maximum_retry:
-                        raise
-                    # warnings.warn(f"<{url}> ServerDisconnectedError", stacklevel=4)
-                    await self.sleep()
-            return ret
+
+            else:
+                # 抛出错误
+                if exc_from_request:
+                    raise exc_from_request
+                # 达到最大请求次数
+                raise RuntimeError(
+                    f'<Response[{response.status if response else None}] '
+                    f'{url}>, max_retries: {self.max_retries}'
+                )
+
+        return result
+
+    def _init_attrs(self):
+        # 最大重试次数
+        if not isinstance(self.max_retries, int) or self.max_retries <= 0:
+            raise ValueError(f'max_retries must be a positive integer(正整数), got {self.max_retries!r}')
+
+        # 状态码重试列表
+        if not isinstance(self.status_retry_list, (list, tuple)):
+            raise ValueError(f'status_retry_list must be a list, got {self.status_retry_list!r}')
+
+        # 状态码错误列表
+        if not isinstance(self.status_error_list, (list, tuple)):
+            raise ValueError(f'status_retry_list must be a list, got {self.status_error_list!r}')
+
+        # 直到请求成功
+        if not isinstance(self.until_request_succeed, (list, tuple)):
+            self.until_request_succeed = [200] if self.until_request_succeed else []
+
+    async def _warning(self, who: str, url: str, warning: dict, response: Response):
+        """打印警告信息"""
+        # 状态码
+        status = response.status if response else None
+        # 全部警告信息
+        who_list = {
+            'status_retry_list':
+                f'<Response[{status}] {url}> be in '
+                f'status_retry_list:{self.status_retry_list!r}',
+            'until_request_succeed':
+                f'<Response[{status}] {url}> be in '
+                f'until_request_succeed:{self.until_request_succeed!r}',
+            'timeout': f'{url}> Timeout',
+            'client': f'{url}> client error',
+            'server_disconnected': f'{url}> server disconnected'
+        }
+
+        # 确保 每个链接每个警告类型 只会打印一次
+        if self.warning and warning[who]:
+            logging.warning(who_list[who])
+            warning[who] = False
+
+        await self.sleep()
 
     async def gather(
         self,
         urls: URLS,
         callback: Optional[Callable] = None,
         *,
         method: str = "GET",
-        cb_kwargs_list: Optional[Union[List[dict], dict]] = None,
+        cb_kwargs_list: Union[List[dict], dict] = None,
         return_exceptions: bool = False,
-        automatic_base_url: bool = False,
+        set_base_url: Union[bool, str] = False,
         **req_kwargs
     ) -> list:
         """发送url列表，创建异步任务 并发发送
 
         :param urls: Url List
         :param callback: 响应response 回调函数(函数是异步的)
         :param method: 请求方法(default: GET)
         :param cb_kwargs_list: 回调函数关键字参数列表
         :param return_exceptions: 错误传递(default: False)
         :param req_kwargs: 异步请求 request参数
+        :param set_base_url: 是否设置base_url
         :return: list
         """
         if not isinstance(urls, (list, tuple)):
-            raise TypeError(f"urls must be 'tuple' or 'list', not {type(urls).__name__!r}")
+            raise TypeError(f'urls must be a list, not {type(urls).__name__!r}')
+
         length = len(urls)
-        # parse cb_kwargs_list
-        if isinstance(cb_kwargs_list, dict):
-            cb_kwargs_list = [cb_kwargs_list for _ in range(length)]
-        elif isinstance(cb_kwargs_list, (list, tuple)):
-            cb_kwargs_list = cb_kwargs_list[:length]
-            if len(cb_kwargs_list) < length:
-                cb_kwargs_list.extend([{} for _ in range(length-len(cb_kwargs_list))])
-        else:
-            cb_kwargs_list = [{} for _ in range(length)]
-        # parse urls
+        cb_kwargs_list = self._parse_gather_cb(length, cb_kwargs_list)
+
         for index, item in enumerate(urls):
-            url, cb_kwargs = None, None
-            if isinstance(item, (list, tuple)) and len(item) >= 2:
-                url, cb_kwargs = item[0], dict(item[1])
-            else:
-                url, cb_kwargs = item, {}
+            url, cb_kwargs = item, {}
+            # 解析 url 和 回调参数
+            if isinstance(item, (list, tuple)):
+                if len(item) >= 2:
+                    url, cb_kwargs = item[0], dict(item[1]).copy()
+                elif len(item) == 1:
+                    url, cb_kwargs = item[0], {}
+                else:
+                    raise ValueError(f'urls invalid, got {item!r}')
+
+            # 更新数据
             urls[index] = url
             cb_kwargs.update(cb_kwargs_list[index])
             cb_kwargs_list[index] = cb_kwargs
-        # 收集任务
-        tasks = []
-        for url, cb_kwargs in zip_longest(urls, cb_kwargs_list):
-            # base url
-            if automatic_base_url and not self.base_url:
-                self.base_url = url
-            task = self.request(
+
+        # 设置base_url
+        if set_base_url and isinstance(set_base_url, str):
+            self.base_url = set_base_url
+        elif set_base_url and not self.base_url:
+            self.base_url = urllib.urljoin(urls[0], '.')
+
+        # 提交异步任务
+        tasks = [
+            self.request(
                 url=url,
                 callback=callback,
                 method=method,
                 cb_kwargs=cb_kwargs,
                 **req_kwargs
             )
-            tasks.append(task)
-        result = await asyncio.gather(*tasks, return_exceptions=return_exceptions)
-        return result
+            for url, cb_kwargs in zip(urls, cb_kwargs_list)
+        ]
+        return await asyncio.gather(*tasks, return_exceptions=return_exceptions)
+
+    @staticmethod
+    def _parse_gather_cb(length, cb_kwargs_list):
+        """解析 gather 的回调参数"""
+        # 设置 cb_kwargs_list
+        if isinstance(cb_kwargs_list, (list, tuple)):
+            cb_kwargs_list = cb_kwargs_list[:length]
+            cb_kwargs_list.extend(
+                [{}] * (length - len(cb_kwargs_list))
+            )
+
+        elif isinstance(cb_kwargs_list, dict):
+            cb_kwargs_list = [cb_kwargs_list] * length
+
+        else:
+            cb_kwargs_list = [{}] * length
+        # 将每项转化为字典
+        cb_kwargs_list = [dict(item) for item in cb_kwargs_list]
+        return cb_kwargs_list
+
+    async def parse(self, response: Response, **kwargs):
+        """默认解析函数"""
+        raise NotImplementedError(f'{self.__class__.__name__}.parse not implemented')
+
+    async def completed(self, result: list):
+        """运行完成结果回调函数"""
+
+    async def open(self):
+        """创建 aiohttp session 之前调用"""
+
+    async def close(self):
+        """关闭 aiohttp session 之后调用"""
+
+    async def start(self):
+        """创建 aiohttp session 之后调用"""
 
-    async def sleep(self, delay: Optional[Union[int, float]] = None, result: Any = None):
+    async def stop(self):
+        """关闭 aiohttp session 之前调用"""
+
+    async def sleep(self, delay: Union[int, float, None] = None, result: Any = None):
         """异步休眠
 
         :param delay: 休眠时间
         :param result: 返回值
         :return: result
         """
-        if not isinstance(delay, (int, float)) or delay < 0:
-            delay = self.async_sleep \
-                if isinstance(self.async_sleep, (int, float)) and self.async_sleep >= 0 \
-                else self.attr["async_sleep"]
+        if delay is None:
+            if not isinstance(self.async_sleep, (int, float)) or self.async_sleep < 0:
+                raise ValueError(f'async_sleep must be a positive integer(正整数), got {self.async_sleep!r}')
+            delay = self.async_sleep
+
+        elif not isinstance(delay, (int, float)) or delay < 0:
+            raise ValueError(f'delay must be a positive integer(正整数), got {delay!r}')
+
         return await asyncio.sleep(delay, result=result)
 
-    def build_url(self, _url) -> StrOrURL:
+    def build_url(self, _url) -> URL:
         """构造完整url地址"""
-        if not isinstance(_url, (str, _yarl.URL)):
+        if not isinstance(_url, (str, yarl.URL)):
             return _url
-        _url = _yarl.URL(_url)
+        _url = yarl.URL(_url)
         if _url.is_absolute():
             return _url
-        if self._base_url and isinstance(self._base_url, _yarl.URL):
+        if self._base_url and isinstance(self._base_url, yarl.URL):
             return self._base_url.join(_url)
         return _url
 
     @staticmethod
-    def set_base_url(url: StrOrURL) -> StrOrURL:
+    def set_base_url(url: URL) -> URL:
         """设置 base_url"""
-        if not url or not isinstance(url, (str, _yarl.URL)):
+        if not url or not isinstance(url, (str, yarl.URL)):
             return None
-        url = _yarl.URL(url)
+        url = yarl.URL(url)
         if not url.is_absolute():
             # 不是绝对路径
             return None
         return url
 
     @property
     def loop(self) -> EventLoop:
         """event loop"""
         return self._loop
 
     @property
-    def base_url(self) -> StrOrURL:
+    def session(self) -> Session:
+        """aiohttp session"""
+        return self._session
+
+    @property
+    def base_url(self) -> URL:
         """base_url"""
         return self._base_url
 
     @base_url.setter
-    def base_url(self, _url: StrOrURL):
+    def base_url(self, _url: URL):
         self._base_url = self.set_base_url(_url)
 
-    async def parse(self, response: Response, **kwargs):
-        """默认解析函数"""
-        raise NotImplementedError(f"'{self.__class__.__name__}.parse' not implemented!")
-
-    async def completed(self, result: list):
-        """运行完成结果回调函数"""
-
-    async def start(self):
-        """创建 aiohttp session 后调用"""
-
-    async def close(self):
-        """关闭 aiohttp session 前调用"""
 
 async def xpath(
     self,
     query: str,
-    namespaces: Optional[Mapping[str, str]] = None,
-    encoding: Optional[str] = None,
+    text: Optional[str] = None,
     type: Optional[str] = None,
-    root: Optional[Any] = None,
+    encoding: str = "utf8",
     base_url: Optional[str] = None,
-    _expr: Optional[str] = None,
-    huge_tree: Optional[bool] = None,
-    errors: str = "strict",
-    **kwargs
+    namespaces: Optional[Mapping[str, str]] = None,
+    **kwargs: Any,
 ):
-    """Response.xpath"""
-    text = await self.text(encoding=encoding, errors=errors)
-    selector = _selector.Selector(
-        text=text,
-        type=type,
-        _expr=_expr,
-        namespaces=namespaces,
-        root=root or _selector._NOT_SET,
-        base_url=base_url,
-        huge_tree=huge_tree or _selector.LXML_SUPPORTS_HUGE_TREE,
+    """aiohttp.ClientResponse - selector.xpath
+
+    :param self: aiohttp.ClientResponse 实例
+    :param query: xpath查询字符串
+    :param text: str对象
+    :param type: 文件类型 - "html"(default), "json", or "xml"
+    :param encoding: text encoding
+    :param base_url: 为文档设置URL
+    :param namespaces: `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
+        for additional prefixes to those registered with `register_namespace(prefix, uri)`.
+        Contrary to `register_namespace()`, these prefixes are not
+        saved for future calls.
+    :param kwargs: xpath kwargs
+    """
+    if not text:
+        text = await self.text()
+    # selector
+    sel = selector.Selector(
+        text=text, type=type, base_url=base_url, encoding=encoding, namespaces=namespaces
     )
-    return selector.xpath(query=query, **kwargs)
+    # xpath
+    return sel.xpath(query=query, **kwargs)
+
 
 async def css(
     self,
     query: str,
-    namespaces: Optional[Mapping[str, str]] = None,
-    encoding: Optional[str] = None,
+    text: Optional[str] = None,
     type: Optional[str] = None,
-    root: Optional[Any] = None,
+    encoding: str = "utf8",
     base_url: Optional[str] = None,
-    _expr: Optional[str] = None,
-    huge_tree: Optional[bool] = None,
-    errors: str = "strict"
+    namespaces: Optional[Mapping[str, str]] = None,
 ):
-    """Response.css"""
-    text = await self.text(encoding=encoding, errors=errors)
-    selector = _selector.Selector(
-        text=text,
-        type=type,
-        _expr=_expr,
-        namespaces=namespaces,
-        root=root or _selector._NOT_SET,
-        base_url=base_url,
-        huge_tree=huge_tree or _selector.LXML_SUPPORTS_HUGE_TREE,
+    """aiohttp.ClientResponse - selector.css
+
+    :param self: aiohttp.ClientResponse 实例
+    :param query: xpath查询字符串
+    :param text: str对象
+    :param type: 文件类型 - "html"(default), "json", or "xml"
+    :param encoding: text encoding
+    :param base_url: 为文档设置URL
+    :param namespaces:
+    `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
+    for additional prefixes to those registered with `register_namespace(prefix, uri)`.
+    Contrary to `register_namespace()`, these prefixes are not
+    saved for future calls.
+    """
+    if not text:
+        text = await self.text()
+    # selector
+    sel = selector.Selector(
+        text=text, type=type, base_url=base_url, encoding=encoding, namespaces=namespaces
     )
-    return selector.css(query=query)
+    # css
+    return sel.css(query=query)
+
 
 async def re(
     self,
-    regex: Union[str, Pattern[str]],
-    replace_entities: bool = True,
-    namespaces: Optional[Mapping[str, str]] = None,
-    encoding: Optional[str] = None,
+    regex: str,
+    text: Optional[str] = None,
     type: Optional[str] = None,
-    root: Optional[Any] = None,
+    encoding: str = "utf8",
     base_url: Optional[str] = None,
-    _expr: Optional[str] = None,
-    huge_tree: Optional[bool] = None,
-    errors: str = "strict",
+    namespaces: Optional[Mapping[str, str]] = None,
+    replace_entities: bool = True,
 ):
-    """Response.re"""
-    text = await self.text(encoding=encoding, errors=errors)
-    selector = _selector.Selector(
-        text=text,
-        type=type,
-        _expr=_expr,
-        namespaces=namespaces,
-        root=root or _selector._NOT_SET,
-        base_url=base_url,
-        huge_tree=huge_tree or _selector.LXML_SUPPORTS_HUGE_TREE,
+    """aiohttp.ClientResponse - selector.re
+
+    :param self: aiohttp.ClientResponse 实例
+    :param regex: 编译的正则表达式 或者 字符串
+    :param text: str对象
+    :param type: 文件类型 - "html"(default), "json", or "xml"
+    :param encoding: text encoding
+    :param base_url: 为文档设置URL
+    :param namespaces:
+    `namespaces` is an optional `prefix: namespace-uri` mapping (dict)
+    for additional prefixes to those registered with `register_namespace(prefix, uri)`.
+    Contrary to `register_namespace()`, these prefixes are not
+    saved for future calls.
+    :param replace_entities:
+    By default, character entity references are replaced by their
+    corresponding character (except for ``&amp;`` and ``&lt;``).
+    Passing ``replace_entities`` as ``False`` switches off these
+    replacements.
+    """
+    if not text:
+        text = await self.text()
+    # selector
+    sel = selector.Selector(
+        text=text, type=type, base_url=base_url, encoding=encoding, namespaces=namespaces
     )
-    return selector.re(regex=regex, replace_entities=replace_entities)
+    # re
+    return sel.re(regex=regex, replace_entities=replace_entities)
+
 
 def urljoin(self, _url):
-    """Response.urljoin"""
+    """urljoin
+
+    :param self: aiohttp.ClientResponse 实例
+    :param _url: url
+    :return: url
+    """
     if isinstance(_url, str):
-        _url = _yarl.URL(_url)
-    elif not isinstance(_url, _yarl.URL):
+        _url = yarl.URL(_url)
+    elif not isinstance(_url, yarl.URL):
         return _url
     if _url.is_absolute():
         return _url
     return self.url.join(_url)
 
-async def apparent_encoding(self):
-    """Response.apparent_encoding"""
-    byte = await self.read()
-    return chardet(byte)["encoding"]
-
-def add_method_to_response(response):
-    """为异步response添加实例方法"""
-    response.re = MethodType(re, response)
-    response.css = MethodType(css, response)
-    response.xpath = MethodType(xpath, response)
-    response.urljoin = MethodType(urljoin, response)
-    response.apparent_encoding = MethodType(apparent_encoding, response)
+
+def add_instance_method(response):
+    """为异步response添加实例方法 - re, css, xpath, urljoin"""
+    setattr(response, 're', MethodType(re, response))
+    setattr(response, 'css', MethodType(css, response))
+    setattr(response, 'xpath', MethodType(xpath, response))
+    setattr(response, 'urljoin', MethodType(urljoin, response))
```

### Comparing `pyxk-0.6.4/pyxk/aclient/typedef.py` & `pyxk-0.6.5/pyxk/aclient/typedef.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from asyncio import AbstractEventLoop
 from typing import Any, Union, List, Dict, Optional
 
 from yarl import URL
 from aiohttp import ClientSession, ClientResponse, ClientTimeout
 
 
-__all__ = ["Session", "EventLoop", "Response", "CIMDict", "StrOrURL", "Timeout"]
+__all__ = ['Session', 'EventLoop', 'Response', 'CIMDict', 'URL', 'Timeout', 'URLS']
 
+URL = Optional[Union[str, URL]]
+URLS = Union[
+    List[URL],
+    List[List[Union[Any, Dict[str, Any]]]]
+]
 EventLoop = Optional[AbstractEventLoop]
 Session = Optional[ClientSession]
 Response = Optional[ClientResponse]
 CIMDict = Optional[CIMultiDict]
-StrOrURL = Optional[Union[str, URL]]
-Timeout = Optional[Union[int, float, ClientTimeout]]
-URLS = Union[
-    List[StrOrURL],
-    List[List[Union[Any, Dict[str, Any]]]]
-]
+Timeout = Union[int, float, ClientTimeout, None]
```

### Comparing `pyxk-0.6.4/pyxk/m3u8/enter_point.py` & `pyxk-0.6.5/pyxk/m3u8/entry_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import click
-from pyxk.utils import LazyLoader, get_user_agent
-
-_m3u8 = LazyLoader("_m3u8", globals(), "pyxk.m3u8")
+from pyxk import get_user_agent
+from pyxk.m3u8 import load_url, load_content
 
 
 @click.group(invoke_without_command=False, chain=False)
 @click.option("-o", "--output", "output", type=str, default=None, help="M3U8存储路径")
 @click.option("--reload", is_flag=True, help="重载m3u8资源")
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
@@ -19,26 +18,26 @@
     # 将参数传递给子命令
     if ctx.invoked_subcommand:
         ctx.obj.update(ctx.params)
 
 
 @main.command
 @click.pass_obj
-@click.argument("content", type=click.Path(exists=True), metavar="<File>")
+@click.argument("content", type=str, metavar="<File>")
 @click.option("-u", "--url", "_url", type=str, default=None, help="m3u8 url")
 @click.option("-o", "--output", "output", type=str, default=None, help="M3U8存储路径")
 @click.option("--reload", is_flag=True, help="重载m3u8资源")
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=None, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
 def file(obj, content, _url, output, reload, reserve, headers, verify, limit, user_agent):
     """使用m3u8文件下载资源"""
-    _m3u8.load_content(
+    load_content(
         content=content,
         url=_url,
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
         headers=dict(headers or obj["headers"]),
         verify=verify,
@@ -55,15 +54,15 @@
 @click.option("--reserve", is_flag=True, help="保留m3u8资源")
 @click.option("-h", "--headers", "headers", type=(str, str), multiple=True, help="Request Headers")
 @click.option("--no-verify", "verify", is_flag=True, default=True, help="Request Verify")
 @click.option("-l", "--limit", "limit", type=int, default=None, help="下载并发量")
 @click.option("-ua", "--user-agent", "user_agent", type=str, default=None, help="User-Agent")
 def url(obj, _url, output, reload, reserve, headers, verify, limit, user_agent):
     """使用m3u8链接下载资源"""
-    _m3u8.load_url(
+    load_url(
         url=_url,
         output=output or obj["output"],
         reload=reload,
         reserve=reserve,
         headers=dict(headers or obj["headers"]),
         verify=verify,
         limit=limit or obj["limit"],
```

### Comparing `pyxk-0.6.4/pyxk/m3u8/m3u8download.py` & `pyxk-0.6.5/pyxk/m3u8/downloader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,130 +1,154 @@
-"""m3u8资源下载器"""
 import os
 import shlex
-import asyncio
-import aiofiles
 import subprocess
+from typing import Optional
 from concurrent.futures import ThreadPoolExecutor
 
-from pyxk.aes import Cryptor
-from pyxk.utils import make_open
-from pyxk.aclient import Client
+import aiofiles
+
+from pyxk import (
+    Client,
+    Response,
+    tasks_progress,
+    download_progress
+)
+from pyxk.aes import Crypto, MODES
 
 
 class Downloader(Client):
-    """m3u8 - segments 下载器"""
 
-    timeout = 30
-    maximum_retry = 30
-    error_status_code = list(range(404, 411))
-    until_request_succeed = True
+    limit = 1000
+    timeout = 100
+    warning = False
+    status_error_list = list(range(400, 411))
+    until_request_succeed = [200]
 
     def __init__(
-        self, *, m3obj, m3u8keys=None, segments=None, progress=None, download=None, **kwargs
+        self,
+        table: object,
+        output: str,
+        m3u8keys: dict,
+        start_urls: list,
+        console: object,
+        temp: str,
+        **kwargs
     ):
-        """m3u8 - segments 下载器
-
-        :param m3obj: pyxk.m3u8downloader.main.M3U8
-        :param m3u8keys: m3u8资源加密密钥
-        :param segments: m3u8 segments
-        :param progress: rich.progress.Progress
-        :param download: rich.progress.Progress
-        :param kwargs: **kwargs
-        """
         super().__init__(**kwargs)
-        self.m3obj = m3obj
-        self.limit = m3obj.limit
-        self.cipher = {index: Cryptor(**cipher) for index, cipher in m3u8keys.items()} if m3u8keys else {}
-        self.temp_file = os.path.join(self.m3obj.temp_file, "segments") if self.m3obj.temp_file else None
-        self.semaphore = m3obj.limit
-        self.start_urls: dict = segments
-        self.task = None
-        self.progress = progress
-        self.download = download
-        self.user_agent = m3obj.user_agent
+
+        self.ciphers = {
+            url: Crypto(keys['key'], MODES.CBC, iv=keys['iv'])
+            for url, keys in m3u8keys.items()
+        }
+        self.table = table
+        self.output = output
+        self.start_urls = start_urls
+
+        # 进度条
+        self.progress = tasks_progress()
+        self.task = self.progress.add_task('', total=len(self.start_urls))
+
+        # 添加进度条到live
+        self.table.add_section()
+        self.table.add_row(self.progress)
+
+        self.temp = temp
+        self.console = console
 
     async def start_request(self):
-        # 数据不齐全 不下载
-        if (
-            not self.start_urls
-            or not self.temp_file
-            or not self.m3obj.output
-        ):
-            return None
-        os.makedirs(self.temp_file, exist_ok=True)
-        # 添加进度条任务
-        self.task = self.progress.add_task(description="", total=len(self.start_urls))
-        # 收集异步任务
-        tasks, result = [], []
-        for index, item in self.start_urls.items():
-            file = os.path.join(self.temp_file, f"{index}.ts")
-            result.append(file)
-            # 跳过已下载文件
+
+        ret = []
+        for item in self.start_urls.copy():
+            file = item[1]['file']
+            ret.append(file)
+
+            # 本地存在文件
             if os.path.isfile(file) and os.path.getsize(file) > 0:
-                self.progress.update(self.task, advance=1)
+                self.start_urls.remove(item)
                 continue
-            task = self.request(
-                item["url"],
-                cb_kwargs={"file": file, "key": item["key"]},
-                callback=self.parse,
-            )
-            tasks.append(task)
-        await asyncio.gather(*tasks)
-        return result
 
-    async def parse(self, response, file, key):
+        # 更新进度条
+        self.progress.update(
+            self.task,
+            completed=len(ret)-len(self.start_urls)
+        )
+
+        # 没有下载数据
+        if not self.start_urls:
+            return ret
+
+        await super().start_request()
+        return ret
+
+    async def parse(self, response: Response, file: str, key: Optional[str]):
+        """解析segment数据"""
+        # 获取segment内容
         content = await response.content.read()
         # 解密
-        if key is not None and self.cipher:
-            content = self.cipher[key].decrypt(content)
-        async with aiofiles.open(file, "wb") as write_fileobj:
-            await write_fileobj.write(content)
+        if key:
+            content = self.ciphers[key].decrypt(content)
+
+        async with aiofiles.open(file, 'wb') as write_file_obj:
+            # 本地存储
+            await write_file_obj.write(content)
+
         # 更新进度条
         self.progress.update(self.task, advance=1)
-        return file
 
-    async def completed(self, result):
-        self.cipher, self.start_urls = None, None
-        if not result:
+    async def completed(self, ret: list):
+        """使用模块ffmpeg合并m3u8"""
+        if not ret:
             return
+
         # 创建 filelist 文件
-        filelist, filesize = os.path.join(self.temp_file, "filelist.txt"), 0
-        with make_open(filelist, "w", encoding="utf-8") as write_fileobj:
-            for file in result:
+        filelist, filesize = os.path.join(self.temp, "filelist.txt"), 0
+
+        with open(filelist, "w", encoding="utf-8") as write_fileobj:
+            for file in ret:
                 write_fileobj.write(f"file '{file}'\n")
                 filesize += (os.path.getsize(file) - 16400)
 
         # ffmpeg 视频合并代码, 监测合并完成状态
         args = shlex.split(
-            f"ffmpeg -loglevel quiet -f concat -safe 0 -i {filelist} -c copy {self.m3obj.output} -y"
+            f"ffmpeg -loglevel quiet -f concat -safe 0 -i {filelist} -c copy {self.output} -y"
         )
         merge_completed = False
 
         # ffmpeg 合并函数
         def merge_segments():
             try:
                 subprocess.run(args=args, check=True)
             except FileNotFoundError:
-                self.m3obj._console.log("[red]ffmpeg is not available![/]")
-                self.m3obj._reserve = True
+                self.console.log("[red]ffmpeg is not available![/]")
             finally:
                 nonlocal merge_completed
                 merge_completed = True
 
         # 合并进度条
         def merge_progress():
-            import time
-            completed_filezise = os.path.getsize(self.m3obj.output) if os.path.isfile(self.m3obj.output) else 0
-            task = self.download.add_task(description="", total=filesize)
+            from time import sleep
+
+            sleep(0.2)
+            if merge_completed:
+                return
+
+            completed_filezise = lambda :os.path.getsize(self.output) if os.path.isfile(self.output) else 0
+            progress = download_progress(transient=True)
+            task = progress.add_task(
+                description="", total=filesize, visible=False
+            )
+            self.table.add_row(progress)
+
             while True:
-                self.download.update(task, completed=completed_filezise)
+                # 停止循环
                 if merge_completed:
-                    if os.path.isfile(self.m3obj.output):
-                        self.download.update(task, completed=filesize)
+                    progress.update(task, completed=filesize, visible=False)
                     break
-                time.sleep(0.25)
+
+                progress.update(task, completed=completed_filezise(), visible=True)
+                sleep(0.25)
+
         # 开启多线程
         pool = ThreadPoolExecutor()
         pool.submit(merge_segments)
         pool.submit(merge_progress)
         pool.shutdown()
```

### Comparing `pyxk-0.6.4/pyxk/m3u8/main.py` & `pyxk-0.6.5/pyxk/m3u8/m3u8parse.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,365 +1,355 @@
-"""m3u8资源解析和下载"""
 import os
-from typing import Union, Optional
+from typing import Optional, Union
+from multidict import CIMultiDict
 
-from pyxk.utils import (
-    rename_file,
-    hash256,
-    make_open,
+import m3u8
+
+from pyxk.m3u8._initial import _M3U8Init
+from pyxk.m3u8.downloader import Downloader
+from pyxk import (
+    chardet,
+    normpath,
     LazyLoader,
-    progress_column,
-    download_column,
-    human_playtime
+    human_playtime,
+    read_file_by_generator
 )
-from pyxk.m3u8.m3u8parse import M3U8Parse
-from pyxk.m3u8.m3u8download import Downloader
 
-_rich_box = LazyLoader("_rich_box", globals(), "rich.box")
-_rich_live = LazyLoader("_rich_live", globals(), "rich.live")
-_rich_table = LazyLoader("_rich_table", globals(), "rich.table")
-_rich_panel = LazyLoader("_rich_panel", globals(), "rich.panel")
-_rich_console = LazyLoader("_rich_console", globals(), "rich.console")
-_requests = LazyLoader("_requests", globals(), "pyxk.requests")
-
-
-class M3U8:
-    """m3u8资源下载器"""
-    def __init__(self):
-        # m3u8文件输出
-        self._output = None
-        # m3u8下载存储路径
-        self._temp_file = None
-        # 重新下载
-        self._reload = False
-        # 下载完成后保留m3u8文件
-        self._reserve = False
-        # request - verify
-        self._verify = True
-        # request - headers
-        self._headers = None
-        # limit
-        self._limit = 16
-        # user agent
-        self._user_agent = None
-        self._session = None
-        self._console = _rich_console.Console()
-
-    @property
-    def output(self):
-        """output"""
-        return self._output
-
-    @output.setter
-    def output(self, path: Optional[str]) -> None:
-        if path and isinstance(path, str):
-            path = "_".join(path.split(" "))
-            path = os.path.normpath(os.path.abspath(path))
-        else:
-            self._output, self._temp_file = None, None
-            return
-        self._output, dir_name, basename = rename_file(path, suffix="mp4")
-        self._temp_file = os.path.join(dir_name, f".{basename.removesuffix('.mp4')}_temp")
+_box = LazyLoader("_box", globals(), "rich.box")
+_live = LazyLoader("_live", globals(), "rich.live")
+_panel = LazyLoader("_panel", globals(), "rich.panel")
+_table = LazyLoader("_table", globals(), "rich.table")
 
-    def load_url(
+
+__all__ = ['M3u8Parser', 'load_url', 'load_content']
+
+
+class M3u8Parser(_M3U8Init):
+
+    def load_content(
         self,
-        url: str,
-        *,
+        content: str,
+        url: Optional[str] = None,
         output: Optional[str] = None,
-        reload: bool = False,
-        reserve: bool = False,
-        headers: Optional[dict] = None,
-        verify: bool = True,
-        limit: int = 16,
+        verify: Optional[bool] = None,
+        headers: Union[dict, CIMultiDict, None] = None,
         user_agent: Optional[str] = None,
+        reload: Optional[bool] = None,
+        reserve: Optional[bool] = None,
+        limit: Optional[int] = None
     ):
-        """使用m3u8链接下载资源
+        """load m3u8 url
 
+        :param content: m3u8 content
         :param url: m3u8 url
-        :param output: m3u8资源输出到文件
-        :param reload: 重新从网络加载m3u8文件
-        :param reserve: 下载完成后保留m3u8文件
-        :param headers: request 请求头
-        :param verify: request verify
-        :param limit: 异步下载并发量
-        :param user_agent: User-Agent
+        :param output: 文件输出路径
+        :param verify: verify ssl
+        :param headers: Headers
+        :param user_agent: User agent
+        :param reload: 重载m3u8文件
+        :param reserve: 下载完成保留m3u8文件
+        :param limit: 异步下载limit
         """
-        self.output, self._limit = output, limit if isinstance(limit, int) and limit > 0 else 16
-        self._reload, self._reserve = bool(reload), bool(reserve)
-        self._headers, self._verify = headers, bool(verify)
-        self._user_agent = user_agent if user_agent and isinstance(user_agent, str) else None
-        self._session = _requests.Session(user_agent=self._user_agent)
-        # 关闭requests警告
-        if self._verify is False:
-            import urllib3
-            urllib3.disable_warnings()
-        content = self.get_m3u8_content(url)
-        # 无效m3u8内容
-        if not self._is_m3u8_content(content):
-            self._console.print("[red b]m3u8 url is not available!")
-            return None
+        # 文件路径
+        self.output = output
+
+        # 初始化数据
+        self._initialization(
+            verify=verify,
+            headers=headers,
+            user_agent=user_agent,
+            reload=reload,
+            reserve=reserve,
+            limit=limit
+        )
+
+        # 无效 m3u8 content
+        if not isinstance(content, str) or not content:
+            raise TypeError('Invalid m3u8 content')
+
+        # 查看是否是本地文件
+        file = normpath(os.path.join(self.store, content))
+        if not self._is_m3u8(content) and os.path.isfile(file):
+            _content = b''
+
+            for index, chunk in enumerate(read_file_by_generator(file, 'rb')):
+                # 检查是否是m3u8内容
+                if index == 0 and not self._is_m3u8(chunk):
+                    break
+                _content += chunk
+            content = _content.decode(
+                chardet(_content).encoding or 'utf-8'
+            )
+
         # 解析m3u8
-        return self.start_parse(content=content, url=url)
+        self.start_parse(content, url)
 
-    def load_content(
+    def load_url(
         self,
-        content: str,
-        url: Optional[str] = None,
-        *,
+        url: str,
         output: Optional[str] = None,
-        reload: bool = False,
-        reserve: bool = False,
-        headers: Optional[dict] = None,
-        verify: bool = True,
-        limit: int = 16,
+        verify: Optional[bool] = None,
+        headers: Union[dict, CIMultiDict, None] = None,
         user_agent: Optional[str] = None,
+        reload: Optional[bool] = None,
+        reserve: Optional[bool] = None,
+        limit: Optional[int] = None
     ):
-        """使用m3u8文件下载资源
+        """load m3u8 url
 
-        :param content: m3u8内容 或 m3u8本地文件路径
         :param url: m3u8 url
-        :param output: m3u8资源输出到文件
-        :param reload: 重新从网络加载m3u8文件
-        :param reserve: 下载完成后保留m3u8文件
-        :param headers: request 请求头
-        :param verify: request verify
-        :param limit: 异步下载并发量
-        :param user_agent: User-Agent
+        :param output: 文件输出路径
+        :param verify: verify ssl
+        :param headers: Headers
+        :param user_agent: User agent
+        :param reload: 重载m3u8文件
+        :param reserve: 下载完成保留m3u8文件
+        :param limit: 异步下载limit
         """
-        self.output, self._limit = output, limit if isinstance(limit, int) and limit > 0 else 16
-        self._reload, self._reserve = bool(reload), bool(reserve)
-        self._headers, self._verify = headers, bool(verify)
-        self._user_agent = user_agent if user_agent and isinstance(user_agent, str) else None
-        self._session = _requests.Session(user_agent=self._user_agent)
-        # 关闭requests警告
-        if self._verify is False:
-            import urllib3
-            urllib3.disable_warnings()
-        # 无效m3u8内容
-        if not self._is_m3u8_content(content):
-            m3u8file = os.path.normpath(os.path.abspath(content)) if isinstance(content, str) else None
-            if m3u8file and os.path.isfile(m3u8file):
-                with open(m3u8file, "r", encoding="utf-8") as read_fileobj:
-                    content = read_fileobj.read()
-                    if not self._is_m3u8_content(content):
-                        self._console.print("[red b]m3u8 content is not available![/]")
-                        return None
-            else:
-                self._console.print("[red b]m3u8 content is not available![/]")
-                return None
+        # 文件路径
+        self.output = output
+
+        # 初始化数据
+        self._initialization(
+            verify=verify,
+            headers=headers,
+            user_agent=user_agent,
+            reload=reload,
+            reserve=reserve,
+            limit=limit
+        )
+        content = self.get_m3u8_content(url)
+
+        # 无效m3u8数据
+        if not content:
+            self.console.print(
+                f'[red b]Invalid m3u8 url[/]: <{url}>'
+            )
+            return
+
         # 解析m3u8
-        return self.start_parse(content=content, url=url)
+        self.start_parse(content=content, url=url)
 
-    def start_parse(self, content: str, url: Optional[str]):
-        """开始解析m3u8内容
+    def start_parse(self, content: str, url: Optional[str] = None):
+        """开始解析m3u8数据
 
-        :param content: m3u8 内容
-        :param url: m3u8 链接
+        :param content: m3u8内容
+        :param url: m3u8 url
         """
-        m3u8parse = M3U8Parse.run(content=content, url=url, instance=self)
-        # 可视化内容
-        table = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD, padding=0)
-        table.add_column(justify="left", overflow="fold")
-        # table1 = _rich_table.Table(show_header=False, box=_rich_box.SIMPLE_HEAD, padding=0)
-        # table1.add_column(justify="left", overflow="ellipsis")
-        # table1.add_row(f"[yellow b]url[/]: [blue u]{url}[/]")
-        table.add_row(f"[yellow b]url[/]: [blue u]{url}[/]")
+        m3u8obj = m3u8.loads(content=content, uri=url)
+        m3u8obj, new_url = self._parse_playlists(m3u8obj, url)
+        m3u8keys = self._parse_m3u8keys(m3u8obj)
+        segments, durations = self._parse_segments(m3u8obj, new_url)
+
+        # 无效m3u8数据
+        if not segments:
+            self.console.print(f'[red b]Invalid m3u8 content[/], url: {url}')
+            return
+
+        # 可视化解析结果
+        table = _table.Table(show_header=False, box=_box.SIMPLE_HEAD)
+
+        table.add_column(overflow='fold')
+        table.add_row(f'[blue u]{url}[/]')
         table.add_section()
-        table.add_row(f"[yellow b]maximum[/]: {m3u8parse['maximum']}")
-        table.add_row(f"[yellow b]duration[/]: {human_playtime(m3u8parse['duration'])}")
-        table.add_row(f"[yellow b]encryption[/]: {bool(m3u8parse['m3u8keys'])}")
-        table.add_row(f"[yellow b]output[/]: [blue]{self.output}[/]")
-        # 添加进度条
-        progress, download = None, None
-        if m3u8parse["segments"] and self.output and self._temp_file:
-            progress = progress_column(add_task=False)
-            download = download_column(add_task=False, show_transfer_speed=False)
-            table.add_section()
-            table.add_row(progress)
-            table.add_row(download)
-        panel = _rich_panel.Panel(
+
+        m3u8_info = [
+            f'[yellow b]maximum[/]: {len(segments)}',
+            f'[yellow b]durations[/]: {human_playtime(durations)}',
+            f'[yellow b]output[/]: {self.output}'
+        ]
+        for row in m3u8_info:
+            table.add_row(row)
+
+        panel = _panel.Panel(
             table,
-            subtitle=f"[dim i]limit: {self._limit}[/]",
-            subtitle_align="right",
-            border_style="bright_blue",
-            title="[red]M3U8 Download[/]",
-            title_align="center",
+            box=_box.ASCII2,
+            border_style='bright_blue',
+            title='[red]M3U8 Downloader[/]',
+            title_align='center',
+            subtitle=f'[dim i]limit: {self.limit}[/]',
+            subtitle_align='right',
+            expand=False,
         )
-        # 下载 segments
-        live = _rich_live.Live(panel, console=self._console)
-        with live:
+
+        # 没有 output 展示解析结果即可
+        if not self.output:
+            self.console.print(panel)
+            return
+
+        # 创建segments文件夹
+        os.makedirs(self._temp_segments, exist_ok=True)
+
+        # 开启下载
+        with _live.Live(panel, console=self.console):
             Downloader.run(
-                m3obj=self,
-                m3u8keys=m3u8parse["m3u8keys"],
-                segments=m3u8parse["segments"],
-                progress=progress,
-                download=download
+                start_urls=segments[:3:],
+                m3u8keys=m3u8keys,
+                semaphore=self.limit,
+                headers=self.headers,
+                user_agent=self.user_agent,
+                verify=self._verify,
+                output=self.output,
+                table=table,
+                console=self.console,
+                temp=self._temp_segments,
             )
-        # 删除m3u8文件
-        if not self._reserve and self._temp_file:
-            import shutil
-            if os.path.isdir(self._temp_file):
-                shutil.rmtree(self._temp_file)
-            
-    def get_m3u8_content(
-        self, url: Optional[str], *, is_m3u8key: bool = False
-    ) -> Optional[Union[str, bytes]]:
-        """获取m3u8内容
-
-        :param url: url
-        :param is_m3u8key: m3u8 key(type: bool)
-        :return: str, bytes
-        """
-        if not(url and isinstance(url, str)):
-            return None
-        # 文件完整路径
-        file = self._generate_filename(url, is_m3u8key)
-        mode, attr, encoding = "r", "text", "utf-8"
-        if is_m3u8key:
-            mode, attr, encoding = "rb", "content", None
-        # 获取网络资源
-        if self._reload or not file or not os.path.isfile(file):
-            response = self._session.get(url, headers=self._headers, verify=self._verify, timeout=10)
-            if response.status_code != 200:
-                self._console.print(f"[red]<Response [{response.status_code}] {url}>[/]")
-            content = getattr(response, attr)
-        # 获取本地资源
-        else:
-            with open(file, mode, encoding=encoding) as read_fileobj:
-                content = read_fileobj.read()
-        return content
 
-    def sava_m3u8_content(
-        self,
-        url: Optional[str],
-        content: Union[str, bytes],
-        *,
-        is_m3u8key: bool = False
-    ):
-        """保存m3u8内容
+        # 删除m3u8文件
+        if not os.path.isfile(self.output):
+            self._reserve = False
 
-        :param url: url
-        :param content: 保存内容
-        :param is_m3u8key: m3u8 key(type: bool)
-        """
-        # 文件完整路径
-        file = self._generate_filename(url, is_m3u8key)
-        mode, encoding = "w", "utf-8"
-        if is_m3u8key:
-            mode, encoding = "wb", None
-        # 保存文件到本地
-        if file and (self._reload or not os.path.isfile(file)):
-            with make_open(file, mode, encoding=encoding) as write_fileobj:
-                write_fileobj.write(content)
-
-    def _generate_filename(
-            self, url: Optional[str], is_m3u8key: bool = False
-    ) -> Optional[str]:
-        """生成完整文件路径
-
-        :param url: url
-        :param is_m3u8key:  m3u8 key(type: bool)
-        :return: str
-        """
-        if not self._temp_file or not url or not isinstance(url, str):
-            return None
-        basename = hash256(url)["ciphertext"] + (".key" if is_m3u8key else ".m3u8")
-        return os.path.join(self._temp_file, basename)
-
-    @staticmethod
-    def _is_m3u8_content(content: Optional[str], /) -> bool:
-        """检查是否是m3u8内容
+        if self._reserve is True:
+            import shutil
+            shutil.rmtree(self.temp)
+        # 清空请求历史
+        self.history.clear()
+
+    def _parse_segments(self, m3u8obj, url):
+        """解析 m3u8 segments"""
+        # 无效的 m3u8 文件
+        if not m3u8obj.is_endlist:
+            return None, None
+
+        # all segments
+        segments, durations = [], 0
+
+        for index, segment in enumerate(m3u8obj.segments):
+            # segments 绝对路径
+            segment.uri = segment.absolute_uri
+
+            # segment key
+            key = segment.key.uri if segment.key else None
+
+            # 保存 segment
+            item = (
+                segment.uri,
+                {
+                    'file': normpath(
+                        os.path.join(self._temp_segments, str(index)+'.ts')
+                    ) if self.output else None,
+                    'key': key
+                }
+            )
+            segments.append(item)
+            # segment 时间累加
+            durations += segment.duration
+
+        # 保存 m3u8 文件
+        self.sava_m3u8_content(url, m3u8obj.dumps())
+        return segments, durations
+
+    def _parse_m3u8keys(self, m3u8obj):
+        """解析 m3u8 keys"""
+        keys = {}
+
+        for key in m3u8obj.keys:
+            # 无效key
+            if not key:
+                continue
+
+            key.uri = key.absolute_uri
+            # 获取 密钥 和 偏移量
+            secret = self.get_m3u8_content(key.uri, True)[:16]
+            iv = key.iv.removeprefix('0x')[:16].encode() if key.iv else secret
+            # 保存key
+            keys[key.uri] = {'key': secret, 'iv': iv}
+
+            # 保存密钥到本地
+            self.sava_m3u8_content(key.uri, secret, True)
+
+        return keys
+
+    def _parse_playlists(self, m3u8obj, url=None):
+        """解析 m3u8 playlists"""
+
+        # 没有 playlists
+        if not m3u8obj.is_variant:
+            return m3u8obj, url
+
+        def sorted_playlists(playlist):
+            """对 playlists 进行排序"""
+            playlist.uri = playlist.absolute_uri
+            return playlist.stream_info.bandwidth
+
+        # 对 playlists 进行排序
+        playlists = sorted(m3u8obj.playlists, key=sorted_playlists)
+
+        # 保存m3u8文件
+        self.sava_m3u8_content(url, m3u8obj.dumps())
+
+        # 获取带宽最大的 playlist
+        new_url = playlists[-1].uri
+        new_m3u8obj = m3u8.loads(self.get_m3u8_content(new_url), new_url)
 
-        :param content: 需要检查的数据
-        :return: bool
-        """
-        if not(content and isinstance(content, str)):
-            return False
-        return content.startswith("#EXTM3U")
-
-    @property
-    def limit(self):
-        """limit"""
-        return self._limit
-
-    @property
-    def user_agent(self):
-        """User_Agent"""
-        return self._user_agent
-
-    @property
-    def temp_file(self):
-        """temp_file"""
-        return self._temp_file
+        return self._parse_playlists(new_m3u8obj, new_url)
 
 
-def load_url(
-    url: str,
-    *,
+def load_content(
+    content: str,
+    url: Optional[str] = None,
     output: Optional[str] = None,
-    reload: bool = False,
-    reserve: bool = False,
-    headers: Optional[dict] = None,
-    verify: bool = True,
-    limit: int = 16,
+    verify: Optional[bool] = None,
+    headers: Union[dict, CIMultiDict, None] = None,
     user_agent: Optional[str] = None,
+    reload: Optional[bool] = None,
+    reserve: Optional[bool] = None,
+    limit: Optional[int] = None
 ):
-    """使用m3u8链接下载资源
+    """load m3u8 url
 
+    :param content: m3u8 content
     :param url: m3u8 url
-    :param output: m3u8资源输出到文件
-    :param reload: 重新从网络加载m3u8文件
-    :param reserve: 下载完成后保留m3u8文件
-    :param headers: request 请求头
-    :param verify: request verify
-    :param limit: 异步下载并发量
-    :param user_agent: User-Agent
+    :param output: 文件输出路径
+    :param verify: verify ssl
+    :param headers: Headers
+    :param user_agent: User agent
+    :param reload: 重载m3u8文件
+    :param reserve: 下载完成保留m3u8文件
+    :param limit: 异步下载limit
     """
-    m3u8obj = M3U8()
-    return m3u8obj.load_url(
-        url,
+    m3u8parse = M3u8Parser()
+    m3u8parse.load_content(
+        content=content,
+        url=url,
         output=output,
+        verify=verify,
+        headers=headers,
+        user_agent=user_agent,
         reload=reload,
         reserve=reserve,
-        headers=headers,
-        verify=verify,
-        limit=limit,
-        user_agent=user_agent
+        limit=limit
     )
 
 
-def load_content(
-    content: str,
-    url: Optional[str] = None,
-    *,
+def load_url(
+    url: str,
     output: Optional[str] = None,
-    reload: bool = False,
-    reserve: bool = False,
-    headers: Optional[dict] = None,
-    verify: bool = True,
-    limit: int = 16,
+    verify: Optional[bool] = None,
+    headers: Union[dict, CIMultiDict, None] = None,
     user_agent: Optional[str] = None,
+    reload: Optional[bool] = None,
+    reserve: Optional[bool] = None,
+    limit: Optional[int] = None
 ):
-    """使用m3u8文件下载资源
+    """load m3u8 url
 
-    :param content: m3u8 content 或 m3u8本地文件路径
     :param url: m3u8 url
-    :param output: m3u8资源输出到文件
-    :param reload: 重新从网络加载m3u8文件
-    :param reserve: 下载完成后保留m3u8文件
-    :param headers: request 请求头
-    :param verify: request verify
-    :param limit: 异步下载并发量
-    :param user_agent: User-Agent
+    :param output: 文件输出路径
+    :param verify: verify ssl
+    :param headers: Headers
+    :param user_agent: User agent
+    :param reload: 重载m3u8文件
+    :param reserve: 下载完成保留m3u8文件
+    :param limit: 异步下载limit
     """
-    m3u8obj = M3U8()
-    return m3u8obj.load_content(
-        content,
-        url,
+    m3u8parse = M3u8Parser()
+    m3u8parse.load_url(
+        url=url,
         output=output,
+        verify=verify,
+        headers=headers,
+        user_agent=user_agent,
         reload=reload,
         reserve=reserve,
-        headers=headers,
-        verify=verify,
-        limit=limit,
-        user_agent=user_agent
+        limit=limit
     )
```

### Comparing `pyxk-0.6.4/pyxk/utils.py` & `pyxk-0.6.5/pyxk/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,542 +1,615 @@
+import io
+import logging
 from types import ModuleType
 from importlib import import_module
-from typing import Any, Union, Optional, Callable
+from collections import namedtuple
+from typing import IO, Any, Union, Optional
 
 
 __all__ = [
-    "LazyLoader",
-    "runtime",
-    "coro_runtime",
-    "make_open",
-    "get_user_agent",
-    "default_headers",
-    "md5",
-    "hash256",
-    "is_base64_from_regex",
-    "base64_conversion_bytes",
-    "rename_file",
-    "rename_folder",
-    "string_conversion_digits",
-    "human_playtime",
-    "pycode_conversion_lazyloader",
-    "pyfile_conversion_lazyloader",
-    "units_conversion_from_byte",
-    "download_column",
-    "progress_column",
-    "chardet"
+    'LazyLoader', 'runtime', 'runtime_coro', 'make_open',
+    'get_user_agent', 'default_headers', 'md5', 'hash256', 'normpath',
+    'is_base64_from_regex', 'base64_conversion_bytes', 'rename_file', 'rename_folder', 'rename',
+    'str_conversion_digit', 'human_playtime', 'pycode_conversion_lazy_loader', 'pyfile_conversion_lazy_loader',
+    'units_conversion_from_byte', 'download_progress', 'tasks_progress', 'chardet', 'read_file_by_generator'
 ]
 
 
 class LazyLoader(ModuleType):
     """模块延迟加载"""
 
-    def __init__(self, local_name, module_life_cycle, import_name=None):
-        """模块延迟加载
+    def __init__(
+        self,
+        local_name: str,
+        parent_module_globals: dict,
+        name: Optional[str] = None,
+        warning: Optional[str] = None
+    ):
+        """模块延迟加载 init
 
-        :param local_name: 模块引用名称
-        :param module_life_cycle: 模块生命周期(建议使用全局变量 globals)
-        :param import_name: 导入模块名称
+        :param local_name: 父模块引用名称
+        :param parent_module_globals: 父模块全局变量
+        :param name: 导入模块名称
+        :param warning: 警告信息
         """
         self._local_name = local_name
-        self._module_life_cycle = module_life_cycle
-        super().__init__(import_name or local_name)
-
-    def _loader(self):
+        self._parent_module_globals = parent_module_globals
+        self._warning = warning
+        super().__init__(name or local_name)
+
+    def _load(self):
+        """加载模块并将其插入父模块的全局变量中"""
+        # 导入模块
         module = import_module(self.__name__)
-        self._module_life_cycle[self._local_name] = module
+        self._parent_module_globals[self._local_name] = module
+
+        # 如果指定了警告，则发出警告
+        if self._warning:
+            logging.warning(self._warning)
+            # 确保只警告一次
+            self._warning = None
+
+        # 将模块的方法和变量注册到当前对象下
         self.__dict__.update(module.__dict__)
         return module
 
-    def __getattr__(self, name):
-        module = self._loader()
-        return getattr(module, name)
+    def __getattr__(self, item):
+        module = self._load()
+        return getattr(module, item)
 
     def __dir__(self):
-        module = self._loader()
+        module = self._load()
         return dir(module)
 
 
-# 计算函数运行时间
-def runtime(func: Callable):
+os = LazyLoader('os', globals(), 'os')
+re = LazyLoader('re', globals(), 're')
+time = LazyLoader('time', globals(), 'time')
+base64 = LazyLoader('base64', globals(), 'base64')
+hashlib = LazyLoader('hashlib', globals(), 'hashlib')
+difflib = LazyLoader('difflib', globals(), 'difflib')
+warnings = LazyLoader('warnings', globals(), 'warnings')
+functools = LazyLoader('functools', globals(), 'functools')
+itertools = LazyLoader('itertools', globals(), 'itertools')
+collections = LazyLoader('collections', globals(), 'collections')
+_console = LazyLoader('_console', globals(), 'rich.console')
+
+
+def runtime(func):
     """装饰器: 计算函数运行时间"""
-    import functools
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        import time
-        from rich import console as rich_console
-        console = rich_console.Console()
+        con = _console.Console()
         start_time = time.perf_counter()
         try:
             result = func(*args, **kwargs)
         finally:
             end_time = time.perf_counter()
-            console.print(f"{func.__name__!r} [magenta]running time[/]: {end_time - start_time}")
+            con.print(f'{func.__name__!r} [magenta]running time[/]: {end_time - start_time}')
         return result
+
     return wrapper
 
 
-# 计算异步函数运行时间
-def coro_runtime(func: Callable):
+def runtime_coro(func):
     """装饰器: 计算异步函数运行时间"""
-    import functools
 
     @functools.wraps(func)
     async def wrapper(*args, **kwargs):
-        import time
-        from rich import console as rich_console
-        console = rich_console.Console()
+        con = _console.Console()
         start_time = time.perf_counter()
         try:
             result = await func(*args, **kwargs)
         finally:
             end_time = time.perf_counter()
-            console.print(f"{func.__name__!r} [magenta]coroutine running time[/]: {end_time - start_time}")
+            con.print(f'{func.__name__!r} [magenta]running time[/]: {end_time - start_time}')
         return result
+
     return wrapper
 
 
-# 内置方法 `open` 装饰器
 def _make_open(func):
     """内置方法open装饰器 - 文件模式 w/a 下，创建不存在的目录"""
-    import functools
 
     @functools.wraps(func)
-    def wrapper(file, mode="r", buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None):
+    def wrapper(
+        file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None
+    ) -> IO:
         if not isinstance(mode, str):
             raise TypeError(f"{func.__name__}() argument 'mode' must be str, not {type(mode).__name__!r}")
-        import os
-        import warnings
-        import itertools
-        import collections
-        # collections.Counter 统计可迭代对象 每项出现的次数
-        # itertools.product 求多个可迭代对象的笛卡尔积
-        mode_list = [collections.Counter(i+j) for i, j in itertools.product("wa", ("b", "b+", "", "+"))]
+
+        # collections.Counter 统计可迭代对象 每项出现的次数 & itertools.product 求多个可迭代对象的笛卡尔积
+        mode_list = [collections.Counter(i + j) for i, j in itertools.product('wa', ('b', 'b+', '', '+'))]
         if collections.Counter(mode) in mode_list:
             os.makedirs(os.path.dirname(file), exist_ok=True)
+
         # 二进制模式下 encoding=None
-        if mode.find("b") != -1 and encoding is not None:
-            warnings.warn(
-                "binary mode doesn't take an encoding argument",
-                DeprecationWarning,
-                stacklevel=4
-            )
+        if mode.find('b') != -1 and encoding is not None:
+            logging.warning("binary mode doesn't take an encoding argument")
             encoding = None
+
         return func(file, mode, buffering, encoding, errors, newline, closefd, opener)
     return wrapper
 
 
-make_open = _make_open(open)
+make_open = _make_open(io.open)
 
 
-# User Agent
-def get_user_agent(ua: Optional[str] = None, overwrite: bool = False) -> Union[str, Any]:
+def get_user_agent(ua: Optional[str] = 'android', overwrite: bool = False) -> Union[str, Any]:
     """获取 UserAgent，默认 Android
 
     :param ua: 模糊查找内置字典User-Agent (android, windows, mac, iphone, ipad, symbian, apad)
     :param overwrite: 若为True, 直接返回  User-Agent
-    :return: "User-Agent"
+    :return: str
     """
     # 重写 UserAgent
     if overwrite:
-        return ua
+        return str(ua)
+
     # UserAgent 全部字典
     user_agent_dict = {
-        "android": "Mozilla/5.0 (Linux; Android 11; Pixel 5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.91 Mobile Safari/537.36",
-        "windows": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36",
-        "mac": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.198 Safari/537.36",
-        "iphone": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1",
-        "ipad": "Mozilla/5.0 (iPad; CPU OS 13_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) CriOS/87.0.4280.77 Mobile/15E148 Safari/604.1",
-        "symbian": "Mozilla/5.0 (Symbian/3; Series60/5.2 NokiaN8-00/012.002; Profile/MIDP-2.1 Configuration/CLDC-1.1 ) AppleWebKit/533.4 (KHTML, like Gecko) NokiaBrowser/7.3.0 Mobile Safari/533.4 3gpp-gba",
-        "apad": "Mozilla/5.0 (Linux; Android 11; Phh-Treble vanilla Build/RQ3A.211001.001;) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/90.0.4430.91 Safari/537.36",
+        'android': 'Mozilla/5.0 (Linux; Android 11; Pixel 5) AppleWebKit/537.36 (KHTML, like Gecko) '
+                   'Chrome/90.0.4430.91 Mobile Safari/537.36',
+        'windows': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
+                   'Chrome/86.0.4240.198 Safari/537.36',
+        'mac': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) '
+               'Chrome/86.0.4240.198 Safari/537.36',
+        'iphone': 'Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) '
+                  'AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1',
+        'ipad': 'Mozilla/5.0 (iPad; CPU OS 13_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) '
+                'CriOS/87.0.4280.77 Mobile/15E148 Safari/604.1',
+        'symbian': 'Mozilla/5.0 (Symbian/3; Series60/5.2 NokiaN8-00/012.002; Profile/MIDP-2.1 Configuration/CLDC-1.1 ) '
+                   'AppleWebKit/533.4 (KHTML, like Gecko) NokiaBrowser/7.3.0 Mobile Safari/533.4 3gpp-gba',
+        'apad': 'Mozilla/5.0 (Linux; Android 11; Phh-Treble vanilla Build/RQ3A.211001.001;) '
+                'AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/90.0.4430.91 Safari/537.36',
     }
-    # 默认UserAgent
-    if not ua or not isinstance(ua, str):
-        return user_agent_dict["android"]
-    # 模糊查找UserAgent
-    import difflib
+
+    if not isinstance(ua, str):
+        return user_agent_dict['android']
+
+    # 模糊查找 UserAgent
     ua = difflib.get_close_matches(ua.lower(), user_agent_dict.keys(), 1)
     if not ua:
-        return user_agent_dict["android"]
+        return user_agent_dict['android']
     return user_agent_dict[ua[0]]
 
 
-# Headers
-def default_headers(ua: Optional[str] = None):
+def default_headers(ua: Optional[str] = 'android'):
     """Headers
 
     :param ua: user-agent
-    :return: {"User-Agent": str}
+    :return: dict -> {'User-Agent': str}
     """
-    return {"User-Agent": get_user_agent(ua)}
+    return {'User-Agent': get_user_agent(ua)}
 
 
-# md5 加密
-def md5(plaintext: Union[str, bytes], encoding: Optional[str] = None):
+def md5(plaintext: Union[str, bytes], encoding: str = 'utf-8', default: Any = None):
     """MD5加密
 
     :param plaintext: 需加密明文
     :param encoding: plaintext编码
-    :return: {"plaintext": str, "ciphertext": str}
+    :param default: ciphertext默认值
+    :return: tuple -> (plaintext: 'plaintext', ciphertext: 'ciphertext')
     """
-    result = {"plaintext": None, "ciphertext": None}
-    if isinstance(plaintext, str):
-        plaintext = plaintext.encode(encoding=encoding or "utf-8")
-    elif not isinstance(plaintext, bytes):
-        result["plaintext"] = plaintext
+
+    _tuple = namedtuple('MD5NameTuple', 'ciphertext,plaintext')
+    result = _tuple(default, plaintext)
+
+    if not isinstance(plaintext, (str, bytes)):
         return result
+
+    # plaintext type str
+    if isinstance(plaintext, str):
+        plaintext = plaintext.encode(encoding=encoding)
+
     # md5加密
-    import hashlib
-    ciphertext = hashlib.md5(plaintext).hexdigest()
-    result["plaintext"], result["ciphertext"] = plaintext, ciphertext
+    result = result._replace(
+        ciphertext=hashlib.md5(plaintext).hexdigest()
+    )
     return result
 
 
-# hash256
-def hash256(plaintext: Union[str, bytes], encoding: Optional[str] = None):
+def hash256(plaintext: Union[str, bytes], encoding: str = 'utf-8', default: Any = None):
     """HASH_256加密
 
     :param plaintext: 需加密明文
     :param encoding: plaintext编码
-    :return: {"plaintext": str, "ciphertext": str}
+    :param default: ciphertext默认值
+    :return: tuple -> (plaintext: 'plaintext', ciphertext: 'ciphertext')
     """
-    result = {"plaintext": None, "ciphertext": None}
-    if isinstance(plaintext, str):
-        plaintext = plaintext.encode(encoding=encoding or "utf-8")
-    elif not isinstance(plaintext, bytes):
-        result["plaintext"] = plaintext
+    _tuple = namedtuple('Hash256NameTuple', 'ciphertext,plaintext')
+    result = _tuple(default, plaintext)
+
+    if not isinstance(plaintext, (str, bytes)):
         return result
+
+    # plaintext type str
+    if isinstance(plaintext, str):
+        plaintext = plaintext.encode(encoding=encoding)
+
     # hash256加密
-    import hashlib
-    ciphertext = hashlib.sha256(plaintext).hexdigest()
-    result["plaintext"], result["ciphertext"] = plaintext, ciphertext
+    result = result._replace(
+        ciphertext=hashlib.sha256(plaintext).hexdigest()
+    )
     return result
 
 
-# 判断base64数据类型
 def is_base64_from_regex(data: Union[str, bytes]) -> bool:
     """判断是否为base64数据类型
 
     :param data: 需检测的数据
     :return: bool
     """
-    import re
+    # base64 数据类型 正则表达式判断
     if isinstance(data, bytes):
-        # base64 数据类型 正则表达式判断
-        pattern_from_bytes = re.compile(rb"^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$")
+        pattern_from_bytes = re.compile(rb'^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$')
         return bool(pattern_from_bytes.match(data))
 
+    # base64 数据类型 正则表达式判断
     if isinstance(data, str):
-        # base64 数据类型 正则表达式判断
-        pattern_from_string = re.compile(r"^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$")
+        pattern_from_string = re.compile(r'^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$')
         return bool(pattern_from_string.match(data))
     # str 或 bytes 以外类型返回 False
     return False
 
 
-# base64数据类型 转化为bytes
-def base64_conversion_bytes(data: Union[str, bytes], encoding: str = "utf-8"):
+def base64_conversion_bytes(data: Union[str, bytes], encoding: str = 'utf-8', default: Any = None):
     """base64数据类型 转化为bytes
 
-    :param data: data: 需要 base64 解密的数据
-    :param encoding: encoding: type(data) is 'str' 通过 encoding 转换为 bytes
-    :return: Tuple(bool, data)
+    :param data: data: data
+    :param encoding: data数据编码
+    :param default: 返回默认值
+    :return: tuple -> (result: 'result', is_base64: 'is_base64')
     """
+    _tuple = namedtuple('Base64NameTuple', 'result,is_base64')
+    result = _tuple(default, False)
+
     if (
         not isinstance(data, (str, bytes))
         or not is_base64_from_regex(data)
     ):
-        return False, data
+        return result
+
     if isinstance(data, str):
         data = data.encode(encoding)
-    import base64
-    return True, base64.b64decode(data)
 
 
-# 重命名本地存在的文件
-def rename_file(file: str, suffix: Optional[str] = None):
+    result = result._replace(
+        result=base64.b64decode(data),
+        is_base64=True
+    )
+
+    return result
+
+
+def normpath(_path) -> str:
+    """规范文件路径"""
+    if not isinstance(_path, str):
+        raise TypeError(f'_path must be a str, got {type(_path).__name__!r}')
+
+    return os.path.normpath(_path.strip()).replace('\\', '/')
+
+
+def rename_file(file: str, suffix: Optional[str] = None, create: bool = False):
     """重命名本地存在的文件
 
     :param file: 文件路径
     :param suffix: 文件后缀名
-    :return: Tuple(rename_file, dir_name, basename)
+    :param create: 创建文件
+    :return: tuple -> (result, dirname, basename)
     """
-    import os
-    import itertools
-    # 绝对路径
-    file = os.path.normpath(os.path.abspath(file))
-    # 后缀名解析
-    if not isinstance(suffix, str) or not suffix:
-        file_split, suffix = file.rsplit(".", 1), ""
-        if len(file_split) == 2 and len(file_split[-1]) < 6:
-            suffix = file_split[-1]
-    suffix = "." + suffix.strip().removeprefix(".") if suffix.strip() else suffix.strip()
-    # 完整文件路径
+    # file 绝对路径
+    file = normpath(os.path.abspath(file))
+    if not os.path.basename(file):
+        raise ValueError('file missing basename')
+
+    # file 后缀名
+    if suffix and isinstance(suffix, str):
+        suffix = '.' + suffix.removeprefix('.')
+    else:
+        basename = os.path.basename(file).rsplit('.', 1)
+        if len(basename) == 2 and 2 <= len(basename[1]) <= 8:
+            suffix = '.' + basename[1].removeprefix('.')
+        else:
+            suffix = ''
+
+    # 拼接完整file
     if not file.endswith(suffix):
         file += suffix
 
+    # 重命名文件
+    def _rename(f):
+        """rename a file"""
+        _tuple = namedtuple('RenameFileNameTuple', 'result,dirname,basename')
+
+        if create:
+            from pathlib import Path
+            Path(f).touch()
+        return _tuple(f, *os.path.split(f))
+
     if not os.path.isfile(file):
-        return file, *os.path.split(file)
-    newfile = None
+        return _rename(file)
+
     for index in itertools.count(1):
-        newfile = file.removesuffix(suffix) + f".{index}" + suffix
+        newfile = file.removesuffix(suffix) + f'.{index}{suffix}'
         if not os.path.isfile(newfile):
-            break
-    return newfile, *os.path.split(newfile)
+            return _rename(newfile)
 
 
-# 重命名本地存在的文件夹
-def rename_folder(folder: str):
+rename = rename_file
+
+
+def rename_folder(folder: str, create: bool = False):
     """重命名本地存在的文件夹
 
     :param folder: 文件夹路径
-    :return: Tuple(rename_folder, dir_name, basename)
+    :param create: 创建文件夹
+    :return: Tuple(result, dirname, basename)
     """
-    import os
-    import itertools
-    folder = os.path.abspath(folder)
+    # 获取folder绝对路径
+    folder = normpath(os.path.abspath(folder))
+
+    def get_folder(f):
+        """获取重命名文件数据"""
+        _tuple = namedtuple('RenameFolderNameTuple', 'result,dirname,basename')
+
+        if create:
+            os.makedirs(f, exist_ok=True)
+        return _tuple(f, *os.path.split(f))
+
     if not os.path.isdir(folder):
-        return folder, *os.path.split(folder)
-    new_folder = None
+        return get_folder(folder)
+
+    # 重命名folder
     for index in itertools.count(1):
         new_folder = folder + f".{index}"
         if not os.path.isdir(new_folder):
-            break
-    return new_folder, *os.path.split(new_folder)
+            return get_folder(new_folder)
 
 
-# 字符串转换为数字
-def string_conversion_digits(target: Union[str, int, float], default: Any = None):
+def str_conversion_digit(target: Union[str, int, float], default: Any = None):
     """字符串转换为数字
 
     :param target: 需要转换的目标
     :param default: 返回默认值
-    :return: {"is_digits": bool, "original": Any, "converted": digits}
+    :return: tuple -> (result: digits, raw, is_digit: bool)
     """
-    result = {"is_digits": False, "original": target, "converted": default}
+    _tuple = namedtuple('StrConversionDigitNameTuple', 'result,raw,is_digit')
+    result = _tuple(default, target, False)
+
     # target type = `int` or `float`
     if isinstance(target, (int, float)):
-        result["is_digits"], result["converted"] = True, target
-        return result
+        return result._replace(
+            is_digit=True, result=target
+        )
+
     # target type != `str`
     if not isinstance(target, str):
         return result
 
     # 判断字符串是否为数字
     def is_digits(string):
-        import re
-        pattern = re.compile(r"^(?P<symbol>-)?(?P<int>\d+)(?P<float>\.\d+)?$")
-        ret = pattern.match(string)
-        if not ret:
-            return {"is_digits": False, "type": None}
-        ret = ret.groupdict()
-        return {"is_digits": True, "type": float if ret["float"] is not None else int}
+        pattern = re.match(r"^(?P<symbol>-)?(?P<int>\d+)(?P<float>\.\d+)?$", string)
+        if not pattern:
+            return {"is_digits": False, "type": lambda x: x}
+        return {"is_digits": True, "type": float if pattern.groupdict()["float"] is not None else int}
+
     # 转换为数字
-    ret = is_digits(target)
-    if ret["is_digits"]:
-        result["is_digits"], result["converted"] = True, ret["type"](target)
+    _result = is_digits(target)
+    if _result["is_digits"]:
+        result = result._replace(
+            is_digit=True, result=_result["type"](target)
+        )
     return result
 
 
-# 人类直观时间展示
-def human_playtime(playtime: Union[str, int, float]):
+def human_playtime(playtime: Union[str, int, float], default: Any = None):
     """人类直观时间展示
 
     :param playtime: 传入一个时间(秒), 返回人类能理解的时间格式
+    :param default: 返回默认值
     :return: str
     """
-    digits = string_conversion_digits(playtime)
-    if not digits["is_digits"]:
-        return None
-    playtime = digits["converted"]
+    digit = str_conversion_digit(playtime)
+
+    if not digit.is_digit:
+        return default
+
+    playtime = digit.result
     symbol, playtime = "-" if playtime < 0 else "", round(abs(playtime))
+
     hour, second = divmod(playtime, 3600)
     minute, second = divmod(second, 60)
+
     return f"{symbol}{hour}:{minute:0>2}:{second:0>2}"
 
 
-# python模块转换懒加载
-def pycode_conversion_lazyloader(string: str):
+def pycode_conversion_lazy_loader(string: str):
     """python代码中的导入模块转换为懒加载
 
     :param string: python代码
     :return: str
     """
-    import re
-    pattern = re.compile(
-        r"^from\s+?(?P<from_name>\S+)\s+?import\s+?(?P<from_import_name>\S+)\s*?(as\s+?(?P<from_import_alias>\S+))?$|^import\s+?(?P<import_name>\S+)(\s+?as\s+(?P<import_alias>\S+?))?\s*?$",
-        flags=re.M
-    )
-
     def repl_string(match):
-        match_dict = match.groupdict()
-        import_name, alias = None, None
-        result = '{alias} = LazyLoader("{alias}", globals(), "{import_name}")'
+        """替换懒加载"""
+        match_dict, import_name, alias = match.groupdict(), None, None
+        repl = '{alias} = LazyLoader("{alias}", globals(), "{import_name}")'
+
         # from导入
         if match_dict["from_name"]:
             import_name = f'{match_dict["from_name"]}.{match_dict["from_import_name"]}'
             alias = match_dict["from_import_name"]
         else:
             import_name = f'{match_dict["import_name"]}'
             alias = match_dict["import_name"]
+
         # alias
         if match_dict["from_import_alias"]:
             alias = match_dict["from_import_alias"]
         elif match_dict["import_alias"]:
             alias = match_dict["import_alias"]
-        return result.format(alias=alias, import_name=import_name)
+        return repl.format(alias=alias, import_name=import_name)
 
     # 替换懒加载
-    string = pattern.sub(repl=repl_string, string=string)
-    return string
+    pattern = [
+        r'^from\s+?(?P<from_name>\S+)\s+?import\s+?(?P<from_import_name>\S+)'
+        r'\s*?(as\s+?(?P<from_import_alias>\S+))?$',
+        r'^import\s+?(?P<import_name>\S+)(\s+?as\s+(?P<import_alias>\S+?))?\s*?$',
+    ]
+    return re.sub(pattern='|'.join(pattern), repl=repl_string, string=string, flags=re.M)
 
 
-# python模块转换懒加载 从文件
-def pyfile_conversion_lazyloader(read_file: str, write_file: str, encoding: Optional[str] = None):
+def pyfile_conversion_lazy_loader(read_file: str, write_file: str, encoding: Optional[str] = None):
     """python文件中的导入模块转换为懒加载
 
     :param read_file: 读取python代码文件
     :param write_file: 写入转换后的python代码文件
     :param encoding: 文件编码
     """
-    with open(read_file, "r", encoding=encoding) as read_fileobj:
-        content = pycode_conversion_lazyloader(read_fileobj.read())
-    with open(write_file, "w", encoding=encoding) as write_fileobj:
-        write_fileobj.write(content)
+    with open(read_file, "r", encoding=encoding) as read_file_obj:
+        content = pycode_conversion_lazy_loader(read_file_obj.read())
+    with open(write_file, "w", encoding=encoding) as write_file_obj:
+        write_file_obj.write(content)
 
 
-# 字节单位自动换算
-def units_conversion_from_byte(target: Union[int, float]):
+def units_conversion_from_byte(target: Union[str, int, float], default: Any = None):
     """字节单位自动换算
 
     :param target: 换算目标(Bytes)
-    :return: str
+    :param default: 返回默认值
+    :return: tuple -> (result, raw, units)
     """
-    target = string_conversion_digits(target)
-    if not target["is_digits"]:
-        return None
-    target, target_units = abs(target["converted"]), "Bytes"
-    units_dict = {"Bytes": 1, "KB": 1024, "MB": 1024, "GB": 1024, "TB": 1024, "PB": 1024, "EB": 1024, "ZB": 1024, "YB": 1024, "BB": 1024}
+    _tuple = namedtuple('UnitsConversionNameTuple', 'result,raw,units')
+    result = _tuple(default, target, None)
+    _temp = str_conversion_digit(target)
+
+    if not _temp.is_digit:
+        return result
+
+    target = abs(_temp.result)
+    target_units = 'Bytes'
+    del _temp
+
+    units_dict = {
+        'Bytes': 1, 'KB': 1024, 'MB': 1024,
+        'GB': 1024, 'TB': 1024, 'PB': 1024,
+        'EB': 1024, 'ZB': 1024, 'YB': 1024, 'BB': 1024
+    }
+
     for units, rate in units_dict.items():
         if target >= rate:
             target, target_units = target/rate, units
             continue
         break
-    return f"{round(target, 2)}{target_units}"
 
+    result = result._replace(
+        units=target_units,
+        result= f'{round(target, 2)}{target_units}'
+
+    )
+    return result
+
+
+def chardet(byte_str: bytes, **kwargs):
+    """字符编码判断
+
+    :param byte_str: bytes数据
+    :param kwargs: kwargs
+    :return: tuple -> (encoding: str, language: str, confidence: float)
+    """
+    try:
+        import chardet as _chardet
+    except ImportError:
+        import charset_normalizer as _chardet
+
+    _tuple = namedtuple('ChardetNameTuple', 'encoding,language,confidence')
+    result = _chardet.detect(byte_str=byte_str, **kwargs)
+
+    return _tuple(
+        encoding=result.get('encoding'),
+        language=result.get('language'),
+        confidence=result.get('confidence')
+    )
 
-# 下载进度条
-def download_column(
+
+
+def download_progress(
     *,
-    start: bool = True,
-    total: Optional[float] = None,
-    console: Optional[object] = None,
-    add_task: bool = False,
-    progress: Optional[object] = None,
-    completed: Optional[float] = None,
     transient: bool = False,
-    description: Optional[str] = None,
-    show_transfer_speed: bool = True,
+    console: object = None,
+    text_column: Optional[str] = '[progress.description]{task.description}',
+    task_progress_column: Optional[str] = '[progress.percentage]{task.percentage:>6.2f}%',
+    show_transfer_speed: bool = True
 ):
-    """rich.progress - 下载进度条
+    """rich.progress.Progress - 下载进度条
 
-    :param start: 立即启动任务，如果为 False 则需要手动启动
-    :param total: 进度总步数
-    :param console: rich.console.Console
-    :param add_task: 是否添加进度任务 默认False
-    :param progress: rich.progress.Progress类 默认自动创建
-    :param completed: task 已完成步数 默认为0
     :param transient: 转瞬即逝
-    :param description: 任务描述
-    :param show_transfer_speed: 显示任务速度
-    :return:
-        `add_task` is `True`  -> progress, task
-        `add_task` is `False` -> progress
-    """
-    import rich.progress as rich_progress
-    if not isinstance(progress, rich_progress.Progress):
-        column = [
-            rich_progress.TextColumn("[progress.description]{task.description}"),
-            rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
-            rich_progress.BarColumn(),
-            rich_progress.DownloadColumn(),
-            rich_progress.TimeElapsedColumn(),
-        ]
-        if show_transfer_speed:
-            column.insert(-1, rich_progress.TransferSpeedColumn())
-        progress = rich_progress.Progress(*column,transient=transient, console=console)
-    # 添加任务
-    if add_task or total is not None:
-        task = progress.add_task(
-            total=total,
-            start=start,
-            description=description or "",
-            completed=completed or 0
-        )
-        return progress, task
-    return progress
+    :param console: rich.console.Console
+    :param text_column: text column 文本格式 [progress.description]{task.description}
+    :param task_progress_column: 任务进度格式 [progress.percentage]{task.percentage:>6.2f}%
+    :param show_transfer_speed: 显示任务下载速度
+    :return: rich.progress.Progress default: True
+    """
+    from rich import progress as _progress
+    columns = [
+        _progress.TextColumn(text_column),
+        _progress.TaskProgressColumn(task_progress_column),
+        _progress.BarColumn(),
+        _progress.DownloadColumn(),
+        _progress.TransferSpeedColumn(),
+        _progress.TimeElapsedColumn()
+    ]
+    # 不显示下载速度
+    if not show_transfer_speed:
+        columns.pop(-2)
+    return _progress.Progress(*columns, transient=transient, console=console)
 
 
-# 任务进度条
-def progress_column(
+def tasks_progress(
     *,
-    start: bool = True,
-    total: Optional[float] = None,
-    console: Optional[object] = None,
-    add_task: bool = False,
-    progress: Optional[object] = None,
-    completed: Optional[float] = None,
     transient: bool = False,
-    description: Optional[str] = None,
-    show_transfer_speed: bool = False,
+    console: object = None,
+    text_column: Optional[str] = '[progress.description]{task.description}',
+    task_progress_column: Optional[str] = '[progress.percentage]{task.percentage:>6.2f}%',
+    task_progress_column_2: Optional[str] = '[cyan]{task.completed}/{task.total}[/]',
+    show_transfer_speed: bool = False
 ):
-    """rich.progress - 任务进度条
+    """rich.progress.Progress - 任务进度条
 
-    :param start: 立即启动任务，如果为 False 则需要手动启动
-    :param total: 进度总步数
-    :param console: rich.console.Console
-    :param add_task: 是否添加进度任务 默认False
-    :param progress: rich.progress.Progress类 默认自动创建
-    :param completed: task 已完成步数 默认为0
     :param transient: 转瞬即逝
-    :param description: 任务描述
-    :param show_transfer_speed: 显示任务速度
+    :param console: rich.console.Console
+    :param text_column: text column 文本格式 [progress.description]{task.description}
+    :param task_progress_column: 任务进度格式 [progress.percentage]{task.percentage:>6.2f}%
+    :param task_progress_column_2: 任务进度格式 [cyan]{task.completed}/{task.total}[/]
+    :param show_transfer_speed: 显示任务下载速度 default: False
     :return:
-        `add_task` is `True`  -> progress, task
-        `add_task` is `False` -> progress
     """
-    import rich.progress as rich_progress
-    if not isinstance(progress, rich_progress.Progress):
-        column = [
-            rich_progress.TextColumn("[progress.description]{task.description}"),
-            rich_progress.TaskProgressColumn("[progress.percentage]{task.percentage:>6.2f}%"),
-            rich_progress.BarColumn(),
-            rich_progress.TaskProgressColumn("[cyan]{task.completed}/{task.total}[/]"),
-            rich_progress.TimeElapsedColumn(),
-        ]
-        if show_transfer_speed:
-            column.insert(-1, rich_progress.TransferSpeedColumn())
-        progress = rich_progress.Progress(*column,transient=transient, console=console)
-    # 添加任务
-    if add_task or total is not None:
-        task = progress.add_task(
-            total=total,
-            start=start,
-            description=description or "",
-            completed=completed or 0
-        )
-        return progress, task
-    return progress
-
-
-def chardet(byte: bytes):
-    """字符编码判断
-
-    :param byte: bytes数据
-    :return: {'encoding': str, 'language': str, 'confidence': float}
-    """
-    try:
-        import chardet as _chardet
-    except ImportError:
-        import charset_normalizer as _chardet
-    return _chardet.detect(byte)
+    from rich import progress as _progress
+    columns = [
+        _progress.TextColumn(text_column),
+        _progress.TaskProgressColumn(task_progress_column),
+        _progress.BarColumn(),
+        _progress.TaskProgressColumn(task_progress_column_2),
+        _progress.TimeElapsedColumn(),
+    ]
+    # 显示下载速度
+    if show_transfer_speed:
+        columns.insert(-1, _progress.TransferSpeedColumn())
+    return _progress.Progress(*columns, transient=transient, console=console)
+
+
+def read_file_by_generator(file: str, mode: str = 'r', *, chunk_size: int = 1024, **kwargs):
+    """基于生成器的文件读取
+
+    :param file: file path
+    :param mode: file open mode
+    :param chunk_size: chunk size
+    :param kwargs: open arguments
+    """
+    with open(file, mode, **kwargs) as read_file_obj:
+        while True:
+            chunk = read_file_obj.read(chunk_size)
+            if not chunk:
+                return
+            yield chunk
```

### Comparing `pyxk-0.6.4/pyxk.egg-info/PKG-INFO` & `pyxk-0.6.5/pyxk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.4
+Version: 0.6.5
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,22 +23,24 @@
 ```python
 from pprint import pprint
 from pyxk import Client, Response
 
 class Downloader(Client):
     start_urls = ['https://pypi.org' for _ in range(2)]
 
-    async def parse(self, response: Response):
+    async def parse(self, response: Response, **kwargs):
         title = await response.xpath('//title/text()')
         return title.get()
 
     async def completed(self, result: list):
         pprint(result)
 
-Downloader.run()
+
+if __name__ == '__main__':
+    Downloader.run()
 
 >> ['PyPI · The Python Package Index', 'PyPI · The Python Package Index']
 ```
 
 ### pyxk.m3u8
 ```python
 from pyxk.m3u8 import load_url, load_content
```

### Comparing `pyxk-0.6.4/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.5/pyxk.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 pyxk.egg-info/entry_points.txt
 pyxk.egg-info/requires.txt
 pyxk.egg-info/top_level.txt
 pyxk/aclient/__init__.py
 pyxk/aclient/client.py
 pyxk/aclient/typedef.py
 pyxk/aes/__init__.py
-pyxk/aes/_fmtdata.py
 pyxk/aes/cryptor.py
 pyxk/m3u8/__init__.py
-pyxk/m3u8/enter_point.py
-pyxk/m3u8/m3u8download.py
+pyxk/m3u8/_initial.py
+pyxk/m3u8/downloader.py
+pyxk/m3u8/entry_point.py
 pyxk/m3u8/m3u8parse.py
-pyxk/m3u8/main.py
 pyxk/requests/__init__.py
 pyxk/requests/api.py
 pyxk/requests/entry_point.py
 pyxk/requests/sessions.py
```

### Comparing `pyxk-0.6.4/setup.py` & `pyxk-0.6.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as read_file_obj:
     long_description = read_file_obj.read()
 
 setuptools.setup(
     name='pyxk',
-    version='0.6.4',
+    version='0.6.5',
     author='kai139',
     install_requires=[
         'requests', 'pycryptodome', 'rich', 'm3u8', 'aiohttp', 'aiofiles', 'click', 'parsel'
     ],
     entry_points={
         'console_scripts': [
             'm3u8 = pyxk.m3u8.enter_point:main',
```

