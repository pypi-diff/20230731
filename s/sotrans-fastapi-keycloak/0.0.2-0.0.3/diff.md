# Comparing `tmp/sotrans_fastapi_keycloak-0.0.2.tar.gz` & `tmp/sotrans_fastapi_keycloak-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotrans_fastapi_keycloak-0.0.2.tar", last modified: Mon Jul 31 14:06:55 2023, max compression
+gzip compressed data, was "sotrans_fastapi_keycloak-0.0.3.tar", last modified: Mon Jul 31 15:51:50 2023, max compression
```

## Comparing `sotrans_fastapi_keycloak-0.0.2.tar` & `sotrans_fastapi_keycloak-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:06:55.914663 sotrans_fastapi_keycloak-0.0.2/
--rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-07-31 14:06:55.914663 sotrans_fastapi_keycloak-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.2/README.md
--rw-rw-rw-   0        0        0     1314 2023-07-31 14:06:47.000000 sotrans_fastapi_keycloak-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 14:06:55.915662 sotrans_fastapi_keycloak-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:06:55.890470 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/
--rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/__init__.py
--rw-rw-rw-   0        0        0    47375 2023-07-31 13:52:30.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/api.py
--rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/exceptions.py
--rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/model.py
--rw-rw-rw-   0        0        0     1768 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/sotrans_model.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:06:55.913662 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 15:51:50.643337 sotrans_fastapi_keycloak-0.0.3/
+-rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-07-31 15:51:50.642830 sotrans_fastapi_keycloak-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1314 2023-07-31 15:51:42.000000 sotrans_fastapi_keycloak-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 15:51:50.643337 sotrans_fastapi_keycloak-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:51:50.624916 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/
+-rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/__init__.py
+-rw-rw-rw-   0        0        0    47534 2023-07-31 15:51:42.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/api.py
+-rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/exceptions.py
+-rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/model.py
+-rw-rw-rw-   0        0        0     1768 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/sotrans_model.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:51:50.640769 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 15:51:50.000000 sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/top_level.txt
```

### Comparing `sotrans_fastapi_keycloak-0.0.2/LICENSE` & `sotrans_fastapi_keycloak-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.2/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans_fastapi_keycloak
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.2/pyproject.toml` & `sotrans_fastapi_keycloak-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     "pydantic_core==2.4.0",
     "requests==2.31.0",
     "sniffio==1.3.0",
     "starlette==0.27.0",
     "typing_extensions==4.7.1",
     "urllib3==2.0.4"
 ]
-version = "0.0.2"
+version = "0.0.3"
```

### Comparing `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/__init__.py` & `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/api.py` & `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -964,31 +964,35 @@
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
         return self._admin_request(
             url = f"{self.users_uri}/{user_id}",
             method = HTTPMethod.DELETE
         )
 
-    def get_all_users(self, skip: int = 0, limit: int = 20) -> list[KeycloakUserModel]:
+    def get_all_users(self, skip: int = 0, limit: int = 20, query: str | None = None) -> list[KeycloakUserModel]:
         """Returns all users of the realm
 
         Args:
             skip: paging offset
             limit: maximum results count
+            query: users find query
 
         Returns:
             list[UserT]: All Keycloak users of the realm
 
         Raises:
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
 
         @result_or_error(response_model = self._user_model, is_list = True)
         def impl():
-            return self._admin_request(url = f"{self.users_uri}?first={skip}&max={limit}", method = HTTPMethod.GET)
+            url = f"{self.users_uri}?first={skip}&max={limit}"
+            if query is not None:
+                url += f"&q={query}"
+            return self._admin_request(url = url, method = HTTPMethod.GET)
 
         return impl()
 
     def get_identity_providers(self) -> list[KeycloakIdentityProviderModel]:
         """Returns all configured identity Providers
 
         Returns:
```

### Comparing `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/exceptions.py` & `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/model.py` & `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/sotrans_model.py` & `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak/sotrans_model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.3/sotrans_fastapi_keycloak.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans-fastapi-keycloak
-Version: 0.0.2
+Version: 0.0.3
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

