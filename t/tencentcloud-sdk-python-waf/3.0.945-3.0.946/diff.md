# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.945.tar", last modified: Fri Jul 28 00:39:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.946.tar", last modified: Mon Jul 31 00:39:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.945.tar` & `tencentcloud-sdk-python-waf-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    48616 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)   314432 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:39:43.000000 tencentcloud-sdk-python-waf-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49515 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)   319007 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:39:58.000000 tencentcloud-sdk-python-waf-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-waf-3.0.945/setup.py` & `tencentcloud-sdk-python-waf-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
 # 根据ID查询证书失败。
 INVALIDPARAMETER_QUERYCERTBYSSLIDFAILED = 'InvalidParameter.QueryCertBySSLIDFailed'
 
 # 语法错误：逻辑表达式语法解析出错
 INVALIDPARAMETER_QUERYSTRINGSYNTAXERR = 'InvalidParameter.QueryStringSyntaxErr'
 
+# 语法错误：SQL检索语句必须遵循特定的语法规则，如果语法错误，就会导致SQL语句无法执行。例如，缺少关键字、拼写错误、缺少分号等。
+INVALIDPARAMETER_SQLSYNTAXERR = 'InvalidParameter.SQLSyntaxErr'
+
 # 数据类型错误：SQL检索语句中的数据类型必须与数据库中的数据类型匹配，否则会导致错误。例如，将字符串与整数进行比较、将日期格式不正确等。
 INVALIDPARAMETER_TYPEMISMATCH = 'InvalidParameter.TypeMismatch'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 超过配额限制。
```

### Comparing `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -898,14 +898,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def GetAttackHistogram(self, request):
+        """生成攻击日志的产生时间柱状图
+
+        :param request: Request instance for GetAttackHistogram.
+        :type request: :class:`tencentcloud.waf.v20180125.models.GetAttackHistogramRequest`
+        :rtype: :class:`tencentcloud.waf.v20180125.models.GetAttackHistogramResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GetAttackHistogram", params, headers=headers)
+            response = json.loads(body)
+            model = models.GetAttackHistogramResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ModifyAccessPeriod(self, request):
         """本接口用于修改访问日志保存期限及大字段是否存储
 
         :param request: Request instance for ModifyAccessPeriod.
         :type request: :class:`tencentcloud.waf.v20180125.models.ModifyAccessPeriodRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.ModifyAccessPeriodResponse`
```

### Comparing `tencentcloud-sdk-python-waf-3.0.945/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.946/tencentcloud/waf/v20180125/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7274,14 +7274,149 @@
             for item in params.get("Records"):
                 obj = DownloadAttackRecordInfo()
                 obj._deserialize(item)
                 self._Records.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class GetAttackHistogramRequest(AbstractModel):
+    """GetAttackHistogram请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Domain: 查询的域名，所有域名使用all
+        :type Domain: str
+        :param _StartTime: 查询起始时间
+        :type StartTime: str
+        :param _EndTime: 查询结束时间
+        :type EndTime: str
+        :param _QueryString: Lucene语法
+        :type QueryString: str
+        """
+        self._Domain = None
+        self._StartTime = None
+        self._EndTime = None
+        self._QueryString = None
+
+    @property
+    def Domain(self):
+        return self._Domain
+
+    @Domain.setter
+    def Domain(self, Domain):
+        self._Domain = Domain
+
+    @property
+    def StartTime(self):
+        return self._StartTime
+
+    @StartTime.setter
+    def StartTime(self, StartTime):
+        self._StartTime = StartTime
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def QueryString(self):
+        return self._QueryString
+
+    @QueryString.setter
+    def QueryString(self, QueryString):
+        self._QueryString = QueryString
+
+
+    def _deserialize(self, params):
+        self._Domain = params.get("Domain")
+        self._StartTime = params.get("StartTime")
+        self._EndTime = params.get("EndTime")
+        self._QueryString = params.get("QueryString")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GetAttackHistogramResponse(AbstractModel):
+    """GetAttackHistogram返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 统计详情
+        :type Data: list of LogHistogramInfo
+        :param _Period: 时间段大小
+        :type Period: int
+        :param _TotalCount: 统计的条目数
+        :type TotalCount: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._Period = None
+        self._TotalCount = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def Period(self):
+        return self._Period
+
+    @Period.setter
+    def Period(self, Period):
+        self._Period = Period
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = LogHistogramInfo()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._Period = params.get("Period")
+        self._TotalCount = params.get("TotalCount")
+        self._RequestId = params.get("RequestId")
+
+
 class HostRecord(AbstractModel):
     """clb-waf防护域名
 
     """
 
     def __init__(self):
         r"""
@@ -8526,14 +8661,59 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class LogHistogramInfo(AbstractModel):
+    """攻击日志统计详情
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Count: 日志条数
+        :type Count: int
+        :param _TimeStamp: 时间戳
+        :type TimeStamp: int
+        """
+        self._Count = None
+        self._TimeStamp = None
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+    @property
+    def TimeStamp(self):
+        return self._TimeStamp
+
+    @TimeStamp.setter
+    def TimeStamp(self, TimeStamp):
+        self._TimeStamp = TimeStamp
+
+
+    def _deserialize(self, params):
+        self._Count = params.get("Count")
+        self._TimeStamp = params.get("TimeStamp")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ModifyAccessPeriodRequest(AbstractModel):
     """ModifyAccessPeriod请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-waf-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.946/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.945/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.946/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.945/README.rst` & `tencentcloud-sdk-python-waf-3.0.946/README.rst`

 * *Files identical despite different names*

