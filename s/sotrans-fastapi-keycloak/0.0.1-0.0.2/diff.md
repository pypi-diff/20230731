# Comparing `tmp/sotrans_fastapi_keycloak-0.0.1.tar.gz` & `tmp/sotrans_fastapi_keycloak-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sotrans_fastapi_keycloak-0.0.1.tar", last modified: Fri Jul 28 14:04:56 2023, max compression
+gzip compressed data, was "sotrans_fastapi_keycloak-0.0.2.tar", last modified: Mon Jul 31 14:06:55 2023, max compression
```

## Comparing `sotrans_fastapi_keycloak-0.0.1.tar` & `sotrans_fastapi_keycloak-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 14:04:56.451726 sotrans_fastapi_keycloak-0.0.1/
--rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1122 2023-07-28 14:04:56.450207 sotrans_fastapi_keycloak-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.1/README.md
--rw-rw-rw-   0        0        0     1307 2023-07-28 14:03:24.000000 sotrans_fastapi_keycloak-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 14:04:56.451726 sotrans_fastapi_keycloak-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:04:56.429633 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/
--rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/__init__.py
--rw-rw-rw-   0        0        0    46914 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/api.py
--rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/exceptions.py
--rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/model.py
--rw-rw-rw-   0        0        0     1768 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/sotrans_model.py
-drwxrwxrwx   0        0        0        0 2023-07-28 14:04:56.448926 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-28 14:04:56.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-28 14:04:56.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 14:04:56.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      211 2023-07-28 14:04:56.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-28 14:04:56.000000 sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 14:06:55.914663 sotrans_fastapi_keycloak-0.0.2/
+-rw-rw-rw-   0        0        0    11564 2023-07-28 12:35:22.000000 sotrans_fastapi_keycloak-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1122 2023-07-31 14:06:55.914663 sotrans_fastapi_keycloak-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1314 2023-07-31 14:06:47.000000 sotrans_fastapi_keycloak-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:06:55.915662 sotrans_fastapi_keycloak-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-07-28 13:49:01.000000 sotrans_fastapi_keycloak-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:06:55.890470 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/
+-rw-rw-rw-   0        0        0      949 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/__init__.py
+-rw-rw-rw-   0        0        0    47375 2023-07-31 13:52:30.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/api.py
+-rw-rw-rw-   0        0        0     2732 2023-07-25 23:29:41.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/exceptions.py
+-rw-rw-rw-   0        0        0     9124 2023-07-28 13:53:54.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/model.py
+-rw-rw-rw-   0        0        0     1768 2023-07-28 12:39:31.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/sotrans_model.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:06:55.913662 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/
+-rw-rw-rw-   0        0        0     1122 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 14:06:55.000000 sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/top_level.txt
```

### Comparing `sotrans_fastapi_keycloak-0.0.1/LICENSE` & `sotrans_fastapi_keycloak-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.1/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans_fastapi_keycloak
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

### Comparing `sotrans_fastapi_keycloak-0.0.1/pyproject.toml` & `sotrans_fastapi_keycloak-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 ]
 requires-python = ">=3.10"
 dependencies = [
     "certifi==2023.7.22",
     "charset-normalizer==3.2.0",
     "fastapi==0.100.1",
     "idna==3.4",
-    "jose==1.0.0",
+    "python-jose==3.3.0",
     "pydantic==2.1.1",
     "pydantic_core==2.4.0",
     "requests==2.31.0",
     "sniffio==1.3.0",
     "starlette==0.27.0",
     "typing_extensions==4.7.1",
     "urllib3==2.0.4"
 ]
-version = "0.0.1"
+version = "0.0.2"
```

### Comparing `sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/__init__.py` & `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/api.py` & `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,24 +504,28 @@
         )
         if response.status_code == 201:
             return self.get_roles(role_names = [role_name])[0]
         else:
             return response
 
     @result_or_error(response_model = KeycloakRoleModel, is_list = True)
-    def get_all_roles(self) -> list[KeycloakRoleModel]:
+    def get_all_roles(self, skip: int = 0, limit: int = 0) -> list[KeycloakRoleModel]:
         """Get all roles of the Keycloak realm
 
+        Args:
+            skip: paging offset
+            limit: maximum results count
+
         Returns:
             list[KeycloakRoleModel]: All roles of the realm
 
         Raises:
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
-        return self._admin_request(url = self.roles_uri, method = HTTPMethod.GET)
+        return self._admin_request(url = f"{self.roles_uri}?first={skip}&max={limit}", method = HTTPMethod.GET)
 
     @result_or_error()
     def delete_role(self, role_name: str) -> dict:
         """Deletes a role on the realm
 
         Args:
             role_name (str): The role (name) to delete
@@ -534,24 +538,28 @@
         """
         return self._admin_request(
             url = f"{self.roles_uri}/{role_name}",
             method = HTTPMethod.DELETE,
         )
 
     @result_or_error(response_model = KeycloakGroupModel, is_list = True)
-    def get_all_groups(self) -> list[KeycloakGroupModel]:
+    def get_all_groups(self, skip: int = 0, limit: int = 20) -> list[KeycloakGroupModel]:
         """Get all base groups of the Keycloak realm
 
+        Args:
+            skip: paging offset
+            limit: maximum results count
+
         Returns:
             list[KeycloakGroupModel]: All base groups of the realm
 
         Raises:
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
-        return self._admin_request(url = self.groups_uri, method = HTTPMethod.GET)
+        return self._admin_request(url = f"{self.groups_uri}?first={skip}&max={limit}", method = HTTPMethod.GET)
 
     @result_or_error(response_model = KeycloakGroupModel, is_list = True)
     def get_groups(self, group_names: list[str]) -> list[Any] | None:
         """Returns full entries of base Groups based on group names
 
         Args:
             group_names (list[str]): Groups that should be looked up (names)
@@ -956,27 +964,31 @@
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
         return self._admin_request(
             url = f"{self.users_uri}/{user_id}",
             method = HTTPMethod.DELETE
         )
 
-    def get_all_users(self) -> list[KeycloakUserModel]:
+    def get_all_users(self, skip: int = 0, limit: int = 20) -> list[KeycloakUserModel]:
         """Returns all users of the realm
 
+        Args:
+            skip: paging offset
+            limit: maximum results count
+
         Returns:
             list[UserT]: All Keycloak users of the realm
 
         Raises:
             KeycloakError: If the resulting response is not a successful HTTP-Code (>299)
         """
 
         @result_or_error(response_model = self._user_model, is_list = True)
         def impl():
-            return self._admin_request(url = self.users_uri, method = HTTPMethod.GET)
+            return self._admin_request(url = f"{self.users_uri}?first={skip}&max={limit}", method = HTTPMethod.GET)
 
         return impl()
 
     def get_identity_providers(self) -> list[KeycloakIdentityProviderModel]:
         """Returns all configured identity Providers
 
         Returns:
```

### Comparing `sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/exceptions.py` & `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/model.py` & `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak/sotrans_model.py` & `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak/sotrans_model.py`

 * *Files identical despite different names*

### Comparing `sotrans_fastapi_keycloak-0.0.1/sotrans_fastapi_keycloak.egg-info/PKG-INFO` & `sotrans_fastapi_keycloak-0.0.2/sotrans_fastapi_keycloak.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sotrans-fastapi-keycloak
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Maintainer-email: Jonas Scholl <jonas@code-specialist.com>, Yannic Schröer <yannic@code-specialist.com>
 Keywords: Keycloak,FastAPI,Authentication,Authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
```

