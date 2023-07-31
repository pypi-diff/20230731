# Comparing `tmp/ocs-authentication-0.2.1.tar.gz` & `tmp/ocs_authentication-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocs-authentication-0.2.1.tar", max compression
+gzip compressed data, was "ocs_authentication-0.2.2.tar", max compression
```

## Comparing `ocs-authentication-0.2.1.tar` & `ocs_authentication-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    35149 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/LICENSE
--rw-r--r--   0        0        0     7571 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/README.md
--rw-r--r--   0        0        0        0 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/__init__.py
--rw-r--r--   0        0        0        0 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/__init__.py
--rw-r--r--   0        0        0      327 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/admin.py
--rw-r--r--   0        0        0      174 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/apps.py
--rw-r--r--   0        0        0      835 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/migrations/__init__.py
--rw-r--r--   0        0        0      319 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/models.py
--rw-r--r--   0        0        0     8995 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/test_login.py
--rw-r--r--   0        0        0      207 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/urls.py
--rw-r--r--   0        0        0     1578 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/auth_profile/views.py
--rw-r--r--   0        0        0     3720 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/backends.py
--rw-r--r--   0        0        0      181 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/exceptions.py
--rw-r--r--   0        0        0      858 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/permissions.py
--rw-r--r--   0        0        0     1482 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/settings.py
--rw-r--r--   0        0        0     3318 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/ocs_authentication/util.py
--rw-r--r--   0        0        0      603 2022-03-21 21:12:39.553395 ocs-authentication-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8590 2022-03-21 21:12:55.533586 ocs-authentication-0.2.1/setup.py
--rw-r--r--   0        0        0     8338 2022-03-21 21:12:55.534450 ocs-authentication-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7571 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/__init__.py
+-rw-r--r--   0        0        0      327 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/admin.py
+-rw-r--r--   0        0        0      174 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/apps.py
+-rw-r--r--   0        0        0      835 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/migrations/__init__.py
+-rw-r--r--   0        0        0      319 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/models.py
+-rw-r--r--   0        0        0     8995 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/test_login.py
+-rw-r--r--   0        0        0      207 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/urls.py
+-rw-r--r--   0        0        0     1578 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/auth_profile/views.py
+-rw-r--r--   0        0        0     3720 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/backends.py
+-rw-r--r--   0        0        0      181 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/exceptions.py
+-rw-r--r--   0        0        0      858 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/permissions.py
+-rw-r--r--   0        0        0     1482 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/settings.py
+-rw-r--r--   0        0        0     3318 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/ocs_authentication/util.py
+-rw-r--r--   0        0        0      597 2023-07-31 21:42:40.514882 ocs_authentication-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8383 1970-01-01 00:00:00.000000 ocs_authentication-0.2.2/PKG-INFO
```

### Comparing `ocs-authentication-0.2.1/LICENSE` & `ocs_authentication-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/README.md` & `ocs_authentication-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/ocs_authentication/auth_profile/migrations/0001_initial.py` & `ocs_authentication-0.2.2/ocs_authentication/auth_profile/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/ocs_authentication/auth_profile/test_login.py` & `ocs_authentication-0.2.2/ocs_authentication/auth_profile/test_login.py`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/ocs_authentication/auth_profile/views.py` & `ocs_authentication-0.2.2/ocs_authentication/auth_profile/views.py`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/ocs_authentication/backends.py` & `ocs_authentication-0.2.2/ocs_authentication/backends.py`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/ocs_authentication/permissions.py` & `ocs_authentication-0.2.2/ocs_authentication/permissions.py`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/ocs_authentication/settings.py` & `ocs_authentication-0.2.2/ocs_authentication/settings.py`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/ocs_authentication/util.py` & `ocs_authentication-0.2.2/ocs_authentication/util.py`

 * *Files identical despite different names*

### Comparing `ocs-authentication-0.2.1/pyproject.toml` & `ocs_authentication-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ocs-authentication"
-version = "0.2.1"
+version = "0.2.2"
 description = "Authentication backends and utilities for the OCS applications"
 authors = ["Observatory Control System Project <ocs@lco.global>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/observatorycontrolsystem/ocs-authentication"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = "^4"
 djangorestframework = "^3.13"
-requests = ">=2.22,<2.27"
+requests = ">=2,<3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.0"
 coverage = "^6.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `ocs-authentication-0.2.1/setup.py` & `ocs_authentication-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,165 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ocs-authentication
+Version: 0.2.2
+Summary: Authentication backends and utilities for the OCS applications
+Home-page: https://github.com/observatorycontrolsystem/ocs-authentication
+License: GPL-3.0-only
+Author: Observatory Control System Project
+Author-email: ocs@lco.global
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django (>=4,<5)
+Requires-Dist: djangorestframework (>=3.13,<4.0)
+Requires-Dist: requests (>=2,<3)
+Description-Content-Type: text/markdown
+
+# OCS Authentication
+
+![Build](https://github.com/observatorycontrolsystem/ocs-authentication/workflows/Build/badge.svg)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/fbba450da5394be0bd626918bbc28788)](https://www.codacy.com/gh/observatorycontrolsystem/ocs-authentication/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=observatorycontrolsystem/ocs-authentication&amp;utm_campaign=Badge_Grade)
+[![Coverage Status](https://coveralls.io/repos/github/observatorycontrolsystem/ocs-authentication/badge.svg)](https://coveralls.io/github/observatorycontrolsystem/ocs-authentication)
+
+Authentication backends and utilities for the OCS.
+
+For the OCS, the authorization server is the Observation Portal.
+
+## Prerequisites
+
+- Python >= 3.7
+
+## Installation and Getting Started
+
+To install the library into your Django application:
+```
+pip install ocs-authentication
+```
+
+Add the following to your Django project's `INSTALLED_APPS` to add the `AuthProfile` app to you project. This app is needed if any backends that use OAuth are used, which create user accounts that are meant to mirror accounts in the authorization server:
+
+```
+INSTALLED_APPS = [
+    ...
+    'ocs_authentication.auth_profile',
+    ...
+]
+```
+Then, run migrations to create the `AuthProfile` objects:
+```
+python manage.py migrate
+```
+
+Then you can configure the authentication backends. See the [Authentication Backends](#authentication-backends) section.
+
+## Authentication Backends
+
+You may need to clear out current sessions when updating the authentication backends in your project. From the [Django documentation](https://docs.djangoproject.com/en/3.2/topics/auth/customizing/#specifying-authentication-backends):
+
+> Once a user has authenticated, Django stores which backend was used to authenticate the user in the user’s session, and re-uses the same backend for the duration of that session whenever access to the currently authenticated user is needed. This effectively means that authentication sources are cached on a per-session basis, so if you change AUTHENTICATION_BACKENDS, you’ll need to clear out session data if you need to force users to re-authenticate using different methods. A simple way to do that is to execute `Session.objects.all().delete()`.
+
+### EmailOrUsernameModelBackend
+
+This backend is similar to Django's `django.contrib.auth.backends.ModelBackend`, except that it allows a user to log in with either their username or email, not just with their username. To add to your project:
+```
+AUTHENTICATION_BACKENDS = [
+    ...
+    'ocs_authentication.backends.EmailOrUsernameModelBackend',
+    ...
+]
+```
+
+### OAuthUsernamePasswordBackend
+
+This backend allows a user to authenticate using username and password with the OAuth authorization server. This backend checks whether the user account exists in the authorization server, and if it does, creates or updates that user account locally. If the intention is to check the local database first for if the user exists before sending a call off to the authorization server, you must add either `ocs_authentication.backends.EmailOrUsernameModelBackend` or `django.contrib.auth.backends.ModelBackend` to the `AUTHENTICATION_BACKENDS` *before* this backend is listed.
+
+```python
+AUTHENTICATION_BACKENDS = [
+     ...
+    # 'ocs_authentication.backends.EmailOrUsernameModelBackend', # Add this to check local DB first
+    'ocs_authentication.backends.OAuthUsernamePasswordBackend',
+    ...
+]
+```
+
+Note that if the you want to check the local DB for if the user exists there first, choose either `EmailOrUsernameModelBackend` or `ModelBackend` based on which of these backends is used in the authorization server. Using `EmailOrUsernameModelBackend` in the authorization server but using `ModelBackend` in the client application will mean that any time a user logs in to the client app with their email, the authentication request will always be forwarded to the authorization server even if the user account already exists in the local DB.
+
+### OCSTokenAuthentication Backend
+
+If the client application is using Django REST Framework and should support API token authentication, switch out use of REST Framework's TokenAuthentication with this backend which performs TokenAuthentication on the authtoken and then falls back on the api_token within the AuthProfile model. It can be included by updating the following in the settings:
+
+```python
+REST_FRAMEWORK = {
+    ...
+    'DEFAULT_AUTHENTICATION_CLASSES': (
+        # Allows authentication against DRF authtoken and then Oauth Server's api_token
+        'ocs_authentication.backends.OCSTokenAuthentication',
+        'rest_framework.authentication.SessionAuthentication',
+    ),
+     ...
+}
+```
+
+### IsServer Permission
+
+This permission is used to allow the OAuth server to call views within other applications, using its `OAUTH_SERVER_KEY`. This key should be kept private and only known by the applications and Oauth server. This permission should be included as the permission class on any view you want only accessible by the OAuth server.
+
+### IsAdminOrReadOnly Permission
+
+This permission is used to specify that a user has read-only access to the safe endpoints if unauthenticated (like `GET`), and must be an admin user (`is_staff=True`) to access writable endpoints (like `POST` or `PUT`). This should be added to individual viewset classes as needed.
+
+### Views
+
+This view is used by client applications to allow the OAuth server application to update the API token of a user when that user revokes their token and generates a new one. This keeps the tokens in sync, so the user can use the same API token to authenticate any client application. To include this view in your client app, add this line to your `urlpatterns` in `urls.py`:
+
+```
+from django.conf.urls import url, include
+import ocs_authentication.auth_profile.urls as authprofile_urls
+
+url(r'^authprofile/', include(authprofile_urls))
+```
+
+You must also set the environment variable `OAUTH_CLIENT_APPS_BASE_URLS` in the Oauth Server, which will trigger the server to call the UpdateToken View on each of those URLs whenever a user's token is revoked and replaced, and the AddUpdateUser View on each of those URLs whenever a user model or profile is created or updated. This keeps the user account details and api_tokens synced up between applications.
+
+## Settings
 
-packages = \
-['ocs_authentication',
- 'ocs_authentication.auth_profile',
- 'ocs_authentication.auth_profile.migrations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['django>=4,<5', 'djangorestframework>=3.13,<4.0', 'requests>=2.22,<2.27']
-
-setup_kwargs = {
-    'name': 'ocs-authentication',
-    'version': '0.2.1',
-    'description': 'Authentication backends and utilities for the OCS applications',
-    'long_description': "# OCS Authentication\n\n![Build](https://github.com/observatorycontrolsystem/ocs-authentication/workflows/Build/badge.svg)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/fbba450da5394be0bd626918bbc28788)](https://www.codacy.com/gh/observatorycontrolsystem/ocs-authentication/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=observatorycontrolsystem/ocs-authentication&amp;utm_campaign=Badge_Grade)\n[![Coverage Status](https://coveralls.io/repos/github/observatorycontrolsystem/ocs-authentication/badge.svg)](https://coveralls.io/github/observatorycontrolsystem/ocs-authentication)\n\nAuthentication backends and utilities for the OCS.\n\nFor the OCS, the authorization server is the Observation Portal.\n\n## Prerequisites\n\n- Python >= 3.7\n\n## Installation and Getting Started\n\nTo install the library into your Django application:\n```\npip install ocs-authentication\n```\n\nAdd the following to your Django project's `INSTALLED_APPS` to add the `AuthProfile` app to you project. This app is needed if any backends that use OAuth are used, which create user accounts that are meant to mirror accounts in the authorization server:\n\n```\nINSTALLED_APPS = [\n    ...\n    'ocs_authentication.auth_profile',\n    ...\n]\n```\nThen, run migrations to create the `AuthProfile` objects:\n```\npython manage.py migrate\n```\n\nThen you can configure the authentication backends. See the [Authentication Backends](#authentication-backends) section.\n\n## Authentication Backends\n\nYou may need to clear out current sessions when updating the authentication backends in your project. From the [Django documentation](https://docs.djangoproject.com/en/3.2/topics/auth/customizing/#specifying-authentication-backends):\n\n> Once a user has authenticated, Django stores which backend was used to authenticate the user in the user’s session, and re-uses the same backend for the duration of that session whenever access to the currently authenticated user is needed. This effectively means that authentication sources are cached on a per-session basis, so if you change AUTHENTICATION_BACKENDS, you’ll need to clear out session data if you need to force users to re-authenticate using different methods. A simple way to do that is to execute `Session.objects.all().delete()`.\n\n### EmailOrUsernameModelBackend\n\nThis backend is similar to Django's `django.contrib.auth.backends.ModelBackend`, except that it allows a user to log in with either their username or email, not just with their username. To add to your project:\n```\nAUTHENTICATION_BACKENDS = [\n    ...\n    'ocs_authentication.backends.EmailOrUsernameModelBackend',\n    ...\n]\n```\n\n### OAuthUsernamePasswordBackend\n\nThis backend allows a user to authenticate using username and password with the OAuth authorization server. This backend checks whether the user account exists in the authorization server, and if it does, creates or updates that user account locally. If the intention is to check the local database first for if the user exists before sending a call off to the authorization server, you must add either `ocs_authentication.backends.EmailOrUsernameModelBackend` or `django.contrib.auth.backends.ModelBackend` to the `AUTHENTICATION_BACKENDS` *before* this backend is listed.\n\n```python\nAUTHENTICATION_BACKENDS = [\n     ...\n    # 'ocs_authentication.backends.EmailOrUsernameModelBackend', # Add this to check local DB first\n    'ocs_authentication.backends.OAuthUsernamePasswordBackend',\n    ...\n]\n```\n\nNote that if the you want to check the local DB for if the user exists there first, choose either `EmailOrUsernameModelBackend` or `ModelBackend` based on which of these backends is used in the authorization server. Using `EmailOrUsernameModelBackend` in the authorization server but using `ModelBackend` in the client application will mean that any time a user logs in to the client app with their email, the authentication request will always be forwarded to the authorization server even if the user account already exists in the local DB.\n\n### OCSTokenAuthentication Backend\n\nIf the client application is using Django REST Framework and should support API token authentication, switch out use of REST Framework's TokenAuthentication with this backend which performs TokenAuthentication on the authtoken and then falls back on the api_token within the AuthProfile model. It can be included by updating the following in the settings:\n\n```python\nREST_FRAMEWORK = {\n    ...\n    'DEFAULT_AUTHENTICATION_CLASSES': (\n        # Allows authentication against DRF authtoken and then Oauth Server's api_token\n        'ocs_authentication.backends.OCSTokenAuthentication',\n        'rest_framework.authentication.SessionAuthentication',\n    ),\n     ...\n}\n```\n\n### IsServer Permission\n\nThis permission is used to allow the OAuth server to call views within other applications, using its `OAUTH_SERVER_KEY`. This key should be kept private and only known by the applications and Oauth server. This permission should be included as the permission class on any view you want only accessible by the OAuth server.\n\n### IsAdminOrReadOnly Permission\n\nThis permission is used to specify that a user has read-only access to the safe endpoints if unauthenticated (like `GET`), and must be an admin user (`is_staff=True`) to access writable endpoints (like `POST` or `PUT`). This should be added to individual viewset classes as needed.\n\n### Views\n\nThis view is used by client applications to allow the OAuth server application to update the API token of a user when that user revokes their token and generates a new one. This keeps the tokens in sync, so the user can use the same API token to authenticate any client application. To include this view in your client app, add this line to your `urlpatterns` in `urls.py`:\n\n```\nfrom django.conf.urls import url, include\nimport ocs_authentication.auth_profile.urls as authprofile_urls\n\nurl(r'^authprofile/', include(authprofile_urls))\n```\n\nYou must also set the environment variable `OAUTH_CLIENT_APPS_BASE_URLS` in the Oauth Server, which will trigger the server to call the UpdateToken View on each of those URLs whenever a user's token is revoked and replaced, and the AddUpdateUser View on each of those URLs whenever a user model or profile is created or updated. This keeps the user account details and api_tokens synced up between applications.\n\n## Settings\n\nAll settings for this library are namespaced under the `OCS_AUTHENTICATION` dictionary. In your settings file:\n```\nOCS_AUTHENTICATION = {\n    # Your settings go here\n}\n```\n\n### OAUTH_TOKEN_URL\nDefault: `''`\n\nThe token url of the authorization server, usually the Observation Portal's `/o/token/` endpoint.\n\n### OAUTH_PROFILE_URL\nDefault: `''`\n\nThe URL from which to retrieve user information, which is the Observation Portal's `/api/profile/` endpoint.\n\n### OAUTH_CLIENT_ID\nDefault: `''`\n\nThe OAuth client ID for the OAuth application in the authorization server used to generate tokens via username and password.\n\n### OAUTH_CLIENT_SECRET\nDefault: `''`\n\nThe OAuth client secret for the OAuth application in the authorization server used to generate tokens via username and password.\n\n### OAUTH_SERVER_KEY\nDefault: `''`\n\nThe OAuth server key is used for OAuth client applications to authenticate that a request to update the api_token for a user is coming from the OAuth server, and not from some random party. This secret token should be sent in requests in the HTTP header with `Authorization: Server <OAUTH_SERVER_TOKEN>`.\n\n### REQUESTS_TIMEOUT_SECONDS\nDefault: `60`\n\nThe timeout for remote network calls.\n",
-    'author': 'Observatory Control System Project',
-    'author_email': 'ocs@lco.global',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/observatorycontrolsystem/ocs-authentication',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+All settings for this library are namespaced under the `OCS_AUTHENTICATION` dictionary. In your settings file:
+```
+OCS_AUTHENTICATION = {
+    # Your settings go here
 }
+```
+
+### OAUTH_TOKEN_URL
+Default: `''`
+
+The token url of the authorization server, usually the Observation Portal's `/o/token/` endpoint.
+
+### OAUTH_PROFILE_URL
+Default: `''`
+
+The URL from which to retrieve user information, which is the Observation Portal's `/api/profile/` endpoint.
+
+### OAUTH_CLIENT_ID
+Default: `''`
+
+The OAuth client ID for the OAuth application in the authorization server used to generate tokens via username and password.
+
+### OAUTH_CLIENT_SECRET
+Default: `''`
+
+The OAuth client secret for the OAuth application in the authorization server used to generate tokens via username and password.
+
+### OAUTH_SERVER_KEY
+Default: `''`
+
+The OAuth server key is used for OAuth client applications to authenticate that a request to update the api_token for a user is coming from the OAuth server, and not from some random party. This secret token should be sent in requests in the HTTP header with `Authorization: Server <OAUTH_SERVER_TOKEN>`.
+
+### REQUESTS_TIMEOUT_SECONDS
+Default: `60`
 
+The timeout for remote network calls.
 
-setup(**setup_kwargs)
```

