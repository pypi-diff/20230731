# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.945.tar", last modified: Fri Jul 28 00:28:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.946.tar", last modified: Mon Jul 31 00:26:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.945.tar` & `tencentcloud-sdk-python-ess-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    65932 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   453727 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:28:10.000000 tencentcloud-sdk-python-ess-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:28:09.000000 tencentcloud-sdk-python-ess-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    65988 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   454866 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:26:10.000000 tencentcloud-sdk-python-ess-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.945/setup.py` & `tencentcloud-sdk-python-ess-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -936,17 +936,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowBriefs(self, request):
-        """查询流程摘要
+        """查询流程基础信息
         适用场景：可用于主动查询某个合同流程的签署状态信息。可以配合回调通知使用。
-        日调用量限制：10W
+        每个企业限制日调用量限制：10W,  当当日超过此限制后再调用接口返回错误
 
         :param request: Request instance for DescribeFlowBriefs.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowBriefsResponse`
 
         """
         try:
@@ -1036,14 +1036,15 @@
 
     def DescribeFlowTemplates(self, request):
         """本接口用于查询本企业模板列表。
 
         当模板较多或模板中的控件较多时，可以通过查询模板接口更方便的获取模板列表，以及每个模板内的控件信息。
 
         > **适用场景**
+        >
         >  该接口常用来配合“模板发起合同-创建电子文档”接口作为前置的接口使用。
         >  一个模板通常会包含以下结构信息
         >- 模板基本信息
         >- 发起方参与信息Promoter、签署参与方 Recipients，后者会在模板发起合同时用于指定参与方
         >- 填写控件 Components
         >- 签署控件 SignComponents
         >- 生成模板的文件基础信息 FileInfos
@@ -1275,16 +1276,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetTaskResultApi(self, request):
-        """通过发起转换任务接口（CreateConvertTaskApi）返回的任务Id查询转换任务状态，通过本接口确认转换任务是否完成。<br/>
-        大文件转换所需的时间可能会比较长。
+        """查询转换任务的状态。转换任务Id通过发起转换任务接口（CreateConvertTaskApi）获取。
+        注意：大文件转换所需的时间可能会比较长。
 
         :param request: Request instance for GetTaskResultApi.
         :type request: :class:`tencentcloud.ess.v20201111.models.GetTaskResultApiRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.GetTaskResultApiResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.945/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.946/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -555,23 +555,40 @@
 
     """
 
     def __init__(self):
         r"""
         :param _UserInfo: 自动签开通个人用户的三要素
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
-        :param _CallbackUrl: 接受自动签开启的回调地址。需要保证post返回200
+        :param _CallbackUrl: 接受回调URL地址。支持http://或者https://协议
+
+Post数据到此地址后后返回httpcode200表示接受回调成功, 返回其他httpcode表示接受回调失败
         :type CallbackUrl: str
-        :param _CertInfoCallback: 是否回调证书信息，默认false-不需要
+        :param _CertInfoCallback: 是否回调证书信息
+false-不需要 (默认值)
+true-需要
         :type CertInfoCallback: bool
-        :param _UserDefineSeal: 是否支持用户自定义签名印章，默认false-不需要
+        :param _UserDefineSeal: 是否支持用户自定义签名印章
+false-不需要(默认)
+true-需要
         :type UserDefineSeal: bool
-        :param _SealImgCallback: 是否需要回调的时候返回印章(签名) 图片的 base64，默认false-不需要
+        :param _SealImgCallback: 是否需要回调的时候返回印章(签名) 图片的 base64
+
+false-不需要(默认)
+true-需要(
         :type SealImgCallback: bool
-        :param _VerifyChannels: 开通时候的验证方式，取值：WEIXINAPP（微信人脸识别），INSIGHT（慧眼人脸认别），TELECOM（运营商三要素验证）。如果是小程序开通链接，支持传 WEIXINAPP / TELECOM。如果是 H5 开通链接，支持传 INSIGHT / TELECOM。默认值 WEIXINAPP / INSIGHT。
+        :param _VerifyChannels: 开通时候的验证方式, 分布为
+
+WEIXINAPP : 微信人脸识别
+INSIGHT : 慧眼人脸认别
+TELECOM : 运营商三要素验证
+
+如果是小程序开通链接，支持传 WEIXINAPP / TELECOM。
+
+如果是 H5 开通链接，支持传 INSIGHT / TELECOM。默认值 WEIXINAPP / INSIGHT。
         :type VerifyChannels: list of str
         """
         self._UserInfo = None
         self._CallbackUrl = None
         self._CertInfoCallback = None
         self._UserDefineSeal = None
         self._SealImgCallback = None
@@ -1708,15 +1725,16 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _FlowIds: 需要执行撤回的签署流程id数组，最多100个
+        :param _FlowIds: 需要执行撤回的流程(合同)的编号列表，最多100个.
+列表中的流程(合同)编号不要重复.
         :type FlowIds: list of str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
 
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._FlowIds = None
@@ -1771,16 +1789,19 @@
     """
 
     def __init__(self):
         r"""
         :param _BatchCancelFlowUrl: 批量撤回签署流程链接
         :type BatchCancelFlowUrl: str
         :param _FailMessages: 签署流程撤回失败信息
+数组里边的错误原因与传进来的FlowIds一一对应,如果是空字符串则标识没有出错
         :type FailMessages: list of str
         :param _UrlExpireOn: 签署连接过期时间字符串：年月日-时分秒
+
+例如:2023-07-28 17:25:59
         :type UrlExpireOn: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._BatchCancelFlowUrl = None
         self._FailMessages = None
         self._UrlExpireOn = None
@@ -3697,15 +3718,15 @@
 
 SignReview:签署审核
 CreateReview:发起审核
 
 默认：SignReview；SignReview:签署审核
 
 该字段不传或者为空，则默认为SignReview签署审核，走签署审核流程
-若发起个人审核，则指定该字段为：SignReview（注意，给个人审核时，需联系客户经理开白使用）
+若发起个人审核，则指定该字段为：SignReview
         :type OperateType: str
         """
         self._Operator = None
         self._FlowId = None
         self._ReviewType = None
         self._ReviewMessage = None
         self._Agent = None
@@ -5259,19 +5280,22 @@
         :param _EndPoint: 链接类型
 HTTP：跳转电子签小程序的http_url，
 APP：第三方APP或小程序跳转电子签小程序的path。
 默认为HTTP类型
         :type EndPoint: str
         :param _FlowId: 签署流程编号 (PathType=1时必传)
         :type FlowId: str
-        :param _FlowGroupId: 合同组ID
+        :param _FlowGroupId: 合同组ID 
         :type FlowGroupId: str
         :param _PathType: 跳转页面 1: 小程序合同详情 2: 小程序合同列表页 0: 不传, 默认主页
         :type PathType: int
-        :param _AutoJumpBack: 是否自动回跳 true：是， false：否。该参数只针对"APP" 类型的签署链接有效
+        :param _AutoJumpBack: 是否自动回跳
+true：是，
+false：否。
+该参数只针对"APP" 类型的签署链接有效
         :type AutoJumpBack: bool
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Hides: 生成的签署链接在签署过程隐藏的按钮列表, 可以设置隐藏的按钮列表如下
 
 0:合同签署页面更多操作按钮
 1:合同签署页面更多操作的拒绝签署按钮
@@ -5897,19 +5921,24 @@
         :param _Operator: 操作人信息,UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param _AutoSignConfig: 自动签开通，签署相关配置
         :type AutoSignConfig: :class:`tencentcloud.ess.v20201111.models.AutoSignConfig`
-        :param _UrlType: 链接类型，空-默认小程序端链接，H5SIGN-h5端链接
+        :param _UrlType: 链接类型，
+空-默认小程序端链接
+H5SIGN-h5端链接
         :type UrlType: str
-        :param _NotifyType: 通知类型，默认不填为不通知开通方，填写 SMS 为短信通知。
+        :param _NotifyType: 通知类型
+
+默认不设置为不通知开通方，
+SMS 为短信通知 , 此种方式需要NotifyAddress填写手机号。
         :type NotifyType: str
-        :param _NotifyAddress: 若上方填写为 SMS，则此处为手机号
+        :param _NotifyAddress: 如果通知类型NotifyType选择为SMS，则此处为手机号, 其他通知类型不需要设置此项
         :type NotifyAddress: str
         :param _ExpiredTime: 链接的过期时间，格式为Unix时间戳，不能早于当前时间，且最大为30天。如果不传，默认有效期为7天。
         :type ExpiredTime: int
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
@@ -6022,15 +6051,15 @@
         :type Url: str
         :param _AppId: 小程序AppId
         :type AppId: str
         :param _AppOriginalId: 小程序 原始 Id
         :type AppOriginalId: str
         :param _Path: 跳转路径
         :type Path: str
-        :param _QrCode: base64格式跳转二维码
+        :param _QrCode: base64格式跳转二维码,可以通过微信扫描后跳转到业务界面
         :type QrCode: str
         :param _UrlType: 链接类型，空-默认小程序端链接，H5SIGN-h5端链接
         :type UrlType: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Url = None
@@ -7321,20 +7350,22 @@
 class DescribeFlowEvidenceReportResponse(AbstractModel):
     """DescribeFlowEvidenceReport返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ReportUrl: 报告 URL
+        :param _ReportUrl: 出证报告PDF的下载 URL
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReportUrl: str
-        :param _Status: 执行中：EvidenceStatusExecuting
-成功：EvidenceStatusSuccess
-失败：EvidenceStatusFailed
+        :param _Status: 出证任务执行的状态, 分布表示下面的含义
+
+EvidenceStatusExecuting  出证任务在执行中
+EvidenceStatusSuccess  出证任务执行成功
+EvidenceStatusFailed  出征任务执行失败
         :type Status: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._ReportUrl = None
         self._Status = None
         self._RequestId = None
@@ -7376,18 +7407,22 @@
     """
 
     def __init__(self):
         r"""
         :param _Operator: 调用方用户信息，userId 必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _FlowIds: 需要查询的流程ID列表，限制最大100个
+
+如果查询合同组的信息,不要传此参数
         :type FlowIds: list of str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
-        :param _FlowGroupId: 合同组ID
+        :param _FlowGroupId: 合同组ID, 如果传此参数会忽略FlowIds入参
+ 所以如传此参数不要传FlowIds参数
+
         :type FlowGroupId: str
         """
         self._Operator = None
         self._FlowIds = None
         self._Agent = None
         self._FlowGroupId = None
 
@@ -8744,15 +8779,15 @@
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
-        :param _UserInfo: 查询开启状态的用户信息
+        :param _UserInfo: 要查询开启状态的用户信息
         :type UserInfo: :class:`tencentcloud.ess.v20201111.models.UserThreeFactor`
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._SceneKey = None
         self._UserInfo = None
@@ -8815,19 +8850,22 @@
 class DescribeUserAutoSignStatusResponse(AbstractModel):
     """DescribeUserAutoSignStatus返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _IsOpen: 是否已开通自动签
+        :param _IsOpen: 查询用户是否已开通自动签
         :type IsOpen: bool
         :param _LicenseFrom: 自动签许可生效时间。当且仅当已开通自动签时有值。
+
+值为unix时间戳,单位为秒。
         :type LicenseFrom: int
         :param _LicenseTo: 自动签许可到期时间。当且仅当已开通自动签时有值。
+值为unix时间戳,单位为秒。
         :type LicenseTo: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._IsOpen = None
         self._LicenseFrom = None
         self._LicenseTo = None
@@ -9995,15 +10033,17 @@
 - 10 拒填
 - 21 已解除
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowStatus: int
         :param _CreatedOn: 流程创建的时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreatedOn: int
-        :param _FlowMessage: 拒签或者取消的原因描述
+        :param _FlowMessage: 当合同被拒签或者取消后(当FlowStatus=3或者FlowStatus=6的时候)
+此字段展示拒签或者取消的原因描述
+
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowMessage: str
         :param _Creator:  合同发起人userId
 注意：此字段可能返回 null，表示取不到有效值。
         :type Creator: str
         :param _Deadline: 合同过期时间，时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
@@ -11055,15 +11095,15 @@
 class GetTaskResultApiRequest(AbstractModel):
     """GetTaskResultApi请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskId: 任务Id，通过CreateConvertTaskApi得到
+        :param _TaskId: 任务Id，通过接口CreateConvertTaskApi或CreateMergeFileTask得到的返回任务id
         :type TaskId: str
         :param _Operator: 操作人信息,UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _Agent: 应用号信息
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Organization: 暂未开放
         :type Organization: :class:`tencentcloud.ess.v20201111.models.OrganizationInfo`
@@ -11156,15 +11196,15 @@
 NeedTranform   - 任务已提交
 Processing     - 文档转换中
 TaskEnd        - 任务处理完成
 DownloadFailed - 下载失败
 ProcessFailed  - 转换失败
 ProcessTimeout - 转换文件超时
         :type TaskMessage: str
-        :param _ResourceId: 资源Id，也是FileId，用于文件发起使用
+        :param _ResourceId: 资源Id，也是FileId，用于文件发起时使用
         :type ResourceId: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TaskId = None
         self._TaskStatus = None
         self._TaskMessage = None
@@ -12675,15 +12715,15 @@
 ORGANIZATION-企业
 ENTERPRISESERVER-企业静默签
         :type ApproverType: str
         :param _ApproverSignComponentType: 签署控件类型，支持自定义企业签署方的签署控件为“印章”或“签名”
 - SIGN_SEAL-默认为印章控件类型
 - SIGN_SIGNATURE-手写签名控件类型
         :type ApproverSignComponentType: str
-        :param _ApproverSignRole: 签署方自定义控件别名，最大长度20个字符
+        :param _ApproverSignRole: 参与方在合同中的角色是按照创建合同的时候来排序的; 解除协议会将第一个参与人叫甲方, 第二个叫乙方,第三个叫丙方, 依次类推.  如果想改动参与人的角色名字, 可以设置此签署方自定义控件别名字段，最大20个字符
         :type ApproverSignRole: str
         """
         self._Name = None
         self._Mobile = None
         self._RelievedApproverReceiptId = None
         self._ApproverType = None
         self._ApproverSignComponentType = None
```

### Comparing `tencentcloud-sdk-python-ess-3.0.945/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.946/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.946/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.945/README.rst` & `tencentcloud-sdk-python-ess-3.0.946/README.rst`

 * *Files identical despite different names*

