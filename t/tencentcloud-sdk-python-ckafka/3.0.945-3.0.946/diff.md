# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.945.tar", last modified: Fri Jul 28 00:24:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.946.tar", last modified: Mon Jul 31 00:22:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.945.tar` & `tencentcloud-sdk-python-ckafka-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    72823 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)   773069 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-28 00:24:23.000000 tencentcloud-sdk-python-ckafka-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    72823 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)   773033 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-31 00:22:37.000000 tencentcloud-sdk-python-ckafka-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-31 00:22:36.000000 tencentcloud-sdk-python-ckafka-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.946/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3095,15 +3095,15 @@
         :type ResourceType: int
         :param _Operation: Acl操作方式，(2:ALL，3:READ，4:WRITE，5:CREATE，6:DELETE，7:ALTER，8:DESCRIBE，9:CLUSTER_ACTION，10:DESCRIBE_CONFIGS，11:ALTER_CONFIGS，12:IDEMPOTENT_WRITE)
         :type Operation: int
         :param _PermissionType: 权限类型，(2:DENY，3:ALLOW)，当前ckakfa支持ALLOW(相当于白名单)，其它用于后续兼容开源kafka的acl时使用
         :type PermissionType: int
         :param _ResourceName: 资源名称，和resourceType相关，如当resourceType为TOPIC时，则该字段表示topic名称，当resourceType为GROUP时，该字段表示group名称，当resourceType为CLUSTER时，该字段可为空。
         :type ResourceName: str
-        :param _Host: 默认为\*，表示任何host都可以访问，当前ckafka不支持host为\*，但是后面开源kafka的产品化会直接支持
+        :param _Host: 默认为*，表示任何host都可以访问。支持填写IP或网段，支持“;”分隔。
         :type Host: str
         :param _Principal: 用户列表，默认为User:*，表示任何user都可以访问，当前用户只能是用户列表中包含的用户。传入时需要加 User: 前缀,如用户A则传入User:A。
         :type Principal: str
         :param _ResourceNameList: 资源名称列表,Json字符串格式。ResourceName和resourceNameList只能指定其中一个。
         :type ResourceNameList: str
         """
         self._InstanceId = None
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.946/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.945/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.946/README.rst`

 * *Files identical despite different names*

