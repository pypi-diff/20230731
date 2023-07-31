# Comparing `tmp/fastapi_azure_auth-4.1.3.tar.gz` & `tmp/fastapi_azure_auth-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_azure_auth-4.1.3.tar", max compression
+gzip compressed data, was "fastapi_azure_auth-4.2.0.tar", max compression
```

## Comparing `fastapi_azure_auth-4.1.3.tar` & `fastapi_azure_auth-4.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-24 11:26:18.686779 fastapi_azure_auth-4.1.3/LICENSE
--rw-r--r--   0        0        0     6468 2023-06-24 11:26:18.686779 fastapi_azure_auth-4.1.3/README.md
--rw-r--r--   0        0        0      339 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/__init__.py
--rw-r--r--   0        0        0    19735 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/auth.py
--rw-r--r--   0        0        0      337 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/exceptions.py
--rw-r--r--   0        0        0     4451 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/openid_config.py
--rw-r--r--   0        0        0        0 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/py.typed
--rw-r--r--   0        0        0     9424 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/user.py
--rw-r--r--   0        0        0      457 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/fastapi_azure_auth/utils.py
--rw-r--r--   0        0        0     2365 2023-06-24 11:26:18.702779 fastapi_azure_auth-4.1.3/pyproject.toml
--rw-r--r--   0        0        0     8033 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-31 14:04:53.089832 fastapi_azure_auth-4.2.0/LICENSE
+-rw-r--r--   0        0        0     6468 2023-07-31 14:04:53.089832 fastapi_azure_auth-4.2.0/README.md
+-rw-r--r--   0        0        0      339 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/fastapi_azure_auth/__init__.py
+-rw-r--r--   0        0        0    19723 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/fastapi_azure_auth/auth.py
+-rw-r--r--   0        0        0      337 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/fastapi_azure_auth/exceptions.py
+-rw-r--r--   0        0        0     4451 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/fastapi_azure_auth/openid_config.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/fastapi_azure_auth/py.typed
+-rw-r--r--   0        0        0     9482 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/fastapi_azure_auth/user.py
+-rw-r--r--   0        0        0      457 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/fastapi_azure_auth/utils.py
+-rw-r--r--   0        0        0     2462 2023-07-31 14:04:53.109832 fastapi_azure_auth-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8138 1970-01-01 00:00:00.000000 fastapi_azure_auth-4.2.0/PKG-INFO
```

### Comparing `fastapi_azure_auth-4.1.3/LICENSE` & `fastapi_azure_auth-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.3/README.md` & `fastapi_azure_auth-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.3/fastapi_azure_auth/auth.py` & `fastapi_azure_auth-4.2.0/fastapi_azure_auth/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,15 +285,15 @@
             allow_guest_users=allow_guest_users,
             token_version=token_version,
             openid_config_use_app_id=openid_config_use_app_id,
             openapi_authorization_url=openapi_authorization_url,
             openapi_token_url=openapi_token_url,
             openapi_description=openapi_description,
         )
-        self.scheme_name: str = 'Azure AD - PKCE, Single-tenant'
+        self.scheme_name: str = 'AzureAD_PKCE_single_tenant'
 
 
 class MultiTenantAzureAuthorizationCodeBearer(AzureAuthorizationCodeBearerBase):
     def __init__(
         self,
         app_client_id: str,
         auto_error: bool = True,
@@ -351,15 +351,15 @@
             allow_guest_users=allow_guest_users,
             multi_tenant=True,
             openid_config_use_app_id=openid_config_use_app_id,
             openapi_authorization_url=openapi_authorization_url,
             openapi_token_url=openapi_token_url,
             openapi_description=openapi_description,
         )
-        self.scheme_name: str = 'Azure AD - PKCE, Multi-tenant'
+        self.scheme_name: str = 'AzureAD_PKCE_multi_tenant'
 
 
 class B2CMultiTenantAuthorizationCodeBearer(AzureAuthorizationCodeBearerBase):
     def __init__(
         self,
         app_client_id: str,
         auto_error: bool = True,
@@ -412,8 +412,8 @@
             allow_guest_users=True,
             openid_config_use_app_id=openid_config_use_app_id,
             openid_config_url=openid_config_url,
             openapi_authorization_url=openapi_authorization_url,
             openapi_token_url=openapi_token_url,
             openapi_description=openapi_description,
         )
-        self.scheme_name: str = 'Azure AD - PKCE, B2C Multi-tenant'
+        self.scheme_name: str = 'AzureAD_PKCE_B2C_multi_tenant'
```

### Comparing `fastapi_azure_auth-4.1.3/fastapi_azure_auth/openid_config.py` & `fastapi_azure_auth-4.2.0/fastapi_azure_auth/openid_config.py`

 * *Files identical despite different names*

### Comparing `fastapi_azure_auth-4.1.3/fastapi_azure_auth/user.py` & `fastapi_azure_auth-4.2.0/fastapi_azure_auth/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,20 +61,20 @@
         default=[],
         description='Provides object IDs that represent the group memberships of the subject.',
     )
     sub: str = Field(
         ...,
         description='The principal associated with the token.',
     )
-    oid: str = Field(
-        ...,
+    oid: Optional[str] = Field(
+        default=None,
         description='The immutable identifier for the requestor, which is the verified identity of the user or service principal',
     )
-    tid: str = Field(
-        ...,
+    tid: Optional[str] = Field(
+        default=None,
         description='Represents the tenant that the user is signing in to',
     )
     uti: Optional[str] = Field(
         default=None,
         description='Token identifier claim, equivalent to jti in the JWT specification. Unique, per-token identifier that is case-sensitive.',
     )
     rh: Optional[str] = Field(
@@ -235,15 +235,15 @@
     def scopes_to_list(cls, v: object) -> object:
         """
         Validator on the scope attribute that convert the space separated list
         of scope into an actual list of scope.
         """
         if isinstance(v, str):
             return v.split(' ')
-        return v
+        return v  # pragma: no cover
 
 
 class User(Claims):
     claims: Dict[str, Any] = Field(
         ...,
         description='The entire decoded token',
     )
```

### Comparing `fastapi_azure_auth-4.1.3/pyproject.toml` & `fastapi_azure_auth-4.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-azure-auth"
-version = "4.1.3"  # Remember to change in __init__.py as well
+version = "4.2.0"  # Remember to change in __init__.py as well
 description = "Easy and secure implementation of Azure AD for your FastAPI APIs"
 authors = ["Jonas Krüger Svensson <jonas.svensson@intility.no>"]
 readme = "README.md"
 homepage = "https://github.com/intility/fastapi-azure-auth"
 repository = "https://github.com/intility/fastapi-azure-auth"
 documentation = "https://github.com/intility/fastapi-azure-auth"
 keywords = [
@@ -41,34 +41,37 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = ">0.68.0"
 cryptography = ">=40.0.1"
 python-jose = {extras = ["cryptography"], version = "^3.3.0"}
 httpx = ">0.18.2"
+pydantic-settings = "^2.0.2"
+openapi-spec-validator = "^0.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.9.3"
 black = "^22.1.0"
 pytest = "^7.0.1"
 pytest-cov = "^3.0.0"
 pytest-asyncio = "^0.18.2"
 pytest-mock = "^3.5.1"
 requests-mock = "^1.8.0"
 pytest-socket = "^0.4.0"
 pytest-dotenv = "^0.5.2"
-pytest-aiohttp = "^0.3.0"
+pytest-aiohttp = "^1.0.4"
 uvicorn = "^0.17.5"
 pytest-freezegun = "^0.4.2"
 pytest-cases = "^3.6.3"
 anyio = "^3.3.4"
-trio = "^0.19.0"
+trio = "^0.22.2"
 respx = "^0.20.1"
 ipython = "^8.2.0"
+openapi-spec-validator = "^0.6.0"
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 target-version = ['py38']
 include = '\.pyi?$'
 exclude = '''
```

### Comparing `fastapi_azure_auth-4.1.3/PKG-INFO` & `fastapi_azure_auth-4.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-azure-auth
-Version: 4.1.3
+Version: 4.2.0
 Summary: Easy and secure implementation of Azure AD for your FastAPI APIs
 Home-page: https://github.com/intility/fastapi-azure-auth
 Keywords: ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi tenant,oauth2,oidc,security,single tenant,starlette,trio
 Author: Jonas Krüger Svensson
 Author-email: jonas.svensson@intility.no
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cryptography (>=40.0.1)
 Requires-Dist: fastapi (>0.68.0)
 Requires-Dist: httpx (>0.18.2)
+Requires-Dist: openapi-spec-validator (>=0.6.0,<0.7.0)
+Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Project-URL: Documentation, https://github.com/intility/fastapi-azure-auth
 Project-URL: Repository, https://github.com/intility/fastapi-azure-auth
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <img margin="0 10px 0 0" src="https://avatars.githubusercontent.com/u/35199565" width="124px"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.1.3 Summary: Easy and
+Metadata-Version: 2.1 Name: fastapi-azure-auth Version: 4.2.0 Summary: Easy and
 secure implementation of Azure AD for your FastAPI APIs Home-page: https://
 github.com/intility/fastapi-azure-auth Keywords:
 ad,async,asyncio,authentication,azure,azure ad,azuread,fastapi,multi
 tenant,oauth2,oidc,security,single tenant,starlette,trio Author: Jonas KrÃ¼ger
 Svensson Author-email: jonas.svensson@intility.no Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
@@ -11,18 +11,20 @@
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Application Frameworks Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Dist: cryptography (>=40.0.1) Requires-
-Dist: fastapi (>0.68.0) Requires-Dist: httpx (>0.18.2) Requires-Dist: python-
-jose[cryptography] (>=3.3.0,<4.0.0) Project-URL: Documentation, https://
-github.com/intility/fastapi-azure-auth Project-URL: Repository, https://
-github.com/intility/fastapi-azure-auth Description-Content-Type: text/markdown
+Dist: fastapi (>0.68.0) Requires-Dist: httpx (>0.18.2) Requires-Dist: openapi-
+spec-validator (>=0.6.0,<0.7.0) Requires-Dist: pydantic-settings
+(>=2.0.2,<3.0.0) Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
+Project-URL: Documentation, https://github.com/intility/fastapi-azure-auth
+Project-URL: Repository, https://github.com/intility/fastapi-azure-auth
+Description-Content-Type: text/markdown
       ****** [https://avatars.githubusercontent.com/u/35199565] [https://
   raw.githubusercontent.com/Intility/fastapi-azure-auth/main/docs/static/img/
                               global/fastad.png]
                            FastAPI-Azure-Auth ******
               Azure AD Authentication for FastAPI apps made easy.
              [Python_version] [FastAPI_Version] [Package_version]
                 [Codecov] [Pre-commit] [Black] [mypy] [isort]
```

