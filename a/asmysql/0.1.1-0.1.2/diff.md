# Comparing `tmp/asmysql-0.1.1.tar.gz` & `tmp/asmysql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmysql-0.1.1.tar", max compression
+gzip compressed data, was "asmysql-0.1.2.tar", max compression
```

## Comparing `asmysql-0.1.1.tar` & `asmysql-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      510 2023-07-25 16:29:04.218975 asmysql-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-07-25 16:29:04.218975 asmysql-0.1.1/LICENSE
--rw-r--r--   0        0        0     1628 2023-07-25 16:29:04.218975 asmysql-0.1.1/README.md
--rw-r--r--   0        0        0     1698 2023-07-25 16:29:04.218975 asmysql-0.1.1/README_zh.md
--rw-r--r--   0        0        0     1530 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/__cursor_client.py
--rw-r--r--   0        0        0       58 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/__init__.py
--rw-r--r--   0        0        0     3567 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/_asmysql.py
--rw-r--r--   0        0        0     1670 2023-07-25 16:29:04.218975 asmysql-0.1.1/asmysql/_result.py
--rw-r--r--   0        0        0     1182 2023-07-27 14:55:25.667736 asmysql-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 asmysql-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-07-25 16:29:04.218975 asmysql-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-07-25 16:29:04.218975 asmysql-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1628 2023-07-25 16:29:04.218975 asmysql-0.1.2/README.md
+-rw-r--r--   0        0        0     1698 2023-07-25 16:29:04.218975 asmysql-0.1.2/README_zh.md
+-rw-r--r--   0        0        0     1530 2023-07-25 16:29:04.218975 asmysql-0.1.2/asmysql/__cursor_client.py
+-rw-r--r--   0        0        0       58 2023-07-25 16:29:04.218975 asmysql-0.1.2/asmysql/__init__.py
+-rw-r--r--   0        0        0     3614 2023-07-27 15:53:51.899825 asmysql-0.1.2/asmysql/_asmysql.py
+-rw-r--r--   0        0        0     1685 2023-07-27 15:53:17.831824 asmysql-0.1.2/asmysql/_result.py
+-rw-r--r--   0        0        0     1182 2023-07-27 15:56:02.091828 asmysql-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 asmysql-0.1.2/PKG-INFO
```

### Comparing `asmysql-0.1.1/LICENSE` & `asmysql-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asmysql-0.1.1/README.md` & `asmysql-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `asmysql-0.1.1/README_zh.md` & `asmysql-0.1.2/README_zh.md`

 * *Files identical despite different names*

### Comparing `asmysql-0.1.1/asmysql/__cursor_client.py` & `asmysql-0.1.2/asmysql/__cursor_client.py`

 * *Files identical despite different names*

### Comparing `asmysql-0.1.1/asmysql/_asmysql.py` & `asmysql-0.1.2/asmysql/_asmysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import lru_cache
 from typing import Final, final, Optional
 from aiomysql import Pool, create_pool
 
 from .__cursor_client import CursorClient
 
 
 class AsMysql:
@@ -34,14 +35,15 @@
         self.pool_recycle: Final[float] = pool_recycle or self.pool_recycle
         self.connect_timeout: Final[int] = connect_timeout or self.connect_timeout
 
         self.url: Final[str] = f'mysql://{self.host}:{self.port}{"/" + self.database if self.database else ""}'
         self.__pool: Optional[Pool] = None
         self.__cursor_client: Optional[CursorClient] = None
 
+    @lru_cache
     def __repr__(self):
         return f'<{self.__class__.__name__} {self.url}>'
 
     @final
     async def connect(self):
         """连接到mysql,建立TCP链接，初始化连接池。"""
         if not self.__pool:
```

### Comparing `asmysql-0.1.1/asmysql/_result.py` & `asmysql-0.1.2/asmysql/_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
             self.query: Final[str] = query
             self.rows: Final[int] = rows
             self.__cursor: Final[Cursor] = cursor
             self.err: Final[Exception] = err
         else:
             raise AttributeError("require arg: cursor or err")
 
+    @lru_cache
     def __repr__(self):
         return f'<{self.__class__.__name__}: {self.query}>'
 
     @property
     @lru_cache
     def err_msg(self):
         if self.err:
```

### Comparing `asmysql-0.1.1/pyproject.toml` & `asmysql-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asmysql"
-version = "0.1.1"
+version = "0.1.2"
 description = "封装aiomysql的异步mysql客户端引擎。"
 license = "MIT"
 authors = ["vastxiao <vastxiao@gmail.com>"]
 homepage = "https://github.com/Vastxiao/asmysql"
 repository = "https://github.com/Vastxiao/asmysql"
 documentation = "https://github.com/Vastxiao/asmysql/blob/main/README.md"
 keywords = ["async", "asyncio", "mysql", "aiomysql"]
```

### Comparing `asmysql-0.1.1/PKG-INFO` & `asmysql-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmysql
-Version: 0.1.1
+Version: 0.1.2
 Summary: 封装aiomysql的异步mysql客户端引擎。
 Home-page: https://github.com/Vastxiao/asmysql
 License: MIT
 Keywords: async,asyncio,mysql,aiomysql
 Author: vastxiao
 Author-email: vastxiao@gmail.com
 Requires-Python: >=3.11,<4.0
```

