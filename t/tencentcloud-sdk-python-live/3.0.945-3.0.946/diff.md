# Comparing `tmp/tencentcloud-sdk-python-live-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.945.tar", last modified: Fri Jul 28 00:31:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.946.tar", last modified: Mon Jul 31 00:31:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.945.tar` & `tencentcloud-sdk-python-live-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20054 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   154723 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)   756776 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-28 00:31:12.000000 tencentcloud-sdk-python-live-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20054 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   154723 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)   756776 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-31 00:31:23.000000 tencentcloud-sdk-python-live-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-live-3.0.945/setup.py` & `tencentcloud-sdk-python-live-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.945/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.946/tencentcloud/live/v20180801/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.946/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.945'
+__version__ = '3.0.946'
```

### Comparing `tencentcloud-sdk-python-live-3.0.945/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.946/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.946/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.945/README.rst` & `tencentcloud-sdk-python-live-3.0.946/README.rst`

 * *Files identical despite different names*

