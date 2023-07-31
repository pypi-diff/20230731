# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.945.tar", last modified: Fri Jul 28 00:31:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.946.tar", last modified: Mon Jul 31 00:31:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.945.tar` & `tencentcloud-sdk-python-lcic-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48865 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   234643 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-28 00:31:02.000000 tencentcloud-sdk-python-lcic-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48865 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   235024 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-31 00:31:11.000000 tencentcloud-sdk-python-lcic-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/setup.py` & `tencentcloud-sdk-python-lcic-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.946/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3987,14 +3987,16 @@
         :type StartTime: int
         :param _EndTime: 预定的房间结束时间，unix时间戳（秒）。
         :type EndTime: int
         :param _TeacherId: 老师的UserId。
         :type TeacherId: str
         :param _SdkAppId: 低代码互动课堂的SdkAppId。
         :type SdkAppId: int
+        :param _AudienceType: 观看类型。互动观看 （默认）	
+        :type AudienceType: int
         :param _Resolution: 分辨率。可以有如下取值：
 1 标清
 2 高清
 3 全高清
         :type Resolution: int
         :param _MaxMicNumber: 最大连麦人数（不包括老师）。取值范围[0, 16]
         :type MaxMicNumber: int
@@ -4043,14 +4045,15 @@
         :type RequestId: str
         """
         self._Name = None
         self._StartTime = None
         self._EndTime = None
         self._TeacherId = None
         self._SdkAppId = None
+        self._AudienceType = None
         self._Resolution = None
         self._MaxMicNumber = None
         self._AutoMic = None
         self._AudioQuality = None
         self._SubType = None
         self._DisableRecord = None
         self._Assistants = None
@@ -4101,14 +4104,22 @@
         return self._SdkAppId
 
     @SdkAppId.setter
     def SdkAppId(self, SdkAppId):
         self._SdkAppId = SdkAppId
 
     @property
+    def AudienceType(self):
+        return self._AudienceType
+
+    @AudienceType.setter
+    def AudienceType(self, AudienceType):
+        self._AudienceType = AudienceType
+
+    @property
     def Resolution(self):
         return self._Resolution
 
     @Resolution.setter
     def Resolution(self, Resolution):
         self._Resolution = Resolution
 
@@ -4235,14 +4246,15 @@
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._TeacherId = params.get("TeacherId")
         self._SdkAppId = params.get("SdkAppId")
+        self._AudienceType = params.get("AudienceType")
         self._Resolution = params.get("Resolution")
         self._MaxMicNumber = params.get("MaxMicNumber")
         self._AutoMic = params.get("AutoMic")
         self._AudioQuality = params.get("AudioQuality")
         self._SubType = params.get("SubType")
         self._DisableRecord = params.get("DisableRecord")
         self._Assistants = params.get("Assistants")
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.946/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.946/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.945/README.rst` & `tencentcloud-sdk-python-lcic-3.0.946/README.rst`

 * *Files identical despite different names*

