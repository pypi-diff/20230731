# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.945.tar", last modified: Fri Jul 28 00:23:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.946.tar", last modified: Mon Jul 31 00:21:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.945.tar` & `tencentcloud-sdk-python-cdb-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   146951 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19678 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   798517 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:23:19.000000 tencentcloud-sdk-python-cdb-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   146951 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   798528 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:21:17.000000 tencentcloud-sdk-python-cdb-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/setup.py` & `tencentcloud-sdk-python-cdb-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.946/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6069,15 +6069,15 @@
         :type ProjectId: int
         :param _Port: 自定义端口，端口支持范围：[ 1024-65535 ]。
         :type Port: int
         :param _InstanceRole: 实例类型，默认为 master，支持值包括：master - 表示主实例，dr - 表示灾备实例，ro - 表示只读实例。
         :type InstanceRole: str
         :param _MasterInstanceId: 实例 ID，购买只读实例时必填，该字段表示只读实例的主实例ID，请使用 [查询实例列表](https://cloud.tencent.com/document/api/236/15872) 接口查询云数据库实例 ID。
         :type MasterInstanceId: str
-        :param _EngineVersion: MySQL 版本，值包括：5.5、5.6 和 5.7，请使用 [获取云数据库可售卖规格](https://cloud.tencent.com/document/api/236/17229) 接口获取可创建的实例版本。
+        :param _EngineVersion: MySQL 版本，值包括：5.5、5.6 、5.7和8.0，请使用 [获取云数据库可售卖规格](https://cloud.tencent.com/document/api/236/17229) 接口获取可创建的实例版本。
         :type EngineVersion: str
         :param _Password: 设置 root 帐号密码，密码规则：8 - 64 个字符，至少包含字母、数字、字符（支持的字符：_+-&=!@#$%^*()）中的两种，购买主实例时可指定该参数，购买只读实例或者灾备实例时指定该参数无意义。
         :type Password: str
         :param _ProtectMode: 数据复制方式，默认为 0，支持值包括：0 - 表示异步复制，1 - 表示半同步复制，2 - 表示强同步复制。
         :type ProtectMode: int
         :param _DeployMode: 多可用区域，默认为 0，支持值包括：0 - 表示单可用区，1 - 表示多可用区。
         :type DeployMode: int
@@ -6536,15 +6536,15 @@
 class CreateDBInstanceResponse(AbstractModel):
     """CreateDBInstance返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _DealIds: 短订单 ID。
+        :param _DealIds: 计费子订单 ID。
         :type DealIds: list of str
         :param _InstanceIds: 实例 ID 列表。
         :type InstanceIds: list of str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._DealIds = None
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.946/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.946/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.945/README.rst` & `tencentcloud-sdk-python-cdb-3.0.946/README.rst`

 * *Files identical despite different names*

