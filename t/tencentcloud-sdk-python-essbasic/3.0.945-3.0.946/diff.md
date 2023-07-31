# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.945.tar", last modified: Fri Jul 28 00:28:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.946.tar", last modified: Mon Jul 31 00:26:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.945.tar` & `tencentcloud-sdk-python-essbasic-3.0.946.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    55990 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   391825 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:28:15.000000 tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    56205 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   392627 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:26:15.000000 tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     _service = 'essbasic'
 
 
     def ChannelBatchCancelFlows(self, request):
         """指定需要批量撤销的签署流程Id，批量撤销合同
         客户指定需要撤销的签署流程Id，最多100个，超过100不处理；
 
+        可以撤回：未全部签署完成
+         不可以撤回：已全部签署完成、已拒签、已过期、已撤回、拒绝填写、已解除等合同状态。
+
         **满足撤销条件的合同会发起异步撤销流程，不满足撤销条件的合同返回失败原因。**
 
         **合同撤销成功后，会通过合同状态为 CANCEL 的回调消息通知调用方 [具体可参考回调消息](https://qian.tencent.com/developers/scenes/partner/callback_data_types#-%E5%90%88%E5%90%8C%E7%8A%B6%E6%80%81%E9%80%9A%E7%9F%A5---flowstatuschange)**
 
         **注意:
         能撤回合同的只能是合同的发起人或者发起企业的超管、法人**
 
@@ -105,15 +108,18 @@
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelCreateBatchCancelFlowUrl(self, request):
         """指定需要批量撤销的签署流程Id，获取批量撤销链接 - 不建议使用此接口，可使用ChannelBatchCancelFlows
         客户指定需要撤销的签署流程Id，最多100个，超过100不处理；
         接口调用成功返回批量撤销合同的链接，通过链接跳转到电子签小程序完成批量撤销;
-        可以撤回：未全部签署完成；不可以撤回（终态）：已全部签署完成、已拒签、已过期、已撤回。
+
+        可以撤回：未全部签署完成
+         不可以撤回：已全部签署完成、已拒签、已过期、已撤回、拒绝填写、已解除等合同状态。
+
         注意:
         能撤回合同的只能是合同的发起人或者发起企业的超管、法人
 
         :param request: Request instance for ChannelCreateBatchCancelFlowUrl.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateBatchCancelFlowUrlRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateBatchCancelFlowUrlResponse`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20210526/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,32 +291,40 @@
     """
 
     def __init__(self):
         r"""
         :param _FlowName: 合同流程名称
         :type FlowName: str
         :param _FlowType: 合同流程类型
+<br/>客户自定义，用于合同分类展示
         :type FlowType: str
         :param _FlowDescription: 合同流程描述信息
         :type FlowDescription: str
         :param _Deadline: 合同流程截止时间，unix时间戳，单位秒
         :type Deadline: int
         :param _Unordered: 是否顺序签署(true:无序签,false:顺序签)
+<br/>默认false，有序签署合同
         :type Unordered: bool
         :param _IntelligentStatus: 是否打开智能添加填写区(默认开启，打开:"OPEN" 关闭："CLOSE")
         :type IntelligentStatus: str
         :param _FormFields: 填写控件内容
         :type FormFields: list of FormField
-        :param _NeedSignReview: 本企业(发起方企业)是否需要签署审批，true：开启本企业签署审批。使用ChannelCreateFlowSignReview接口提交审批结果，才能继续完成签署
+        :param _NeedSignReview: 本企业(发起方企业)是否需要签署审批
+<br/>true：开启发起方签署审批
+<br/>false：不开启发起方签署审批
+<br/>开启后，使用ChannelCreateFlowSignReview接口提交审批结果，才能继续完成签署
         :type NeedSignReview: bool
         :param _UserData: 用户流程自定义数据参数
         :type UserData: str
         :param _CcInfos: 抄送人信息
         :type CcInfos: list of CcInfo
-        :param _NeedCreateReview: 是否需要发起前审核，当指定NeedCreateReview=true，则发起后，需要使用接口：ChannelCreateFlowSignReview，来完成发起前审核，审核通过后，可以继续查看，签署合同
+        :param _NeedCreateReview: 是否需要开启发起方发起前审核
+<br/>true：开启发起方发起前审核
+<br/>false：不开启发起方发起前审核
+<br/>当指定NeedCreateReview=true，则提交审核后，需要使用接口：ChannelCreateFlowSignReview，来完成发起前审核，审核通过后，可以继续查看，签署合同
         :type NeedCreateReview: bool
         """
         self._FlowName = None
         self._FlowType = None
         self._FlowDescription = None
         self._Deadline = None
         self._Unordered = None
@@ -530,18 +538,19 @@
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 签署流程Id数组，最多100个，超过100不处理
         :type FlowIds: list of str
         :param _CancelMessage: 撤销理由,不超过200个字符
         :type CancelMessage: str
         :param _CancelMessageFormat: 撤销理由自定义格式；选项：
-0 默认格式
-1 只保留身份信息：展示为【发起方】
-2 保留身份信息+企业名称：展示为【发起方xxx公司】
-3 保留身份信息+企业名称+经办人名称：展示为【发起方xxxx公司-经办人姓名】
+
+- 0 默认格式
+- 1 只保留身份信息：展示为【发起方】
+- 2 保留身份信息+企业名称：展示为【发起方xxx公司】
+- 3 保留身份信息+企业名称+经办人名称：展示为【发起方xxxx公司-经办人姓名】
         :type CancelMessageFormat: int
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
         self._FlowIds = None
         self._CancelMessage = None
@@ -1224,29 +1233,31 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Agent: 渠道应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param _EmbedType: WEB嵌入资源类型。
-CREATE_SEAL: 创建印章
-CREATE_TEMPLATE：创建模板
-MODIFY_TEMPLATE：修改模板
-PREVIEW_TEMPLATE：预览模板
-PREVIEW_FLOW：预览合同文档
-PREVIEW_FLOW_DETAIL：预览合同详情
-PREVIEW_SEAL_LIST：预览印章列表
-PREVIEW_SEAL_DETAIL：预览印章详情
-EXTEND_SERVICE：扩展服务
+        :param _EmbedType: 要生成WEB嵌入界面的类型, 可以选择的值如下: 
+
+- CREATE_SEAL: 生成创建印章的嵌入页面
+- CREATE_TEMPLATE：生成创建模板的嵌入页面
+- MODIFY_TEMPLATE：生成修改模板的嵌入页面
+- PREVIEW_TEMPLATE：生成预览模板的嵌入页面
+- PREVIEW_FLOW：生成预览合同文档的嵌入页面
+- PREVIEW_FLOW_DETAIL：生成预览合同详情的嵌入页面
+- PREVIEW_SEAL_LIST：生成预览印章列表的嵌入页面
+- PREVIEW_SEAL_DETAIL：生成预览印章详情的嵌入页面
+- EXTEND_SERVICE：生成扩展服务的嵌入页面
         :type EmbedType: str
         :param _BusinessId: WEB嵌入的业务资源ID
-EmbedType取值MODIFY_TEMPLATE，PREVIEW_TEMPLATE时必填，取值为模板id
-PREVIEW_FLOW，PREVIEW_FLOW_DETAIL时必填，取值为合同id
-PREVIEW_SEAL_DETAIL，必填，取值为印章id
+
+- 当EmbedType取值MODIFY_TEMPLATE，PREVIEW_TEMPLATE时需要填写模板id作为BusinessId
+- 当EmbedType取值PREVIEW_FLOW，PREVIEW_FLOW_DETAIL时需要填写合同id作为BusinessId
+- 当EmbedType取值PREVIEW_SEAL_DETAIL需要填写印章id作为BusinessId
         :type BusinessId: str
         :param _HiddenComponents: 是否隐藏控件，只有预览模板时生效
         :type HiddenComponents: bool
         :param _Operator: 渠道操作者信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -2059,15 +2070,15 @@
         :type ReviewMessage: str
         :param _RecipientId: 签署节点审核时需要指定，给个人审核时必填。
         :type RecipientId: str
         :param _OperateType: 操作类型，默认：SignReview；SignReview:签署审核，CreateReview：发起审核
 注：接口通过该字段区分操作类型
 该字段不传或者为空，则默认为SignReview签署审核，走签署审核流程
 若想使用发起审核，请指定该字段为：CreateReview
-若发起个人审核，则指定该字段为：SignReview（注意，给个人审核时，需联系客户经理开白使用）
+若发起个人审核，则指定该字段为：SignReview
         :type OperateType: str
         """
         self._Agent = None
         self._FlowId = None
         self._ReviewType = None
         self._ReviewMessage = None
         self._RecipientId = None
@@ -2629,35 +2640,35 @@
         r"""
         :param _ResourceId: 资源id，与ResourceType对应
         :type ResourceId: str
         :param _ResourceType: 资源类型，1：模板，目前仅支持模板，与ResourceId对应
         :type ResourceType: int
         :param _FlowInfo: 合同流程基础信息
         :type FlowInfo: :class:`tencentcloud.essbasic.v20210526.models.BaseFlowInfo`
-        :param _FlowApproverList: 合同签署人信息
-        :type FlowApproverList: list of CommonFlowApprover
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowOption: 合同流程配置信息，用于配置发起合同时定制化
         :type FlowOption: :class:`tencentcloud.essbasic.v20210526.models.CreateFlowOption`
+        :param _FlowApproverList: 合同签署人信息
+        :type FlowApproverList: list of CommonFlowApprover
         :param _FlowId: 通过flowid快速获得之前成功通过页面发起的合同生成链接
         :type FlowId: str
         :param _NeedPreview: 该参数不可用，请通过获取 web 可嵌入接口获取合同流程预览 URL
         :type NeedPreview: bool
         :param _Organization: 企业机构信息，不用传
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
         :param _Operator: 操作人（用户）信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._ResourceId = None
         self._ResourceType = None
         self._FlowInfo = None
-        self._FlowApproverList = None
         self._Agent = None
         self._FlowOption = None
+        self._FlowApproverList = None
         self._FlowId = None
         self._NeedPreview = None
         self._Organization = None
         self._Operator = None
 
     @property
     def ResourceId(self):
@@ -2680,22 +2691,14 @@
         return self._FlowInfo
 
     @FlowInfo.setter
     def FlowInfo(self, FlowInfo):
         self._FlowInfo = FlowInfo
 
     @property
-    def FlowApproverList(self):
-        return self._FlowApproverList
-
-    @FlowApproverList.setter
-    def FlowApproverList(self, FlowApproverList):
-        self._FlowApproverList = FlowApproverList
-
-    @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
         self._Agent = Agent
 
@@ -2704,14 +2707,22 @@
         return self._FlowOption
 
     @FlowOption.setter
     def FlowOption(self, FlowOption):
         self._FlowOption = FlowOption
 
     @property
+    def FlowApproverList(self):
+        return self._FlowApproverList
+
+    @FlowApproverList.setter
+    def FlowApproverList(self, FlowApproverList):
+        self._FlowApproverList = FlowApproverList
+
+    @property
     def FlowId(self):
         return self._FlowId
 
     @FlowId.setter
     def FlowId(self, FlowId):
         self._FlowId = FlowId
 
@@ -2754,26 +2765,26 @@
 
     def _deserialize(self, params):
         self._ResourceId = params.get("ResourceId")
         self._ResourceType = params.get("ResourceType")
         if params.get("FlowInfo") is not None:
             self._FlowInfo = BaseFlowInfo()
             self._FlowInfo._deserialize(params.get("FlowInfo"))
-        if params.get("FlowApproverList") is not None:
-            self._FlowApproverList = []
-            for item in params.get("FlowApproverList"):
-                obj = CommonFlowApprover()
-                obj._deserialize(item)
-                self._FlowApproverList.append(obj)
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         if params.get("FlowOption") is not None:
             self._FlowOption = CreateFlowOption()
             self._FlowOption._deserialize(params.get("FlowOption"))
+        if params.get("FlowApproverList") is not None:
+            self._FlowApproverList = []
+            for item in params.get("FlowApproverList"):
+                obj = CommonFlowApprover()
+                obj._deserialize(item)
+                self._FlowApproverList.append(obj)
         self._FlowId = params.get("FlowId")
         self._NeedPreview = params.get("NeedPreview")
         if params.get("Organization") is not None:
             self._Organization = OrganizationInfo()
             self._Organization._deserialize(params.get("Organization"))
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
@@ -5462,20 +5473,23 @@
 class CreateChannelFlowEvidenceReportResponse(AbstractModel):
     """CreateChannelFlowEvidenceReport返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ReportId: 出证报告 ID，用于查询出证报告接口DescribeChannelFlowEvidenceReport时用到
+        :param _ReportId: 出证报告 ID，可用户DescribeChannelFlowEvidenceReport接口查询出证PDF的下载地址
+
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReportId: str
-        :param _Status: 执行中：EvidenceStatusExecuting
-成功：EvidenceStatusSuccess
-失败：EvidenceStatusFailed
+        :param _Status: 出征任务的执行状态,状态列表如下
+
+- EvidenceStatusExecuting : 出征任务正在执行中
+- EvidenceStatusSuccess : 出征任务执行成功
+- EvidenceStatusFailed : 出征任务执行失败
         :type Status: str
         :param _ReportUrl: 废除，字段无效
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReportUrl: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
@@ -6524,20 +6538,22 @@
 class DescribeChannelFlowEvidenceReportResponse(AbstractModel):
     """DescribeChannelFlowEvidenceReport返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _ReportUrl: 出证报告 URL
+        :param _ReportUrl: 出证报告下载 URL
 注意：此字段可能返回 null，表示取不到有效值。
         :type ReportUrl: str
-        :param _Status: 执行中：EvidenceStatusExecuting
-成功：EvidenceStatusSuccess
-失败：EvidenceStatusFailed
+        :param _Status: 出征任务的执行状态,状态列表如下
+
+- EvidenceStatusExecuting : 出征任务正在执行中
+- EvidenceStatusSuccess : 出征任务执行成功
+- EvidenceStatusFailed : 出征任务执行失败
         :type Status: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._ReportUrl = None
         self._Status = None
         self._RequestId = None
@@ -6660,15 +6676,15 @@
     """
 
     def __init__(self):
         r"""
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 合同(流程)编号数组，最多支持100个。
-（备注：该参数和合同组编号必须二选一）
+（备注：该参数和合同组编号必须二选一, 如果填写FlowGroupId则忽略此FlowIds的入参）
         :type FlowIds: list of str
         :param _FlowGroupId: 合同组编号（备注：该参数和合同(流程)编号数组必须二选一）
         :type FlowGroupId: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.946/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.946/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.945/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.946/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

