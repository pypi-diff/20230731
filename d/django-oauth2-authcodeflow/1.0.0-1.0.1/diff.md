# Comparing `tmp/django_oauth2_authcodeflow-1.0.0.tar.gz` & `tmp/django_oauth2_authcodeflow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth2_authcodeflow-1.0.0.tar", max compression
+gzip compressed data, was "django_oauth2_authcodeflow-1.0.1.tar", max compression
```

## Comparing `django_oauth2_authcodeflow-1.0.0.tar` & `django_oauth2_authcodeflow-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     3540 2023-02-16 09:41:00.203768 django_oauth2_authcodeflow-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/LICENSE
--rw-r--r--   0        0        0     1890 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/OP.md
--rw-r--r--   0        0        0    13733 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/__init__.py
--rw-r--r--   0        0        0       65 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/admin.py
--rw-r--r--   0        0        0      112 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/apps.py
--rw-r--r--   0        0        0    10910 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/auth.py
--rw-r--r--   0        0        0    10951 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/conf.py
--rw-r--r--   0        0        0     1112 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/constants.py
--rw-r--r--   0        0        0        0 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/management/__init__.py
--rw-r--r--   0        0        0        0 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/management/commands/__init__.py
--rw-r--r--   0        0        0     1228 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/management/commands/oidc_urls.py
--rw-r--r--   0        0        0      346 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/management/commands/purge_blacklisted_tokens.py
--rw-r--r--   0        0        0    14008 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/middleware.py
--rw-r--r--   0        0        0      997 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0001_initial.py
--rw-r--r--   0        0        0      698 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0002_auto_20210528_1422.py
--rw-r--r--   0        0        0      770 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0003_auto_20210528_1432.py
--rw-r--r--   0        0        0     1008 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0004_alter_blacklistedtoken_id_and_more.py
--rw-r--r--   0        0        0        0 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/__init__.py
--rw-r--r--   0        0        0     2663 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/models.py
--rw-r--r--   0        0        0        0 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/py.typed
--rw-r--r--   0        0        0      632 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/urls.py
--rw-r--r--   0        0        0     3824 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/utils.py
--rw-r--r--   0        0        0    19631 2023-02-16 09:21:36.392974 django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/views.py
--rw-r--r--   0        0        0     3487 2023-02-16 09:40:59.303753 django_oauth2_authcodeflow-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    14880 1970-01-01 00:00:00.000000 django_oauth2_authcodeflow-1.0.0/setup.py
--rw-r--r--   0        0        0    16025 1970-01-01 00:00:00.000000 django_oauth2_authcodeflow-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3647 2023-07-31 15:17:25.020316 django_oauth2_authcodeflow-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2020-09-30 13:13:33.461751 django_oauth2_authcodeflow-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1890 2021-05-28 13:57:46.792981 django_oauth2_authcodeflow-1.0.1/OP.md
+-rw-r--r--   0        0        0    13986 2023-02-16 09:57:08.381515 django_oauth2_authcodeflow-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2022-12-01 09:44:48.669881 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/__init__.py
+-rw-r--r--   0        0        0       65 2022-12-01 09:44:48.673214 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/admin.py
+-rw-r--r--   0        0        0      112 2022-12-01 09:44:48.673214 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/apps.py
+-rw-r--r--   0        0        0    10910 2023-05-30 20:11:16.171658 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/auth.py
+-rw-r--r--   0        0        0    10951 2023-02-13 17:30:56.104743 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/conf.py
+-rw-r--r--   0        0        0     1112 2023-01-23 09:42:52.860223 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/constants.py
+-rw-r--r--   0        0        0        0 2022-12-01 09:44:48.676548 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-01 09:44:48.676548 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/management/commands/__init__.py
+-rw-r--r--   0        0        0     1228 2023-02-13 17:30:56.104743 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/management/commands/oidc_urls.py
+-rw-r--r--   0        0        0      346 2022-12-01 09:44:48.676548 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/management/commands/purge_blacklisted_tokens.py
+-rw-r--r--   0        0        0    14039 2023-07-31 14:55:36.791285 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/middleware.py
+-rw-r--r--   0        0        0      997 2022-12-01 09:44:48.679881 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0001_initial.py
+-rw-r--r--   0        0        0      698 2022-12-01 09:44:48.679881 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0002_auto_20210528_1422.py
+-rw-r--r--   0        0        0      770 2022-12-01 09:44:48.679881 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0003_auto_20210528_1432.py
+-rw-r--r--   0        0        0     1008 2022-12-01 09:44:48.679881 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0004_alter_blacklistedtoken_id_and_more.py
+-rw-r--r--   0        0        0        0 2022-12-01 09:44:48.683214 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/__init__.py
+-rw-r--r--   0        0        0     2663 2023-02-16 09:19:49.168720 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/models.py
+-rw-r--r--   0        0        0        0 2022-12-01 09:44:48.683214 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/py.typed
+-rw-r--r--   0        0        0      632 2022-12-01 09:44:48.683214 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/urls.py
+-rw-r--r--   0        0        0     3824 2023-02-13 17:30:56.108076 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/utils.py
+-rw-r--r--   0        0        0    19631 2023-02-16 09:19:49.168720 django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/views.py
+-rw-r--r--   0        0        0     3534 2023-07-31 15:14:34.092889 django_oauth2_authcodeflow-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    16026 1970-01-01 00:00:00.000000 django_oauth2_authcodeflow-1.0.1/PKG-INFO
```

### Comparing `django_oauth2_authcodeflow-1.0.0/CHANGELOG.md` & `django_oauth2_authcodeflow-1.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## 1.0.1
+### Fixed
+- Fix timestamp-awareness inside `RefreshSession` and `RefreshAccessToken` middlewares
+
 ## 1.0.0
 ### Changed
 - Each log (debug, warning, error) is now correctly bound to the module name.
 - Mypy 1.0
 ### Added
 - Added documentation and changelog urls for PyPI
```

### Comparing `django_oauth2_authcodeflow-1.0.0/LICENSE` & `django_oauth2_authcodeflow-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/OP.md` & `django_oauth2_authcodeflow-1.0.1/OP.md`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/README.md` & `django_oauth2_authcodeflow-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 =======
 
 [![pypi downloads][dl-image]][pypi-url]
 [![pypi status][status-image]][pypi-url]
 [![python versions][py-image]][pypi-url]
 [![django versions][django-image]][pypi-url]
 [![pipeline status][pipeline-image]][pipeline-url]
+[![coverage status][coverage-image]][coverage-url]
 [![license][license-image]](./LICENSE)
 
 [pypi-url]: https://pypi.org/project/django-oauth2-authcodeflow/
 [dl-image]: https://img.shields.io/pypi/dm/django-oauth2-authcodeflow
 [status-image]: https://img.shields.io/pypi/status/django-oauth2-authcodeflow
 [py-image]: https://img.shields.io/pypi/pyversions/django-oauth2-authcodeflow.svg
 [django-image]: https://img.shields.io/pypi/djversions/django-oauth2-authcodeflow.svg
 [pipeline-image]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/badges/master/pipeline.svg?ignore_skipped=true
 [pipeline-url]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/commits/master
+[coverage-image]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/badges/master/coverage.svg
+[coverage-url]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/commits/master
 [license-image]: https://img.shields.io/pypi/l/django-oauth2-authcodeflow.svg
 
 Authenticate with any OpenId Connect/Oauth2 provider through authorization code flow with [Django](https://www.djangoproject.com/).
 
 PKCE is also supported.
 
 Wording
```

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/auth.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/auth.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/conf.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/conf.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/constants.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/constants.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/management/commands/oidc_urls.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/management/commands/oidc_urls.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/middleware.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+from datetime import (
+    datetime,
+    timezone,
+)
 from logging import getLogger
 from re import search
-from time import (
-    gmtime,
-    mktime,
-    strftime,
-)
 from typing import (
     Callable,
     Optional,
     Tuple,
     Union,
 )
 from urllib.parse import urlencode
@@ -228,22 +227,21 @@
         if not self.is_refreshable_url(request):
             logger.debug(f"{request.path} is not refreshable")
             return
         logger.debug(f"{request.path} is refreshable")
         if constants.SESSION_REFRESH_TOKEN not in request.session:
             return
         utc_expiration = request.session[constants.SESSION_ACCESS_EXPIRES_AT]
-        utc_now_struct = gmtime()
-        utc_now = mktime(utc_now_struct)
+        utc_now = int(datetime.now(tz=timezone.utc).timestamp())
         if utc_expiration > utc_now:
             # The id_token is still valid, so we don't have to do anything.
             logger.debug(
                 'access token is still valid (%s > %s)',
-                strftime('%d/%m/%Y, %H:%M:%S', gmtime(utc_expiration)),
-                strftime('%d/%m/%Y, %H:%M:%S', utc_now_struct),
+                datetime.fromtimestamp(utc_expiration).strftime('%d/%m/%Y, %H:%M:%S'),
+                datetime.fromtimestamp(utc_now).strftime('%d/%m/%Y, %H:%M:%S'),
             )
             return
         logger.debug('access token has expired')
         # The access_token has expired, so we have to refresh silently.
         # Build the parameters.
         params = {
             'grant_type': 'refresh_token',
@@ -290,22 +288,21 @@
             return
         logger.debug(f"{request.path} is refreshable")
         utc_expiration = request.session.get(constants.SESSION_EXPIRES_AT)
         if not utc_expiration:
             msg = f"No {constants.SESSION_EXPIRES_AT} parameter in the backend session"
             logger.debug(msg)
             raise MiddlewareException(msg)
-        utc_now_struct = gmtime()
-        utc_now = mktime(utc_now_struct)
+        utc_now = datetime.now(tz=timezone.utc).timestamp()
         if utc_expiration > utc_now:
             # The session is still valid, so we don't have to do anything.
             logger.debug(
                 'session is still valid (%s > %s)',
-                strftime('%d/%m/%Y, %H:%M:%S', gmtime(utc_expiration)),
-                strftime('%d/%m/%Y, %H:%M:%S', utc_now_struct),
+                datetime.fromtimestamp(utc_expiration).strftime('%d/%m/%Y, %H:%M:%S'),
+                datetime.fromtimestamp(utc_now).strftime('%d/%m/%Y, %H:%M:%S'),
             )
             return
         # The session has expired, an authentication is now required
         # Blacklist the current id token
         BlacklistedToken.blacklist(request.session[constants.SESSION_ID_TOKEN])
         msg = "Session has expired"
         logger.debug(msg)
```

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0001_initial.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0002_auto_20210528_1422.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0002_auto_20210528_1422.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0003_auto_20210528_1432.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0003_auto_20210528_1432.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/migrations/0004_alter_blacklistedtoken_id_and_more.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/migrations/0004_alter_blacklistedtoken_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/models.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/models.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/urls.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/urls.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/utils.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/utils.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/oauth2_authcodeflow/views.py` & `django_oauth2_authcodeflow-1.0.1/oauth2_authcodeflow/views.py`

 * *Files identical despite different names*

### Comparing `django_oauth2_authcodeflow-1.0.0/pyproject.toml` & `django_oauth2_authcodeflow-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-oauth2-authcodeflow"
-version = "1.0.0"
+version = "1.0.1"
 description = "Authenticate with any OpenId Connect/Oauth2 provider through authorization code flow. PKCE is also supported."
 authors = ["Cyrille Pontvieux <cpontvieux@systra.com>"]
 maintainers = ["Cyrille Pontvieux <cyrille@enialis.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jrd/django-oauth2-authcodeflow"
 repository = "https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow"
@@ -95,15 +95,18 @@
 [tool.coverage.xml]
 output = "reports/coverage.xml"
 [tool.coverage.html]
 directory = "reports/coverage"
 title = "Django OAuth2 Auth Code Flow coverage"
 
 [[tool.poetry.source]]
-name = "testpypi"
+name = "PyPI"
+priority = "primary"
+
+[[tool.poetry.source]]
+name = "testPyPI"
 url = "https://test.pypi.org/legacy/"
-default = false
-secondary = false
+priority = "explicit"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_oauth2_authcodeflow-1.0.0/setup.py` & `django_oauth2_authcodeflow-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,226 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-oauth2-authcodeflow
+Version: 1.0.1
+Summary: Authenticate with any OpenId Connect/Oauth2 provider through authorization code flow. PKCE is also supported.
+Home-page: https://github.com/jrd/django-oauth2-authcodeflow
+License: MIT
+Keywords: oauth2,oidc,openid
+Author: Cyrille Pontvieux
+Author-email: cpontvieux@systra.com
+Maintainer: Cyrille Pontvieux
+Maintainer-email: cyrille@enialis.net
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Session
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: django (>=3.2,<5)
+Requires-Dist: python-jose[cryptography] (>=3.3)
+Requires-Dist: requests (>=2.28)
+Project-URL: Bug Tracker, https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/issues
+Project-URL: Changelog, https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/blob/master/README.md
+Project-URL: Merge Requests, https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/merge_requests
+Project-URL: Repository, https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow
+Description-Content-Type: text/markdown
+
+Summary
+=======
+
+[![pypi downloads][dl-image]][pypi-url]
+[![pypi status][status-image]][pypi-url]
+[![python versions][py-image]][pypi-url]
+[![django versions][django-image]][pypi-url]
+[![pipeline status][pipeline-image]][pipeline-url]
+[![coverage status][coverage-image]][coverage-url]
+[![license][license-image]](./LICENSE)
+
+[pypi-url]: https://pypi.org/project/django-oauth2-authcodeflow/
+[dl-image]: https://img.shields.io/pypi/dm/django-oauth2-authcodeflow
+[status-image]: https://img.shields.io/pypi/status/django-oauth2-authcodeflow
+[py-image]: https://img.shields.io/pypi/pyversions/django-oauth2-authcodeflow.svg
+[django-image]: https://img.shields.io/pypi/djversions/django-oauth2-authcodeflow.svg
+[pipeline-image]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/badges/master/pipeline.svg?ignore_skipped=true
+[pipeline-url]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/commits/master
+[coverage-image]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/badges/master/coverage.svg
+[coverage-url]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/commits/master
+[license-image]: https://img.shields.io/pypi/l/django-oauth2-authcodeflow.svg
+
+Authenticate with any OpenId Connect/Oauth2 provider through authorization code flow with [Django](https://www.djangoproject.com/).
+
+PKCE is also supported.
+
+Wording
+-------
+
+- OP = OpenId Connect Provider, the auth server
+- RP = Relying Party, the client, your application
+
+Setup
+-----
+
+- add `oauth2_authcodeflow` to the `INSTALLED_APPS` (after `django.contrib.auth` and `django.contrib.session` apps)
+- add `path('oidc/', include('oauth2_authcodeflow.urls')),` in your global `urls.py` file.
+
+    You can change the path prefix to what you want
+
+- add `oauth2_authcodeflow.auth.AuthenticationBackend` to the `AUTHENTICATION_BACKENDS` config.
+
+    You can keep `django.contrib.auth.backends.ModelBackend` as a second-fallback auth mechanism.
+
+- get your callback urls by doing:
+```sh
+./manage.py oidc_urls [--secure] <HOST_NAME>
+```
+- Configure your application on the OpenId Connect Provider.
+
+    This should give you a `client_id` and a `secret_id`.
+
+    You will need to fill the `redirect_url` and `logout_url` there.
+
+- Ensue to include the `sid`, email, first name, last name (if applicable) parameters in the id token claims on the OP.
+- Ensure that `django.contrib.sessions.middleware.SessionMiddleware` is in `MIDDLEWARE`
+
+Minimal configuration
+---------------------
+
+- `SESSION_COOKIE_SECURE` to `True` if your Django is served through *HTTPS*
+- `OIDC_OP_DISCOVERY_DOCUMENT_URL` to the well-known openid configuration url of the OP
+- `OIDC_RP_CLIENT_ID` client id provided by the OP
+- `OIDC_RP_CLIENT_SECRET` secrect id provided by the OP
+
+Login
+-----
+
+Get your browser/frontend to go to the `oidc_authentication` page name (`/oidc/authenticate` by default) with the following parameters:
+
+- `next`: the url to redirect on success
+- `fail`: the url to redirect on failure, `error` query string may contain an error description
+
+Logout
+------
+
+Get your browser/frontend to go to the `oidc_logout` page name (`/oidc/logout` by default) with the following parameters:
+
+- `next`: the url to redirect on success
+- `fail`: the url to redirect on failure, `error` query string may contain an error description
+
+Logout from the OP as well
+--------------------------
+
+This will logout the user from the application but also from the OP (if user say yes) and the OP should also logout the user from all other apps connected to this OP.
+
+The spec is not well followed by the OP, so you mileage may vary.
+
+Get your browser/frontend to go to the `oidc_total_logout` page name (`/oidc/total_logout` by default) with the following parameters:
+
+- `next`: the url to redirect on success
+- `fail`: the url to redirect on failure, `error` query string may contain an error description
+
+Protect your urls
+-----------------
+
+At least three options are possible.
+
+1. Use default django way to [limit access to logged-in users](https://docs.djangoproject.com/en/4.1/topics/auth/default/#limiting-access-to-logged-in-users) by defining `LOGIN_URL` in your settings and and `login_required` decorators in your views.  
+  ```python
+  # settings.py
+  from django.urls import reverse_lazy
+  from django.utils.text import format_lazy
+  LOGIN_URL = format_lazy('{url}?fail=/', url=reverse_lazy(OIDC_URL_AUTHENTICATION_NAME))
+  # urls.py
+  from django.contrib.auth.decorators import login_required
+  path('restricted_url/', login_required(your_view)),
+  ```
+2. A slightly different version, by directly and only using the `login_required` from `oauth2_authcodeflow.utils`.
+3. Use the `LoginRequiredMiddleware` with `OIDC_MIDDLEWARE_NO_AUTH_URL_PATTERNS` configuration.
+
+Optional middlewares
+--------------------
+
+You can add some middlewares to add some features:
+
+- `oauth2_authcodeflow.middleware.LoginRequiredMiddleware` to automaticaly force a login request to urls not in `OIDC_MIDDLEWARE_NO_AUTH_URL_PATTERNS` if not authenticated.
+- `oauth2_authcodeflow.middleware.RefreshAccessTokenMiddleware` to automaticaly refresh the access token when it’s expired.
+- `oauth2_authcodeflow.middleware.RefreshSessionMiddleware` to automaticaly ask for a new id token when it’s considered expired.
+- `oauth2_authcodeflow.middleware.BearerAuthMiddleware` to authenticate the user using `Authorization` HTTP header (API, scripts, CLI usage).
+
+`LoginRequiredMiddleware` will refresh to the original page uppon user logged-in.
+
+`RefreshAccessTokenMiddleware` and `RefreshSessionMiddleware` will try the refresh and return a redirect to the same page (or the one configured as next in the login phase) if the refresh cannot happen.
+
+Use them to silently refresh your access/id tokens.
+
+BearerAuthMiddleware will use `oauth2_authcodeflow.auth.BearerAuthenticationBackend` to authenticate the user based on `Authorization` HTTP header instead of using the sessions.
+
+Use this to allow to authenticate without cookies/session. You then need to login with `from_cli=1` in your `login` url. You then needs to go to the displayed url with a browser and copy the result http header to make further requests.
+
+
+Full configuration
+------------------
+Secure session cookie settings:
+
+- `SESSION_COOKIE_AGE` to a reasonable time (default 2 weeks)
+- `SESSION_COOKIE_HTTPONLY` **must** be `True` (default `True`)
+- `SESSION_COOKIE_PATH` be sure to use `/` to prevent some weird behavior (default `/`)
+- `SESSION_COOKIE_SAMESITE` **should** be `Lax` (default `Lax`)
+- `SESSION_COOKIE_SECURE` **should** be `True` in *https* context (default `False`)
+
+Specific OIDC settings:
+
+| Settings | Description | Default |
+| -------- | ----------- | ------- |
+| `OIDC_OP_DISCOVERY_DOCUMENT_URL` | URL of your OpenID connect Provider discovery document url (*recommended*).<br>If you provide this, the following configs will be ignored:<br>- `OIDC_OP_AUTHORIZATION_URL`<br>- `OIDC_OP_TOKEN_URL`<br>- `OIDC_OP_USERINFO_URL`<br>- `OIDC_OP_JWKS_URL` | `None` |
+| `OIDC_OP_AUTHORIZATION_URL` | URL of your OpenID connect Provider authorization endpoint (**not recommended**, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |
+| `OIDC_OP_TOKEN_URL` | URL of your OpenID connect Provider token endpoint (**not recommended**, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |
+| `OIDC_OP_USERINFO_URL` | URL of your OpenID connect Provider userinfo endpoint (**not recommended**, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |
+| `OIDC_OP_JWKS_URL` | URL of your OpenId connect Provider endpoint to get public signing keys (in `PEM` or `DER` format).<br>This is used to verify the `id_token`.<br>This is **not recommended** to provide this url here but rather use `OIDC_OP_DISCOVERY_DOCUMENT_URL` config. | `None` |
+| `OIDC_OP_END_SESSION_URL` | URL of your OpenID connect Provider end session endpoint (not recommended, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |
+| `OIDC_OP_FETCH_USER_INFO` | Fetch user info on login or not. | `True` |
+| `OIDC_OP_TOTAL_LOGOUT` | Do a call to total logout will call the OP for a logout. Default true.<br>Be careful, some OP will not follow the RFC and will not allow the user to NOT logout all connected apps.<br>Azure is such a bad example. | `True` |
+| `OIDC_OP_EXPECTED_EMAIL_CLAIM` | expected email key. | `'email'` |
+| `OIDC_OP_EXPECTED_CLAIMS` | `OIDC_OP_EXPECTED_EMAIL_CLAIM` value is automatically included in this list. | `[]` |
+| `OIDC_RP_CLIENT_ID` | OpenID Connect client ID provided for your Relaying Party/client by your OpenIdConnect Provider | |
+| `OIDC_RP_CLIENT_SECRET` | OpenID Connect client secret provided for your Relaying Party/client by your OpenIdConnect Provider | |
+| `OIDC_RP_USE_PKCE` | `PKCE` improve security, disable it only if your provider cannot handle it. | `True` |
+| `OIDC_RP_FORCE_CONSENT_PROMPT` | Force to ask for consent on login, even if `offline_access` is not in scopes | `False` |
+| `OIDC_RP_SCOPES` | The OpenID Connect scopes to request during login.<br>The scopes could be usefull later to get access to other ressources.<br>`openid` must be in the list.<br>You can also include the `email` scope to ensure that the email field will be in the claims (*recommended*).<br>You can also include the `profile` scope to get more (like names, …) info in the `id_token` (*recommended*).<br>You can also get a `refresh_token` by specifying the `offline_access` scope. | `['openid', 'email', 'profile', 'offline_access']` |
+| `OIDC_RP_USERINFO_CLAIMS` | OpenID Connect authorization [request parameter `userinfo` member](https://openid.net/specs/openid-connect-core-1_0.html#ClaimsParameter) to optionaly add to id token request (dict type). | `None` |
+| `OIDC_RP_TOKEN_CLAIMS` | OpenID Connect authorization [request parameter `id_token` member](https://openid.net/specs/openid-connect-core-1_0.html#ClaimsParameter) to optionaly add to id token request (dict type). | `None` |
+| `OIDC_RP_SIGN_ALGOS_ALLOWED` | Sets the algorithms the IdP may use to sign ID tokens.<br>Typical values ar `HS256` (no key required) and `RS256` (public key required)<br>The public keys might be defined in `OIDC_RP_IDP_SIGN_KEY` or deduced using the `OIDC_OP_JWKS_URL` config. | `['HS256', 'HS384', 'HS512', 'RS256', 'RS384', 'RS512']` |
+| `OIDC_RP_IDP_SIGN_KEY` | Public RSA used to verify signatures. Overrides keys from JWKS endpoint.<br>Should be in `PEM` or `DER` format. | `None` |
+| `OIDC_CREATE_USER` | Enables or disables automatic user creation during authentication | `True` |
+| `OIDC_RANDOM_SIZE` | Sets the length of the random string used in the OAuth2 protocol. | `32` |
+| `OIDC_PROXY` | Defines a proxy for all requests to the OpenID Connect provider (fetch JWS, retrieve JWT tokens, Userinfo Endpoint).<br>The default is set to `None` which means the library will not use a proxy and connect directly.<br>For configuring a proxy check the Python requests documentation: <https://requests.readthedocs.io/en/master/user/advanced/#proxies> | `None` |
+| `OIDC_TIMEOUT` | Defines a timeout for all requests to the OpenID Connect provider (fetch JWS, retrieve JWT tokens, Userinfo Endpoint).<br>The default is set to `None` which means the library will wait indefinitely.<br>The time can be defined as seconds (integer).<br>More information about possible configuration values, see Python requests: <https://requests.readthedocs.io/en/master/user/quickstart/#timeouts> | `None` |
+| `OIDC_REDIRECT_OK_FIELD_NAME` | Sets the GET parameter that is being used to define the redirect URL after succesful authentication | `'next'` |
+| `OIDC_REDIRECT_ERROR_FIELD_NAME` | Sets the GET parameter that is being used to define the redirect URL after failed authentication | `'fail'` |
+| `OIDC_DJANGO_USERNAME_FUNC` | Function or dotted path to a function that compute the django username based on claims.<br>The username should be unique for this app.<br>The default is to use a base64 url encode of the email hash (sha1). | `get_default_django_username` |
+| `OIDC_EMAIL_CLAIM` | Claim name for email<br>`None` value means use `OIDC_OP_EXPECTED_EMAIL_CLAIM` value<br>You can also provide a lambda that takes all the claims as argument and return an email | `None` |
+| `OIDC_FIRSTNAME_CLAIM` | You can also provide a lambda that takes all the claims as argument and return a firstname | `'given_name'` |
+| `OIDC_LASTNAME_CLAIM` | You can also provide a lambda that takes all the claims as argument and return a lastname | `'family_name'` |
+| `OIDC_EXTEND_USER` | Callable that takes the `user`, the `claims` and optionaly the `request` and `access_token` as arguments and that can extend user properties.<br>You can also specify a dotted path to a callable. | `None` |
+| `OIDC_UNUSABLE_PASSWORD` | Scramble the password on each SSO connection/renewal.<br>If `False`, it will only scramble it when creating an account | `True` |
+| `OIDC_BLACKLIST_TOKEN_TIMEOUT_SECONDS` | 7 days by default | `7 * 86400` |
+| `OIDC_AUTHORIZATION_HEADER_PREFIX` | Only used when using authorization in header:<br>`Authorization: Bearer id_token`<br>This is only possible if `oauth2_authcodeflow.middleware.BearerAuthMiddleware` has been added to `MIDDLEWARE` setting list. | `'Bearer'` |
+| `OIDC_MIDDLEWARE_NO_AUTH_URL_PATTERNS` | The `RefreshAccessTokenMiddleware` and `RefreshSessionMiddleware` will use this list to bypass auth checks.<br>Any url listed here will not be tried to be authenticated using Auth Code Flow.<br>You should include at least any failure/error or admin urls in it. | `[]` |
+| `OIDC_MIDDLEWARE_LOGIN_REQUIRED_REDIRECT` | Redirect to login page if not authenticated when using `LoginRequiredMiddleware`. | `True` |
+| `OIDC_MIDDLEWARE_API_URL_PATTERNS` | The `RefreshAccessTokenMiddleware` and `RefreshSessionMiddleware` will use this list to answer JSON response in case of refresh failure.<br>Expected list of regexp URL patterns. | `['^/api/']` |
+| `OIDC_MIDDLEWARE_SESSION_TIMEOUT_SECONDS` | 7 days by default | `7 * 86400` |
 
-packages = \
-['oauth2_authcodeflow',
- 'oauth2_authcodeflow.management',
- 'oauth2_authcodeflow.management.commands',
- 'oauth2_authcodeflow.migrations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['django>=3.2,<5', 'python-jose[cryptography]>=3.3', 'requests>=2.28']
-
-setup_kwargs = {
-    'name': 'django-oauth2-authcodeflow',
-    'version': '1.0.0',
-    'description': 'Authenticate with any OpenId Connect/Oauth2 provider through authorization code flow. PKCE is also supported.',
-    'long_description': "Summary\n=======\n\n[![pypi downloads][dl-image]][pypi-url]\n[![pypi status][status-image]][pypi-url]\n[![python versions][py-image]][pypi-url]\n[![django versions][django-image]][pypi-url]\n[![pipeline status][pipeline-image]][pipeline-url]\n[![license][license-image]](./LICENSE)\n\n[pypi-url]: https://pypi.org/project/django-oauth2-authcodeflow/\n[dl-image]: https://img.shields.io/pypi/dm/django-oauth2-authcodeflow\n[status-image]: https://img.shields.io/pypi/status/django-oauth2-authcodeflow\n[py-image]: https://img.shields.io/pypi/pyversions/django-oauth2-authcodeflow.svg\n[django-image]: https://img.shields.io/pypi/djversions/django-oauth2-authcodeflow.svg\n[pipeline-image]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/badges/master/pipeline.svg?ignore_skipped=true\n[pipeline-url]: https://gitlab.com/systra/qeto/lib/django-oauth2-authcodeflow/-/commits/master\n[license-image]: https://img.shields.io/pypi/l/django-oauth2-authcodeflow.svg\n\nAuthenticate with any OpenId Connect/Oauth2 provider through authorization code flow with [Django](https://www.djangoproject.com/).\n\nPKCE is also supported.\n\nWording\n-------\n\n- OP = OpenId Connect Provider, the auth server\n- RP = Relying Party, the client, your application\n\nSetup\n-----\n\n- add `oauth2_authcodeflow` to the `INSTALLED_APPS` (after `django.contrib.auth` and `django.contrib.session` apps)\n- add `path('oidc/', include('oauth2_authcodeflow.urls')),` in your global `urls.py` file.\n\n    You can change the path prefix to what you want\n\n- add `oauth2_authcodeflow.auth.AuthenticationBackend` to the `AUTHENTICATION_BACKENDS` config.\n\n    You can keep `django.contrib.auth.backends.ModelBackend` as a second-fallback auth mechanism.\n\n- get your callback urls by doing:\n```sh\n./manage.py oidc_urls [--secure] <HOST_NAME>\n```\n- Configure your application on the OpenId Connect Provider.\n\n    This should give you a `client_id` and a `secret_id`.\n\n    You will need to fill the `redirect_url` and `logout_url` there.\n\n- Ensue to include the `sid`, email, first name, last name (if applicable) parameters in the id token claims on the OP.\n- Ensure that `django.contrib.sessions.middleware.SessionMiddleware` is in `MIDDLEWARE`\n\nMinimal configuration\n---------------------\n\n- `SESSION_COOKIE_SECURE` to `True` if your Django is served through *HTTPS*\n- `OIDC_OP_DISCOVERY_DOCUMENT_URL` to the well-known openid configuration url of the OP\n- `OIDC_RP_CLIENT_ID` client id provided by the OP\n- `OIDC_RP_CLIENT_SECRET` secrect id provided by the OP\n\nLogin\n-----\n\nGet your browser/frontend to go to the `oidc_authentication` page name (`/oidc/authenticate` by default) with the following parameters:\n\n- `next`: the url to redirect on success\n- `fail`: the url to redirect on failure, `error` query string may contain an error description\n\nLogout\n------\n\nGet your browser/frontend to go to the `oidc_logout` page name (`/oidc/logout` by default) with the following parameters:\n\n- `next`: the url to redirect on success\n- `fail`: the url to redirect on failure, `error` query string may contain an error description\n\nLogout from the OP as well\n--------------------------\n\nThis will logout the user from the application but also from the OP (if user say yes) and the OP should also logout the user from all other apps connected to this OP.\n\nThe spec is not well followed by the OP, so you mileage may vary.\n\nGet your browser/frontend to go to the `oidc_total_logout` page name (`/oidc/total_logout` by default) with the following parameters:\n\n- `next`: the url to redirect on success\n- `fail`: the url to redirect on failure, `error` query string may contain an error description\n\nProtect your urls\n-----------------\n\nAt least three options are possible.\n\n1. Use default django way to [limit access to logged-in users](https://docs.djangoproject.com/en/4.1/topics/auth/default/#limiting-access-to-logged-in-users) by defining `LOGIN_URL` in your settings and and `login_required` decorators in your views.  \n  ```python\n  # settings.py\n  from django.urls import reverse_lazy\n  from django.utils.text import format_lazy\n  LOGIN_URL = format_lazy('{url}?fail=/', url=reverse_lazy(OIDC_URL_AUTHENTICATION_NAME))\n  # urls.py\n  from django.contrib.auth.decorators import login_required\n  path('restricted_url/', login_required(your_view)),\n  ```\n2. A slightly different version, by directly and only using the `login_required` from `oauth2_authcodeflow.utils`.\n3. Use the `LoginRequiredMiddleware` with `OIDC_MIDDLEWARE_NO_AUTH_URL_PATTERNS` configuration.\n\nOptional middlewares\n--------------------\n\nYou can add some middlewares to add some features:\n\n- `oauth2_authcodeflow.middleware.LoginRequiredMiddleware` to automaticaly force a login request to urls not in `OIDC_MIDDLEWARE_NO_AUTH_URL_PATTERNS` if not authenticated.\n- `oauth2_authcodeflow.middleware.RefreshAccessTokenMiddleware` to automaticaly refresh the access token when it’s expired.\n- `oauth2_authcodeflow.middleware.RefreshSessionMiddleware` to automaticaly ask for a new id token when it’s considered expired.\n- `oauth2_authcodeflow.middleware.BearerAuthMiddleware` to authenticate the user using `Authorization` HTTP header (API, scripts, CLI usage).\n\n`LoginRequiredMiddleware` will refresh to the original page uppon user logged-in.\n\n`RefreshAccessTokenMiddleware` and `RefreshSessionMiddleware` will try the refresh and return a redirect to the same page (or the one configured as next in the login phase) if the refresh cannot happen.\n\nUse them to silently refresh your access/id tokens.\n\nBearerAuthMiddleware will use `oauth2_authcodeflow.auth.BearerAuthenticationBackend` to authenticate the user based on `Authorization` HTTP header instead of using the sessions.\n\nUse this to allow to authenticate without cookies/session. You then need to login with `from_cli=1` in your `login` url. You then needs to go to the displayed url with a browser and copy the result http header to make further requests.\n\n\nFull configuration\n------------------\nSecure session cookie settings:\n\n- `SESSION_COOKIE_AGE` to a reasonable time (default 2 weeks)\n- `SESSION_COOKIE_HTTPONLY` **must** be `True` (default `True`)\n- `SESSION_COOKIE_PATH` be sure to use `/` to prevent some weird behavior (default `/`)\n- `SESSION_COOKIE_SAMESITE` **should** be `Lax` (default `Lax`)\n- `SESSION_COOKIE_SECURE` **should** be `True` in *https* context (default `False`)\n\nSpecific OIDC settings:\n\n| Settings | Description | Default |\n| -------- | ----------- | ------- |\n| `OIDC_OP_DISCOVERY_DOCUMENT_URL` | URL of your OpenID connect Provider discovery document url (*recommended*).<br>If you provide this, the following configs will be ignored:<br>- `OIDC_OP_AUTHORIZATION_URL`<br>- `OIDC_OP_TOKEN_URL`<br>- `OIDC_OP_USERINFO_URL`<br>- `OIDC_OP_JWKS_URL` | `None` |\n| `OIDC_OP_AUTHORIZATION_URL` | URL of your OpenID connect Provider authorization endpoint (**not recommended**, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |\n| `OIDC_OP_TOKEN_URL` | URL of your OpenID connect Provider token endpoint (**not recommended**, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |\n| `OIDC_OP_USERINFO_URL` | URL of your OpenID connect Provider userinfo endpoint (**not recommended**, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |\n| `OIDC_OP_JWKS_URL` | URL of your OpenId connect Provider endpoint to get public signing keys (in `PEM` or `DER` format).<br>This is used to verify the `id_token`.<br>This is **not recommended** to provide this url here but rather use `OIDC_OP_DISCOVERY_DOCUMENT_URL` config. | `None` |\n| `OIDC_OP_END_SESSION_URL` | URL of your OpenID connect Provider end session endpoint (not recommended, `OIDC_OP_DISCOVERY_DOCUMENT_URL` is preferred). | `None` |\n| `OIDC_OP_FETCH_USER_INFO` | Fetch user info on login or not. | `True` |\n| `OIDC_OP_TOTAL_LOGOUT` | Do a call to total logout will call the OP for a logout. Default true.<br>Be careful, some OP will not follow the RFC and will not allow the user to NOT logout all connected apps.<br>Azure is such a bad example. | `True` |\n| `OIDC_OP_EXPECTED_EMAIL_CLAIM` | expected email key. | `'email'` |\n| `OIDC_OP_EXPECTED_CLAIMS` | `OIDC_OP_EXPECTED_EMAIL_CLAIM` value is automatically included in this list. | `[]` |\n| `OIDC_RP_CLIENT_ID` | OpenID Connect client ID provided for your Relaying Party/client by your OpenIdConnect Provider | |\n| `OIDC_RP_CLIENT_SECRET` | OpenID Connect client secret provided for your Relaying Party/client by your OpenIdConnect Provider | |\n| `OIDC_RP_USE_PKCE` | `PKCE` improve security, disable it only if your provider cannot handle it. | `True` |\n| `OIDC_RP_FORCE_CONSENT_PROMPT` | Force to ask for consent on login, even if `offline_access` is not in scopes | `False` |\n| `OIDC_RP_SCOPES` | The OpenID Connect scopes to request during login.<br>The scopes could be usefull later to get access to other ressources.<br>`openid` must be in the list.<br>You can also include the `email` scope to ensure that the email field will be in the claims (*recommended*).<br>You can also include the `profile` scope to get more (like names, …) info in the `id_token` (*recommended*).<br>You can also get a `refresh_token` by specifying the `offline_access` scope. | `['openid', 'email', 'profile', 'offline_access']` |\n| `OIDC_RP_USERINFO_CLAIMS` | OpenID Connect authorization [request parameter `userinfo` member](https://openid.net/specs/openid-connect-core-1_0.html#ClaimsParameter) to optionaly add to id token request (dict type). | `None` |\n| `OIDC_RP_TOKEN_CLAIMS` | OpenID Connect authorization [request parameter `id_token` member](https://openid.net/specs/openid-connect-core-1_0.html#ClaimsParameter) to optionaly add to id token request (dict type). | `None` |\n| `OIDC_RP_SIGN_ALGOS_ALLOWED` | Sets the algorithms the IdP may use to sign ID tokens.<br>Typical values ar `HS256` (no key required) and `RS256` (public key required)<br>The public keys might be defined in `OIDC_RP_IDP_SIGN_KEY` or deduced using the `OIDC_OP_JWKS_URL` config. | `['HS256', 'HS384', 'HS512', 'RS256', 'RS384', 'RS512']` |\n| `OIDC_RP_IDP_SIGN_KEY` | Public RSA used to verify signatures. Overrides keys from JWKS endpoint.<br>Should be in `PEM` or `DER` format. | `None` |\n| `OIDC_CREATE_USER` | Enables or disables automatic user creation during authentication | `True` |\n| `OIDC_RANDOM_SIZE` | Sets the length of the random string used in the OAuth2 protocol. | `32` |\n| `OIDC_PROXY` | Defines a proxy for all requests to the OpenID Connect provider (fetch JWS, retrieve JWT tokens, Userinfo Endpoint).<br>The default is set to `None` which means the library will not use a proxy and connect directly.<br>For configuring a proxy check the Python requests documentation: <https://requests.readthedocs.io/en/master/user/advanced/#proxies> | `None` |\n| `OIDC_TIMEOUT` | Defines a timeout for all requests to the OpenID Connect provider (fetch JWS, retrieve JWT tokens, Userinfo Endpoint).<br>The default is set to `None` which means the library will wait indefinitely.<br>The time can be defined as seconds (integer).<br>More information about possible configuration values, see Python requests: <https://requests.readthedocs.io/en/master/user/quickstart/#timeouts> | `None` |\n| `OIDC_REDIRECT_OK_FIELD_NAME` | Sets the GET parameter that is being used to define the redirect URL after succesful authentication | `'next'` |\n| `OIDC_REDIRECT_ERROR_FIELD_NAME` | Sets the GET parameter that is being used to define the redirect URL after failed authentication | `'fail'` |\n| `OIDC_DJANGO_USERNAME_FUNC` | Function or dotted path to a function that compute the django username based on claims.<br>The username should be unique for this app.<br>The default is to use a base64 url encode of the email hash (sha1). | `get_default_django_username` |\n| `OIDC_EMAIL_CLAIM` | Claim name for email<br>`None` value means use `OIDC_OP_EXPECTED_EMAIL_CLAIM` value<br>You can also provide a lambda that takes all the claims as argument and return an email | `None` |\n| `OIDC_FIRSTNAME_CLAIM` | You can also provide a lambda that takes all the claims as argument and return a firstname | `'given_name'` |\n| `OIDC_LASTNAME_CLAIM` | You can also provide a lambda that takes all the claims as argument and return a lastname | `'family_name'` |\n| `OIDC_EXTEND_USER` | Callable that takes the `user`, the `claims` and optionaly the `request` and `access_token` as arguments and that can extend user properties.<br>You can also specify a dotted path to a callable. | `None` |\n| `OIDC_UNUSABLE_PASSWORD` | Scramble the password on each SSO connection/renewal.<br>If `False`, it will only scramble it when creating an account | `True` |\n| `OIDC_BLACKLIST_TOKEN_TIMEOUT_SECONDS` | 7 days by default | `7 * 86400` |\n| `OIDC_AUTHORIZATION_HEADER_PREFIX` | Only used when using authorization in header:<br>`Authorization: Bearer id_token`<br>This is only possible if `oauth2_authcodeflow.middleware.BearerAuthMiddleware` has been added to `MIDDLEWARE` setting list. | `'Bearer'` |\n| `OIDC_MIDDLEWARE_NO_AUTH_URL_PATTERNS` | The `RefreshAccessTokenMiddleware` and `RefreshSessionMiddleware` will use this list to bypass auth checks.<br>Any url listed here will not be tried to be authenticated using Auth Code Flow.<br>You should include at least any failure/error or admin urls in it. | `[]` |\n| `OIDC_MIDDLEWARE_LOGIN_REQUIRED_REDIRECT` | Redirect to login page if not authenticated when using `LoginRequiredMiddleware`. | `True` |\n| `OIDC_MIDDLEWARE_API_URL_PATTERNS` | The `RefreshAccessTokenMiddleware` and `RefreshSessionMiddleware` will use this list to answer JSON response in case of refresh failure.<br>Expected list of regexp URL patterns. | `['^/api/']` |\n| `OIDC_MIDDLEWARE_SESSION_TIMEOUT_SECONDS` | 7 days by default | `7 * 86400` |\n",
-    'author': 'Cyrille Pontvieux',
-    'author_email': 'cpontvieux@systra.com',
-    'maintainer': 'Cyrille Pontvieux',
-    'maintainer_email': 'cyrille@enialis.net',
-    'url': 'https://github.com/jrd/django-oauth2-authcodeflow',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

