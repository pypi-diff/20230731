# Comparing `tmp/boinc_client-1.4.5.tar.gz` & `tmp/boinc_client-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boinc_client-1.4.5.tar", max compression
+gzip compressed data, was "boinc_client-1.4.6.tar", max compression
```

## Comparing `boinc_client-1.4.5.tar` & `boinc_client-1.4.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35148 2023-07-28 13:48:57.509448 boinc_client-1.4.5/LICENSE.md
--rw-r--r--   0        0        0     2273 2023-07-28 13:48:57.509448 boinc_client-1.4.5/README.md
--rw-r--r--   0        0        0      917 2023-07-28 13:49:11.794031 boinc_client-1.4.5/pyproject.toml
--rw-r--r--   0        0        0       28 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/__init__.py
--rw-r--r--   0        0        0     3246 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/boinc_client.py
--rw-r--r--   0        0        0        0 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/clients/__init__.py
--rw-r--r--   0        0        0     2846 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/clients/rpc_client.py
--rw-r--r--   0        0        0     1152 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/messages.py
--rw-r--r--   0        0        0        0 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/__init__.py
--rw-r--r--   0        0        0      735 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/cc_status.py
--rw-r--r--   0        0        0     5195 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/client_state.py
--rw-r--r--   0        0        0      210 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/client_update.py
--rw-r--r--   0        0        0      254 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/client_version.py
--rw-r--r--   0        0        0      532 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/disk_stats.py
--rw-r--r--   0        0        0     1190 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/file_transfer.py
--rw-r--r--   0        0        0      274 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/generic_response.py
--rw-r--r--   0        0        0      852 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/helpers.py
--rw-r--r--   0        0        0     1340 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/host_info.py
--rw-r--r--   0        0        0      118 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/message_count.py
--rw-r--r--   0        0        0      925 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/messages.py
--rw-r--r--   0        0        0     1173 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/network_transfers.py
--rw-r--r--   0        0        0      738 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/old_results.py
--rw-r--r--   0        0        0      294 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/project_attach.py
--rw-r--r--   0        0        0     3364 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/project_status.py
--rw-r--r--   0        0        0     1167 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/projects.py
--rw-r--r--   0        0        0     1326 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/projects_stats.py
--rw-r--r--   0        0        0     1054 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/public_notice.py
--rw-r--r--   0        0        0     2185 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/result.py
--rw-r--r--   0        0        0      382 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/screensaver_tasks.py
--rw-r--r--   0        0        0      612 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/models/simple_gui_info.py
--rw-r--r--   0        0        0     2856 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/projects.py
--rw-r--r--   0        0        0      723 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/results.py
--rw-r--r--   0        0        0      830 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/stats.py
--rw-r--r--   0        0        0     2742 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/status.py
--rw-r--r--   0        0        0      793 2023-07-28 13:48:57.509448 boinc_client-1.4.5/src/boinc_client/versions.py
--rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 boinc_client-1.4.5/setup.py
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 boinc_client-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-31 10:36:23.866632 boinc_client-1.4.6/LICENSE.md
+-rw-r--r--   0        0        0     2273 2023-07-31 10:36:23.866632 boinc_client-1.4.6/README.md
+-rw-r--r--   0        0        0      917 2023-07-31 10:36:35.522584 boinc_client-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/__init__.py
+-rw-r--r--   0        0        0     3246 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/boinc_client.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/clients/__init__.py
+-rw-r--r--   0        0        0     2846 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/clients/rpc_client.py
+-rw-r--r--   0        0        0     1152 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/messages.py
+-rw-r--r--   0        0        0        0 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/cc_status.py
+-rw-r--r--   0        0        0     5195 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/client_state.py
+-rw-r--r--   0        0        0      210 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/client_update.py
+-rw-r--r--   0        0        0      254 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/client_version.py
+-rw-r--r--   0        0        0      532 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/disk_stats.py
+-rw-r--r--   0        0        0     1190 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/file_transfer.py
+-rw-r--r--   0        0        0      274 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/generic_response.py
+-rw-r--r--   0        0        0      852 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/helpers.py
+-rw-r--r--   0        0        0     1340 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/host_info.py
+-rw-r--r--   0        0        0      118 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/message_count.py
+-rw-r--r--   0        0        0      925 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/messages.py
+-rw-r--r--   0        0        0     1173 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/network_transfers.py
+-rw-r--r--   0        0        0      738 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/old_results.py
+-rw-r--r--   0        0        0      294 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/project_attach.py
+-rw-r--r--   0        0        0     3364 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/project_status.py
+-rw-r--r--   0        0        0     1167 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/projects.py
+-rw-r--r--   0        0        0     1326 2023-07-31 10:36:23.866632 boinc_client-1.4.6/src/boinc_client/models/projects_stats.py
+-rw-r--r--   0        0        0     1054 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/models/public_notice.py
+-rw-r--r--   0        0        0     2185 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/models/result.py
+-rw-r--r--   0        0        0      382 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/models/screensaver_tasks.py
+-rw-r--r--   0        0        0      612 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/models/simple_gui_info.py
+-rw-r--r--   0        0        0     2856 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/projects.py
+-rw-r--r--   0        0        0      723 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/results.py
+-rw-r--r--   0        0        0      830 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/stats.py
+-rw-r--r--   0        0        0     2742 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/status.py
+-rw-r--r--   0        0        0      793 2023-07-31 10:36:23.870631 boinc_client-1.4.6/src/boinc_client/versions.py
+-rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 boinc_client-1.4.6/setup.py
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 boinc_client-1.4.6/PKG-INFO
```

### Comparing `boinc_client-1.4.5/LICENSE.md` & `boinc_client-1.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/README.md` & `boinc_client-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/pyproject.toml` & `boinc_client-1.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boinc-client"
-version = "1.4.5"
+version = "1.4.6"
 description = "Python API for interacting with a BOINC client via RPC"
 authors = ["Lewis England <lewis2004@hotmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 homepage = "https://github.com/SplinterHead/boinc-client"
 issues = "https://github.com/SplinterHead/boinc-client/issues"
```

### Comparing `boinc_client-1.4.5/src/boinc_client/boinc_client.py` & `boinc_client-1.4.6/src/boinc_client/boinc_client.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/clients/rpc_client.py` & `boinc_client-1.4.6/src/boinc_client/clients/rpc_client.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/messages.py` & `boinc_client-1.4.6/src/boinc_client/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 def message_count(client: RpcClient) -> dict:
     """Show the largest message seqno."""
     rpc_resp = client.make_request("<get_message_count/>")
     rpc_json = xmltodict.parse(rpc_resp)
     return MessageCount().load(rpc_json)
 
 
-def public_notices(client: RpcClient, start: int = 0) -> dict:
+def public_notices(client: RpcClient, start: int = 1) -> dict:
     """Returns only non-private notices, doesn't require authentication."""
     rpc_resp = client.make_request(
         f"<get_notices_public><seqno>{start}</seqno></get_notices_public>"
     )
     rpc_json = xmltodict.parse(rpc_resp, force_list="notice")
     return Notices().load(rpc_json)
```

### Comparing `boinc_client-1.4.5/src/boinc_client/models/cc_status.py` & `boinc_client-1.4.6/src/boinc_client/models/cc_status.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/client_state.py` & `boinc_client-1.4.6/src/boinc_client/models/client_state.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/disk_stats.py` & `boinc_client-1.4.6/src/boinc_client/models/disk_stats.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/file_transfer.py` & `boinc_client-1.4.6/src/boinc_client/models/file_transfer.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/helpers.py` & `boinc_client-1.4.6/src/boinc_client/models/helpers.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/host_info.py` & `boinc_client-1.4.6/src/boinc_client/models/host_info.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/messages.py` & `boinc_client-1.4.6/src/boinc_client/models/messages.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/network_transfers.py` & `boinc_client-1.4.6/src/boinc_client/models/network_transfers.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/old_results.py` & `boinc_client-1.4.6/src/boinc_client/models/old_results.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/project_status.py` & `boinc_client-1.4.6/src/boinc_client/models/project_status.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/projects.py` & `boinc_client-1.4.6/src/boinc_client/models/projects.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/projects_stats.py` & `boinc_client-1.4.6/src/boinc_client/models/projects_stats.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/public_notice.py` & `boinc_client-1.4.6/src/boinc_client/models/public_notice.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/result.py` & `boinc_client-1.4.6/src/boinc_client/models/result.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/models/simple_gui_info.py` & `boinc_client-1.4.6/src/boinc_client/models/simple_gui_info.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/projects.py` & `boinc_client-1.4.6/src/boinc_client/projects.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/results.py` & `boinc_client-1.4.6/src/boinc_client/results.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/stats.py` & `boinc_client-1.4.6/src/boinc_client/stats.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/status.py` & `boinc_client-1.4.6/src/boinc_client/status.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/src/boinc_client/versions.py` & `boinc_client-1.4.6/src/boinc_client/versions.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.4.5/setup.py` & `boinc_client-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = \
 ['lxml>=4.9.2,<5.0.0',
  'marshmallow>=3.19.0,<4.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'boinc-client',
-    'version': '1.4.5',
+    'version': '1.4.6',
     'description': 'Python API for interacting with a BOINC client via RPC',
     'long_description': '# BOINC Client\n\n![Test and Release](https://github.com/SplinterHead/boinc-client/actions/workflows/test-and-release.yml/badge.svg)\n[![boinc-client](https://snyk.io/advisor/python/boinc-client/badge.svg)](https://snyk.io/advisor/python/boinc-client)\n\nPython native library for interacting with a BOINC client via RPC. This library has been designed to have consistent response types.\n\n## Usage\n\n### Setup\n\n```python\nfrom boinc_client import Boinc\nfrom boinc_client.clients.rpc_client import RpcClient\n\n# Hostname or IP of the running BOINC client\nBOINC_HOSTNAME = "192.168.0.2"\n\n# Create an RPC client to connect to the BOINC socket\nrpc_client = RpcClient(hostname=BOINC_HOSTNAME)\nrpc_client.authenticate()\n\n# Create a BOINC client to interact with the RPC socket\nboinc_client = Boinc(rpc_client=rpc_client)\n```\n\n#### RPC Client options\nThe following options can be passed when creating an `RpcClient` instance\n\n| Argument   | Description                                                                | Required | Default |\n|------------|----------------------------------------------------------------------------|----------|---------|\n| `hostname` | Hostname or IP address of the BOINC client                                 | Yes      | None    |\n| `port`     | Exposed port of the BOINC client                                           | No       | 31416   |\n| `timeout`  | Seconds to wait for a successful connection to the RPC socket              | No       | 30      |\n| `password` | Password to authenticate to the BOINC client, required for most operations | No       | None    |\n\n#### Boinc options\nThe following options can be passed when creating a `Boinc` instance\n\n| Argument     | Description                        | Required | Default |\n|--------------|------------------------------------|----------|---------|\n| `rpc_client` | Instance of a configured RpcClient | Yes      | None    |\n\n### Interacting with Boinc\n\n* [Unauthorised Operations](docs/unauthorised.md)\n* [Project Operations](docs/project.md)\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->',
     'author': 'Lewis England',
     'author_email': 'lewis2004@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `boinc_client-1.4.5/PKG-INFO` & `boinc_client-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boinc-client
-Version: 1.4.5
+Version: 1.4.6
 Summary: Python API for interacting with a BOINC client via RPC
 Author: Lewis England
 Author-email: lewis2004@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

