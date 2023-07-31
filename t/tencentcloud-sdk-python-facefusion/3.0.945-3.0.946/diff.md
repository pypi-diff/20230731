# Comparing `tmp/tencentcloud-sdk-python-facefusion-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-facefusion-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.945.tar", last modified: Fri Jul 28 00:28:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-facefusion-3.0.946.tar", last modified: Mon Jul 31 00:26:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-facefusion-3.0.945.tar` & `tencentcloud-sdk-python-facefusion-3.0.946.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud_sdk_python_facefusion.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     5459 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24611 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39231 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1694 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      758 2023-07-28 00:28:21.000000 tencentcloud-sdk-python-facefusion-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24611 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39231 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-31 00:26:20.000000 tencentcloud-sdk-python-facefusion-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/setup.py` & `tencentcloud-sdk-python-facefusion-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud_sdk_python_facefusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,36 +118,36 @@
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
 # 资源正在发货中。
 RESOURCEUNAVAILABLE_DELIVERING = 'ResourceUnavailable.Delivering'
 
-# 帐号已被冻结。
+# 账号已被冻结。
 RESOURCEUNAVAILABLE_FREEZE = 'ResourceUnavailable.Freeze'
 
 # 获取认证信息失败。
 RESOURCEUNAVAILABLE_GETAUTHINFOERROR = 'ResourceUnavailable.GetAuthInfoError'
 
-# 帐号已欠费。
+# 账号已欠费。
 RESOURCEUNAVAILABLE_INARREARS = 'ResourceUnavailable.InArrears'
 
 # 余额不足。
 RESOURCEUNAVAILABLE_LOWBALANCE = 'ResourceUnavailable.LowBalance'
 
 # 计费状态未知，请确认是否已在控制台开通服务。
 RESOURCEUNAVAILABLE_NOTEXIST = 'ResourceUnavailable.NotExist'
 
 # 服务未开通。
 RESOURCEUNAVAILABLE_NOTREADY = 'ResourceUnavailable.NotReady'
 
 # 资源已被回收。
 RESOURCEUNAVAILABLE_RECOVER = 'ResourceUnavailable.Recover'
 
-# 帐号已停服。
+# 账号已停服。
 RESOURCEUNAVAILABLE_STOPUSING = 'ResourceUnavailable.StopUsing'
 
 # 计费状态未知。
 RESOURCEUNAVAILABLE_UNKNOWNSTATUS = 'ResourceUnavailable.UnknownStatus'
 
-# 帐号已欠费。
+# 账号已欠费。
 RESOURCESSOLDOUT_CHARGESTATUSEXCEPTION = 'ResourcesSoldOut.ChargeStatusException'
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20220927/models.py` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20220927/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/facefusion_client.py` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/errorcodes.py` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,36 +154,36 @@
 
 # 参数字段或者值有误。
 INVALIDPARAMETERVALUE_PARAMETERVALUEERROR = 'InvalidParameterValue.ParameterValueError'
 
 # 资源正在发货中。
 RESOURCEUNAVAILABLE_DELIVERING = 'ResourceUnavailable.Delivering'
 
-# 帐号已被冻结。
+# 账号已被冻结。
 RESOURCEUNAVAILABLE_FREEZE = 'ResourceUnavailable.Freeze'
 
 # 获取认证信息失败。
 RESOURCEUNAVAILABLE_GETAUTHINFOERROR = 'ResourceUnavailable.GetAuthInfoError'
 
-# 帐号已欠费。
+# 账号已欠费。
 RESOURCEUNAVAILABLE_INARREARS = 'ResourceUnavailable.InArrears'
 
 # 余额不足。
 RESOURCEUNAVAILABLE_LOWBALANCE = 'ResourceUnavailable.LowBalance'
 
 # 计费状态未知，请确认是否已在控制台开通服务。
 RESOURCEUNAVAILABLE_NOTEXIST = 'ResourceUnavailable.NotExist'
 
 # 服务未开通。
 RESOURCEUNAVAILABLE_NOTREADY = 'ResourceUnavailable.NotReady'
 
 # 资源已被回收。
 RESOURCEUNAVAILABLE_RECOVER = 'ResourceUnavailable.Recover'
 
-# 帐号已停服。
+# 账号已停服。
 RESOURCEUNAVAILABLE_STOPUSING = 'ResourceUnavailable.StopUsing'
 
 # 计费状态未知。
 RESOURCEUNAVAILABLE_UNKNOWNSTATUS = 'ResourceUnavailable.UnknownStatus'
 
-# 帐号已欠费。
+# 账号已欠费。
 RESOURCESSOLDOUT_CHARGESTATUSEXCEPTION = 'ResourcesSoldOut.ChargeStatusException'
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/facefusion/v20181201/models.py` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/facefusion/v20181201/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-facefusion-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-facefusion-3.0.946/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-facefusion
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Facefusion SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-facefusion-3.0.945/README.rst` & `tencentcloud-sdk-python-facefusion-3.0.946/README.rst`

 * *Files identical despite different names*

