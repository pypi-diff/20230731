# Comparing `tmp/pysnyk-0.9.5.tar.gz` & `tmp/pysnyk-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnyk-0.9.5.tar", max compression
+gzip compressed data, was "pysnyk-0.9.7.tar", max compression
```

## Comparing `pysnyk-0.9.5.tar` & `pysnyk-0.9.7.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1057 2023-01-20 11:42:17.299718 pysnyk-0.9.5/LICENSE
--rw-r--r--   0        0        0    11993 2023-01-20 11:42:17.299718 pysnyk-0.9.5/README.md
--rw-r--r--   0        0        0      913 2023-01-20 11:42:17.303717 pysnyk-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      679 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/__init__.py
--rw-r--r--   0        0        0      219 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/__version__.py
--rw-r--r--   0        0        0     8474 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/client.py
--rw-r--r--   0        0        0      655 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/errors.py
--rw-r--r--   0        0        0    15344 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/managers.py
--rw-r--r--   0        0        0    21879 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/models.py
--rw-r--r--   0        0        0    12798 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_client.py
--rw-r--r--   0        0        0      497 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/organizations.json
--rw-r--r--   0        0        0      613 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/projects.json
--rw-r--r--   0        0        0      397 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/rest_groups.json
--rw-r--r--   0        0        0     3340 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/rest_targets_page1.json
--rw-r--r--   0        0        0     3359 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/rest_targets_page2.json
--rw-r--r--   0        0        0     3339 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/rest_targets_page3.json
--rw-r--r--   0        0        0      397 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/v3_groups.json
--rw-r--r--   0        0        0     3340 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/v3_targets_page1.json
--rw-r--r--   0        0        0     3359 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/v3_targets_page2.json
--rw-r--r--   0        0        0     3339 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_data/v3_targets_page3.json
--rw-r--r--   0        0        0      460 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_manager.py
--rw-r--r--   0        0        0    34952 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_models.py
--rw-r--r--   0        0        0      722 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/test_utils.py
--rw-r--r--   0        0        0     1253 2023-01-20 11:42:17.303717 pysnyk-0.9.5/snyk/utils.py
--rw-r--r--   0        0        0    13071 1970-01-01 00:00:00.000000 pysnyk-0.9.5/setup.py
--rw-r--r--   0        0        0    12893 1970-01-01 00:00:00.000000 pysnyk-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-07-31 08:05:18.373277 pysnyk-0.9.7/LICENSE
+-rw-r--r--   0        0        0    11993 2023-07-31 08:05:18.373277 pysnyk-0.9.7/README.md
+-rw-r--r--   0        0        0      913 2023-07-31 08:05:18.373277 pysnyk-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0      679 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/__version__.py
+-rw-r--r--   0        0        0     8969 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/client.py
+-rw-r--r--   0        0        0      655 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/errors.py
+-rw-r--r--   0        0        0    17705 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/managers.py
+-rw-r--r--   0        0        0    24867 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/models.py
+-rw-r--r--   0        0        0    12805 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_client.py
+-rw-r--r--   0        0        0      497 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/organizations.json
+-rw-r--r--   0        0        0     2172 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/projects.json
+-rw-r--r--   0        0        0      397 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_groups.json
+-rw-r--r--   0        0        0     3340 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_targets_page1.json
+-rw-r--r--   0        0        0     3359 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_targets_page2.json
+-rw-r--r--   0        0        0     3339 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/rest_targets_page3.json
+-rw-r--r--   0        0        0      397 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_groups.json
+-rw-r--r--   0        0        0     3340 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_targets_page1.json
+-rw-r--r--   0        0        0     3359 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_targets_page2.json
+-rw-r--r--   0        0        0     3339 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_data/v3_targets_page3.json
+-rw-r--r--   0        0        0      460 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_manager.py
+-rw-r--r--   0        0        0    34583 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_models.py
+-rw-r--r--   0        0        0      722 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/test_utils.py
+-rw-r--r--   0        0        0     1253 2023-07-31 08:05:18.373277 pysnyk-0.9.7/snyk/utils.py
+-rw-r--r--   0        0        0    12893 1970-01-01 00:00:00.000000 pysnyk-0.9.7/PKG-INFO
```

### Comparing `pysnyk-0.9.5/LICENSE` & `pysnyk-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/README.md` & `pysnyk-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/pyproject.toml` & `pysnyk-0.9.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnyk"
-version = "0.9.5"
+version = "0.9.7"
 description = "A Python client for the Snyk API"
 authors = [
   "Gareth Rushgrove <garethr@snyk.io>",
 ]
 license = "MIT"
 packages = [
   { include = "snyk" },
```

### Comparing `pysnyk-0.9.5/snyk/__init__.py` & `pysnyk-0.9.7/snyk/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/client.py` & `pysnyk-0.9.7/snyk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from .models import Organization, Project
 from .utils import cleanup_path
 
 logger = logging.getLogger(__name__)
 
 
 class SnykClient(object):
-    API_URL = "https://snyk.io/api/v1"
+    API_URL = "https://api.snyk.io/v1"
+    REST_API_URL = "https://api.snyk.io/rest"
     USER_AGENT = "pysnyk/%s" % __version__
 
     def __init__(
         self,
         token: str,
         url: Optional[str] = None,
         user_agent: Optional[str] = USER_AGENT,
@@ -113,30 +114,41 @@
         if not resp.ok:
             logger.error(resp.text)
             raise SnykHTTPError(resp)
 
         return resp
 
     def get(
-        self, path: str, params: dict = None, version: str = None
+        self,
+        path: str,
+        params: dict = None,
+        version: str = None,
+        exclude_version: bool = False,
     ) -> requests.Response:
         """
         Rest (formerly v3) Compatible Snyk Client, assumes the presence of Version, either set in the client
         or called in this method means that we're talking to a rest API endpoint and will ensure the
         params are encoded properly with the version.
 
         Since certain endpoints can exist only in certain versions, being able to override the
         client version with each GET is necessary
 
         Returns a standard requests Response object
         """
 
         path = cleanup_path(path)
-
-        url = f"{self.api_url}/{path}"
+        if version:
+            # When calling a "next page" link, it fails if a version parameter is appended on to the URL - this is a
+            # workaround to prevent that from happening...
+            if exclude_version:
+                url = f"{self.REST_API_URL}/{path}"
+            else:
+                url = f"{self.REST_API_URL}/{path}?version={version}"
+        else:
+            url = f"{self.api_url}/{path}"
 
         if params or self.version:
 
             if not params:
                 params = {}
 
             # we use the presence of version to determine if we are REST or not
```

### Comparing `pysnyk-0.9.5/snyk/errors.py` & `pysnyk-0.9.7/snyk/errors.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/managers.py` & `pysnyk-0.9.7/snyk/managers.py`

 * *Files 20% similar despite different names*

```diff
@@ -134,39 +134,96 @@
             self.instance.organization.id,
             self.instance.id,
         )
         return bool(self.client.post(path, tag))
 
 
 class ProjectManager(Manager):
-    def _query(self, tags: List[Dict[str, str]] = []):
+    def _rest_to_v1_response_format(self, project):
+        attributes = project.get("attributes", {})
+        settings = attributes.get("settings", {})
+        recurring_tests = settings.get("recurring_tests", {})
+        issue_counts = project.get("meta", {}).get("latest_issue_counts")
+
+        return {
+            "name": attributes.get("name"),
+            "id": project.get("id"),
+            "created": attributes.get("created"),
+            "origin": attributes.get("origin"),
+            "type": attributes.get("type"),
+            "readOnly": attributes.get("read_only"),
+            "testFrequency": recurring_tests.get("frequency"),
+            "isMonitored": True
+            if project.get("meta", {}).get("cli_monitored_at")
+            else False,
+            "issueCountsBySeverity": {
+                "low": issue_counts.get("low"),
+                "medium": issue_counts.get("medium"),
+                "high": issue_counts.get("high"),
+                "critical": issue_counts.get("critical"),
+            },
+            "targetReference": attributes.get("target_reference"),
+            "_tags": attributes.get("tags", []),
+            "importingUserId": project.get("relationships", {})
+            .get("importer", {})
+            .get("data", {})
+            .get("id"),
+            "owningUserId": project.get("relationships", {})
+            .get("owner", {})
+            .get("data", {})
+            .get("id"),
+        }
+
+    def _query(self, tags: List[Dict[str, str]] = [], next_url: str = None):
         projects = []
+        params = {}
         if self.instance:
-            path = "org/%s/projects" % self.instance.id
+            path = "/orgs/%s/projects" % self.instance.id if not next_url else next_url
+
+            # Append to params if we've got tags
             if tags:
                 for tag in tags:
                     if "key" not in tag or "value" not in tag or len(tag.keys()) != 2:
                         raise SnykError("Each tag must contain only a key and a value")
-                data = {"filters": {"tags": {"includes": tags}}}
-                resp = self.client.post(path, data)
-            else:
-                resp = self.client.get(path)
-            if "projects" in resp.json():
-                for project_data in resp.json()["projects"]:
+                data = [f'{d["key"]}:{d["value"]}' for d in tags]
+                params["tags"] = ",".join(data)
+
+            # Append the issue count param to the params if this is the first page
+            if not next_url:
+                params["meta.latest_issue_counts"] = "true"
+
+            # And lastly, make the API call
+            resp = self.client.get(
+                path,
+                version="2023-06-19",
+                params=params,
+                exclude_version=True if next_url else False,
+            )
+
+            if "data" in resp.json():
+                # Process projects in current response
+                for response_data in resp.json()["data"]:
+                    project_data = self._rest_to_v1_response_format(response_data)
                     project_data["organization"] = self.instance.to_dict()
-                    # We move tags to _tags as a cache, to avoid the need for additional requests
-                    # when working with tags. We want tags to be the manager
                     try:
-                        project_data["_tags"] = project_data["tags"]
-                        del project_data["tags"]
+                        project_data["attributes"]["_tags"] = project_data[
+                            "attributes"
+                        ]["tags"]
+                        del project_data["attributes"]["tags"]
                     except KeyError:
                         pass
-                    if project_data["totalDependencies"] is None:
+                    if not project_data.get("totalDependencies"):
                         project_data["totalDependencies"] = 0
                     projects.append(self.klass.from_dict(project_data))
+
+                # If we have another page, then process this page too
+                if "next" in resp.json().get("links", {}):
+                    next_url = resp.json().get("links", {})["next"]
+                    projects.extend(self._query(tags, next_url))
+
             for x in projects:
                 x.organization = self.instance
         else:
             for org in self.client.organizations.all():
                 projects.extend(org.projects.all())
         return projects
 
@@ -188,14 +245,16 @@
             # We move tags to _tags as a cache, to avoid the need for additional requests
             # when working with tags. We want tags to be the manager
             try:
                 project_data["_tags"] = project_data["tags"]
                 del project_data["tags"]
             except KeyError:
                 pass
+            if project_data.get("totalDependencies") is None:
+                project_data["totalDependencies"] = 0
             project_klass = self.klass.from_dict(project_data)
             project_klass.organization = self.instance
             return project_klass
         else:
             return super().get(id)
```

### Comparing `pysnyk-0.9.5/snyk/models.py` & `pysnyk-0.9.7/snyk/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+import re
 from dataclasses import InitVar, dataclass, field
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 from deprecation import deprecated  # type: ignore
 from mashumaro.mixins.json import DataClassJSONMixin  # type: ignore
 
@@ -558,39 +559,40 @@
     isDeprecated: Optional[bool] = None
     type: Optional[str] = None
     deprecatedVersions: Optional[List[Any]] = field(default_factory=list)
     dependenciesWithIssues: Optional[List[Any]] = field(default_factory=list)
 
 
 @dataclass
+class User(DataClassJSONMixin):
+    id: str
+    name: str
+    username: str
+    email: str
+
+
+@dataclass
 class Project(DataClassJSONMixin):
     name: str
     organization: Organization
     id: str
     created: str
     origin: str
     type: str
     readOnly: bool
     testFrequency: str
-    totalDependencies: int
-    lastTestedDate: str
-    browseUrl: str
     isMonitored: bool
     issueCountsBySeverity: IssueCounts
-    imageTag: Optional[str] = None
-    imageId: Optional[str] = None
-    imageBaseImage: Optional[str] = None
-    imagePlatform: Optional[str] = None
-    imageCluster: Optional[str] = None
+    importingUserId: Optional[str] = None
+    owningUserId: Optional[str] = None
     hostname: Optional[str] = None
     remoteRepoUrl: Optional[str] = None
     branch: Optional[str] = None
     attributes: Optional[Dict[str, List[str]]] = None
     _tags: Optional[List[Any]] = field(default_factory=list)
-    remediation: Optional[Dict[Any, Any]] = field(default_factory=dict)
 
     def delete(self) -> bool:
         path = "org/%s/project/%s" % (self.organization.id, self.id)
 
         if self.organization.client is None:
             raise SnykError
 
@@ -618,14 +620,87 @@
         payload = {"targetOrgId": new_org_id}
 
         if self.organization.client is None:
             raise SnykError
 
         return bool(self.organization.client.put(path, payload))
 
+    def _get_project_snapshot(self):
+        """
+        Gets the latest project snapshot
+        """
+        project_snapshot_result = self.organization.client.post(
+            f"org/{self.organization.id}/project/{self.id}/history?perPage=1&page=1",
+            {},
+        )
+        return project_snapshot_result.json().get("snapshots", [{}])[0]
+
+    def __getattr__(self, item):
+        """
+        Will handle lazy loading of attributes which require further API calls or are computationally expensive. This
+        avoids having to load them when we retrieve the full list from the API.
+        """
+        # These attributes require us to get the latest snapshot
+        if item in [
+            "totalDependencies",
+            "lastTestedDate",
+            "imageId",
+            "imageTag",
+            "imageBaseImage",
+            "imagePlatform",
+        ]:
+            snapshot = self._get_project_snapshot()
+            if item == "totalDependencies":
+                return snapshot.get("totalDependencies", 0)
+            elif item == "lastTestedDate":
+                return snapshot.get("created")
+            elif item == "imageId":
+                return snapshot.get("imageId")
+            elif item == "imageTag":
+                return snapshot.get("imageTag")
+            elif item == "imageBaseImage":
+                return snapshot.get("baseImageName")
+            elif item == "imagePlatform":
+                return snapshot.get("imagePlatform")
+        # These attributes require us to call the user API to get a users details
+        elif item in ["importingUser", "owner"]:
+            if item == "importingUser":
+                selected_user = self.importingUserId
+            else:
+                selected_user = self.owningUserId
+            user_response = self.organization.client.get(
+                f"orgs/{self.organization.id}/users/{selected_user}",
+                version="2023-05-29~beta",
+            )
+            user = user_response.json()
+            user_data = user.get("data", {})
+            user_attributes = user_data.get("attributes", {})
+            return User(
+                id=self.importingUserId,
+                name=user_attributes.get("name"),
+                username=user_attributes.get("username"),
+                email=user_attributes.get("email"),
+            )
+        elif item == "browseUrl":
+            # Ensure that our browse URL matches the tenant the user is making a request to
+            tenant_matches = match = re.match(
+                r"^https://api\.(.*?)\.snyk\.io", self.organization.client.api_url
+            )
+            if tenant_matches:
+                # If a tenant is found, insert it into the URL
+                url_prefix = f"https://app.{match.group(1)}.snyk.io"
+            else:
+                # If no tenant is found, use a default URL
+                url_prefix = "https://app.snyk.io"
+            return f"{url_prefix}/org/{self.organization.slug}/project/{self.id}"
+        else:
+            raise AttributeError(
+                f"'{type(self).__name__}' object has no attribute '{item}'"
+            )
+
     @property
     def settings(self) -> Manager:
         return Manager.factory("Setting", self.organization.client, self)
 
     @property
     def ignores(self) -> Manager:
         return Manager.factory("Ignore", self.organization.client, self)
```

### Comparing `pysnyk-0.9.5/snyk/test_client.py` & `pysnyk-0.9.7/snyk/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 class TestSnykClient(object):
     @pytest.fixture
     def client(self):
         return SnykClient("token")
 
     def test_default_api_url(self, client):
-        assert client.api_url == "https://snyk.io/api/v1"
+        assert client.api_url == "https://api.snyk.io/v1"
 
     def test_overriding_api_url(self):
-        url = "https://notsnyk.io/api/v1"
+        url = "https://api.notsnyk.io/v1"
         client = SnykClient("token", url)
         assert client.api_url == url
 
     def test_token_added_to_headers(self, client):
         assert client.api_headers["Authorization"] == "token token"
 
     def test_user_agent_added_to_headers(self, client):
@@ -47,164 +47,164 @@
     def test_token_added_to_post_headers(self, client):
         assert client.api_post_headers["Authorization"] == "token token"
 
     def test_post_headers_use_correct_mimetype(self, client):
         assert client.api_post_headers["Content-Type"] == "application/json"
 
     def test_get_sends_request_to_snyk(self, requests_mock, client):
-        requests_mock.get("https://snyk.io/api/v1/sample", text="pong")
+        requests_mock.get("https://api.snyk.io/v1/sample", text="pong")
         assert client.get("sample")
 
     def test_put_sends_request_to_snyk(self, requests_mock, client):
-        requests_mock.put("https://snyk.io/api/v1/sample", text="pong")
+        requests_mock.put("https://api.snyk.io/v1/sample", text="pong")
         assert client.put("sample", {})
 
     def test_delete_sends_request_to_snyk(self, requests_mock, client):
-        requests_mock.delete("https://snyk.io/api/v1/sample")
+        requests_mock.delete("https://api.snyk.io/v1/sample")
         assert client.delete("sample")
 
     def test_post_sends_request_to_snyk(self, requests_mock, client):
-        requests_mock.post("https://snyk.io/api/v1/sample")
+        requests_mock.post("https://api.snyk.io/v1/sample")
         assert client.post("sample", {})
         assert requests_mock.call_count == 1
 
     def test_post_raises_error(self, requests_mock, client):
-        requests_mock.post("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.post("https://api.snyk.io/v1/sample", status_code=500, json={})
         with pytest.raises(SnykError):
             client.post("sample", {})
         assert requests_mock.call_count == 1
 
     def test_put_retries_and_raises_error(self, requests_mock, client):
-        requests_mock.put("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.put("https://api.snyk.io/v1/sample", status_code=500, json={})
         client = SnykClient("token", tries=4, delay=0, backoff=2)
         with pytest.raises(SnykError):
             client.put("sample", {})
         assert requests_mock.call_count == 4
 
     def test_delete_retries_and_raises_error(self, requests_mock, client):
-        requests_mock.delete("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.delete("https://api.snyk.io/v1/sample", status_code=500, json={})
         client = SnykClient("token", tries=4, delay=0, backoff=2)
         with pytest.raises(SnykError):
             client.delete("sample")
         assert requests_mock.call_count == 4
 
     def test_get_retries_and_raises_error(self, requests_mock, client):
-        requests_mock.get("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.get("https://api.snyk.io/v1/sample", status_code=500, json={})
         client = SnykClient("token", tries=4, delay=0, backoff=2)
         with pytest.raises(SnykError):
             client.get("sample")
         assert requests_mock.call_count == 4
 
     def test_post_retries_and_raises_error(self, requests_mock, client):
-        requests_mock.post("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.post("https://api.snyk.io/v1/sample", status_code=500, json={})
         client = SnykClient("token", tries=4, delay=0, backoff=2)
         with pytest.raises(SnykError):
             client.post("sample", {})
         assert requests_mock.call_count == 4
 
     def test_put_raises_error(self, requests_mock, client):
-        requests_mock.put("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.put("https://api.snyk.io/v1/sample", status_code=500, json={})
         with pytest.raises(SnykError):
             client.put("sample", {})
         assert requests_mock.call_count == 1
 
     def test_delete_raises_error(self, requests_mock, client):
-        requests_mock.delete("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.delete("https://api.snyk.io/v1/sample", status_code=500, json={})
         with pytest.raises(SnykError):
             client.delete("sample")
         assert requests_mock.call_count == 1
 
     def test_get_raises_error(self, requests_mock, client):
-        requests_mock.get("https://snyk.io/api/v1/sample", status_code=500, json={})
+        requests_mock.get("https://api.snyk.io/v1/sample", status_code=500, json={})
         with pytest.raises(SnykError):
             client.get("sample")
         assert requests_mock.call_count == 1
 
     def test_empty_organizations(self, requests_mock, client):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json={})
+        requests_mock.get("https://api.snyk.io/v1/orgs", json={})
         assert [] == client.organizations.all()
 
     @pytest.fixture
     def organizations(self):
         return load_test_data(TEST_DATA, "organizations")
 
     @pytest.fixture
     def projects(self):
         return load_test_data(TEST_DATA, "projects")
 
     def test_loads_organizations(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         assert len(client.organizations.all()) == 2
 
     def test_first_organizations(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         org = client.organizations.first()
         assert "defaultOrg" == org.name
 
     def test_first_organizations_on_empty(self, requests_mock, client):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json={})
+        requests_mock.get("https://api.snyk.io/v1/orgs", json={})
         with pytest.raises(SnykNotFoundError):
             client.organizations.first()
 
     def test_filter_organizations(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         assert 1 == len(client.organizations.filter(name="defaultOrg"))
 
     def test_filter_organizations_empty(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         assert [] == client.organizations.filter(name="not present")
 
     def test_loads_organization(self, requests_mock, client, organizations):
         key = organizations["orgs"][0]["id"]
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         org = client.organizations.get(key)
         assert "defaultOrg" == org.name
 
     def test_non_existent_organization(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         with pytest.raises(SnykNotFoundError):
             client.organizations.get("not-present")
 
     def test_organization_type(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         assert all(type(x) is Organization for x in client.organizations.all())
 
     def test_organization_attributes(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         assert client.organizations.first().name == "defaultOrg"
 
     def test_organization_load_group(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
         assert client.organizations.all()[1].group.name == "ACME Inc."
 
     def test_empty_projects(self, requests_mock, client, organizations):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
-        matcher = re.compile("projects$")
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
+        matcher = re.compile("projects.*$")
         requests_mock.get(matcher, json={})
         assert [] == client.projects.all()
 
     def test_projects(self, requests_mock, client, organizations, projects):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
-        matcher = re.compile("projects$")
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
+        matcher = re.compile("projects.*$")
         requests_mock.get(matcher, json=projects)
         assert len(client.projects.all()) == 2
         assert all(type(x) is Project for x in client.projects.all())
 
     def test_project(self, requests_mock, client, organizations, projects):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
-        matcher = re.compile("projects$")
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
+        matcher = re.compile("projects.*$")
         requests_mock.get(matcher, json=projects)
         assert (
-            "atokeneduser/goof"
-            == client.projects.get("6d5813be-7e6d-4ab8-80c2-1e3e2a454545").name
+            "testing-new-name"
+            == client.projects.get("f9fec29a-d288-40d9-a019-cedf825e6efb").name
         )
 
     def test_non_existent_project(self, requests_mock, client, organizations, projects):
-        requests_mock.get("https://snyk.io/api/v1/orgs", json=organizations)
-        matcher = re.compile("projects$")
+        requests_mock.get("https://api.snyk.io/v1/orgs", json=organizations)
+        matcher = re.compile("projects.*$")
         requests_mock.get(matcher, json=projects)
         with pytest.raises(SnykNotFoundError):
             client.projects.get("not-present")
 
     @pytest.fixture
     def rest_client(self):
         return SnykClient(
```

### Comparing `pysnyk-0.9.5/snyk/test_data/rest_targets_page1.json` & `pysnyk-0.9.7/snyk/test_data/rest_targets_page1.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/test_data/rest_targets_page2.json` & `pysnyk-0.9.7/snyk/test_data/rest_targets_page2.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/test_data/rest_targets_page3.json` & `pysnyk-0.9.7/snyk/test_data/rest_targets_page3.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/test_data/v3_targets_page1.json` & `pysnyk-0.9.7/snyk/test_data/v3_targets_page1.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/test_data/v3_targets_page2.json` & `pysnyk-0.9.7/snyk/test_data/v3_targets_page2.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/test_data/v3_targets_page3.json` & `pysnyk-0.9.7/snyk/test_data/v3_targets_page3.json`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/test_models.py` & `pysnyk-0.9.7/snyk/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             url="https://api.snyk.io/org/my-other-org",
         )
         org.client = SnykClient("token")
         return org
 
     @pytest.fixture
     def base_url(self):
-        return "https://snyk.io/api/v1"
+        return "https://api.snyk.io/v1"
 
     @pytest.fixture
     def organization_url(self, base_url, organization):
         return "%s/org/%s" % (base_url, organization.id)
 
 
 class TestOrganization(TestModels):
@@ -42,23 +42,20 @@
             "id": "6d5813be-7e6d-4ab8-80c2-1e3e2a454545",
             "created": "2018-10-29T09:50:54.014Z",
             "origin": "cli",
             "type": "npm",
             "readOnly": "false",
             "testFrequency": "daily",
             "isMonitored": "true",
-            "totalDependencies": 438,
             "issueCountsBySeverity": {
                 "critical": 1,
                 "low": 8,
                 "high": 13,
                 "medium": 15,
             },
-            "lastTestedDate": "2019-02-05T06:21:00.000Z",
-            "browseUrl": "https://app.snyk.io/org/pysnyk-test-org/project/6d5813be-7e6d-4ab8-80c2-1e3e2a454545",
             "tags": [{"key": "some-key", "value": "some-value"}],
         }
 
     @pytest.fixture
     def blank_test(self):
         return {
             "ok": True,
@@ -307,30 +304,31 @@
         with pytest.raises(SnykError):
             organization.projects.filter(
                 tags=[{"key": "some-key", "value": "some-value", "extra": "extra"}]
             )
 
     def test_filter_projects_by_tag(self, organization, requests_mock):
         tags = [{"key": "some-key", "value": "some-value"}]
-        projects_matcher = re.compile("projects$")
+        projects_matcher = re.compile("projects.*$")
         requests_mock.post(projects_matcher, json=[])
+        requests_mock.get(projects_matcher, json=[])
         organization.projects.filter(tags=tags)
-        payload = requests_mock.last_request.json()
-        assert payload == {"filters": {"tags": {"includes": tags}}}
+        assert requests_mock.called
 
     def test_filter_projects_not_by_tag(self, organization, requests_mock):
-        projects_matcher = re.compile("projects$")
+        projects_matcher = re.compile("projects.*$")
         requests_mock.get(projects_matcher, json=[])
         assert organization.projects.filter() == []
 
     def test_tags_cache(self, organization, project, requests_mock):
-        projects_matcher = re.compile("projects$")
-        requests_mock.get(projects_matcher, json={"projects": [project]})
-        projects = organization.projects.all()
-        assert projects[0]._tags == [{"key": "some-key", "value": "some-value"}]
+        matcher = re.compile("project/6d5813be-7e6d-4ab8-80c2-1e3e2a454545$")
+        requests_mock.get(matcher, json=project)
+        assert organization.projects.get(
+            "6d5813be-7e6d-4ab8-80c2-1e3e2a454545"
+        )._tags == [{"key": "some-key", "value": "some-value"}]
 
     def test_get_organization_project_has_tags(
         self, organization, project, requests_mock
     ):
         matcher = re.compile("project/6d5813be-7e6d-4ab8-80c2-1e3e2a454545$")
         requests_mock.get(matcher, json=project)
         assert organization.projects.get(
@@ -346,18 +344,15 @@
             id="6d5813be-7e6d-4ab8-80c2-1e3e2a454545",
             created="2018-10-29T09:50:54.014Z",
             origin="cli",
             type="npm",
             readOnly="false",
             isMonitored="true",
             testFrequency="daily",
-            totalDependencies=438,
             issueCountsBySeverity={"critical": 1, "low": 8, "high": 13, "medium": 15},
-            lastTestedDate="2019-02-05T06:21:00.000Z",
-            browseUrl="https://app.snyk.io/org/pysnyk-test-org/project/6d5813be-7e6d-4ab8-80c2-1e3e2a454545",
             organization=organization,
         )
 
     @pytest.fixture
     def project_url(self, organization_url, project):
         return "%s/project/%s" % (organization_url, project.id)
 
@@ -525,16 +520,16 @@
                         "pkgName": "ms",
                         "pkgVersions": ["1.0.0"],
                         "issueData": {
                             "id": "npm:ms:20170412",
                             "title": "Regular Expression Denial of Service (ReDoS)",
                             "severity": "low",
                             "originalSeverity": "high",
-                            "url": "https://snyk.io/vuln/npm:ms:20170412",
-                            "description": "`## Overview\\r\\n[`ms`](https://www.npmjs.com/package/ms) is a tiny millisecond conversion utility.\\r\\n\\r\\nAffected versions of this package are vulnerable to Regular Expression Denial of Service (ReDoS) due to an incomplete fix for previously reported vulnerability [npm:ms:20151024](https://snyk.io/vuln/npm:ms:20151024). The fix limited the length of accepted input string to 10,000 characters, and turned to be insufficient making it possible to block the event loop for 0.3 seconds (on a typical laptop) with a specially crafted string passed to `ms",
+                            "url": "https://security.snyk.io/vuln/npm:ms:20170412",
+                            "description": "`## Overview\\r\\n[`ms`](https://www.npmjs.com/package/ms) is a tiny millisecond conversion utility.\\r\\n\\r\\nAffected versions of this package are vulnerable to Regular Expression Denial of Service (ReDoS) due to an incomplete fix for previously reported vulnerability [npm:ms:20151024](https://security.snyk.io/vuln/npm:ms:20151024). The fix limited the length of accepted input string to 10,000 characters, and turned to be insufficient making it possible to block the event loop for 0.3 seconds (on a typical laptop) with a specially crafted string passed to `ms",
                             "identifiers": {"CVE": [], "CWE": ["CWE-400"], "OSVDB": []},
                             "credit": ["Snyk Security Research Team"],
                             "exploitMaturity": "no-known-exploit",
                             "semver": {
                                 "vulnerable": ">=0.7.1 <2.0.0",
                                 "unaffected": "",
                             },
@@ -613,17 +608,17 @@
                 "total": 1,
             },
         )
 
         expected = [
             Vulnerability(
                 id="npm:ms:20170412",
-                url="https://snyk.io/vuln/npm:ms:20170412",
+                url="https://security.snyk.io/vuln/npm:ms:20170412",
                 title="Regular Expression Denial of Service (ReDoS)",
-                description="`## Overview\\r\\n[`ms`](https://www.npmjs.com/package/ms) is a tiny millisecond conversion utility.\\r\\n\\r\\nAffected versions of this package are vulnerable to Regular Expression Denial of Service (ReDoS) due to an incomplete fix for previously reported vulnerability [npm:ms:20151024](https://snyk.io/vuln/npm:ms:20151024). The fix limited the length of accepted input string to 10,000 characters, and turned to be insufficient making it possible to block the event loop for 0.3 seconds (on a typical laptop) with a specially crafted string passed to `ms",
+                description="`## Overview\\r\\n[`ms`](https://www.npmjs.com/package/ms) is a tiny millisecond conversion utility.\\r\\n\\r\\nAffected versions of this package are vulnerable to Regular Expression Denial of Service (ReDoS) due to an incomplete fix for previously reported vulnerability [npm:ms:20151024](https://security.snyk.io/vuln/npm:ms:20151024). The fix limited the length of accepted input string to 10,000 characters, and turned to be insufficient making it possible to block the event loop for 0.3 seconds (on a typical laptop) with a specially crafted string passed to `ms",
                 upgradePath=[
                     "tap@11.1.5",
                     "nyc@11.9.0",
                     "istanbul-lib-instrument@1.10.1",
                     "babel-template@6.26.0",
                     "lodash@4.17.10",
                 ],
```

### Comparing `pysnyk-0.9.5/snyk/test_utils.py` & `pysnyk-0.9.7/snyk/test_utils.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/snyk/utils.py` & `pysnyk-0.9.7/snyk/utils.py`

 * *Files identical despite different names*

### Comparing `pysnyk-0.9.5/setup.py` & `pysnyk-0.9.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,301 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pysnyk
+Version: 0.9.7
+Summary: A Python client for the Snyk API
+Home-page: https://github.com/snyk-labs/pysnyk
+License: MIT
+Author: Gareth Rushgrove
+Author-email: garethr@snyk.io
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: importlib_metadata (>=4.11.2,<5.0.0)
+Requires-Dist: mashumaro (>=3,<4)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: retry (>=0.9.2,<0.10.0)
+Project-URL: Repository, https://github.com/snyk-labs/pysnyk
+Description-Content-Type: text/markdown
 
-packages = \
-['snyk']
+# pysnyk
 
-package_data = \
-{'': ['*'], 'snyk': ['test_data/*']}
 
-install_requires = \
-['deprecation>=2.1.0,<3.0.0',
- 'importlib_metadata>=4.11.2,<5.0.0',
- 'mashumaro>=3,<4',
- 'requests>=2.27.1,<3.0.0',
- 'retry>=0.9.2,<0.10.0']
-
-setup_kwargs = {
-    'name': 'pysnyk',
-    'version': '0.9.5',
-    'description': 'A Python client for the Snyk API',
-    'long_description': '# pysnyk\n\n\n[![Build status](https://github.com/snyk-labs/pysnyk/actions/workflows/test.yml/badge.svg)](https://github.com/snyk-labs/pysnyk/actions/workflows/test.yml)\n\n\nA Python client for the [Snyk API](https://snyk.docs.apiary.io/#).\n\n## Client\n\nUsing the client requires you to provide your Snyk API token.\n\n```python\nimport snyk\nclient = snyk.SnykClient("<your-api-token>")\n```\n\nBy default the client will connect to the public Snyk service. If you are using a local installation then you can provide the API url as the second argument.\n\n```python\nimport snyk\nclient = snyk.SnykClient("<your-api-token>", "<your-instance-of-snyk>")\n```\n\nBy default the `User-Agent` string for the API requests will be `pysnyk/<version>`. If you would like to send a custom user agent you can do so as follows:\n\n```python\nimport snyk\nclient = snyk.SnykClient("<your-api-token>", user_agent="<your-instance-of-snyk>")\n```\n\nBy default the requests are not retried. If you would like to retry failed requests with `backoff` and `delay` you can do so as follows:\n\n```python\nimport snyk\nclient = snyk.SnykClient("<your-api-token>", tries=4, delay=1, backoff=2)\n```\n\n- `tries` - the maximum number of attempts. **Default:** `1` (no retries)\n- `delay` - initial delay between attempts. **Default:** `1`\n- `backoff` - multiplier applied to delay between attempts. **Default:** `2`\n- `debug` - run client in debug mode, useful for debugging API requests. **Default:** `False`\n\n## Organizations\n\nWith the client we can get a list of Snyk organizations you are a member of:\n\n```python\nclient.organizations.all()\n```\n\nThis returns a list of `snyk.models.Organization` objects.\n\nIf you already have the ID of the organization you\'re after you can grab it directly:\n\n```python\nclient.organizations.get("<organization-id>")\n```\n\nThis will return a single `snyk.models.Organization` object.\n\nMost of the API is scoped to organizations, so most other methods are found on the `snyk.models.Organization` objects returned by these two methods.\n\nThe `snyk.models.Organization` object has the following properties related to the API:\n\n- `entitlements` - returns the set of Snyk features available to this account\n- `dependencies`- returns a Manager for packages in use in this organization\n- `licenses` - returns a Manager for licenses currently in use by projects in this organisation\n- `members` - returns a Manager for members\n- `projects` - returns a Manager for associated projects\n- `integrations` - returns a Manager for active integrations\n\n### A note on Managers\n\nManagers provide a consistent API for accessing objects from the Snyk API. Each manager implements the following methods:\n\n- `all()` - return a list of all of the relevant objects\n- `get("<id>")` - return a single instance of the object if it exists\n- `first()` - grab the first instance of the object if one exists\n- `filter(<key>="<value>")` - return a list filtered by one or more key/value pairs\n\n### Projects\n\nOnce you have an organization you\'re likely to want to grab the related projects:\n\n```python\nclient.organizations.first().projects.all()\n```\n\nThis will return a list of `snyk.models.Project` objects.\n\nIn the case where you want to get all of the projects across all of your organizations then you can use the handy method on the client.\n\n```python\nclient.projects.all()\n```\n\nThe `snyk.models.Project` object has the following useful properties and methods:\n\n- `delete()` - deletes the project in question. Be careful as this will delete all associated data too\n- `move(new_org_id)` - moves the project to a new organization\n- `dependencies` - returns a Manager for packages in use in this project\n- `dependency_graph` - returns a `snyk.models.DependencyGraph` object which represents the full dependency graph of package dependencies\n- `ignores` - returns a Manager for ignore rules set on the project\n- `vulnerabilities` - returns a list of `snyk.models.Vulnerability` objects with information about vulnerabilities in this project\n- `jira_issues` - returns a Manager with access to any associated Jira issues\n- `licenses` - returns a Manager for licenses currently in use by this project\n- `settings` - returns a Manager for interacting with the current project settings\n- `tags` - returns a Manager for interacting with the current project tags\n\nYou can add and delete tags using the manager:\n\n- `tags.add(key, value)` - adds a tag with the provided key/value pair to the project\n- `tags.delete(key, value)` - deletes a tag with the provided key/value pair from the project\n\nIn the case of Projects, as well as filtering by properties (as mentioned above) you can also filter by tag:\n\n```python\nclient.organizations.first().projects.filter(tags = [{"key": "some-key", "value": "some-value"}])\n```\n\nNote that the `settings` Manager can also be used to update settings like so, assuming you have a `snyk.models.Project` object in the variable `project`.\n\n```python\nproject.settings.update(pull_request_test_enabled=True)\n```\n\n### Importing new projects\n\nThe client supports a high-level `import_project` method on organizations for adding new projects to be monitored by Snyk.\n\n```python\norg = client.organizations.first()\norg.import_project("github.com/user/project@branch")\norg.import_project("docker.io/repository:tag")\n```\n\nIf you are targetting a specific manifest file or files you can pass those as an optional argument, for instance:\n\n```python\norg.import_project("github.com/user/project@branch", files=["Gemfile.lock"])\n```\n\nThis method currently only supports importing projects from GitHub and Docker Hub. For other integrations you will need to grab the lower-level `snyk.models.Integration` object from the `snyk.models.Organization.integrations` manager noted above. Other services will be added to this API soon.\n\n### Testing for vulnerabilities\n\nThe API also exposes methods to discover vulnerability information about individual packages. These methods are found on the Organization object.\n\n- `test_maven(<package_group_id>, <package_artifact_id>, <version>)` - returns an IssueSet containing vulnerability information for a Maven artifact\n- `test_rubygem(<name>, <version>)` - returns an IssueSet containing vulnerability information for a Ruby Gem\n- `test_python(<name>, <version>)` - returns an IssueSet containing vulnerability information for Python package from PyPi\n- `test_npm(<name>, <version>)` - returns an IssueSet containing vulnerability information for an NPM package\n\nHere\'s an example of checking a particular Python package.\n\n```python\n>>> org = client.organizations.first()\n>>> result = org.test_python("flask", "0.12.2")\n>>> assert result.ok\nFalse\n# You can access details of the vulnerabilities too, for example\n>>> result.issues.vulnerabilities[0].title\n\'Improper Input Validation\'\n>>> result.issues.vulnerabilities[0].identifiers\n{\'CVE\': [\'CVE-2018-1000656\'], \'CWE\': [\'CWE-20\']\n```\n\nAs well as testing individual packages you can also test all packages found in various dependency management manifests. The client currently supports the following methods:\n\n- `test_pipfile(<file-handle-or-string>)` - returns an IssueSet for all Python dependencies in a `Pipfile`\n- `test_gemfilelock(<file-handle-or-string>)` - returns an IssueSet for all Ruby dependencies in a `Gemfile`\n- `test_packagejson(<file-handle-or-string>, (<lock-file-handle-or-string>))` - returns an IssueSet for all Javascript dependencies in a `package.json` file. Optionally takes a `package.lock` file\n- `test_gradlefile(<file-handle-or-string>)` - returns an IssueSet for all dependencies in a `Gradlefile`\n- `test_sbt(<file-handle-or-string>)` - returns an IssueSet for all dependencies defined in a `.sbt` file\n- `test_pom(<file-handle-or-string>)` - returns an IssueSet for all dependencies in a Maven `pom.xml` file\n- `test_yarn(<file-handle-or-string>, <lock-file-handle-or-string>)` - returns an IssueSet for all dependencies in Yarn `package.json` and `yarn.lock` files\n- `test_composer(<file-handle-or-string>, <lock-file-handle-or-string>)` - returns an IssueSet for all dependencies in Composer `composer.json` and `composer.lock` files\n\nFor example, here we are testing a Python `Pipfile`.\n\n```python\n>>> org = client.organizations.first()\n>>> file = open("Pipfile")\n>>> org.test_pipfile(file)\n```\n\n### Inviting new users\n\nYou can invite new users to the organization via the API.\n\n```python\n>>> org = client.organizations.first()\n>>> org.invite("example@example.com")\n```\n\nYou can also invite new users as administrators:\n\n```python\n>>> org = client.organizations.first()\n>>> org.invite("example@example.com", admin=True)\n```\n\n### Low-level client\n\nAs well as the high-level API of the Snyk client you can use the HTTP methods directly. For these you simply need to pass the path, and optionally a data payload. The full domain, and the authentication details, are already provided by the client.\n\n```python\nclient.get("<path>")\nclient.delete("<path>")\nclient.put("<path>", <data>)\nclient.post("<path>", <data>)\n```\n\nMost of the time you shouldn\'t need to use these. They are mainly useful if new methods are added to the API which are not yet supported in the client. This can also be useful if you want to pass very specific parameters, or to parse the raw JSON output from the API.\n\n## Experimental rest low-level client\n\npysnyk >= 0.9.0 now includes support for basic rest (formerly referred to as v3) compatibility. To switch to use a rest client, pass the rest API url and version when initializing a client. Right now it supports the `GET` method. Refer to the [rest API docs](https://apidocs.snyk.io/) for more information and examples.\n\nGetting the rest information of an organization:\n\n```python\n# To get this value, get it from a Snyk organizations settings page\nsnyk_org = "df734bed-d75c-4f11-bb47-1d119913bcc7"\n\n# to use the rest endpoint you MUST include a version value and the url of the v3 api endpoint as shown below\nrest_client = SnykClient(snyk_token, version="2022-02-16~experimental", url="https://api.snyk.io/rest")\n\nprint(rest_client.get(f"/orgs/{snyk_org}").json())\n\n# this supports overriding rest versions for a specific GET requests:\nuser = rest_client.get(f"orgs/{snyk_org}/users/{snyk_user}", version="2022-02-01~experimental").json()\n\n# pass parameters such as how many results per page\nparams = {"limit": 10}\n\ntargets = rest_client.get(f"orgs/{snyk_org}/targets", params=params)\n```\n\nV1 and rest can work at the same time by instantiating two clients:\n\n```python\nsnyk_org = "df734bed-d75c-4f11-bb47-1d119913bcc7"\n\nv1client = SnykClient(snyk_token)\n\nrest_client = SnykClient(snyk_token, version="2022-02-16~experimental", url="https://api.snyk.io/rest")\n\nv1_org = v1client.organizations.get(snyk_org)\n\nrest_org = rest_client.get(f"/orgs/{snyk_org}").json()\n```\n\nThe rest API introduces consistent pagination across all endpoints. The v3 client includes a helper method `.get_rest_pages` which collects the paginated responses and returns a single list combining the contents of the "data" key from all pages. It takes the same values as the get method.\n\n```python\nrest_client = SnykClient(snyk_token, version="2022-02-16~experimental", url="https://api.snyk.io/rest")\n\nparams = {"limit": 10}\n\ntargets = rest_client.get(f"orgs/{snyk_org}/targets", params=params).json()\n\nprint(len(targets["data"]))\n# returns 10 targets\n\nall_targets = rest_client.get_rest_pages(f"orgs/{snyk_org}/targets", params=params)\n\nprint(len(all_targets))\n# returns 33 targets, note we don\'t have to add .json() to the call or access the "data" key, get_rest_pages does that for us\n\n# Override Content-Type header (or others) as needed for \nresponse = rest_client.post(f"orgs/{snyk_org}/invites", body={"email": "some.body@snyk.io", "role": "f8223479-01a9-4774-8e29-06ce9a0513d6", headers={"Content-Type": "application/vnd.api+json"}})\n```\n\nFor backwards compatibility the get_rest_pages method has an alternative name of get_v3_pages to not break code already rewritten replatformed to the 0.9.0 pysnyk module.\n',
-    'author': 'Gareth Rushgrove',
-    'author_email': 'garethr@snyk.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/snyk-labs/pysnyk',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+[![Build status](https://github.com/snyk-labs/pysnyk/actions/workflows/test.yml/badge.svg)](https://github.com/snyk-labs/pysnyk/actions/workflows/test.yml)
 
 
-setup(**setup_kwargs)
+A Python client for the [Snyk API](https://snyk.docs.apiary.io/#).
+
+## Client
+
+Using the client requires you to provide your Snyk API token.
+
+```python
+import snyk
+client = snyk.SnykClient("<your-api-token>")
+```
+
+By default the client will connect to the public Snyk service. If you are using a local installation then you can provide the API url as the second argument.
+
+```python
+import snyk
+client = snyk.SnykClient("<your-api-token>", "<your-instance-of-snyk>")
+```
+
+By default the `User-Agent` string for the API requests will be `pysnyk/<version>`. If you would like to send a custom user agent you can do so as follows:
+
+```python
+import snyk
+client = snyk.SnykClient("<your-api-token>", user_agent="<your-instance-of-snyk>")
+```
+
+By default the requests are not retried. If you would like to retry failed requests with `backoff` and `delay` you can do so as follows:
+
+```python
+import snyk
+client = snyk.SnykClient("<your-api-token>", tries=4, delay=1, backoff=2)
+```
+
+- `tries` - the maximum number of attempts. **Default:** `1` (no retries)
+- `delay` - initial delay between attempts. **Default:** `1`
+- `backoff` - multiplier applied to delay between attempts. **Default:** `2`
+- `debug` - run client in debug mode, useful for debugging API requests. **Default:** `False`
+
+## Organizations
+
+With the client we can get a list of Snyk organizations you are a member of:
+
+```python
+client.organizations.all()
+```
+
+This returns a list of `snyk.models.Organization` objects.
+
+If you already have the ID of the organization you're after you can grab it directly:
+
+```python
+client.organizations.get("<organization-id>")
+```
+
+This will return a single `snyk.models.Organization` object.
+
+Most of the API is scoped to organizations, so most other methods are found on the `snyk.models.Organization` objects returned by these two methods.
+
+The `snyk.models.Organization` object has the following properties related to the API:
+
+- `entitlements` - returns the set of Snyk features available to this account
+- `dependencies`- returns a Manager for packages in use in this organization
+- `licenses` - returns a Manager for licenses currently in use by projects in this organisation
+- `members` - returns a Manager for members
+- `projects` - returns a Manager for associated projects
+- `integrations` - returns a Manager for active integrations
+
+### A note on Managers
+
+Managers provide a consistent API for accessing objects from the Snyk API. Each manager implements the following methods:
+
+- `all()` - return a list of all of the relevant objects
+- `get("<id>")` - return a single instance of the object if it exists
+- `first()` - grab the first instance of the object if one exists
+- `filter(<key>="<value>")` - return a list filtered by one or more key/value pairs
+
+### Projects
+
+Once you have an organization you're likely to want to grab the related projects:
+
+```python
+client.organizations.first().projects.all()
+```
+
+This will return a list of `snyk.models.Project` objects.
+
+In the case where you want to get all of the projects across all of your organizations then you can use the handy method on the client.
+
+```python
+client.projects.all()
+```
+
+The `snyk.models.Project` object has the following useful properties and methods:
+
+- `delete()` - deletes the project in question. Be careful as this will delete all associated data too
+- `move(new_org_id)` - moves the project to a new organization
+- `dependencies` - returns a Manager for packages in use in this project
+- `dependency_graph` - returns a `snyk.models.DependencyGraph` object which represents the full dependency graph of package dependencies
+- `ignores` - returns a Manager for ignore rules set on the project
+- `vulnerabilities` - returns a list of `snyk.models.Vulnerability` objects with information about vulnerabilities in this project
+- `jira_issues` - returns a Manager with access to any associated Jira issues
+- `licenses` - returns a Manager for licenses currently in use by this project
+- `settings` - returns a Manager for interacting with the current project settings
+- `tags` - returns a Manager for interacting with the current project tags
+
+You can add and delete tags using the manager:
+
+- `tags.add(key, value)` - adds a tag with the provided key/value pair to the project
+- `tags.delete(key, value)` - deletes a tag with the provided key/value pair from the project
+
+In the case of Projects, as well as filtering by properties (as mentioned above) you can also filter by tag:
+
+```python
+client.organizations.first().projects.filter(tags = [{"key": "some-key", "value": "some-value"}])
+```
+
+Note that the `settings` Manager can also be used to update settings like so, assuming you have a `snyk.models.Project` object in the variable `project`.
+
+```python
+project.settings.update(pull_request_test_enabled=True)
+```
+
+### Importing new projects
+
+The client supports a high-level `import_project` method on organizations for adding new projects to be monitored by Snyk.
+
+```python
+org = client.organizations.first()
+org.import_project("github.com/user/project@branch")
+org.import_project("docker.io/repository:tag")
+```
+
+If you are targetting a specific manifest file or files you can pass those as an optional argument, for instance:
+
+```python
+org.import_project("github.com/user/project@branch", files=["Gemfile.lock"])
+```
+
+This method currently only supports importing projects from GitHub and Docker Hub. For other integrations you will need to grab the lower-level `snyk.models.Integration` object from the `snyk.models.Organization.integrations` manager noted above. Other services will be added to this API soon.
+
+### Testing for vulnerabilities
+
+The API also exposes methods to discover vulnerability information about individual packages. These methods are found on the Organization object.
+
+- `test_maven(<package_group_id>, <package_artifact_id>, <version>)` - returns an IssueSet containing vulnerability information for a Maven artifact
+- `test_rubygem(<name>, <version>)` - returns an IssueSet containing vulnerability information for a Ruby Gem
+- `test_python(<name>, <version>)` - returns an IssueSet containing vulnerability information for Python package from PyPi
+- `test_npm(<name>, <version>)` - returns an IssueSet containing vulnerability information for an NPM package
+
+Here's an example of checking a particular Python package.
+
+```python
+>>> org = client.organizations.first()
+>>> result = org.test_python("flask", "0.12.2")
+>>> assert result.ok
+False
+# You can access details of the vulnerabilities too, for example
+>>> result.issues.vulnerabilities[0].title
+'Improper Input Validation'
+>>> result.issues.vulnerabilities[0].identifiers
+{'CVE': ['CVE-2018-1000656'], 'CWE': ['CWE-20']
+```
+
+As well as testing individual packages you can also test all packages found in various dependency management manifests. The client currently supports the following methods:
+
+- `test_pipfile(<file-handle-or-string>)` - returns an IssueSet for all Python dependencies in a `Pipfile`
+- `test_gemfilelock(<file-handle-or-string>)` - returns an IssueSet for all Ruby dependencies in a `Gemfile`
+- `test_packagejson(<file-handle-or-string>, (<lock-file-handle-or-string>))` - returns an IssueSet for all Javascript dependencies in a `package.json` file. Optionally takes a `package.lock` file
+- `test_gradlefile(<file-handle-or-string>)` - returns an IssueSet for all dependencies in a `Gradlefile`
+- `test_sbt(<file-handle-or-string>)` - returns an IssueSet for all dependencies defined in a `.sbt` file
+- `test_pom(<file-handle-or-string>)` - returns an IssueSet for all dependencies in a Maven `pom.xml` file
+- `test_yarn(<file-handle-or-string>, <lock-file-handle-or-string>)` - returns an IssueSet for all dependencies in Yarn `package.json` and `yarn.lock` files
+- `test_composer(<file-handle-or-string>, <lock-file-handle-or-string>)` - returns an IssueSet for all dependencies in Composer `composer.json` and `composer.lock` files
+
+For example, here we are testing a Python `Pipfile`.
+
+```python
+>>> org = client.organizations.first()
+>>> file = open("Pipfile")
+>>> org.test_pipfile(file)
+```
+
+### Inviting new users
+
+You can invite new users to the organization via the API.
+
+```python
+>>> org = client.organizations.first()
+>>> org.invite("example@example.com")
+```
+
+You can also invite new users as administrators:
+
+```python
+>>> org = client.organizations.first()
+>>> org.invite("example@example.com", admin=True)
+```
+
+### Low-level client
+
+As well as the high-level API of the Snyk client you can use the HTTP methods directly. For these you simply need to pass the path, and optionally a data payload. The full domain, and the authentication details, are already provided by the client.
+
+```python
+client.get("<path>")
+client.delete("<path>")
+client.put("<path>", <data>)
+client.post("<path>", <data>)
+```
+
+Most of the time you shouldn't need to use these. They are mainly useful if new methods are added to the API which are not yet supported in the client. This can also be useful if you want to pass very specific parameters, or to parse the raw JSON output from the API.
+
+## Experimental rest low-level client
+
+pysnyk >= 0.9.0 now includes support for basic rest (formerly referred to as v3) compatibility. To switch to use a rest client, pass the rest API url and version when initializing a client. Right now it supports the `GET` method. Refer to the [rest API docs](https://apidocs.snyk.io/) for more information and examples.
+
+Getting the rest information of an organization:
+
+```python
+# To get this value, get it from a Snyk organizations settings page
+snyk_org = "df734bed-d75c-4f11-bb47-1d119913bcc7"
+
+# to use the rest endpoint you MUST include a version value and the url of the v3 api endpoint as shown below
+rest_client = SnykClient(snyk_token, version="2022-02-16~experimental", url="https://api.snyk.io/rest")
+
+print(rest_client.get(f"/orgs/{snyk_org}").json())
+
+# this supports overriding rest versions for a specific GET requests:
+user = rest_client.get(f"orgs/{snyk_org}/users/{snyk_user}", version="2022-02-01~experimental").json()
+
+# pass parameters such as how many results per page
+params = {"limit": 10}
+
+targets = rest_client.get(f"orgs/{snyk_org}/targets", params=params)
+```
+
+V1 and rest can work at the same time by instantiating two clients:
+
+```python
+snyk_org = "df734bed-d75c-4f11-bb47-1d119913bcc7"
+
+v1client = SnykClient(snyk_token)
+
+rest_client = SnykClient(snyk_token, version="2022-02-16~experimental", url="https://api.snyk.io/rest")
+
+v1_org = v1client.organizations.get(snyk_org)
+
+rest_org = rest_client.get(f"/orgs/{snyk_org}").json()
+```
+
+The rest API introduces consistent pagination across all endpoints. The v3 client includes a helper method `.get_rest_pages` which collects the paginated responses and returns a single list combining the contents of the "data" key from all pages. It takes the same values as the get method.
+
+```python
+rest_client = SnykClient(snyk_token, version="2022-02-16~experimental", url="https://api.snyk.io/rest")
+
+params = {"limit": 10}
+
+targets = rest_client.get(f"orgs/{snyk_org}/targets", params=params).json()
+
+print(len(targets["data"]))
+# returns 10 targets
+
+all_targets = rest_client.get_rest_pages(f"orgs/{snyk_org}/targets", params=params)
+
+print(len(all_targets))
+# returns 33 targets, note we don't have to add .json() to the call or access the "data" key, get_rest_pages does that for us
+
+# Override Content-Type header (or others) as needed for 
+response = rest_client.post(f"orgs/{snyk_org}/invites", body={"email": "some.body@snyk.io", "role": "f8223479-01a9-4774-8e29-06ce9a0513d6", headers={"Content-Type": "application/vnd.api+json"}})
+```
+
+For backwards compatibility the get_rest_pages method has an alternative name of get_v3_pages to not break code already rewritten replatformed to the 0.9.0 pysnyk module.
+
```

