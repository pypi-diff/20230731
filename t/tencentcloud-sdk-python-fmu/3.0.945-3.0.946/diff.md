# Comparing `tmp/tencentcloud-sdk-python-fmu-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-fmu-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.945.tar", last modified: Fri Jul 28 00:28:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.946.tar", last modified: Mon Jul 31 00:26:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-fmu-3.0.945.tar` & `tencentcloud-sdk-python-fmu-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/
--rw-r--r--   0 root         (0) root         (0)    10618 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/fmu_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    45807 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud_sdk_python_fmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:28:31.000000 tencentcloud-sdk-python-fmu-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/
+-rw-r--r--   0 root         (0) root         (0)    10618 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/fmu_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    45807 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud_sdk_python_fmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:26:29.000000 tencentcloud-sdk-python-fmu-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/setup.py` & `tencentcloud-sdk-python-fmu-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/fmu_client.py` & `tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/fmu_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/errorcodes.py` & `tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/tencentcloud/fmu/v20191213/models.py` & `tencentcloud-sdk-python-fmu-3.0.946/tencentcloud/fmu/v20191213/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.946/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.946/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.945/README.rst` & `tencentcloud-sdk-python-fmu-3.0.946/README.rst`

 * *Files identical despite different names*
