# Comparing `tmp/kerberos_auth_proxy-0.1.0a0.tar.gz` & `tmp/kerberos_auth_proxy-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerberos_auth_proxy-0.1.0a0.tar", max compression
+gzip compressed data, was "kerberos_auth_proxy-0.1.0a1.tar", max compression
```

## Comparing `kerberos_auth_proxy-0.1.0a0.tar` & `kerberos_auth_proxy-0.1.0a1.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     1075 2023-07-01 17:16:05.974247 kerberos_auth_proxy-0.1.0a0/LICENSE
--rw-r--r--   0        0        0       68 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a0/README.md
--rw-r--r--   0        0        0        0 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a0/kerberos_auth_proxy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 19:42:12.010594 kerberos_auth_proxy-0.1.0a0/kerberos_auth_proxy/mitm/__init__.py
--rw-r--r--   0        0        0     1499 2023-07-03 00:53:02.856536 kerberos_auth_proxy-0.1.0a0/kerberos_auth_proxy/mitm/addon.py
--rw-r--r--   0        0        0     6877 2023-07-02 23:05:18.310202 kerberos_auth_proxy-0.1.0a0/kerberos_auth_proxy/mitm/filters.py
--rw-r--r--   0        0        0      849 2023-07-01 23:45:21.397510 kerberos_auth_proxy-0.1.0a0/kerberos_auth_proxy/utils.py
--rw-r--r--   0        0        0      747 2023-07-03 01:00:57.642937 kerberos_auth_proxy-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 kerberos_auth_proxy-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-01 17:16:05.974247 kerberos_auth_proxy-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0       68 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a1/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 17:13:15.814927 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 19:42:12.010594 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/__init__.py
+-rw-r--r--   0        0        0     2963 2023-07-06 10:40:39.368152 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/addon.py
+-rw-r--r--   0        0        0     1520 2023-07-06 10:44:52.213364 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/auth.py
+-rw-r--r--   0        0        0        0 2023-07-03 22:09:06.654893 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-03 22:15:14.534627 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/base.py
+-rw-r--r--   0        0        0     3805 2023-07-05 16:18:00.380638 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/hosts.py
+-rw-r--r--   0        0        0     5807 2023-07-05 09:09:36.660046 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/kerberos.py
+-rw-r--r--   0        0        0     8478 2023-07-05 16:19:25.493892 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/hostutils.py
+-rw-r--r--   0        0        0     1385 2023-07-04 16:06:59.191830 kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/utils.py
+-rw-r--r--   0        0        0      747 2023-07-31 13:30:39.429283 kerberos_auth_proxy-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 kerberos_auth_proxy-0.1.0a1/PKG-INFO
```

### Comparing `kerberos_auth_proxy-0.1.0a0/LICENSE` & `kerberos_auth_proxy-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kerberos_auth_proxy-0.1.0a0/kerberos_auth_proxy/mitm/filters.py` & `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/mitm/filters/kerberos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,118 @@
 '''
-Module containing the built-in MITM filters
+Filters for handling Kerberos negotiations
 '''
 
 import logging
-from re import Pattern
-from typing import Annotated, Awaitable, Callable, List, Optional, Set
+from typing import List, Optional, Set
 from urllib.parse import ParseResult, urlparse
 
 import aiohttp
 import gssapi
-from multidict import CIMultiDict, MultiDict
 from requests_gssapi import HTTPSPNEGOAuth
 from requests_gssapi.exceptions import SPNEGOExchangeError
-from mitmproxy.http import Headers, HTTPFlow, Response
+from mitmproxy.http import HTTPFlow, Response
 
+from kerberos_auth_proxy.mitm.filters.base import Filter
+from kerberos_auth_proxy.mitm.hostutils import url_matches
 
-Filter = Annotated[
-    Callable[[HTTPFlow], Awaitable[Optional['Filter']]],
-    'A function that accepts a flow, processes it and optionally returns the next filter to apply'
-]
 logger = logging.getLogger(__name__)
 
 METADATA_KERBEROS_PRINCIPAL = 'kerberos_auth_proxy.principal'
 METADATA_KERBEROS_WRAPPED = 'kerberos_auth_proxy.wrapped-by-kerberos'
+METADATA_HOST_REMAPPED = 'kerberos_auth_proxy.host-remapped'
 
 
 def check_spnego(unauthorized_codes: Set[int], next_filter: Filter) -> Filter:
     '''
     Adds the next filter to retry the request to the same server if the response was
     a SPNEGO authentication denial.
 
     Args:
         redirect_codes: recognized HTTP codes for access denial (e.g.: 401, 407)
     '''
-    @debug_filter
     async def filter_check_spnego(flow: HTTPFlow) -> Optional[Filter]:
         www_authenticate = flow.response.headers.get(b'WWW-Authenticate') or ''
         if (
             flow.response.status_code in unauthorized_codes
             and (www_authenticate.startswith('Negotiate ') or www_authenticate == 'Negotiate')
         ):
             logger.info('SPNEGO access denial, will retry with Kerberos')
-            # flow.response = None
             return next_filter
 
     return filter_check_spnego
 
 
 def check_knox(
     redirect_codes: Set[int],
-    urls: List[ParseResult],
+    knox_urls: List[ParseResult],
     user_agent_override: Optional[str],
     next_filter: Filter,
 ) -> Filter:
     '''
     Adds the next filter to retry the request to the same server if the response was a redirect to KNOX.
 
     Args:
         redirect_codes: recognized HTTP codes for redirections (e.g., 301, 307...)
         urls: list of possible KNOX URLs. The retry will be done if the Location header starts with any of these
         user_agent_override: override the request header 'User-Agent' before retrying the request. This can help
             convince some apps we're not a browser so it shouldn't just redirect to KNOX again.
     '''
-    @debug_filter
     async def filter_check_knox(flow: HTTPFlow) -> Optional[Filter]:
         if flow.response.status_code not in redirect_codes:
-            logging.info('not KNOX, unknown redirect code %s', flow.response.status_code)
+            logger.debug('not KNOX, unknown redirect code %s', flow.response.status_code)
             return
 
         if flow.request.method != "GET":
-            logging.info('not KNOX, unknown method %s', flow.request.method)
+            logger.debug('not KNOX, unknown method %s', flow.request.method)
             return
 
-        location = flow.response.headers.get(b'Location') or ''
+        location_url = urlparse(flow.response.headers.get(b'Location') or '')
 
-        # let's play safe and let Python parse the URL instead of doing a simple .startswith()
-        parsed = urlparse(location)
-        for u in urls:
-            if u.hostname == parsed.hostname and u.port == parsed.port and parsed.path.startswith(u.path):
-                if user_agent_override:
-                    flow.request.headers[b'User-Agent'] = user_agent_override
-                    logger.info('KNOX redirect, will retry with Kerberos overriding the user agent')
-                else:
-                    logger.info('KNOX redirect, will retry with Kerberos')
-                # flow.response = None
-                return next_filter
+        for knox_url in knox_urls:
+            if not url_matches(knox_url, location_url):
+                continue
+
+            if user_agent_override:
+                flow.request.headers[b'User-Agent'] = user_agent_override
+                logger.info('KNOX redirect, will retry with Kerberos overriding the user agent')
+            else:
+                logger.info('KNOX redirect, will retry with Kerberos')
+
+            return next_filter
+        else:
+            logger.debug('not a recognized KNOX redirect')
 
     return filter_check_knox
 
 
 def do_with_kerberos(
     next_filter: Optional[Filter] = None,
-) -> None:
+) -> Filter:
     '''
     Sends the request with Kerberos authentication.
 
     This requires the flow.metadata[METADATA_KERBEROS_PRINCIPAL] to point to the principal full name
     (i.e., with the realm spec) and such principal to already be authenticated in the ticket cache
     '''
-    def _to_headers(headers: Headers) -> MultiDict:
-        return CIMultiDict()
-
-    @debug_filter
     async def filter_do_with_kerberos(flow: HTTPFlow) -> Optional[Filter]:
         principal = flow.metadata[METADATA_KERBEROS_PRINCIPAL]
         name = gssapi.Name(principal, gssapi.NameType.kerberos_principal)
         creds = gssapi.Credentials(name=name, usage="initiate")
 
         gssapi_auth = HTTPSPNEGOAuth(
             creds=creds,
             opportunistic_auth=True,
             target_name='HTTP',
         )
         try:
             negotiate = gssapi_auth.generate_request_header(None, flow.request.host, True)
             flow.request.headers[b'Authorization'] = negotiate
         except SPNEGOExchangeError:
-            logger.exception('error while generating header')
+            logger.exception('error while generating SPNEGO header')
             return None
 
         async with aiohttp.ClientSession() as session:
             kwargs = dict(
                 method=flow.request.method,
                 url=flow.request.url,
                 headers=flow.request.headers,
@@ -138,52 +130,29 @@
 
         flow.metadata[METADATA_KERBEROS_WRAPPED] = True
         return next_filter
 
     return filter_do_with_kerberos
 
 
-def match_hosts(host_regexps: List[Pattern], next_filter: Filter) -> Filter:
-    """
-    Applies the next filter if the hostname matches any of the given regexps
-
-    Args:
-        host_regexps: list of regexp patterns to match the host against (including the port)
-        next_filter: filter to apply if the host matches
-    """
-    async def filter_match_hosts(flow: HTTPFlow) -> Optional[Filter]:
-        for host_regexp in host_regexps:
-            if host_regexp.match(flow.request.host):
-                return next_filter
-
-    return filter_match_hosts
-
-
 def kerberos_flow(
     realm: str,
     spnego_filter: Filter,
     knox_filter: Filter,
-) -> None:
+) -> Filter:
     '''
     Sets the kerberos.metadata[METADATA_KERBEROS_PRINCIPAL] based on the authentication
     '''
-    @debug_filter
     async def filter_kerberos_flow(flow: HTTPFlow) -> Optional[Filter]:
-        username, *_ = list(flow.metadata.get('proxyauth') or []) + ['']
-        if not username:
+        proxy_auth = flow.metadata.get('proxyauth')
+        if not proxy_auth:
             logger.info('no authenticated user, skipping Kerberos flow')
             return
 
+        username = proxy_auth[0]
         principal = f'{username}@{realm}'
         flow.metadata[METADATA_KERBEROS_PRINCIPAL] = principal
         logger.info('enabling Kerberos flow with principal %s', principal)
 
-        filter = await spnego_filter(flow) or await knox_filter(flow)
-        if filter:
-            return await filter(flow)
+        return (await spnego_filter(flow)) or (await knox_filter(flow))
 
     return filter_kerberos_flow
-
-
-def debug_filter(f):
-    # nothing to do by now
-    return f
```

### Comparing `kerberos_auth_proxy-0.1.0a0/kerberos_auth_proxy/utils.py` & `kerberos_auth_proxy-0.1.0a1/kerberos_auth_proxy/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 '''
 Miscellaneous utilities
 '''
+
 from contextlib import contextmanager
 import os
-from typing import Callable, Generator, List, TypeVar
+from typing import Callable, Generator, List, Mapping, TypeVar
 import warnings
 
 T = TypeVar('T')
 Mapper = Callable[[str], T]
 
 
+def env_to_map(name: str) -> Mapping[str, str]:
+    '''
+    Extracts the mappings defined by '=' contained in the environment variable
+
+    An empty or unset environment variable always yields an empty list
+    '''
+    value = (os.getenv(name) or '').replace(',', ' ')
+    parts = value.split()
+    result = {}
+
+    for part in parts:
+        key, sep, value = part.partition('=')
+        if not (key and sep and value):
+            raise ValueError('Invalid mapping ' + part)
+        result[key] = value
+
+    return result
+
+
 def env_to_list(name: str, mapper: Mapper) -> List[T]:
     '''
     Splits the environment variable value by whitespace or comma, removing empty
     items from the result
 
     An empty or unset environment variable always yields an empty list
     '''
```

### Comparing `kerberos_auth_proxy-0.1.0a0/pyproject.toml` & `kerberos_auth_proxy-0.1.0a1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kerberos-auth-proxy"
-version = "0.1.0a0"
+version = "0.1.0a1"
 description = "Proxy requests to Kerberos-enabled endpoints"
 authors = ["Diógenes Oliveira <diogenes1oliveira@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "kerberos_auth_proxy" }]
 
 [tool.poetry.dependencies]
```

### Comparing `kerberos_auth_proxy-0.1.0a0/PKG-INFO` & `kerberos_auth_proxy-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerberos-auth-proxy
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Proxy requests to Kerberos-enabled endpoints
 License: MIT
 Author: Diógenes Oliveira
 Author-email: diogenes1oliveira@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

