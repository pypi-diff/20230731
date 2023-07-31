# Comparing `tmp/flagsmith-3.3.0.tar.gz` & `tmp/flagsmith-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-3.3.0.tar", max compression
+gzip compressed data, was "flagsmith-3.4.0.tar", max compression
```

## Comparing `flagsmith-3.3.0.tar` & `flagsmith-3.4.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1476 2023-07-27 12:57:23.741132 flagsmith-3.3.0/LICENSE
--rw-r--r--   0        0        0     1118 2023-07-27 12:57:23.741132 flagsmith-3.3.0/Readme.md
--rw-r--r--   0        0        0       41 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/__init__.py
--rw-r--r--   0        0        0     2008 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/analytics.py
--rw-r--r--   0        0        0      106 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/exceptions.py
--rw-r--r--   0        0        0    11095 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/flagsmith.py
--rw-r--r--   0        0        0     4633 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/models.py
--rw-r--r--   0        0        0      822 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/polling_manager.py
--rw-r--r--   0        0        0        0 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/utils/__init__.py
--rw-r--r--   0        0        0      204 2023-07-27 12:57:23.741132 flagsmith-3.3.0/flagsmith/utils/identities.py
--rw-r--r--   0        0        0      723 2023-07-27 12:57:23.741132 flagsmith-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 flagsmith-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1476 2023-07-31 09:35:39.545656 flagsmith-3.4.0/LICENSE
+-rw-r--r--   0        0        0     1118 2023-07-31 09:35:39.545656 flagsmith-3.4.0/Readme.md
+-rw-r--r--   0        0        0       41 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/__init__.py
+-rw-r--r--   0        0        0     2008 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/analytics.py
+-rw-r--r--   0        0        0      106 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/exceptions.py
+-rw-r--r--   0        0        0    12919 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/flagsmith.py
+-rw-r--r--   0        0        0     4633 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/models.py
+-rw-r--r--   0        0        0      702 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/offline_handlers.py
+-rw-r--r--   0        0        0      822 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/polling_manager.py
+-rw-r--r--   0        0        0        0 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/utils/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-31 09:35:39.545656 flagsmith-3.4.0/flagsmith/utils/identities.py
+-rw-r--r--   0        0        0      723 2023-07-31 09:35:39.545656 flagsmith-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 flagsmith-3.4.0/PKG-INFO
```

### Comparing `flagsmith-3.3.0/LICENSE` & `flagsmith-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flagsmith-3.3.0/Readme.md` & `flagsmith-3.4.0/Readme.md`

 * *Files identical despite different names*

### Comparing `flagsmith-3.3.0/flagsmith/analytics.py` & `flagsmith-3.4.0/flagsmith/analytics.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.3.0/flagsmith/flagsmith.py` & `flagsmith-3.4.0/flagsmith/flagsmith.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from flag_engine.segments.evaluator import get_identity_segments
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 from flagsmith.analytics import AnalyticsProcessor
 from flagsmith.exceptions import FlagsmithAPIError, FlagsmithClientError
 from flagsmith.models import DefaultFlag, Flags, Segment
+from flagsmith.offline_handlers import BaseOfflineHandler
 from flagsmith.polling_manager import EnvironmentDataPollingManager
 from flagsmith.utils.identities import generate_identities_data
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_API_URL = "https://edge.api.flagsmith.com/api/v1/"
 
@@ -35,93 +36,120 @@
       >>> feature_enabled = environment_flags.is_feature_enabled("foo")
       >>> identity_flags = flagsmith.get_identity_flags("identifier", {"foo": "bar"})
       >>> feature_enabled_for_identity = identity_flags.is_feature_enabled("foo")
     """
 
     def __init__(
         self,
-        environment_key: str,
-        api_url: str = DEFAULT_API_URL,
+        environment_key: str = None,
+        api_url: str = None,
         custom_headers: typing.Dict[str, typing.Any] = None,
         request_timeout_seconds: int = None,
         enable_local_evaluation: bool = False,
         environment_refresh_interval_seconds: typing.Union[int, float] = 60,
         retries: Retry = None,
         enable_analytics: bool = False,
         default_flag_handler: typing.Callable[[str], DefaultFlag] = None,
         proxies: typing.Dict[str, str] = None,
+        offline_mode: bool = False,
+        offline_handler: BaseOfflineHandler = None,
     ):
         """
-        :param environment_key: The environment key obtained from Flagsmith interface
+        :param environment_key: The environment key obtained from Flagsmith interface.
+            Required unless offline_mode is True.
         :param api_url: Override the URL of the Flagsmith API to communicate with
         :param custom_headers: Additional headers to add to requests made to the
             Flagsmith API
         :param request_timeout_seconds: Number of seconds to wait for a request to
             complete before terminating the request
         :param enable_local_evaluation: Enables local evaluation of flags
         :param environment_refresh_interval_seconds: If using local evaluation,
             specify the interval period between refreshes of local environment data
         :param retries: a urllib3.Retry object to use on all http requests to the
             Flagsmith API
         :param enable_analytics: if enabled, sends additional requests to the Flagsmith
             API to power flag analytics charts
         :param default_flag_handler: callable which will be used in the case where
-            flags cannot be retrieved from the API or a non existent feature is
+            flags cannot be retrieved from the API or a non-existent feature is
             requested
         :param proxies: as per https://requests.readthedocs.io/en/latest/api/#requests.Session.proxies
+        :param offline_mode: sets the client into offline mode. Relies on offline_handler for
+            evaluating flags.
+        :param offline_handler: provide a handler for offline logic. Used to get environment
+            document from another source when in offline_mode. Works in place of
+            default_flag_handler if offline_mode is not set and using remote evaluation.
         """
-        self.session = requests.Session()
-        self.session.headers.update(
-            **{"X-Environment-Key": environment_key}, **(custom_headers or {})
-        )
-        self.session.proxies.update(proxies or {})
-        retries = retries or Retry(total=3, backoff_factor=0.1)
-
-        self.api_url = api_url if api_url.endswith("/") else f"{api_url}/"
-        self.request_timeout_seconds = request_timeout_seconds
-        self.session.mount(self.api_url, HTTPAdapter(max_retries=retries))
-
-        self.environment_flags_url = f"{self.api_url}flags/"
-        self.identities_url = f"{self.api_url}identities/"
-        self.environment_url = f"{self.api_url}environment-document/"
 
+        self.offline_mode = offline_mode
+        self.enable_local_evaluation = enable_local_evaluation
+        self.offline_handler = offline_handler
+        self.default_flag_handler = default_flag_handler
+        self._analytics_processor = None
         self._environment = None
-        if enable_local_evaluation:
-            if not environment_key.startswith("ser."):
-                raise ValueError(
-                    "In order to use local evaluation, please generate a server key "
-                    "in the environment settings page."
-                )
 
-            self.environment_data_polling_manager_thread = (
-                EnvironmentDataPollingManager(
-                    main=self,
-                    refresh_interval_seconds=environment_refresh_interval_seconds,
-                    daemon=True,  # noqa
+        # argument validation
+        if offline_mode and not offline_handler:
+            raise ValueError("offline_handler must be provided to use offline mode.")
+        elif default_flag_handler and offline_handler:
+            raise ValueError(
+                "Cannot use both default_flag_handler and offline_handler."
+            )
+
+        if self.offline_handler:
+            self._environment = self.offline_handler.get_environment()
+
+        if not self.offline_mode:
+            if not environment_key:
+                raise ValueError("environment_key is required.")
+
+            self.session = requests.Session()
+            self.session.headers.update(
+                **{"X-Environment-Key": environment_key}, **(custom_headers or {})
+            )
+            self.session.proxies.update(proxies or {})
+            retries = retries or Retry(total=3, backoff_factor=0.1)
+
+            api_url = api_url or DEFAULT_API_URL
+            self.api_url = api_url if api_url.endswith("/") else f"{api_url}/"
+
+            self.request_timeout_seconds = request_timeout_seconds
+            self.session.mount(self.api_url, HTTPAdapter(max_retries=retries))
+
+            self.environment_flags_url = f"{self.api_url}flags/"
+            self.identities_url = f"{self.api_url}identities/"
+            self.environment_url = f"{self.api_url}environment-document/"
+
+            if self.enable_local_evaluation:
+                if not environment_key.startswith("ser."):
+                    raise ValueError(
+                        "In order to use local evaluation, please generate a server key "
+                        "in the environment settings page."
+                    )
+
+                self.environment_data_polling_manager_thread = (
+                    EnvironmentDataPollingManager(
+                        main=self,
+                        refresh_interval_seconds=environment_refresh_interval_seconds,
+                        daemon=True,  # noqa
+                    )
                 )
-            )
-            self.environment_data_polling_manager_thread.start()
+                self.environment_data_polling_manager_thread.start()
 
-        self._analytics_processor = (
-            AnalyticsProcessor(
-                environment_key, self.api_url, timeout=self.request_timeout_seconds
-            )
-            if enable_analytics
-            else None
-        )
-
-        self.default_flag_handler = default_flag_handler
+            if enable_analytics:
+                self._analytics_processor = AnalyticsProcessor(
+                    environment_key, self.api_url, timeout=self.request_timeout_seconds
+                )
 
     def get_environment_flags(self) -> Flags:
         """
         Get all the default for flags for the current environment.
 
         :return: Flags object holding all the flags for the current environment.
         """
-        if self._environment:
+        if (self.offline_mode or self.enable_local_evaluation) and self._environment:
             return self._get_environment_flags_from_document()
         return self._get_environment_flags_from_api()
 
     def get_identity_flags(
         self, identifier: str, traits: typing.Dict[str, typing.Any] = None
     ) -> Flags:
         """
@@ -132,15 +160,15 @@
         :param identifier: a unique identifier for the identity in the current
             environment, e.g. email address, username, uuid
         :param traits: a dictionary of traits to add / update on the identity in
             Flagsmith, e.g. {"num_orders": 10}
         :return: Flags object holding all the flags for the given identity.
         """
         traits = traits or {}
-        if self._environment:
+        if (self.offline_mode or self.enable_local_evaluation) and self._environment:
             return self._get_identity_flags_from_document(identifier, traits)
         return self._get_identity_flags_from_api(identifier, traits)
 
     def get_identity_segments(
         self, identifier: str, traits: typing.Dict[str, typing.Any] = None
     ) -> typing.List[Segment]:
         """
@@ -198,15 +226,17 @@
             )
             return Flags.from_api_flags(
                 api_flags=api_flags,
                 analytics_processor=self._analytics_processor,
                 default_flag_handler=self.default_flag_handler,
             )
         except FlagsmithAPIError:
-            if self.default_flag_handler:
+            if self.offline_handler:
+                return self._get_environment_flags_from_document()
+            elif self.default_flag_handler:
                 return Flags(default_flag_handler=self.default_flag_handler)
             raise
 
     def _get_identity_flags_from_api(
         self, identifier: str, traits: typing.Dict[str, typing.Any]
     ) -> Flags:
         try:
@@ -216,15 +246,17 @@
             )
             return Flags.from_api_flags(
                 api_flags=json_response["flags"],
                 analytics_processor=self._analytics_processor,
                 default_flag_handler=self.default_flag_handler,
             )
         except FlagsmithAPIError:
-            if self.default_flag_handler:
+            if self.offline_handler:
+                return self._get_identity_flags_from_document(identifier, traits)
+            elif self.default_flag_handler:
                 return Flags(default_flag_handler=self.default_flag_handler)
             raise
 
     def _get_json_response(self, url: str, method: str, body: dict = None):
         try:
             request_method = getattr(self.session, method.lower())
             response = request_method(
```

### Comparing `flagsmith-3.3.0/flagsmith/models.py` & `flagsmith-3.4.0/flagsmith/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.3.0/flagsmith/polling_manager.py` & `flagsmith-3.4.0/flagsmith/polling_manager.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.3.0/pyproject.toml` & `flagsmith-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flagsmith"
-version = "3.3.0"
+version = "3.4.0"
 description = "Flagsmith Python SDK"
 authors = ["Flagsmith <support@flagsmith.com>"]
 license = "BSD3"
 readme = "Readme.md"
 keywords = ["feature", "flag", "flagsmith", "remote", "config"]
 documentation = "https://docs.flagsmith.com"
 packages = [
```

### Comparing `flagsmith-3.3.0/PKG-INFO` & `flagsmith-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith
-Version: 3.3.0
+Version: 3.4.0
 Summary: Flagsmith Python SDK
 License: BSD3
 Keywords: feature,flag,flagsmith,remote,config
 Author: Flagsmith
 Author-email: support@flagsmith.com
 Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flagsmith Version: 3.3.0 Summary: Flagsmith Python
+Metadata-Version: 2.1 Name: flagsmith Version: 3.4.0 Summary: Flagsmith Python
 SDK License: BSD3 Keywords: feature,flag,flagsmith,remote,config Author:
 Flagsmith Author-email: support@flagsmith.com Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: flagsmith-
```

