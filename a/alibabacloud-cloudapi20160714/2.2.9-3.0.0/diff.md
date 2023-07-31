# Comparing `tmp/alibabacloud_cloudapi20160714-2.2.9.tar.gz` & `tmp/alibabacloud_cloudapi20160714-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudapi20160714-2.2.9.tar", last modified: Thu Oct 13 02:24:01 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cloudapi20160714-3.0.0.tar", last modified: Mon Jul 31 02:29:31 2023, max compression
```

## Comparing `alibabacloud_cloudapi20160714-2.2.9.tar` & `alibabacloud_cloudapi20160714-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/
--rw-r--r--   0 root         (0) root         (0)     1493 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714/__init__.py
--rw-r--r--   0 root         (0) root         (0)   585022 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714/client.py
--rw-r--r--   0 root         (0) root         (0)  1149175 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2022-10-13 02:24:01.000000 alibabacloud_cloudapi20160714-2.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   710306 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/client.py
+-rw-r--r--   0 root         (0) root         (0)  1396813 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-07-31 02:29:31.000000 alibabacloud_cloudapi20160714-3.0.0/setup.py
```

### Comparing `alibabacloud_cloudapi20160714-2.2.9/ChangeLog.md` & `alibabacloud_cloudapi20160714-3.0.0/ChangeLog.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,47 @@
+2023-06-19 Version: 2.2.20
+- Republish.
+
+2023-06-19 Version: 2.2.19
+- Update DescribeApiGroup and DescribeInstances.
+- Add DescribeSummaryData.
+
+2023-05-30 Version: 2.2.18
+- Modify parameter location of CreateApi.
+
+2023-05-25 Version: 2.2.17
+- Add ValidateVpcConnectivity.
+
+2023-04-13 Version: 2.2.16
+- DescribeDomain add CertificateValid date.
+
+2023-03-23 Version: 2.2.15
+- DescribeApis add tag parameter.
+- CreateApp hidden parameter. 
+
+2023-01-30 Version: 2.2.14
+- Modify DescribeApis.
+
+2022-12-05 Version: 2.2.13
+- Modify QueryRequestLogs.
+
+2022-11-29 Version: 2.2.12
+- Add DescribePluginApis.
+- Modify CreateApp.
+- Modify DeleteApp.
+
+2022-11-16 Version: 2.2.11
+- Add ImportOAS.
+
+2022-11-03 Version: 2.2.10
+- Add QueryRequestLogs.
+
+2022-10-13 Version: 2.2.9
+- Add DatasetMethods.
+
 2022-09-09 Version: 2.2.8
 - Update SetDomainWebSocketStatus.
 
 2022-09-02 Version: 2.2.7
 - Add input parameters of DescribeApps and DescribeDeployedApis.
 
 2022-08-29 Version: 2.2.6
```

### Comparing `alibabacloud_cloudapi20160714-2.2.9/LICENSE` & `alibabacloud_cloudapi20160714-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714-2.2.9/PKG-INFO` & `alibabacloud_cloudapi20160714-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudapi20160714
-Version: 2.2.9
+Version: 3.0.0
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714-2.2.9/README-CN.md` & `alibabacloud_cloudapi20160714-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714-2.2.9/README.md` & `alibabacloud_cloudapi20160714-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714/client.py` & `alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -228,14 +228,26 @@
         return await self.add_access_control_list_entry_with_options_async(request, runtime)
 
     def add_ip_control_policy_item_with_options(
         self,
         request: cloud_api20160714_models.AddIpControlPolicyItemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.AddIpControlPolicyItemResponse:
+        """
+        The restriction policy on app IDs for a specific policy. You can restrict app IDs only for whitelists. The IpControlType values of whitelists are ALLOW.
+        *   You can add only one app ID restriction policy at a time.
+        *   If this parameter is empty, no restriction is imposed on the app IDs.
+        *   If this parameter is not empty, there is restriction not only on IP addresses, but also on apps.
+        *   Please note that if this parameter is not empty and the security authentication method of the API is No Authentication, all API calls are restricted.
+        *   If this parameter is not empty for a blacklist, API Gateway automatically skips this parameter and sets only restriction on IP addresses. The IpControlType value of a blacklist is REFUSE.
+        
+        @param request: AddIpControlPolicyItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cidr_ip):
             query['CidrIp'] = request.cidr_ip
         if not UtilClient.is_unset(request.ip_control_id):
@@ -262,14 +274,26 @@
         )
 
     async def add_ip_control_policy_item_with_options_async(
         self,
         request: cloud_api20160714_models.AddIpControlPolicyItemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.AddIpControlPolicyItemResponse:
+        """
+        The restriction policy on app IDs for a specific policy. You can restrict app IDs only for whitelists. The IpControlType values of whitelists are ALLOW.
+        *   You can add only one app ID restriction policy at a time.
+        *   If this parameter is empty, no restriction is imposed on the app IDs.
+        *   If this parameter is not empty, there is restriction not only on IP addresses, but also on apps.
+        *   Please note that if this parameter is not empty and the security authentication method of the API is No Authentication, all API calls are restricted.
+        *   If this parameter is not empty for a blacklist, API Gateway automatically skips this parameter and sets only restriction on IP addresses. The IpControlType value of a blacklist is REFUSE.
+        
+        @param request: AddIpControlPolicyItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cidr_ip):
             query['CidrIp'] = request.cidr_ip
         if not UtilClient.is_unset(request.ip_control_id):
@@ -295,29 +319,60 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_ip_control_policy_item(
         self,
         request: cloud_api20160714_models.AddIpControlPolicyItemRequest,
     ) -> cloud_api20160714_models.AddIpControlPolicyItemResponse:
+        """
+        The restriction policy on app IDs for a specific policy. You can restrict app IDs only for whitelists. The IpControlType values of whitelists are ALLOW.
+        *   You can add only one app ID restriction policy at a time.
+        *   If this parameter is empty, no restriction is imposed on the app IDs.
+        *   If this parameter is not empty, there is restriction not only on IP addresses, but also on apps.
+        *   Please note that if this parameter is not empty and the security authentication method of the API is No Authentication, all API calls are restricted.
+        *   If this parameter is not empty for a blacklist, API Gateway automatically skips this parameter and sets only restriction on IP addresses. The IpControlType value of a blacklist is REFUSE.
+        
+        @param request: AddIpControlPolicyItemRequest
+        @return: AddIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_ip_control_policy_item_with_options(request, runtime)
 
     async def add_ip_control_policy_item_async(
         self,
         request: cloud_api20160714_models.AddIpControlPolicyItemRequest,
     ) -> cloud_api20160714_models.AddIpControlPolicyItemResponse:
+        """
+        The restriction policy on app IDs for a specific policy. You can restrict app IDs only for whitelists. The IpControlType values of whitelists are ALLOW.
+        *   You can add only one app ID restriction policy at a time.
+        *   If this parameter is empty, no restriction is imposed on the app IDs.
+        *   If this parameter is not empty, there is restriction not only on IP addresses, but also on apps.
+        *   Please note that if this parameter is not empty and the security authentication method of the API is No Authentication, all API calls are restricted.
+        *   If this parameter is not empty for a blacklist, API Gateway automatically skips this parameter and sets only restriction on IP addresses. The IpControlType value of a blacklist is REFUSE.
+        
+        @param request: AddIpControlPolicyItemRequest
+        @return: AddIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.add_ip_control_policy_item_with_options_async(request, runtime)
 
     def add_traffic_special_control_with_options(
         self,
         request: cloud_api20160714_models.AddTrafficSpecialControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.AddTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: AddTrafficSpecialControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.special_key):
             query['SpecialKey'] = request.special_key
         if not UtilClient.is_unset(request.special_type):
@@ -346,14 +401,23 @@
         )
 
     async def add_traffic_special_control_with_options_async(
         self,
         request: cloud_api20160714_models.AddTrafficSpecialControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.AddTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: AddTrafficSpecialControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.special_key):
             query['SpecialKey'] = request.special_key
         if not UtilClient.is_unset(request.special_type):
@@ -381,21 +445,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_traffic_special_control(
         self,
         request: cloud_api20160714_models.AddTrafficSpecialControlRequest,
     ) -> cloud_api20160714_models.AddTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: AddTrafficSpecialControlRequest
+        @return: AddTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_traffic_special_control_with_options(request, runtime)
 
     async def add_traffic_special_control_async(
         self,
         request: cloud_api20160714_models.AddTrafficSpecialControlRequest,
     ) -> cloud_api20160714_models.AddTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: AddTrafficSpecialControlRequest
+        @return: AddTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.add_traffic_special_control_with_options_async(request, runtime)
 
     def attach_plugin_with_options(
         self,
         request: cloud_api20160714_models.AttachPluginRequest,
         runtime: util_models.RuntimeOptions,
@@ -646,14 +726,16 @@
         request: cloud_api20160714_models.CreateAccessControlListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateAccessControlListResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_name):
             query['AclName'] = request.acl_name
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateAccessControlList',
@@ -676,14 +758,16 @@
         request: cloud_api20160714_models.CreateAccessControlListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateAccessControlListResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_name):
             query['AclName'] = request.acl_name
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateAccessControlList',
@@ -716,72 +800,84 @@
         return await self.create_access_control_list_with_options_async(request, runtime)
 
     def create_api_with_options(
         self,
         request: cloud_api20160714_models.CreateApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateApiResponse:
+        """
+        This operation is intended for API providers.
+        *   The name of each API within the same group must be unique.
+        *   Each request path within the same group must be unique.
+        *   The QPS limit on this operation is 50 per user.
+        
+        @param request: CreateApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_signature_method):
             query['AllowSignatureMethod'] = request.allow_signature_method
         if not UtilClient.is_unset(request.api_name):
             query['ApiName'] = request.api_name
         if not UtilClient.is_unset(request.app_code_auth_type):
             query['AppCodeAuthType'] = request.app_code_auth_type
         if not UtilClient.is_unset(request.auth_type):
             query['AuthType'] = request.auth_type
         if not UtilClient.is_unset(request.backend_enable):
             query['BackendEnable'] = request.backend_enable
         if not UtilClient.is_unset(request.backend_id):
             query['BackendId'] = request.backend_id
-        if not UtilClient.is_unset(request.constant_parameters):
-            query['ConstantParameters'] = request.constant_parameters
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.disable_internet):
             query['DisableInternet'] = request.disable_internet
-        if not UtilClient.is_unset(request.error_code_samples):
-            query['ErrorCodeSamples'] = request.error_code_samples
-        if not UtilClient.is_unset(request.fail_result_sample):
-            query['FailResultSample'] = request.fail_result_sample
         if not UtilClient.is_unset(request.force_nonce_check):
             query['ForceNonceCheck'] = request.force_nonce_check
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.open_id_connect_config):
             query['OpenIdConnectConfig'] = request.open_id_connect_config
         if not UtilClient.is_unset(request.request_config):
             query['RequestConfig'] = request.request_config
-        if not UtilClient.is_unset(request.request_parameters):
-            query['RequestParameters'] = request.request_parameters
         if not UtilClient.is_unset(request.result_body_model):
             query['ResultBodyModel'] = request.result_body_model
-        if not UtilClient.is_unset(request.result_descriptions):
-            query['ResultDescriptions'] = request.result_descriptions
-        if not UtilClient.is_unset(request.result_sample):
-            query['ResultSample'] = request.result_sample
         if not UtilClient.is_unset(request.result_type):
             query['ResultType'] = request.result_type
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.service_config):
             query['ServiceConfig'] = request.service_config
-        if not UtilClient.is_unset(request.service_parameters):
-            query['ServiceParameters'] = request.service_parameters
-        if not UtilClient.is_unset(request.service_parameters_map):
-            query['ServiceParametersMap'] = request.service_parameters_map
-        if not UtilClient.is_unset(request.system_parameters):
-            query['SystemParameters'] = request.system_parameters
         if not UtilClient.is_unset(request.visibility):
             query['Visibility'] = request.visibility
         if not UtilClient.is_unset(request.web_socket_api_type):
             query['WebSocketApiType'] = request.web_socket_api_type
+        body = {}
+        if not UtilClient.is_unset(request.constant_parameters):
+            body['ConstantParameters'] = request.constant_parameters
+        if not UtilClient.is_unset(request.error_code_samples):
+            body['ErrorCodeSamples'] = request.error_code_samples
+        if not UtilClient.is_unset(request.fail_result_sample):
+            body['FailResultSample'] = request.fail_result_sample
+        if not UtilClient.is_unset(request.request_parameters):
+            body['RequestParameters'] = request.request_parameters
+        if not UtilClient.is_unset(request.result_descriptions):
+            body['ResultDescriptions'] = request.result_descriptions
+        if not UtilClient.is_unset(request.result_sample):
+            body['ResultSample'] = request.result_sample
+        if not UtilClient.is_unset(request.service_parameters):
+            body['ServiceParameters'] = request.service_parameters
+        if not UtilClient.is_unset(request.service_parameters_map):
+            body['ServiceParametersMap'] = request.service_parameters_map
+        if not UtilClient.is_unset(request.system_parameters):
+            body['SystemParameters'] = request.system_parameters
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateApi',
             version='2016-07-14',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -796,72 +892,84 @@
         )
 
     async def create_api_with_options_async(
         self,
         request: cloud_api20160714_models.CreateApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateApiResponse:
+        """
+        This operation is intended for API providers.
+        *   The name of each API within the same group must be unique.
+        *   Each request path within the same group must be unique.
+        *   The QPS limit on this operation is 50 per user.
+        
+        @param request: CreateApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_signature_method):
             query['AllowSignatureMethod'] = request.allow_signature_method
         if not UtilClient.is_unset(request.api_name):
             query['ApiName'] = request.api_name
         if not UtilClient.is_unset(request.app_code_auth_type):
             query['AppCodeAuthType'] = request.app_code_auth_type
         if not UtilClient.is_unset(request.auth_type):
             query['AuthType'] = request.auth_type
         if not UtilClient.is_unset(request.backend_enable):
             query['BackendEnable'] = request.backend_enable
         if not UtilClient.is_unset(request.backend_id):
             query['BackendId'] = request.backend_id
-        if not UtilClient.is_unset(request.constant_parameters):
-            query['ConstantParameters'] = request.constant_parameters
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.disable_internet):
             query['DisableInternet'] = request.disable_internet
-        if not UtilClient.is_unset(request.error_code_samples):
-            query['ErrorCodeSamples'] = request.error_code_samples
-        if not UtilClient.is_unset(request.fail_result_sample):
-            query['FailResultSample'] = request.fail_result_sample
         if not UtilClient.is_unset(request.force_nonce_check):
             query['ForceNonceCheck'] = request.force_nonce_check
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.open_id_connect_config):
             query['OpenIdConnectConfig'] = request.open_id_connect_config
         if not UtilClient.is_unset(request.request_config):
             query['RequestConfig'] = request.request_config
-        if not UtilClient.is_unset(request.request_parameters):
-            query['RequestParameters'] = request.request_parameters
         if not UtilClient.is_unset(request.result_body_model):
             query['ResultBodyModel'] = request.result_body_model
-        if not UtilClient.is_unset(request.result_descriptions):
-            query['ResultDescriptions'] = request.result_descriptions
-        if not UtilClient.is_unset(request.result_sample):
-            query['ResultSample'] = request.result_sample
         if not UtilClient.is_unset(request.result_type):
             query['ResultType'] = request.result_type
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.service_config):
             query['ServiceConfig'] = request.service_config
-        if not UtilClient.is_unset(request.service_parameters):
-            query['ServiceParameters'] = request.service_parameters
-        if not UtilClient.is_unset(request.service_parameters_map):
-            query['ServiceParametersMap'] = request.service_parameters_map
-        if not UtilClient.is_unset(request.system_parameters):
-            query['SystemParameters'] = request.system_parameters
         if not UtilClient.is_unset(request.visibility):
             query['Visibility'] = request.visibility
         if not UtilClient.is_unset(request.web_socket_api_type):
             query['WebSocketApiType'] = request.web_socket_api_type
+        body = {}
+        if not UtilClient.is_unset(request.constant_parameters):
+            body['ConstantParameters'] = request.constant_parameters
+        if not UtilClient.is_unset(request.error_code_samples):
+            body['ErrorCodeSamples'] = request.error_code_samples
+        if not UtilClient.is_unset(request.fail_result_sample):
+            body['FailResultSample'] = request.fail_result_sample
+        if not UtilClient.is_unset(request.request_parameters):
+            body['RequestParameters'] = request.request_parameters
+        if not UtilClient.is_unset(request.result_descriptions):
+            body['ResultDescriptions'] = request.result_descriptions
+        if not UtilClient.is_unset(request.result_sample):
+            body['ResultSample'] = request.result_sample
+        if not UtilClient.is_unset(request.service_parameters):
+            body['ServiceParameters'] = request.service_parameters
+        if not UtilClient.is_unset(request.service_parameters_map):
+            body['ServiceParametersMap'] = request.service_parameters_map
+        if not UtilClient.is_unset(request.system_parameters):
+            body['SystemParameters'] = request.system_parameters
         req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateApi',
             version='2016-07-14',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -875,21 +983,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_api(
         self,
         request: cloud_api20160714_models.CreateApiRequest,
     ) -> cloud_api20160714_models.CreateApiResponse:
+        """
+        This operation is intended for API providers.
+        *   The name of each API within the same group must be unique.
+        *   Each request path within the same group must be unique.
+        *   The QPS limit on this operation is 50 per user.
+        
+        @param request: CreateApiRequest
+        @return: CreateApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_api_with_options(request, runtime)
 
     async def create_api_async(
         self,
         request: cloud_api20160714_models.CreateApiRequest,
     ) -> cloud_api20160714_models.CreateApiResponse:
+        """
+        This operation is intended for API providers.
+        *   The name of each API within the same group must be unique.
+        *   Each request path within the same group must be unique.
+        *   The QPS limit on this operation is 50 per user.
+        
+        @param request: CreateApiRequest
+        @return: CreateApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_api_with_options_async(request, runtime)
 
     def create_api_group_with_options(
         self,
         request: cloud_api20160714_models.CreateApiGroupRequest,
         runtime: util_models.RuntimeOptions,
@@ -1086,18 +1212,18 @@
             query['AppKey'] = request.app_key
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.app_secret):
             query['AppSecret'] = request.app_secret
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
+        if not UtilClient.is_unset(request.extend):
+            query['Extend'] = request.extend
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
-        if not UtilClient.is_unset(request.source):
-            query['Source'] = request.source
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateApp',
@@ -1128,18 +1254,18 @@
             query['AppKey'] = request.app_key
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.app_secret):
             query['AppSecret'] = request.app_secret
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
+        if not UtilClient.is_unset(request.extend):
+            query['Extend'] = request.extend
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
-        if not UtilClient.is_unset(request.source):
-            query['Source'] = request.source
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateApp',
@@ -1522,24 +1648,34 @@
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.https_policy):
             query['HttpsPolicy'] = request.https_policy
+        if not UtilClient.is_unset(request.instance_cidr):
+            query['InstanceCidr'] = request.instance_cidr
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.instance_spec):
             query['InstanceSpec'] = request.instance_spec
+        if not UtilClient.is_unset(request.instance_type):
+            query['InstanceType'] = request.instance_type
         if not UtilClient.is_unset(request.pricing_cycle):
             query['PricingCycle'] = request.pricing_cycle
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.token):
             query['Token'] = request.token
+        if not UtilClient.is_unset(request.user_vpc_id):
+            query['UserVpcId'] = request.user_vpc_id
         if not UtilClient.is_unset(request.zone_id):
             query['ZoneId'] = request.zone_id
+        if not UtilClient.is_unset(request.zone_vswitch_security_group):
+            query['ZoneVSwitchSecurityGroup'] = request.zone_vswitch_security_group
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateInstance',
             version='2016-07-14',
             protocol='HTTPS',
@@ -1566,24 +1702,34 @@
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.https_policy):
             query['HttpsPolicy'] = request.https_policy
+        if not UtilClient.is_unset(request.instance_cidr):
+            query['InstanceCidr'] = request.instance_cidr
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.instance_spec):
             query['InstanceSpec'] = request.instance_spec
+        if not UtilClient.is_unset(request.instance_type):
+            query['InstanceType'] = request.instance_type
         if not UtilClient.is_unset(request.pricing_cycle):
             query['PricingCycle'] = request.pricing_cycle
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.token):
             query['Token'] = request.token
+        if not UtilClient.is_unset(request.user_vpc_id):
+            query['UserVpcId'] = request.user_vpc_id
         if not UtilClient.is_unset(request.zone_id):
             query['ZoneId'] = request.zone_id
+        if not UtilClient.is_unset(request.zone_vswitch_security_group):
+            query['ZoneVSwitchSecurityGroup'] = request.zone_vswitch_security_group
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateInstance',
             version='2016-07-14',
             protocol='HTTPS',
@@ -1856,14 +2002,22 @@
         return await self.create_log_config_with_options_async(request, runtime)
 
     def create_model_with_options(
         self,
         request: cloud_api20160714_models.CreateModelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateModelResponse:
+        """
+        For more information about the model definition, see [JSON Schema Draft 4](https://tools.ietf.org/html/draft-zyp-json-schema-04?spm=a2c4g.11186623.2.10.2e977ff7p4BpQd).
+        *   JSON Schema supports only element attributes of the Object type.
+        
+        @param request: CreateModelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateModelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.model_name):
@@ -1890,14 +2044,22 @@
         )
 
     async def create_model_with_options_async(
         self,
         request: cloud_api20160714_models.CreateModelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateModelResponse:
+        """
+        For more information about the model definition, see [JSON Schema Draft 4](https://tools.ietf.org/html/draft-zyp-json-schema-04?spm=a2c4g.11186623.2.10.2e977ff7p4BpQd).
+        *   JSON Schema supports only element attributes of the Object type.
+        
+        @param request: CreateModelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateModelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.model_name):
@@ -1923,21 +2085,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_model(
         self,
         request: cloud_api20160714_models.CreateModelRequest,
     ) -> cloud_api20160714_models.CreateModelResponse:
+        """
+        For more information about the model definition, see [JSON Schema Draft 4](https://tools.ietf.org/html/draft-zyp-json-schema-04?spm=a2c4g.11186623.2.10.2e977ff7p4BpQd).
+        *   JSON Schema supports only element attributes of the Object type.
+        
+        @param request: CreateModelRequest
+        @return: CreateModelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_model_with_options(request, runtime)
 
     async def create_model_async(
         self,
         request: cloud_api20160714_models.CreateModelRequest,
     ) -> cloud_api20160714_models.CreateModelResponse:
+        """
+        For more information about the model definition, see [JSON Schema Draft 4](https://tools.ietf.org/html/draft-zyp-json-schema-04?spm=a2c4g.11186623.2.10.2e977ff7p4BpQd).
+        *   JSON Schema supports only element attributes of the Object type.
+        
+        @param request: CreateModelRequest
+        @return: CreateModelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_model_with_options_async(request, runtime)
 
     def create_monitor_group_with_options(
         self,
         request: cloud_api20160714_models.CreateMonitorGroupRequest,
         runtime: util_models.RuntimeOptions,
@@ -2110,14 +2286,21 @@
         return await self.create_plugin_with_options_async(request, runtime)
 
     def create_signature_with_options(
         self,
         request: cloud_api20160714_models.CreateSignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateSignatureResponse:
+        """
+        The Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: CreateSignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_key):
             query['SignatureKey'] = request.signature_key
         if not UtilClient.is_unset(request.signature_name):
@@ -2144,14 +2327,21 @@
         )
 
     async def create_signature_with_options_async(
         self,
         request: cloud_api20160714_models.CreateSignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateSignatureResponse:
+        """
+        The Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: CreateSignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_key):
             query['SignatureKey'] = request.signature_key
         if not UtilClient.is_unset(request.signature_name):
@@ -2177,29 +2367,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_signature(
         self,
         request: cloud_api20160714_models.CreateSignatureRequest,
     ) -> cloud_api20160714_models.CreateSignatureResponse:
+        """
+        The Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: CreateSignatureRequest
+        @return: CreateSignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_signature_with_options(request, runtime)
 
     async def create_signature_async(
         self,
         request: cloud_api20160714_models.CreateSignatureRequest,
     ) -> cloud_api20160714_models.CreateSignatureResponse:
+        """
+        The Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: CreateSignatureRequest
+        @return: CreateSignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_signature_with_options_async(request, runtime)
 
     def create_traffic_control_with_options(
         self,
         request: cloud_api20160714_models.CreateTrafficControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateTrafficControlResponse:
+        """
+        ThrottlingTest
+        
+        @param request: CreateTrafficControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_default):
             query['ApiDefault'] = request.api_default
         if not UtilClient.is_unset(request.app_default):
             query['AppDefault'] = request.app_default
         if not UtilClient.is_unset(request.description):
@@ -2232,14 +2441,21 @@
         )
 
     async def create_traffic_control_with_options_async(
         self,
         request: cloud_api20160714_models.CreateTrafficControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.CreateTrafficControlResponse:
+        """
+        ThrottlingTest
+        
+        @param request: CreateTrafficControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_default):
             query['ApiDefault'] = request.api_default
         if not UtilClient.is_unset(request.app_default):
             query['AppDefault'] = request.app_default
         if not UtilClient.is_unset(request.description):
@@ -2271,21 +2487,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_traffic_control(
         self,
         request: cloud_api20160714_models.CreateTrafficControlRequest,
     ) -> cloud_api20160714_models.CreateTrafficControlResponse:
+        """
+        ThrottlingTest
+        
+        @param request: CreateTrafficControlRequest
+        @return: CreateTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_traffic_control_with_options(request, runtime)
 
     async def create_traffic_control_async(
         self,
         request: cloud_api20160714_models.CreateTrafficControlRequest,
     ) -> cloud_api20160714_models.CreateTrafficControlResponse:
+        """
+        ThrottlingTest
+        
+        @param request: CreateTrafficControlRequest
+        @return: CreateTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_traffic_control_with_options_async(request, runtime)
 
     def delete_access_control_list_with_options(
         self,
         request: cloud_api20160714_models.DeleteAccessControlListRequest,
         runtime: util_models.RuntimeOptions,
@@ -2360,14 +2588,21 @@
         return await self.delete_access_control_list_with_options_async(request, runtime)
 
     def delete_all_traffic_special_control_with_options(
         self,
         request: cloud_api20160714_models.DeleteAllTrafficSpecialControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteAllTrafficSpecialControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteAllTrafficSpecialControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAllTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.traffic_control_id):
             query['TrafficControlId'] = request.traffic_control_id
         req = open_api_models.OpenApiRequest(
@@ -2390,14 +2625,21 @@
         )
 
     async def delete_all_traffic_special_control_with_options_async(
         self,
         request: cloud_api20160714_models.DeleteAllTrafficSpecialControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteAllTrafficSpecialControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteAllTrafficSpecialControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAllTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.traffic_control_id):
             query['TrafficControlId'] = request.traffic_control_id
         req = open_api_models.OpenApiRequest(
@@ -2419,21 +2661,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_all_traffic_special_control(
         self,
         request: cloud_api20160714_models.DeleteAllTrafficSpecialControlRequest,
     ) -> cloud_api20160714_models.DeleteAllTrafficSpecialControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteAllTrafficSpecialControlRequest
+        @return: DeleteAllTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_all_traffic_special_control_with_options(request, runtime)
 
     async def delete_all_traffic_special_control_async(
         self,
         request: cloud_api20160714_models.DeleteAllTrafficSpecialControlRequest,
     ) -> cloud_api20160714_models.DeleteAllTrafficSpecialControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteAllTrafficSpecialControlRequest
+        @return: DeleteAllTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_all_traffic_special_control_with_options_async(request, runtime)
 
     def delete_api_with_options(
         self,
         request: cloud_api20160714_models.DeleteApiRequest,
         runtime: util_models.RuntimeOptions,
@@ -3058,14 +3312,21 @@
         return await self.delete_dataset_item_with_options_async(request, runtime)
 
     def delete_domain_with_options(
         self,
         request: cloud_api20160714_models.DeleteDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteDomainResponse:
+        """
+        The custom domain name.
+        
+        @param request: DeleteDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -3090,14 +3351,21 @@
         )
 
     async def delete_domain_with_options_async(
         self,
         request: cloud_api20160714_models.DeleteDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteDomainResponse:
+        """
+        The custom domain name.
+        
+        @param request: DeleteDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -3121,21 +3389,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_domain(
         self,
         request: cloud_api20160714_models.DeleteDomainRequest,
     ) -> cloud_api20160714_models.DeleteDomainResponse:
+        """
+        The custom domain name.
+        
+        @param request: DeleteDomainRequest
+        @return: DeleteDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_domain_with_options(request, runtime)
 
     async def delete_domain_async(
         self,
         request: cloud_api20160714_models.DeleteDomainRequest,
     ) -> cloud_api20160714_models.DeleteDomainResponse:
+        """
+        The custom domain name.
+        
+        @param request: DeleteDomainRequest
+        @return: DeleteDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_domain_with_options_async(request, runtime)
 
     def delete_domain_certificate_with_options(
         self,
         request: cloud_api20160714_models.DeleteDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
@@ -3292,14 +3572,21 @@
         return await self.delete_instance_with_options_async(request, runtime)
 
     def delete_ip_control_with_options(
         self,
         request: cloud_api20160714_models.DeleteIpControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteIpControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteIpControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
@@ -3322,14 +3609,21 @@
         )
 
     async def delete_ip_control_with_options_async(
         self,
         request: cloud_api20160714_models.DeleteIpControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteIpControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteIpControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
@@ -3351,21 +3645,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_ip_control(
         self,
         request: cloud_api20160714_models.DeleteIpControlRequest,
     ) -> cloud_api20160714_models.DeleteIpControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteIpControlRequest
+        @return: DeleteIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_ip_control_with_options(request, runtime)
 
     async def delete_ip_control_async(
         self,
         request: cloud_api20160714_models.DeleteIpControlRequest,
     ) -> cloud_api20160714_models.DeleteIpControlResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteIpControlRequest
+        @return: DeleteIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_ip_control_with_options_async(request, runtime)
 
     def delete_log_config_with_options(
         self,
         request: cloud_api20160714_models.DeleteLogConfigRequest,
         runtime: util_models.RuntimeOptions,
@@ -3670,14 +3976,21 @@
         return await self.delete_plugin_with_options_async(request, runtime)
 
     def delete_signature_with_options(
         self,
         request: cloud_api20160714_models.DeleteSignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteSignatureResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteSignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteSignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_id):
             query['SignatureId'] = request.signature_id
         req = open_api_models.OpenApiRequest(
@@ -3700,14 +4013,21 @@
         )
 
     async def delete_signature_with_options_async(
         self,
         request: cloud_api20160714_models.DeleteSignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteSignatureResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteSignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteSignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_id):
             query['SignatureId'] = request.signature_id
         req = open_api_models.OpenApiRequest(
@@ -3729,21 +4049,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_signature(
         self,
         request: cloud_api20160714_models.DeleteSignatureRequest,
     ) -> cloud_api20160714_models.DeleteSignatureResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteSignatureRequest
+        @return: DeleteSignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_signature_with_options(request, runtime)
 
     async def delete_signature_async(
         self,
         request: cloud_api20160714_models.DeleteSignatureRequest,
     ) -> cloud_api20160714_models.DeleteSignatureResponse:
+        """
+        The ID of the request.
+        
+        @param request: DeleteSignatureRequest
+        @return: DeleteSignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_signature_with_options_async(request, runtime)
 
     def delete_traffic_control_with_options(
         self,
         request: cloud_api20160714_models.DeleteTrafficControlRequest,
         runtime: util_models.RuntimeOptions,
@@ -3818,14 +4150,23 @@
         return await self.delete_traffic_control_with_options_async(request, runtime)
 
     def delete_traffic_special_control_with_options(
         self,
         request: cloud_api20160714_models.DeleteTrafficSpecialControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: DeleteTrafficSpecialControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.special_key):
             query['SpecialKey'] = request.special_key
         if not UtilClient.is_unset(request.special_type):
@@ -3852,14 +4193,23 @@
         )
 
     async def delete_traffic_special_control_with_options_async(
         self,
         request: cloud_api20160714_models.DeleteTrafficSpecialControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeleteTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: DeleteTrafficSpecialControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.special_key):
             query['SpecialKey'] = request.special_key
         if not UtilClient.is_unset(request.special_type):
@@ -3885,29 +4235,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_traffic_special_control(
         self,
         request: cloud_api20160714_models.DeleteTrafficSpecialControlRequest,
     ) -> cloud_api20160714_models.DeleteTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: DeleteTrafficSpecialControlRequest
+        @return: DeleteTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_traffic_special_control_with_options(request, runtime)
 
     async def delete_traffic_special_control_async(
         self,
         request: cloud_api20160714_models.DeleteTrafficSpecialControlRequest,
     ) -> cloud_api20160714_models.DeleteTrafficSpecialControlResponse:
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+        @param request: DeleteTrafficSpecialControlRequest
+        @return: DeleteTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_traffic_special_control_with_options_async(request, runtime)
 
     def deploy_api_with_options(
         self,
         request: cloud_api20160714_models.DeployApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeployApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DeployApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeployApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
@@ -3936,14 +4309,21 @@
         )
 
     async def deploy_api_with_options_async(
         self,
         request: cloud_api20160714_models.DeployApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DeployApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DeployApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeployApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
@@ -3971,21 +4351,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def deploy_api(
         self,
         request: cloud_api20160714_models.DeployApiRequest,
     ) -> cloud_api20160714_models.DeployApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DeployApiRequest
+        @return: DeployApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.deploy_api_with_options(request, runtime)
 
     async def deploy_api_async(
         self,
         request: cloud_api20160714_models.DeployApiRequest,
     ) -> cloud_api20160714_models.DeployApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DeployApiRequest
+        @return: DeployApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.deploy_api_with_options_async(request, runtime)
 
     def describe_abolish_api_task_with_options(
         self,
         request: cloud_api20160714_models.DescribeAbolishApiTaskRequest,
         runtime: util_models.RuntimeOptions,
@@ -4138,14 +4530,16 @@
         request: cloud_api20160714_models.DescribeAccessControlListsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeAccessControlListsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_name):
             query['AclName'] = request.acl_name
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
@@ -4172,14 +4566,16 @@
         request: cloud_api20160714_models.DescribeAccessControlListsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeAccessControlListsResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_name):
             query['AclName'] = request.acl_name
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
@@ -4216,14 +4612,21 @@
         return await self.describe_access_control_lists_with_options_async(request, runtime)
 
     def describe_api_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -4248,14 +4651,21 @@
         )
 
     async def describe_api_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -4279,21 +4689,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_api(
         self,
         request: cloud_api20160714_models.DescribeApiRequest,
     ) -> cloud_api20160714_models.DescribeApiResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiRequest
+        @return: DescribeApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_with_options(request, runtime)
 
     async def describe_api_async(
         self,
         request: cloud_api20160714_models.DescribeApiRequest,
     ) -> cloud_api20160714_models.DescribeApiResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiRequest
+        @return: DescribeApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_api_with_options_async(request, runtime)
 
     def describe_api_doc_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiDocRequest,
         runtime: util_models.RuntimeOptions,
@@ -4376,14 +4798,21 @@
         return await self.describe_api_doc_with_options_async(request, runtime)
 
     def describe_api_group_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiGroupResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.tag):
@@ -4408,14 +4837,21 @@
         )
 
     async def describe_api_group_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApiGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiGroupResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.tag):
@@ -4439,21 +4875,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_api_group(
         self,
         request: cloud_api20160714_models.DescribeApiGroupRequest,
     ) -> cloud_api20160714_models.DescribeApiGroupResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiGroupRequest
+        @return: DescribeApiGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_group_with_options(request, runtime)
 
     async def describe_api_group_async(
         self,
         request: cloud_api20160714_models.DescribeApiGroupRequest,
     ) -> cloud_api20160714_models.DescribeApiGroupResponse:
+        """
+        This operation is intended for API providers.
+        
+        @param request: DescribeApiGroupRequest
+        @return: DescribeApiGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_api_group_with_options_async(request, runtime)
 
     def describe_api_group_vpc_whitelist_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiGroupVpcWhitelistRequest,
         runtime: util_models.RuntimeOptions,
@@ -4630,14 +5078,23 @@
         return await self.describe_api_groups_with_options_async(request, runtime)
 
     def describe_api_histories_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiHistoriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiHistoriesResponse:
+        """
+        The name of the runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST: the test environment**\
+        
+        @param request: DescribeApiHistoriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiHistoriesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_name):
             query['ApiName'] = request.api_name
         if not UtilClient.is_unset(request.group_id):
@@ -4670,14 +5127,23 @@
         )
 
     async def describe_api_histories_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApiHistoriesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiHistoriesResponse:
+        """
+        The name of the runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST: the test environment**\
+        
+        @param request: DescribeApiHistoriesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiHistoriesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_name):
             query['ApiName'] = request.api_name
         if not UtilClient.is_unset(request.group_id):
@@ -4709,29 +5175,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_api_histories(
         self,
         request: cloud_api20160714_models.DescribeApiHistoriesRequest,
     ) -> cloud_api20160714_models.DescribeApiHistoriesResponse:
+        """
+        The name of the runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST: the test environment**\
+        
+        @param request: DescribeApiHistoriesRequest
+        @return: DescribeApiHistoriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_histories_with_options(request, runtime)
 
     async def describe_api_histories_async(
         self,
         request: cloud_api20160714_models.DescribeApiHistoriesRequest,
     ) -> cloud_api20160714_models.DescribeApiHistoriesResponse:
+        """
+        The name of the runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST: the test environment**\
+        
+        @param request: DescribeApiHistoriesRequest
+        @return: DescribeApiHistoriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_api_histories_with_options_async(request, runtime)
 
     def describe_api_history_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiHistoryResponse:
+        """
+        You can call this operation to query the definition of a specified published version of an API.
+        *   This operation is intended for API providers.
+        *   Each time an API is published, API Gateway records the publishing details, such as the time and the API definition. You can use the version number obtained from other API operations to query the details of an API definition that is published on a specific occasion.
+        
+        @param request: DescribeApiHistoryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiHistoryResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.history_version):
@@ -4760,14 +5251,23 @@
         )
 
     async def describe_api_history_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApiHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiHistoryResponse:
+        """
+        You can call this operation to query the definition of a specified published version of an API.
+        *   This operation is intended for API providers.
+        *   Each time an API is published, API Gateway records the publishing details, such as the time and the API definition. You can use the version number obtained from other API operations to query the details of an API definition that is published on a specific occasion.
+        
+        @param request: DescribeApiHistoryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiHistoryResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.history_version):
@@ -4795,29 +5295,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_api_history(
         self,
         request: cloud_api20160714_models.DescribeApiHistoryRequest,
     ) -> cloud_api20160714_models.DescribeApiHistoryResponse:
+        """
+        You can call this operation to query the definition of a specified published version of an API.
+        *   This operation is intended for API providers.
+        *   Each time an API is published, API Gateway records the publishing details, such as the time and the API definition. You can use the version number obtained from other API operations to query the details of an API definition that is published on a specific occasion.
+        
+        @param request: DescribeApiHistoryRequest
+        @return: DescribeApiHistoryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_history_with_options(request, runtime)
 
     async def describe_api_history_async(
         self,
         request: cloud_api20160714_models.DescribeApiHistoryRequest,
     ) -> cloud_api20160714_models.DescribeApiHistoryResponse:
+        """
+        You can call this operation to query the definition of a specified published version of an API.
+        *   This operation is intended for API providers.
+        *   Each time an API is published, API Gateway records the publishing details, such as the time and the API definition. You can use the version number obtained from other API operations to query the details of an API definition that is published on a specific occasion.
+        
+        @param request: DescribeApiHistoryRequest
+        @return: DescribeApiHistoryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_api_history_with_options_async(request, runtime)
 
     def describe_api_ip_controls_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiIpControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiIpControlsResponse:
+        """
+        The ID of the API group.
+        
+        @param request: DescribeApiIpControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiIpControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -4848,14 +5371,21 @@
         )
 
     async def describe_api_ip_controls_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApiIpControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiIpControlsResponse:
+        """
+        The ID of the API group.
+        
+        @param request: DescribeApiIpControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiIpControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -4885,21 +5415,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_api_ip_controls(
         self,
         request: cloud_api20160714_models.DescribeApiIpControlsRequest,
     ) -> cloud_api20160714_models.DescribeApiIpControlsResponse:
+        """
+        The ID of the API group.
+        
+        @param request: DescribeApiIpControlsRequest
+        @return: DescribeApiIpControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_ip_controls_with_options(request, runtime)
 
     async def describe_api_ip_controls_async(
         self,
         request: cloud_api20160714_models.DescribeApiIpControlsRequest,
     ) -> cloud_api20160714_models.DescribeApiIpControlsResponse:
+        """
+        The ID of the API group.
+        
+        @param request: DescribeApiIpControlsRequest
+        @return: DescribeApiIpControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_api_ip_controls_with_options_async(request, runtime)
 
     def describe_api_latency_data_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiLatencyDataRequest,
         runtime: util_models.RuntimeOptions,
@@ -5158,14 +5700,23 @@
         return await self.describe_api_qps_data_with_options_async(request, runtime)
 
     def describe_api_signatures_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiSignaturesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiSignaturesResponse:
+        """
+        The runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST**\
+        
+        @param request: DescribeApiSignaturesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiSignaturesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -5196,14 +5747,23 @@
         )
 
     async def describe_api_signatures_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApiSignaturesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiSignaturesResponse:
+        """
+        The runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST**\
+        
+        @param request: DescribeApiSignaturesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiSignaturesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -5233,29 +5793,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_api_signatures(
         self,
         request: cloud_api20160714_models.DescribeApiSignaturesRequest,
     ) -> cloud_api20160714_models.DescribeApiSignaturesResponse:
+        """
+        The runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST**\
+        
+        @param request: DescribeApiSignaturesRequest
+        @return: DescribeApiSignaturesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_signatures_with_options(request, runtime)
 
     async def describe_api_signatures_async(
         self,
         request: cloud_api20160714_models.DescribeApiSignaturesRequest,
     ) -> cloud_api20160714_models.DescribeApiSignaturesResponse:
+        """
+        The runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST**\
+        
+        @param request: DescribeApiSignaturesRequest
+        @return: DescribeApiSignaturesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_api_signatures_with_options_async(request, runtime)
 
     def describe_api_traffic_controls_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiTrafficControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiTrafficControlsResponse:
+        """
+        The runtime environment of the API. Valid values:
+        *   **RELEASE**\
+        *   **TEST**: the test environment
+        
+        @param request: DescribeApiTrafficControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiTrafficControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -5286,14 +5871,23 @@
         )
 
     async def describe_api_traffic_controls_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApiTrafficControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApiTrafficControlsResponse:
+        """
+        The runtime environment of the API. Valid values:
+        *   **RELEASE**\
+        *   **TEST**: the test environment
+        
+        @param request: DescribeApiTrafficControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApiTrafficControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -5323,21 +5917,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_api_traffic_controls(
         self,
         request: cloud_api20160714_models.DescribeApiTrafficControlsRequest,
     ) -> cloud_api20160714_models.DescribeApiTrafficControlsResponse:
+        """
+        The runtime environment of the API. Valid values:
+        *   **RELEASE**\
+        *   **TEST**: the test environment
+        
+        @param request: DescribeApiTrafficControlsRequest
+        @return: DescribeApiTrafficControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_traffic_controls_with_options(request, runtime)
 
     async def describe_api_traffic_controls_async(
         self,
         request: cloud_api20160714_models.DescribeApiTrafficControlsRequest,
     ) -> cloud_api20160714_models.DescribeApiTrafficControlsResponse:
+        """
+        The runtime environment of the API. Valid values:
+        *   **RELEASE**\
+        *   **TEST**: the test environment
+        
+        @param request: DescribeApiTrafficControlsRequest
+        @return: DescribeApiTrafficControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_api_traffic_controls_with_options_async(request, runtime)
 
     def describe_api_traffic_data_with_options(
         self,
         request: cloud_api20160714_models.DescribeApiTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
@@ -5428,14 +6038,23 @@
         return await self.describe_api_traffic_data_with_options_async(request, runtime)
 
     def describe_apis_with_options(
         self,
         request: cloud_api20160714_models.DescribeApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation returns a list of all APIs that are being defined. The basic information about these APIs is also returned in the list.
+        *   This operation returns all APIs that are being edited, regardless of their environments. The returned definitions may be different from the definitions in the environments.
+        
+        @param request: DescribeApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_method):
             query['ApiMethod'] = request.api_method
         if not UtilClient.is_unset(request.api_name):
@@ -5450,14 +6069,16 @@
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.un_deployed):
             query['UnDeployed'] = request.un_deployed
         if not UtilClient.is_unset(request.visibility):
             query['Visibility'] = request.visibility
         req = open_api_models.OpenApiRequest(
@@ -5480,14 +6101,23 @@
         )
 
     async def describe_apis_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation returns a list of all APIs that are being defined. The basic information about these APIs is also returned in the list.
+        *   This operation returns all APIs that are being edited, regardless of their environments. The returned definitions may be different from the definitions in the environments.
+        
+        @param request: DescribeApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_method):
             query['ApiMethod'] = request.api_method
         if not UtilClient.is_unset(request.api_name):
@@ -5502,14 +6132,16 @@
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.un_deployed):
             query['UnDeployed'] = request.un_deployed
         if not UtilClient.is_unset(request.visibility):
             query['Visibility'] = request.visibility
         req = open_api_models.OpenApiRequest(
@@ -5531,21 +6163,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_apis(
         self,
         request: cloud_api20160714_models.DescribeApisRequest,
     ) -> cloud_api20160714_models.DescribeApisResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation returns a list of all APIs that are being defined. The basic information about these APIs is also returned in the list.
+        *   This operation returns all APIs that are being edited, regardless of their environments. The returned definitions may be different from the definitions in the environments.
+        
+        @param request: DescribeApisRequest
+        @return: DescribeApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_with_options(request, runtime)
 
     async def describe_apis_async(
         self,
         request: cloud_api20160714_models.DescribeApisRequest,
     ) -> cloud_api20160714_models.DescribeApisResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation returns a list of all APIs that are being defined. The basic information about these APIs is also returned in the list.
+        *   This operation returns all APIs that are being edited, regardless of their environments. The returned definitions may be different from the definitions in the environments.
+        
+        @param request: DescribeApisRequest
+        @return: DescribeApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_apis_with_options_async(request, runtime)
 
     def describe_apis_by_app_with_options(
         self,
         request: cloud_api20160714_models.DescribeApisByAppRequest,
         runtime: util_models.RuntimeOptions,
@@ -5734,14 +6382,21 @@
         return await self.describe_apis_by_backend_with_options_async(request, runtime)
 
     def describe_apis_by_ip_control_with_options(
         self,
         request: cloud_api20160714_models.DescribeApisByIpControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisByIpControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByIpControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisByIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -5768,14 +6423,21 @@
         )
 
     async def describe_apis_by_ip_control_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApisByIpControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisByIpControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByIpControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisByIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -5801,29 +6463,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_apis_by_ip_control(
         self,
         request: cloud_api20160714_models.DescribeApisByIpControlRequest,
     ) -> cloud_api20160714_models.DescribeApisByIpControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByIpControlRequest
+        @return: DescribeApisByIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_by_ip_control_with_options(request, runtime)
 
     async def describe_apis_by_ip_control_async(
         self,
         request: cloud_api20160714_models.DescribeApisByIpControlRequest,
     ) -> cloud_api20160714_models.DescribeApisByIpControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByIpControlRequest
+        @return: DescribeApisByIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_apis_by_ip_control_with_options_async(request, runtime)
 
     def describe_apis_by_signature_with_options(
         self,
         request: cloud_api20160714_models.DescribeApisBySignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisBySignatureResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: DescribeApisBySignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisBySignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -5850,14 +6531,21 @@
         )
 
     async def describe_apis_by_signature_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApisBySignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisBySignatureResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: DescribeApisBySignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisBySignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -5883,29 +6571,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_apis_by_signature(
         self,
         request: cloud_api20160714_models.DescribeApisBySignatureRequest,
     ) -> cloud_api20160714_models.DescribeApisBySignatureResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: DescribeApisBySignatureRequest
+        @return: DescribeApisBySignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_by_signature_with_options(request, runtime)
 
     async def describe_apis_by_signature_async(
         self,
         request: cloud_api20160714_models.DescribeApisBySignatureRequest,
     ) -> cloud_api20160714_models.DescribeApisBySignatureResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: DescribeApisBySignatureRequest
+        @return: DescribeApisBySignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_apis_by_signature_with_options_async(request, runtime)
 
     def describe_apis_by_traffic_control_with_options(
         self,
         request: cloud_api20160714_models.DescribeApisByTrafficControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisByTrafficControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByTrafficControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisByTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -5932,14 +6639,21 @@
         )
 
     async def describe_apis_by_traffic_control_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeApisByTrafficControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeApisByTrafficControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByTrafficControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeApisByTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -5965,21 +6679,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_apis_by_traffic_control(
         self,
         request: cloud_api20160714_models.DescribeApisByTrafficControlRequest,
     ) -> cloud_api20160714_models.DescribeApisByTrafficControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByTrafficControlRequest
+        @return: DescribeApisByTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_by_traffic_control_with_options(request, runtime)
 
     async def describe_apis_by_traffic_control_async(
         self,
         request: cloud_api20160714_models.DescribeApisByTrafficControlRequest,
     ) -> cloud_api20160714_models.DescribeApisByTrafficControlResponse:
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+        @param request: DescribeApisByTrafficControlRequest
+        @return: DescribeApisByTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_apis_by_traffic_control_with_options_async(request, runtime)
 
     def describe_app_with_options(
         self,
         request: cloud_api20160714_models.DescribeAppRequest,
         runtime: util_models.RuntimeOptions,
@@ -6066,14 +6792,16 @@
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_key):
             query['AppKey'] = request.app_key
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.enable_tag_auth):
             query['EnableTagAuth'] = request.enable_tag_auth
+        if not UtilClient.is_unset(request.extend):
+            query['Extend'] = request.extend
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.sort):
@@ -6112,14 +6840,16 @@
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_key):
             query['AppKey'] = request.app_key
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.enable_tag_auth):
             query['EnableTagAuth'] = request.enable_tag_auth
+        if not UtilClient.is_unset(request.extend):
+            query['Extend'] = request.extend
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.sort):
@@ -6238,14 +6968,21 @@
         return await self.describe_app_security_with_options_async(request, runtime)
 
     def describe_apps_with_options(
         self,
         request: cloud_api20160714_models.DescribeAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeAppsResponse:
+        """
+        The ID of the app.
+        
+        @param request: DescribeAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_owner):
             query['AppOwner'] = request.app_owner
         if not UtilClient.is_unset(request.page_number):
@@ -6274,14 +7011,21 @@
         )
 
     async def describe_apps_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeAppsResponse:
+        """
+        The ID of the app.
+        
+        @param request: DescribeAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_owner):
             query['AppOwner'] = request.app_owner
         if not UtilClient.is_unset(request.page_number):
@@ -6309,29 +7053,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_apps(
         self,
         request: cloud_api20160714_models.DescribeAppsRequest,
     ) -> cloud_api20160714_models.DescribeAppsResponse:
+        """
+        The ID of the app.
+        
+        @param request: DescribeAppsRequest
+        @return: DescribeAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apps_with_options(request, runtime)
 
     async def describe_apps_async(
         self,
         request: cloud_api20160714_models.DescribeAppsRequest,
     ) -> cloud_api20160714_models.DescribeAppsResponse:
+        """
+        The ID of the app.
+        
+        @param request: DescribeAppsRequest
+        @return: DescribeAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_apps_with_options_async(request, runtime)
 
     def describe_authorized_apis_with_options(
         self,
         request: cloud_api20160714_models.DescribeAuthorizedApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeAuthorizedApisResponse:
+        """
+        The number of the page to return. Pages start from page 1. Default value: 1.
+        
+        @param request: DescribeAuthorizedApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAuthorizedApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -6358,14 +7121,21 @@
         )
 
     async def describe_authorized_apis_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeAuthorizedApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeAuthorizedApisResponse:
+        """
+        The number of the page to return. Pages start from page 1. Default value: 1.
+        
+        @param request: DescribeAuthorizedApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAuthorizedApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -6391,21 +7161,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_authorized_apis(
         self,
         request: cloud_api20160714_models.DescribeAuthorizedApisRequest,
     ) -> cloud_api20160714_models.DescribeAuthorizedApisResponse:
+        """
+        The number of the page to return. Pages start from page 1. Default value: 1.
+        
+        @param request: DescribeAuthorizedApisRequest
+        @return: DescribeAuthorizedApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_authorized_apis_with_options(request, runtime)
 
     async def describe_authorized_apis_async(
         self,
         request: cloud_api20160714_models.DescribeAuthorizedApisRequest,
     ) -> cloud_api20160714_models.DescribeAuthorizedApisResponse:
+        """
+        The number of the page to return. Pages start from page 1. Default value: 1.
+        
+        @param request: DescribeAuthorizedApisRequest
+        @return: DescribeAuthorizedApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_authorized_apis_with_options_async(request, runtime)
 
     def describe_authorized_apps_with_options(
         self,
         request: cloud_api20160714_models.DescribeAuthorizedAppsRequest,
         runtime: util_models.RuntimeOptions,
@@ -7258,14 +8040,21 @@
         return await self.describe_deployed_apis_with_options_async(request, runtime)
 
     def describe_domain_with_options(
         self,
         request: cloud_api20160714_models.DescribeDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: DescribeDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -7290,14 +8079,21 @@
         )
 
     async def describe_domain_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: DescribeDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -7321,21 +8117,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_domain(
         self,
         request: cloud_api20160714_models.DescribeDomainRequest,
     ) -> cloud_api20160714_models.DescribeDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: DescribeDomainRequest
+        @return: DescribeDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_with_options(request, runtime)
 
     async def describe_domain_async(
         self,
         request: cloud_api20160714_models.DescribeDomainRequest,
     ) -> cloud_api20160714_models.DescribeDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: DescribeDomainRequest
+        @return: DescribeDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_with_options_async(request, runtime)
 
     def describe_history_apis_with_options(
         self,
         request: cloud_api20160714_models.DescribeHistoryApisRequest,
         runtime: util_models.RuntimeOptions,
@@ -7425,14 +8233,862 @@
     async def describe_history_apis_async(
         self,
         request: cloud_api20160714_models.DescribeHistoryApisRequest,
     ) -> cloud_api20160714_models.DescribeHistoryApisResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_history_apis_with_options_async(request, runtime)
 
+    def describe_import_oastask_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeImportOASTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeImportOASTaskResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operation_id):
+            query['OperationId'] = request.operation_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeImportOASTask',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeImportOASTaskResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_import_oastask_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeImportOASTaskRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeImportOASTaskResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.operation_id):
+            query['OperationId'] = request.operation_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeImportOASTask',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeImportOASTaskResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_import_oastask(
+        self,
+        request: cloud_api20160714_models.DescribeImportOASTaskRequest,
+    ) -> cloud_api20160714_models.DescribeImportOASTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_import_oastask_with_options(request, runtime)
+
+    async def describe_import_oastask_async(
+        self,
+        request: cloud_api20160714_models.DescribeImportOASTaskRequest,
+    ) -> cloud_api20160714_models.DescribeImportOASTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_import_oastask_with_options_async(request, runtime)
+
+    def describe_instance_drop_connections_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropConnectionsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceDropConnectionsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceDropConnections',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceDropConnectionsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_drop_connections_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropConnectionsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceDropConnectionsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceDropConnections',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceDropConnectionsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_drop_connections(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropConnectionsRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceDropConnectionsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_drop_connections_with_options(request, runtime)
+
+    async def describe_instance_drop_connections_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropConnectionsRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceDropConnectionsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_drop_connections_with_options_async(request, runtime)
+
+    def describe_instance_drop_packet_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropPacketRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceDropPacketResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceDropPacket',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceDropPacketResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_drop_packet_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropPacketRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceDropPacketResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceDropPacket',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceDropPacketResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_drop_packet(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropPacketRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceDropPacketResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_drop_packet_with_options(request, runtime)
+
+    async def describe_instance_drop_packet_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceDropPacketRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceDropPacketResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_drop_packet_with_options_async(request, runtime)
+
+    def describe_instance_http_code_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceHttpCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceHttpCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceHttpCode',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceHttpCodeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_http_code_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceHttpCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceHttpCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceHttpCode',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceHttpCodeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_http_code(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceHttpCodeRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceHttpCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_http_code_with_options(request, runtime)
+
+    async def describe_instance_http_code_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceHttpCodeRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceHttpCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_http_code_with_options_async(request, runtime)
+
+    def describe_instance_latency_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceLatencyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceLatencyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceLatency',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceLatencyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_latency_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceLatencyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceLatencyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceLatency',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceLatencyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_latency(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceLatencyRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceLatencyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_latency_with_options(request, runtime)
+
+    async def describe_instance_latency_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceLatencyRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceLatencyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_latency_with_options_async(request, runtime)
+
+    def describe_instance_new_connections_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceNewConnectionsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceNewConnectionsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceNewConnections',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceNewConnectionsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_new_connections_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceNewConnectionsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceNewConnectionsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceNewConnections',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceNewConnectionsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_new_connections(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceNewConnectionsRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceNewConnectionsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_new_connections_with_options(request, runtime)
+
+    async def describe_instance_new_connections_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceNewConnectionsRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceNewConnectionsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_new_connections_with_options_async(request, runtime)
+
+    def describe_instance_packets_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstancePacketsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstancePacketsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstancePackets',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstancePacketsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_packets_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstancePacketsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstancePacketsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstancePackets',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstancePacketsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_packets(
+        self,
+        request: cloud_api20160714_models.DescribeInstancePacketsRequest,
+    ) -> cloud_api20160714_models.DescribeInstancePacketsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_packets_with_options(request, runtime)
+
+    async def describe_instance_packets_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstancePacketsRequest,
+    ) -> cloud_api20160714_models.DescribeInstancePacketsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_packets_with_options_async(request, runtime)
+
+    def describe_instance_qps_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceQpsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceQpsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceQps',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceQpsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_qps_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceQpsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceQpsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceQps',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceQpsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_qps(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceQpsRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceQpsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_qps_with_options(request, runtime)
+
+    async def describe_instance_qps_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceQpsRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceQpsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_qps_with_options_async(request, runtime)
+
+    def describe_instance_slb_connect_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceSlbConnectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceSlbConnectResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceSlbConnect',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceSlbConnectResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_slb_connect_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceSlbConnectRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceSlbConnectResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sbc_name):
+            query['SbcName'] = request.sbc_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceSlbConnect',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceSlbConnectResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_slb_connect(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceSlbConnectRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceSlbConnectResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_slb_connect_with_options(request, runtime)
+
+    async def describe_instance_slb_connect_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceSlbConnectRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceSlbConnectResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_slb_connect_with_options_async(request, runtime)
+
+    def describe_instance_traffic_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceTrafficRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceTrafficResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceTraffic',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceTrafficResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_instance_traffic_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceTrafficRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeInstanceTrafficResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.stage_name):
+            query['StageName'] = request.stage_name
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeInstanceTraffic',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeInstanceTrafficResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_instance_traffic(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceTrafficRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceTrafficResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_traffic_with_options(request, runtime)
+
+    async def describe_instance_traffic_async(
+        self,
+        request: cloud_api20160714_models.DescribeInstanceTrafficRequest,
+    ) -> cloud_api20160714_models.DescribeInstanceTrafficResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_instance_traffic_with_options_async(request, runtime)
+
     def describe_instances_with_options(
         self,
         request: cloud_api20160714_models.DescribeInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeInstancesResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7602,14 +9258,24 @@
         return await self.describe_ip_control_policy_items_with_options_async(request, runtime)
 
     def describe_ip_controls_with_options(
         self,
         request: cloud_api20160714_models.DescribeIpControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeIpControlsResponse:
+        """
+        This operation is intended for API providers.
+        *   This operation is used to query the ACLs in a region. Region is a system parameter.
+        *   You can filter the query results by ACL ID, name, or type.
+        *   This operation cannot be used to query specific policies. If you want to query specific policies, call the [DescribeIpControlPolicyItems](~~65532~~) operation.
+        
+        @param request: DescribeIpControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeIpControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.ip_control_name):
             query['IpControlName'] = request.ip_control_name
         if not UtilClient.is_unset(request.ip_control_type):
@@ -7640,14 +9306,24 @@
         )
 
     async def describe_ip_controls_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeIpControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeIpControlsResponse:
+        """
+        This operation is intended for API providers.
+        *   This operation is used to query the ACLs in a region. Region is a system parameter.
+        *   You can filter the query results by ACL ID, name, or type.
+        *   This operation cannot be used to query specific policies. If you want to query specific policies, call the [DescribeIpControlPolicyItems](~~65532~~) operation.
+        
+        @param request: DescribeIpControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeIpControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.ip_control_name):
             query['IpControlName'] = request.ip_control_name
         if not UtilClient.is_unset(request.ip_control_type):
@@ -7677,21 +9353,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_ip_controls(
         self,
         request: cloud_api20160714_models.DescribeIpControlsRequest,
     ) -> cloud_api20160714_models.DescribeIpControlsResponse:
+        """
+        This operation is intended for API providers.
+        *   This operation is used to query the ACLs in a region. Region is a system parameter.
+        *   You can filter the query results by ACL ID, name, or type.
+        *   This operation cannot be used to query specific policies. If you want to query specific policies, call the [DescribeIpControlPolicyItems](~~65532~~) operation.
+        
+        @param request: DescribeIpControlsRequest
+        @return: DescribeIpControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_ip_controls_with_options(request, runtime)
 
     async def describe_ip_controls_async(
         self,
         request: cloud_api20160714_models.DescribeIpControlsRequest,
     ) -> cloud_api20160714_models.DescribeIpControlsResponse:
+        """
+        This operation is intended for API providers.
+        *   This operation is used to query the ACLs in a region. Region is a system parameter.
+        *   You can filter the query results by ACL ID, name, or type.
+        *   This operation cannot be used to query specific policies. If you want to query specific policies, call the [DescribeIpControlPolicyItems](~~65532~~) operation.
+        
+        @param request: DescribeIpControlsRequest
+        @return: DescribeIpControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ip_controls_with_options_async(request, runtime)
 
     def describe_log_config_with_options(
         self,
         request: cloud_api20160714_models.DescribeLogConfigRequest,
         runtime: util_models.RuntimeOptions,
@@ -7840,14 +9534,21 @@
         return await self.describe_market_remains_quota_with_options_async(request, runtime)
 
     def describe_models_with_options(
         self,
         request: cloud_api20160714_models.DescribeModelsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeModelsResponse:
+        """
+        The name of the model.
+        
+        @param request: DescribeModelsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeModelsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.model_id):
             query['ModelId'] = request.model_id
         if not UtilClient.is_unset(request.model_name):
@@ -7876,14 +9577,21 @@
         )
 
     async def describe_models_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeModelsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeModelsResponse:
+        """
+        The name of the model.
+        
+        @param request: DescribeModelsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeModelsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.model_id):
             query['ModelId'] = request.model_id
         if not UtilClient.is_unset(request.model_name):
@@ -7911,24 +9619,142 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_models(
         self,
         request: cloud_api20160714_models.DescribeModelsRequest,
     ) -> cloud_api20160714_models.DescribeModelsResponse:
+        """
+        The name of the model.
+        
+        @param request: DescribeModelsRequest
+        @return: DescribeModelsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_models_with_options(request, runtime)
 
     async def describe_models_async(
         self,
         request: cloud_api20160714_models.DescribeModelsRequest,
     ) -> cloud_api20160714_models.DescribeModelsResponse:
+        """
+        The name of the model.
+        
+        @param request: DescribeModelsRequest
+        @return: DescribeModelsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_models_with_options_async(request, runtime)
 
+    def describe_plugin_apis_with_options(
+        self,
+        request: cloud_api20160714_models.DescribePluginApisRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribePluginApisResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_id):
+            query['ApiId'] = request.api_id
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.method):
+            query['Method'] = request.method
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.path):
+            query['Path'] = request.path
+        if not UtilClient.is_unset(request.plugin_id):
+            query['PluginId'] = request.plugin_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePluginApis',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribePluginApisResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_plugin_apis_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribePluginApisRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribePluginApisResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.api_id):
+            query['ApiId'] = request.api_id
+        if not UtilClient.is_unset(request.api_name):
+            query['ApiName'] = request.api_name
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.method):
+            query['Method'] = request.method
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.path):
+            query['Path'] = request.path
+        if not UtilClient.is_unset(request.plugin_id):
+            query['PluginId'] = request.plugin_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePluginApis',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribePluginApisResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_plugin_apis(
+        self,
+        request: cloud_api20160714_models.DescribePluginApisRequest,
+    ) -> cloud_api20160714_models.DescribePluginApisResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_plugin_apis_with_options(request, runtime)
+
+    async def describe_plugin_apis_async(
+        self,
+        request: cloud_api20160714_models.DescribePluginApisRequest,
+    ) -> cloud_api20160714_models.DescribePluginApisResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_plugin_apis_with_options_async(request, runtime)
+
     def describe_plugin_schemas_with_options(
         self,
         request: cloud_api20160714_models.DescribePluginSchemasRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribePluginSchemasResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -8172,20 +9998,32 @@
         return await self.describe_plugins_with_options_async(request, runtime)
 
     def describe_plugins_by_api_with_options(
         self,
         request: cloud_api20160714_models.DescribePluginsByApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribePluginsByApiResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation supports pagination.
+        
+        @param request: DescribePluginsByApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePluginsByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.stage_name):
             query['StageName'] = request.stage_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -8206,20 +10044,32 @@
         )
 
     async def describe_plugins_by_api_with_options_async(
         self,
         request: cloud_api20160714_models.DescribePluginsByApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribePluginsByApiResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation supports pagination.
+        
+        @param request: DescribePluginsByApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePluginsByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.stage_name):
             query['StageName'] = request.stage_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -8239,21 +10089,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_plugins_by_api(
         self,
         request: cloud_api20160714_models.DescribePluginsByApiRequest,
     ) -> cloud_api20160714_models.DescribePluginsByApiResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation supports pagination.
+        
+        @param request: DescribePluginsByApiRequest
+        @return: DescribePluginsByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_plugins_by_api_with_options(request, runtime)
 
     async def describe_plugins_by_api_async(
         self,
         request: cloud_api20160714_models.DescribePluginsByApiRequest,
     ) -> cloud_api20160714_models.DescribePluginsByApiResponse:
+        """
+        This operation is intended for API callers.
+        *   This operation supports pagination.
+        
+        @param request: DescribePluginsByApiRequest
+        @return: DescribePluginsByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_plugins_by_api_with_options_async(request, runtime)
 
     def describe_purchased_api_group_with_options(
         self,
         request: cloud_api20160714_models.DescribePurchasedApiGroupRequest,
         runtime: util_models.RuntimeOptions,
@@ -8578,14 +10442,21 @@
         return await self.describe_regions_with_options_async(request, runtime)
 
     def describe_signatures_with_options(
         self,
         request: cloud_api20160714_models.DescribeSignaturesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeSignaturesResponse:
+        """
+        The IDs of the keys to query.
+        
+        @param request: DescribeSignaturesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSignaturesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -8614,14 +10485,21 @@
         )
 
     async def describe_signatures_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeSignaturesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeSignaturesResponse:
+        """
+        The IDs of the keys to query.
+        
+        @param request: DescribeSignaturesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSignaturesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -8649,29 +10527,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_signatures(
         self,
         request: cloud_api20160714_models.DescribeSignaturesRequest,
     ) -> cloud_api20160714_models.DescribeSignaturesResponse:
+        """
+        The IDs of the keys to query.
+        
+        @param request: DescribeSignaturesRequest
+        @return: DescribeSignaturesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_signatures_with_options(request, runtime)
 
     async def describe_signatures_async(
         self,
         request: cloud_api20160714_models.DescribeSignaturesRequest,
     ) -> cloud_api20160714_models.DescribeSignaturesResponse:
+        """
+        The IDs of the keys to query.
+        
+        @param request: DescribeSignaturesRequest
+        @return: DescribeSignaturesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_signatures_with_options_async(request, runtime)
 
     def describe_signatures_by_api_with_options(
         self,
         request: cloud_api20160714_models.DescribeSignaturesByApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeSignaturesByApiResponse:
+        """
+        The ID of the group to which the API belongs.
+        
+        @param request: DescribeSignaturesByApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSignaturesByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -8698,14 +10595,21 @@
         )
 
     async def describe_signatures_by_api_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeSignaturesByApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeSignaturesByApiResponse:
+        """
+        The ID of the group to which the API belongs.
+        
+        @param request: DescribeSignaturesByApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSignaturesByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -8731,29 +10635,118 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_signatures_by_api(
         self,
         request: cloud_api20160714_models.DescribeSignaturesByApiRequest,
     ) -> cloud_api20160714_models.DescribeSignaturesByApiResponse:
+        """
+        The ID of the group to which the API belongs.
+        
+        @param request: DescribeSignaturesByApiRequest
+        @return: DescribeSignaturesByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_signatures_by_api_with_options(request, runtime)
 
     async def describe_signatures_by_api_async(
         self,
         request: cloud_api20160714_models.DescribeSignaturesByApiRequest,
     ) -> cloud_api20160714_models.DescribeSignaturesByApiResponse:
+        """
+        The ID of the group to which the API belongs.
+        
+        @param request: DescribeSignaturesByApiRequest
+        @return: DescribeSignaturesByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_signatures_by_api_with_options_async(request, runtime)
 
+    def describe_summary_data_with_options(
+        self,
+        request: cloud_api20160714_models.DescribeSummaryDataRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeSummaryDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeSummaryData',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeSummaryDataResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_summary_data_with_options_async(
+        self,
+        request: cloud_api20160714_models.DescribeSummaryDataRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.DescribeSummaryDataResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeSummaryData',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeSummaryDataResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_summary_data(
+        self,
+        request: cloud_api20160714_models.DescribeSummaryDataRequest,
+    ) -> cloud_api20160714_models.DescribeSummaryDataResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_summary_data_with_options(request, runtime)
+
+    async def describe_summary_data_async(
+        self,
+        request: cloud_api20160714_models.DescribeSummaryDataRequest,
+    ) -> cloud_api20160714_models.DescribeSummaryDataResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_summary_data_with_options_async(request, runtime)
+
     def describe_system_parameters_with_options(
         self,
         request: cloud_api20160714_models.DescribeSystemParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeSystemParametersResponse:
+        """
+        The returned information about system parameters. It is an array that consists of SystemParam data.
+        
+        @param request: DescribeSystemParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSystemParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -8774,14 +10767,21 @@
         )
 
     async def describe_system_parameters_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeSystemParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeSystemParametersResponse:
+        """
+        The returned information about system parameters. It is an array that consists of SystemParam data.
+        
+        @param request: DescribeSystemParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSystemParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -8801,29 +10801,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_system_parameters(
         self,
         request: cloud_api20160714_models.DescribeSystemParametersRequest,
     ) -> cloud_api20160714_models.DescribeSystemParametersResponse:
+        """
+        The returned information about system parameters. It is an array that consists of SystemParam data.
+        
+        @param request: DescribeSystemParametersRequest
+        @return: DescribeSystemParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_system_parameters_with_options(request, runtime)
 
     async def describe_system_parameters_async(
         self,
         request: cloud_api20160714_models.DescribeSystemParametersRequest,
     ) -> cloud_api20160714_models.DescribeSystemParametersResponse:
+        """
+        The returned information about system parameters. It is an array that consists of SystemParam data.
+        
+        @param request: DescribeSystemParametersRequest
+        @return: DescribeSystemParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_system_parameters_with_options_async(request, runtime)
 
     def describe_traffic_controls_with_options(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeTrafficControlsResponse:
+        """
+        The specified group ID. This parameter must be specified together with ApiId and StageName.
+        
+        @param request: DescribeTrafficControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTrafficControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -8858,14 +10877,21 @@
         )
 
     async def describe_traffic_controls_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeTrafficControlsResponse:
+        """
+        The specified group ID. This parameter must be specified together with ApiId and StageName.
+        
+        @param request: DescribeTrafficControlsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTrafficControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -8899,29 +10925,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_traffic_controls(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsRequest,
     ) -> cloud_api20160714_models.DescribeTrafficControlsResponse:
+        """
+        The specified group ID. This parameter must be specified together with ApiId and StageName.
+        
+        @param request: DescribeTrafficControlsRequest
+        @return: DescribeTrafficControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_traffic_controls_with_options(request, runtime)
 
     async def describe_traffic_controls_async(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsRequest,
     ) -> cloud_api20160714_models.DescribeTrafficControlsResponse:
+        """
+        The specified group ID. This parameter must be specified together with ApiId and StageName.
+        
+        @param request: DescribeTrafficControlsRequest
+        @return: DescribeTrafficControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_traffic_controls_with_options_async(request, runtime)
 
     def describe_traffic_controls_by_api_with_options(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsByApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeTrafficControlsByApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DescribeTrafficControlsByApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTrafficControlsByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -8948,14 +10993,21 @@
         )
 
     async def describe_traffic_controls_by_api_with_options_async(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsByApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DescribeTrafficControlsByApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DescribeTrafficControlsByApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTrafficControlsByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -8981,21 +11033,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_traffic_controls_by_api(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsByApiRequest,
     ) -> cloud_api20160714_models.DescribeTrafficControlsByApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DescribeTrafficControlsByApiRequest
+        @return: DescribeTrafficControlsByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_traffic_controls_by_api_with_options(request, runtime)
 
     async def describe_traffic_controls_by_api_async(
         self,
         request: cloud_api20160714_models.DescribeTrafficControlsByApiRequest,
     ) -> cloud_api20160714_models.DescribeTrafficControlsByApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: DescribeTrafficControlsByApiRequest
+        @return: DescribeTrafficControlsByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_traffic_controls_by_api_with_options_async(request, runtime)
 
     def describe_update_backend_task_with_options(
         self,
         request: cloud_api20160714_models.DescribeUpdateBackendTaskRequest,
         runtime: util_models.RuntimeOptions,
@@ -9406,14 +11470,16 @@
         request: cloud_api20160714_models.DisableInstanceAccessControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DisableInstanceAccessControlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -9438,14 +11504,16 @@
         request: cloud_api20160714_models.DisableInstanceAccessControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.DisableInstanceAccessControlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -9588,14 +11656,16 @@
     ) -> cloud_api20160714_models.EnableInstanceAccessControlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_type):
             query['AclType'] = request.acl_type
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -9622,14 +11692,16 @@
     ) -> cloud_api20160714_models.EnableInstanceAccessControlResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
             query['AclId'] = request.acl_id
         if not UtilClient.is_unset(request.acl_type):
             query['AclType'] = request.acl_type
+        if not UtilClient.is_unset(request.address_ipversion):
+            query['AddressIPVersion'] = request.address_ipversion
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -9659,19 +11731,136 @@
     async def enable_instance_access_control_async(
         self,
         request: cloud_api20160714_models.EnableInstanceAccessControlRequest,
     ) -> cloud_api20160714_models.EnableInstanceAccessControlResponse:
         runtime = util_models.RuntimeOptions()
         return await self.enable_instance_access_control_with_options_async(request, runtime)
 
+    def import_oaswith_options(
+        self,
+        request: cloud_api20160714_models.ImportOASRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.ImportOASResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_type):
+            query['AuthType'] = request.auth_type
+        if not UtilClient.is_unset(request.backend_name):
+            query['BackendName'] = request.backend_name
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.ignore_warning):
+            query['IgnoreWarning'] = request.ignore_warning
+        if not UtilClient.is_unset(request.oasversion):
+            query['OASVersion'] = request.oasversion
+        if not UtilClient.is_unset(request.overwrite):
+            query['Overwrite'] = request.overwrite
+        if not UtilClient.is_unset(request.request_mode):
+            query['RequestMode'] = request.request_mode
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.skip_dry_run):
+            query['SkipDryRun'] = request.skip_dry_run
+        body = {}
+        if not UtilClient.is_unset(request.data):
+            body['Data'] = request.data
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ImportOAS',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.ImportOASResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def import_oaswith_options_async(
+        self,
+        request: cloud_api20160714_models.ImportOASRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.ImportOASResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_type):
+            query['AuthType'] = request.auth_type
+        if not UtilClient.is_unset(request.backend_name):
+            query['BackendName'] = request.backend_name
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.ignore_warning):
+            query['IgnoreWarning'] = request.ignore_warning
+        if not UtilClient.is_unset(request.oasversion):
+            query['OASVersion'] = request.oasversion
+        if not UtilClient.is_unset(request.overwrite):
+            query['Overwrite'] = request.overwrite
+        if not UtilClient.is_unset(request.request_mode):
+            query['RequestMode'] = request.request_mode
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.skip_dry_run):
+            query['SkipDryRun'] = request.skip_dry_run
+        body = {}
+        if not UtilClient.is_unset(request.data):
+            body['Data'] = request.data
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ImportOAS',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.ImportOASResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def import_oas(
+        self,
+        request: cloud_api20160714_models.ImportOASRequest,
+    ) -> cloud_api20160714_models.ImportOASResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.import_oaswith_options(request, runtime)
+
+    async def import_oas_async(
+        self,
+        request: cloud_api20160714_models.ImportOASRequest,
+    ) -> cloud_api20160714_models.ImportOASResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.import_oaswith_options_async(request, runtime)
+
     def import_swagger_with_options(
         self,
         tmp_req: cloud_api20160714_models.ImportSwaggerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ImportSwaggerResponse:
+        """
+        0009db9c828549768a200320714b8930
+        
+        @param tmp_req: ImportSwaggerRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ImportSwaggerResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = cloud_api20160714_models.ImportSwaggerShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.global_condition):
             request.global_condition_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.global_condition, 'GlobalCondition', 'json')
         query = {}
         if not UtilClient.is_unset(request.data_format):
@@ -9710,14 +11899,21 @@
         )
 
     async def import_swagger_with_options_async(
         self,
         tmp_req: cloud_api20160714_models.ImportSwaggerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ImportSwaggerResponse:
+        """
+        0009db9c828549768a200320714b8930
+        
+        @param tmp_req: ImportSwaggerRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ImportSwaggerResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = cloud_api20160714_models.ImportSwaggerShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.global_condition):
             request.global_condition_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.global_condition, 'GlobalCondition', 'json')
         query = {}
         if not UtilClient.is_unset(request.data_format):
@@ -9755,21 +11951,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def import_swagger(
         self,
         request: cloud_api20160714_models.ImportSwaggerRequest,
     ) -> cloud_api20160714_models.ImportSwaggerResponse:
+        """
+        0009db9c828549768a200320714b8930
+        
+        @param request: ImportSwaggerRequest
+        @return: ImportSwaggerResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.import_swagger_with_options(request, runtime)
 
     async def import_swagger_async(
         self,
         request: cloud_api20160714_models.ImportSwaggerRequest,
     ) -> cloud_api20160714_models.ImportSwaggerResponse:
+        """
+        0009db9c828549768a200320714b8930
+        
+        @param request: ImportSwaggerRequest
+        @return: ImportSwaggerResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.import_swagger_with_options_async(request, runtime)
 
     def list_tag_resources_with_options(
         self,
         request: cloud_api20160714_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
@@ -9852,14 +12060,21 @@
         return await self.list_tag_resources_with_options_async(request, runtime)
 
     def modify_api_with_options(
         self,
         request: cloud_api20160714_models.ModifyApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyApiResponse:
+        """
+        58928
+        
+        @param request: ModifyApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_signature_method):
             query['AllowSignatureMethod'] = request.allow_signature_method
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_name):
@@ -9934,14 +12149,21 @@
         )
 
     async def modify_api_with_options_async(
         self,
         request: cloud_api20160714_models.ModifyApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyApiResponse:
+        """
+        58928
+        
+        @param request: ModifyApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_signature_method):
             query['AllowSignatureMethod'] = request.allow_signature_method
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_name):
@@ -10015,21 +12237,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_api(
         self,
         request: cloud_api20160714_models.ModifyApiRequest,
     ) -> cloud_api20160714_models.ModifyApiResponse:
+        """
+        58928
+        
+        @param request: ModifyApiRequest
+        @return: ModifyApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_api_with_options(request, runtime)
 
     async def modify_api_async(
         self,
         request: cloud_api20160714_models.ModifyApiRequest,
     ) -> cloud_api20160714_models.ModifyApiResponse:
+        """
+        58928
+        
+        @param request: ModifyApiRequest
+        @return: ModifyApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_api_with_options_async(request, runtime)
 
     def modify_api_configuration_with_options(
         self,
         request: cloud_api20160714_models.ModifyApiConfigurationRequest,
         runtime: util_models.RuntimeOptions,
@@ -10264,14 +12498,16 @@
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.passthrough_headers):
             query['PassthroughHeaders'] = request.passthrough_headers
         if not UtilClient.is_unset(request.rpc_pattern):
             query['RpcPattern'] = request.rpc_pattern
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.support_sse):
+            query['SupportSSE'] = request.support_sse
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.user_log_config):
             query['UserLogConfig'] = request.user_log_config
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -10316,14 +12552,16 @@
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.passthrough_headers):
             query['PassthroughHeaders'] = request.passthrough_headers
         if not UtilClient.is_unset(request.rpc_pattern):
             query['RpcPattern'] = request.rpc_pattern
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.support_sse):
+            query['SupportSSE'] = request.support_sse
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         if not UtilClient.is_unset(request.user_log_config):
             query['UserLogConfig'] = request.user_log_config
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -10444,14 +12682,16 @@
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
+        if not UtilClient.is_unset(request.extend):
+            query['Extend'] = request.extend
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -10480,14 +12720,16 @@
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
+        if not UtilClient.is_unset(request.extend):
+            query['Extend'] = request.extend
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -10956,14 +13198,21 @@
         return await self.modify_instance_spec_with_options_async(request, runtime)
 
     def modify_ip_control_with_options(
         self,
         request: cloud_api20160714_models.ModifyIpControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyIpControlResponse:
+        """
+        The name of the ACL. The name must be 4 to 50 characters in length, and can contain letters, digits, and underscores (\\_). The name cannot start with an underscore (\\_).
+        
+        @param request: ModifyIpControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.ip_control_name):
@@ -10990,14 +13239,21 @@
         )
 
     async def modify_ip_control_with_options_async(
         self,
         request: cloud_api20160714_models.ModifyIpControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyIpControlResponse:
+        """
+        The name of the ACL. The name must be 4 to 50 characters in length, and can contain letters, digits, and underscores (\\_). The name cannot start with an underscore (\\_).
+        
+        @param request: ModifyIpControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.ip_control_name):
@@ -11023,29 +13279,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_ip_control(
         self,
         request: cloud_api20160714_models.ModifyIpControlRequest,
     ) -> cloud_api20160714_models.ModifyIpControlResponse:
+        """
+        The name of the ACL. The name must be 4 to 50 characters in length, and can contain letters, digits, and underscores (\\_). The name cannot start with an underscore (\\_).
+        
+        @param request: ModifyIpControlRequest
+        @return: ModifyIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_ip_control_with_options(request, runtime)
 
     async def modify_ip_control_async(
         self,
         request: cloud_api20160714_models.ModifyIpControlRequest,
     ) -> cloud_api20160714_models.ModifyIpControlResponse:
+        """
+        The name of the ACL. The name must be 4 to 50 characters in length, and can contain letters, digits, and underscores (\\_). The name cannot start with an underscore (\\_).
+        
+        @param request: ModifyIpControlRequest
+        @return: ModifyIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_ip_control_with_options_async(request, runtime)
 
     def modify_ip_control_policy_item_with_options(
         self,
         request: cloud_api20160714_models.ModifyIpControlPolicyItemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyIpControlPolicyItemResponse:
+        """
+        The ID of the policy.
+        
+        @param request: ModifyIpControlPolicyItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cidr_ip):
             query['CidrIp'] = request.cidr_ip
         if not UtilClient.is_unset(request.ip_control_id):
@@ -11074,14 +13349,21 @@
         )
 
     async def modify_ip_control_policy_item_with_options_async(
         self,
         request: cloud_api20160714_models.ModifyIpControlPolicyItemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyIpControlPolicyItemResponse:
+        """
+        The ID of the policy.
+        
+        @param request: ModifyIpControlPolicyItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cidr_ip):
             query['CidrIp'] = request.cidr_ip
         if not UtilClient.is_unset(request.ip_control_id):
@@ -11109,21 +13391,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_ip_control_policy_item(
         self,
         request: cloud_api20160714_models.ModifyIpControlPolicyItemRequest,
     ) -> cloud_api20160714_models.ModifyIpControlPolicyItemResponse:
+        """
+        The ID of the policy.
+        
+        @param request: ModifyIpControlPolicyItemRequest
+        @return: ModifyIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_ip_control_policy_item_with_options(request, runtime)
 
     async def modify_ip_control_policy_item_async(
         self,
         request: cloud_api20160714_models.ModifyIpControlPolicyItemRequest,
     ) -> cloud_api20160714_models.ModifyIpControlPolicyItemResponse:
+        """
+        The ID of the policy.
+        
+        @param request: ModifyIpControlPolicyItemRequest
+        @return: ModifyIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_ip_control_policy_item_with_options_async(request, runtime)
 
     def modify_log_config_with_options(
         self,
         request: cloud_api20160714_models.ModifyLogConfigRequest,
         runtime: util_models.RuntimeOptions,
@@ -11382,14 +13676,21 @@
         return await self.modify_plugin_with_options_async(request, runtime)
 
     def modify_signature_with_options(
         self,
         request: cloud_api20160714_models.ModifySignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifySignatureResponse:
+        """
+        The new name of the key. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: ModifySignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifySignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_id):
             query['SignatureId'] = request.signature_id
         if not UtilClient.is_unset(request.signature_key):
@@ -11418,14 +13719,21 @@
         )
 
     async def modify_signature_with_options_async(
         self,
         request: cloud_api20160714_models.ModifySignatureRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifySignatureResponse:
+        """
+        The new name of the key. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: ModifySignatureRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifySignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_id):
             query['SignatureId'] = request.signature_id
         if not UtilClient.is_unset(request.signature_key):
@@ -11453,29 +13761,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_signature(
         self,
         request: cloud_api20160714_models.ModifySignatureRequest,
     ) -> cloud_api20160714_models.ModifySignatureResponse:
+        """
+        The new name of the key. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: ModifySignatureRequest
+        @return: ModifySignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_signature_with_options(request, runtime)
 
     async def modify_signature_async(
         self,
         request: cloud_api20160714_models.ModifySignatureRequest,
     ) -> cloud_api20160714_models.ModifySignatureResponse:
+        """
+        The new name of the key. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+        @param request: ModifySignatureRequest
+        @return: ModifySignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_signature_with_options_async(request, runtime)
 
     def modify_traffic_control_with_options(
         self,
         request: cloud_api20160714_models.ModifyTrafficControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyTrafficControlResponse:
+        """
+        The throttling policy name. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It cannot start with an underscore.
+        
+        @param request: ModifyTrafficControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_default):
             query['ApiDefault'] = request.api_default
         if not UtilClient.is_unset(request.app_default):
             query['AppDefault'] = request.app_default
         if not UtilClient.is_unset(request.description):
@@ -11510,14 +13837,21 @@
         )
 
     async def modify_traffic_control_with_options_async(
         self,
         request: cloud_api20160714_models.ModifyTrafficControlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ModifyTrafficControlResponse:
+        """
+        The throttling policy name. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It cannot start with an underscore.
+        
+        @param request: ModifyTrafficControlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_default):
             query['ApiDefault'] = request.api_default
         if not UtilClient.is_unset(request.app_default):
             query['AppDefault'] = request.app_default
         if not UtilClient.is_unset(request.description):
@@ -11551,21 +13885,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_traffic_control(
         self,
         request: cloud_api20160714_models.ModifyTrafficControlRequest,
     ) -> cloud_api20160714_models.ModifyTrafficControlResponse:
+        """
+        The throttling policy name. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It cannot start with an underscore.
+        
+        @param request: ModifyTrafficControlRequest
+        @return: ModifyTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_traffic_control_with_options(request, runtime)
 
     async def modify_traffic_control_async(
         self,
         request: cloud_api20160714_models.ModifyTrafficControlRequest,
     ) -> cloud_api20160714_models.ModifyTrafficControlResponse:
+        """
+        The throttling policy name. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It cannot start with an underscore.
+        
+        @param request: ModifyTrafficControlRequest
+        @return: ModifyTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_traffic_control_with_options_async(request, runtime)
 
     def modify_vpc_access_and_update_apis_with_options(
         self,
         request: cloud_api20160714_models.ModifyVpcAccessAndUpdateApisRequest,
         runtime: util_models.RuntimeOptions,
@@ -11713,19 +14059,100 @@
         runtime = util_models.RuntimeOptions()
         return self.open_api_gateway_service_with_options(runtime)
 
     async def open_api_gateway_service_async(self) -> cloud_api20160714_models.OpenApiGatewayServiceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.open_api_gateway_service_with_options_async(runtime)
 
+    def query_request_logs_with_options(
+        self,
+        request: cloud_api20160714_models.QueryRequestLogsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.QueryRequestLogsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.request_log_id):
+            query['RequestLogId'] = request.request_log_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryRequestLogs',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.QueryRequestLogsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def query_request_logs_with_options_async(
+        self,
+        request: cloud_api20160714_models.QueryRequestLogsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.QueryRequestLogsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.request_log_id):
+            query['RequestLogId'] = request.request_log_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryRequestLogs',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.QueryRequestLogsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def query_request_logs(
+        self,
+        request: cloud_api20160714_models.QueryRequestLogsRequest,
+    ) -> cloud_api20160714_models.QueryRequestLogsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.query_request_logs_with_options(request, runtime)
+
+    async def query_request_logs_async(
+        self,
+        request: cloud_api20160714_models.QueryRequestLogsRequest,
+    ) -> cloud_api20160714_models.QueryRequestLogsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.query_request_logs_with_options_async(request, runtime)
+
     def reactivate_domain_with_options(
         self,
         request: cloud_api20160714_models.ReactivateDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ReactivateDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: ReactivateDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReactivateDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -11750,14 +14177,21 @@
         )
 
     async def reactivate_domain_with_options_async(
         self,
         request: cloud_api20160714_models.ReactivateDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ReactivateDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: ReactivateDomainRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReactivateDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -11781,21 +14215,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reactivate_domain(
         self,
         request: cloud_api20160714_models.ReactivateDomainRequest,
     ) -> cloud_api20160714_models.ReactivateDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: ReactivateDomainRequest
+        @return: ReactivateDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reactivate_domain_with_options(request, runtime)
 
     async def reactivate_domain_async(
         self,
         request: cloud_api20160714_models.ReactivateDomainRequest,
     ) -> cloud_api20160714_models.ReactivateDomainResponse:
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+        @param request: ReactivateDomainRequest
+        @return: ReactivateDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.reactivate_domain_with_options_async(request, runtime)
 
     def remove_access_control_list_entry_with_options(
         self,
         request: cloud_api20160714_models.RemoveAccessControlListEntryRequest,
         runtime: util_models.RuntimeOptions,
@@ -11874,14 +14320,21 @@
         return await self.remove_access_control_list_entry_with_options_async(request, runtime)
 
     def remove_apis_authorities_with_options(
         self,
         request: cloud_api20160714_models.RemoveApisAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveApisAuthoritiesResponse:
+        """
+        The ID of the app. The ID is generated by the system and globally unique.
+        
+        @param request: RemoveApisAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveApisAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.description):
@@ -11912,14 +14365,21 @@
         )
 
     async def remove_apis_authorities_with_options_async(
         self,
         request: cloud_api20160714_models.RemoveApisAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveApisAuthoritiesResponse:
+        """
+        The ID of the app. The ID is generated by the system and globally unique.
+        
+        @param request: RemoveApisAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveApisAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.description):
@@ -11949,29 +14409,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_apis_authorities(
         self,
         request: cloud_api20160714_models.RemoveApisAuthoritiesRequest,
     ) -> cloud_api20160714_models.RemoveApisAuthoritiesResponse:
+        """
+        The ID of the app. The ID is generated by the system and globally unique.
+        
+        @param request: RemoveApisAuthoritiesRequest
+        @return: RemoveApisAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_apis_authorities_with_options(request, runtime)
 
     async def remove_apis_authorities_async(
         self,
         request: cloud_api20160714_models.RemoveApisAuthoritiesRequest,
     ) -> cloud_api20160714_models.RemoveApisAuthoritiesResponse:
+        """
+        The ID of the app. The ID is generated by the system and globally unique.
+        
+        @param request: RemoveApisAuthoritiesRequest
+        @return: RemoveApisAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_apis_authorities_with_options_async(request, runtime)
 
     def remove_apps_authorities_with_options(
         self,
         request: cloud_api20160714_models.RemoveAppsAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: RemoveAppsAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveAppsAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.app_ids):
             query['AppIds'] = request.app_ids
         if not UtilClient.is_unset(request.group_id):
@@ -12000,14 +14479,21 @@
         )
 
     async def remove_apps_authorities_with_options_async(
         self,
         request: cloud_api20160714_models.RemoveAppsAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: RemoveAppsAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveAppsAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.app_ids):
             query['AppIds'] = request.app_ids
         if not UtilClient.is_unset(request.group_id):
@@ -12035,29 +14521,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_apps_authorities(
         self,
         request: cloud_api20160714_models.RemoveAppsAuthoritiesRequest,
     ) -> cloud_api20160714_models.RemoveAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: RemoveAppsAuthoritiesRequest
+        @return: RemoveAppsAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_apps_authorities_with_options(request, runtime)
 
     async def remove_apps_authorities_async(
         self,
         request: cloud_api20160714_models.RemoveAppsAuthoritiesRequest,
     ) -> cloud_api20160714_models.RemoveAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: RemoveAppsAuthoritiesRequest
+        @return: RemoveAppsAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_apps_authorities_with_options_async(request, runtime)
 
     def remove_ip_control_apis_with_options(
         self,
         request: cloud_api20160714_models.RemoveIpControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveIpControlApisResponse:
+        """
+        The ID of the API group containing the API to be managed.
+        
+        @param request: RemoveIpControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveIpControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.ip_control_id):
@@ -12086,14 +14591,21 @@
         )
 
     async def remove_ip_control_apis_with_options_async(
         self,
         request: cloud_api20160714_models.RemoveIpControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveIpControlApisResponse:
+        """
+        The ID of the API group containing the API to be managed.
+        
+        @param request: RemoveIpControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveIpControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.ip_control_id):
@@ -12121,29 +14633,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_ip_control_apis(
         self,
         request: cloud_api20160714_models.RemoveIpControlApisRequest,
     ) -> cloud_api20160714_models.RemoveIpControlApisResponse:
+        """
+        The ID of the API group containing the API to be managed.
+        
+        @param request: RemoveIpControlApisRequest
+        @return: RemoveIpControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_ip_control_apis_with_options(request, runtime)
 
     async def remove_ip_control_apis_async(
         self,
         request: cloud_api20160714_models.RemoveIpControlApisRequest,
     ) -> cloud_api20160714_models.RemoveIpControlApisResponse:
+        """
+        The ID of the API group containing the API to be managed.
+        
+        @param request: RemoveIpControlApisRequest
+        @return: RemoveIpControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_ip_control_apis_with_options_async(request, runtime)
 
     def remove_ip_control_policy_item_with_options(
         self,
         request: cloud_api20160714_models.RemoveIpControlPolicyItemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveIpControlPolicyItemResponse:
+        """
+        The ID of a policy. Separate multiple IDs with semicolons (;). A maximum of 100 IDs can be entered.
+        
+        @param request: RemoveIpControlPolicyItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.policy_item_ids):
             query['PolicyItemIds'] = request.policy_item_ids
         if not UtilClient.is_unset(request.security_token):
@@ -12168,14 +14699,21 @@
         )
 
     async def remove_ip_control_policy_item_with_options_async(
         self,
         request: cloud_api20160714_models.RemoveIpControlPolicyItemRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveIpControlPolicyItemResponse:
+        """
+        The ID of a policy. Separate multiple IDs with semicolons (;). A maximum of 100 IDs can be entered.
+        
+        @param request: RemoveIpControlPolicyItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.policy_item_ids):
             query['PolicyItemIds'] = request.policy_item_ids
         if not UtilClient.is_unset(request.security_token):
@@ -12199,29 +14737,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_ip_control_policy_item(
         self,
         request: cloud_api20160714_models.RemoveIpControlPolicyItemRequest,
     ) -> cloud_api20160714_models.RemoveIpControlPolicyItemResponse:
+        """
+        The ID of a policy. Separate multiple IDs with semicolons (;). A maximum of 100 IDs can be entered.
+        
+        @param request: RemoveIpControlPolicyItemRequest
+        @return: RemoveIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_ip_control_policy_item_with_options(request, runtime)
 
     async def remove_ip_control_policy_item_async(
         self,
         request: cloud_api20160714_models.RemoveIpControlPolicyItemRequest,
     ) -> cloud_api20160714_models.RemoveIpControlPolicyItemResponse:
+        """
+        The ID of a policy. Separate multiple IDs with semicolons (;). A maximum of 100 IDs can be entered.
+        
+        @param request: RemoveIpControlPolicyItemRequest
+        @return: RemoveIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_ip_control_policy_item_with_options_async(request, runtime)
 
     def remove_signature_apis_with_options(
         self,
         request: cloud_api20160714_models.RemoveSignatureApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: RemoveSignatureApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveSignatureApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -12250,14 +14807,21 @@
         )
 
     async def remove_signature_apis_with_options_async(
         self,
         request: cloud_api20160714_models.RemoveSignatureApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: RemoveSignatureApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveSignatureApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -12285,29 +14849,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_signature_apis(
         self,
         request: cloud_api20160714_models.RemoveSignatureApisRequest,
     ) -> cloud_api20160714_models.RemoveSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: RemoveSignatureApisRequest
+        @return: RemoveSignatureApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_signature_apis_with_options(request, runtime)
 
     async def remove_signature_apis_async(
         self,
         request: cloud_api20160714_models.RemoveSignatureApisRequest,
     ) -> cloud_api20160714_models.RemoveSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: RemoveSignatureApisRequest
+        @return: RemoveSignatureApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_signature_apis_with_options_async(request, runtime)
 
     def remove_traffic_control_apis_with_options(
         self,
         request: cloud_api20160714_models.RemoveTrafficControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs from which you want to unbind a specified throttling policy.
+        
+        @param request: RemoveTrafficControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveTrafficControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -12336,14 +14919,21 @@
         )
 
     async def remove_traffic_control_apis_with_options_async(
         self,
         request: cloud_api20160714_models.RemoveTrafficControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.RemoveTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs from which you want to unbind a specified throttling policy.
+        
+        @param request: RemoveTrafficControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveTrafficControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -12371,21 +14961,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_traffic_control_apis(
         self,
         request: cloud_api20160714_models.RemoveTrafficControlApisRequest,
     ) -> cloud_api20160714_models.RemoveTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs from which you want to unbind a specified throttling policy.
+        
+        @param request: RemoveTrafficControlApisRequest
+        @return: RemoveTrafficControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_traffic_control_apis_with_options(request, runtime)
 
     async def remove_traffic_control_apis_async(
         self,
         request: cloud_api20160714_models.RemoveTrafficControlApisRequest,
     ) -> cloud_api20160714_models.RemoveTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs from which you want to unbind a specified throttling policy.
+        
+        @param request: RemoveTrafficControlApisRequest
+        @return: RemoveTrafficControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_traffic_control_apis_with_options_async(request, runtime)
 
     def remove_vpc_access_with_options(
         self,
         request: cloud_api20160714_models.RemoveVpcAccessRequest,
         runtime: util_models.RuntimeOptions,
@@ -12558,14 +15160,21 @@
         return await self.remove_vpc_access_and_abolish_apis_with_options_async(request, runtime)
 
     def reset_app_code_with_options(
         self,
         request: cloud_api20160714_models.ResetAppCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ResetAppCodeResponse:
+        """
+        The new AppCode takes effect about 2 seconds after you call this operation.
+        
+        @param request: ResetAppCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetAppCodeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_code):
             query['AppCode'] = request.app_code
         if not UtilClient.is_unset(request.new_app_code):
             query['NewAppCode'] = request.new_app_code
         if not UtilClient.is_unset(request.security_token):
@@ -12590,14 +15199,21 @@
         )
 
     async def reset_app_code_with_options_async(
         self,
         request: cloud_api20160714_models.ResetAppCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ResetAppCodeResponse:
+        """
+        The new AppCode takes effect about 2 seconds after you call this operation.
+        
+        @param request: ResetAppCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetAppCodeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_code):
             query['AppCode'] = request.app_code
         if not UtilClient.is_unset(request.new_app_code):
             query['NewAppCode'] = request.new_app_code
         if not UtilClient.is_unset(request.security_token):
@@ -12621,33 +15237,56 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reset_app_code(
         self,
         request: cloud_api20160714_models.ResetAppCodeRequest,
     ) -> cloud_api20160714_models.ResetAppCodeResponse:
+        """
+        The new AppCode takes effect about 2 seconds after you call this operation.
+        
+        @param request: ResetAppCodeRequest
+        @return: ResetAppCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reset_app_code_with_options(request, runtime)
 
     async def reset_app_code_async(
         self,
         request: cloud_api20160714_models.ResetAppCodeRequest,
     ) -> cloud_api20160714_models.ResetAppCodeResponse:
+        """
+        The new AppCode takes effect about 2 seconds after you call this operation.
+        
+        @param request: ResetAppCodeRequest
+        @return: ResetAppCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.reset_app_code_with_options_async(request, runtime)
 
     def reset_app_secret_with_options(
         self,
         request: cloud_api20160714_models.ResetAppSecretRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ResetAppSecretResponse:
+        """
+        This operation is intended for API callers.
+        *   A new secret is automatically generated after you have called this operation. This secret cannot be customized.
+        *   The results returned by this operation do not contain the application secret. You can obtain the secret by calling DescribeAppSecurity.
+        
+        @param request: ResetAppSecretRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetAppSecretResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_key):
             query['AppKey'] = request.app_key
+        if not UtilClient.is_unset(request.new_app_key):
+            query['NewAppKey'] = request.new_app_key
         if not UtilClient.is_unset(request.new_app_secret):
             query['NewAppSecret'] = request.new_app_secret
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -12668,18 +15307,29 @@
         )
 
     async def reset_app_secret_with_options_async(
         self,
         request: cloud_api20160714_models.ResetAppSecretRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.ResetAppSecretResponse:
+        """
+        This operation is intended for API callers.
+        *   A new secret is automatically generated after you have called this operation. This secret cannot be customized.
+        *   The results returned by this operation do not contain the application secret. You can obtain the secret by calling DescribeAppSecurity.
+        
+        @param request: ResetAppSecretRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetAppSecretResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_key):
             query['AppKey'] = request.app_key
+        if not UtilClient.is_unset(request.new_app_key):
+            query['NewAppKey'] = request.new_app_key
         if not UtilClient.is_unset(request.new_app_secret):
             query['NewAppSecret'] = request.new_app_secret
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -12699,21 +15349,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reset_app_secret(
         self,
         request: cloud_api20160714_models.ResetAppSecretRequest,
     ) -> cloud_api20160714_models.ResetAppSecretResponse:
+        """
+        This operation is intended for API callers.
+        *   A new secret is automatically generated after you have called this operation. This secret cannot be customized.
+        *   The results returned by this operation do not contain the application secret. You can obtain the secret by calling DescribeAppSecurity.
+        
+        @param request: ResetAppSecretRequest
+        @return: ResetAppSecretResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reset_app_secret_with_options(request, runtime)
 
     async def reset_app_secret_async(
         self,
         request: cloud_api20160714_models.ResetAppSecretRequest,
     ) -> cloud_api20160714_models.ResetAppSecretResponse:
+        """
+        This operation is intended for API callers.
+        *   A new secret is automatically generated after you have called this operation. This secret cannot be customized.
+        *   The results returned by this operation do not contain the application secret. You can obtain the secret by calling DescribeAppSecurity.
+        
+        @param request: ResetAppSecretRequest
+        @return: ResetAppSecretResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.reset_app_secret_with_options_async(request, runtime)
 
     def sdk_generate_by_app_with_options(
         self,
         request: cloud_api20160714_models.SdkGenerateByAppRequest,
         runtime: util_models.RuntimeOptions,
@@ -13026,14 +15692,21 @@
         return await self.set_access_control_list_attribute_with_options_async(request, runtime)
 
     def set_apis_authorities_with_options(
         self,
         request: cloud_api20160714_models.SetApisAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetApisAuthoritiesResponse:
+        """
+        The ID of the app. This ID is generated by the system and globally unique.
+        
+        @param request: SetApisAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetApisAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.auth_valid_time):
@@ -13066,14 +15739,21 @@
         )
 
     async def set_apis_authorities_with_options_async(
         self,
         request: cloud_api20160714_models.SetApisAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetApisAuthoritiesResponse:
+        """
+        The ID of the app. This ID is generated by the system and globally unique.
+        
+        @param request: SetApisAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetApisAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.auth_valid_time):
@@ -13105,29 +15785,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_apis_authorities(
         self,
         request: cloud_api20160714_models.SetApisAuthoritiesRequest,
     ) -> cloud_api20160714_models.SetApisAuthoritiesResponse:
+        """
+        The ID of the app. This ID is generated by the system and globally unique.
+        
+        @param request: SetApisAuthoritiesRequest
+        @return: SetApisAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_apis_authorities_with_options(request, runtime)
 
     async def set_apis_authorities_async(
         self,
         request: cloud_api20160714_models.SetApisAuthoritiesRequest,
     ) -> cloud_api20160714_models.SetApisAuthoritiesResponse:
+        """
+        The ID of the app. This ID is generated by the system and globally unique.
+        
+        @param request: SetApisAuthoritiesRequest
+        @return: SetApisAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_apis_authorities_with_options_async(request, runtime)
 
     def set_apps_authorities_with_options(
         self,
         request: cloud_api20160714_models.SetAppsAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: SetAppsAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetAppsAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.app_ids):
             query['AppIds'] = request.app_ids
         if not UtilClient.is_unset(request.auth_valid_time):
@@ -13160,14 +15859,21 @@
         )
 
     async def set_apps_authorities_with_options_async(
         self,
         request: cloud_api20160714_models.SetAppsAuthoritiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: SetAppsAuthoritiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetAppsAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.app_ids):
             query['AppIds'] = request.app_ids
         if not UtilClient.is_unset(request.auth_valid_time):
@@ -13199,21 +15905,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_apps_authorities(
         self,
         request: cloud_api20160714_models.SetAppsAuthoritiesRequest,
     ) -> cloud_api20160714_models.SetAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: SetAppsAuthoritiesRequest
+        @return: SetAppsAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_apps_authorities_with_options(request, runtime)
 
     async def set_apps_authorities_async(
         self,
         request: cloud_api20160714_models.SetAppsAuthoritiesRequest,
     ) -> cloud_api20160714_models.SetAppsAuthoritiesResponse:
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+        @param request: SetAppsAuthoritiesRequest
+        @return: SetAppsAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_apps_authorities_with_options_async(request, runtime)
 
     def set_domain_with_options(
         self,
         request: cloud_api20160714_models.SetDomainRequest,
         runtime: util_models.RuntimeOptions,
@@ -13304,14 +16022,21 @@
         return await self.set_domain_with_options_async(request, runtime)
 
     def set_domain_certificate_with_options(
         self,
         request: cloud_api20160714_models.SetDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetDomainCertificateResponse:
+        """
+        382271
+        
+        @param request: SetDomainCertificateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetDomainCertificateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ca_certificate_body):
             query['CaCertificateBody'] = request.ca_certificate_body
         if not UtilClient.is_unset(request.certificate_body):
             query['CertificateBody'] = request.certificate_body
         if not UtilClient.is_unset(request.certificate_name):
@@ -13346,14 +16071,21 @@
         )
 
     async def set_domain_certificate_with_options_async(
         self,
         request: cloud_api20160714_models.SetDomainCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetDomainCertificateResponse:
+        """
+        382271
+        
+        @param request: SetDomainCertificateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetDomainCertificateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ca_certificate_body):
             query['CaCertificateBody'] = request.ca_certificate_body
         if not UtilClient.is_unset(request.certificate_body):
             query['CertificateBody'] = request.certificate_body
         if not UtilClient.is_unset(request.certificate_name):
@@ -13387,21 +16119,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_domain_certificate(
         self,
         request: cloud_api20160714_models.SetDomainCertificateRequest,
     ) -> cloud_api20160714_models.SetDomainCertificateResponse:
+        """
+        382271
+        
+        @param request: SetDomainCertificateRequest
+        @return: SetDomainCertificateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_domain_certificate_with_options(request, runtime)
 
     async def set_domain_certificate_async(
         self,
         request: cloud_api20160714_models.SetDomainCertificateRequest,
     ) -> cloud_api20160714_models.SetDomainCertificateResponse:
+        """
+        382271
+        
+        @param request: SetDomainCertificateRequest
+        @return: SetDomainCertificateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_domain_certificate_with_options_async(request, runtime)
 
     def set_domain_web_socket_status_with_options(
         self,
         request: cloud_api20160714_models.SetDomainWebSocketStatusRequest,
         runtime: util_models.RuntimeOptions,
@@ -13483,19 +16227,104 @@
     async def set_domain_web_socket_status_async(
         self,
         request: cloud_api20160714_models.SetDomainWebSocketStatusRequest,
     ) -> cloud_api20160714_models.SetDomainWebSocketStatusResponse:
         runtime = util_models.RuntimeOptions()
         return await self.set_domain_web_socket_status_with_options_async(request, runtime)
 
+    def set_group_auth_app_code_with_options(
+        self,
+        request: cloud_api20160714_models.SetGroupAuthAppCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.SetGroupAuthAppCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_app_code):
+            query['AuthAppCode'] = request.auth_app_code
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetGroupAuthAppCode',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.SetGroupAuthAppCodeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_group_auth_app_code_with_options_async(
+        self,
+        request: cloud_api20160714_models.SetGroupAuthAppCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.SetGroupAuthAppCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_app_code):
+            query['AuthAppCode'] = request.auth_app_code
+        if not UtilClient.is_unset(request.group_id):
+            query['GroupId'] = request.group_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetGroupAuthAppCode',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.SetGroupAuthAppCodeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_group_auth_app_code(
+        self,
+        request: cloud_api20160714_models.SetGroupAuthAppCodeRequest,
+    ) -> cloud_api20160714_models.SetGroupAuthAppCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_group_auth_app_code_with_options(request, runtime)
+
+    async def set_group_auth_app_code_async(
+        self,
+        request: cloud_api20160714_models.SetGroupAuthAppCodeRequest,
+    ) -> cloud_api20160714_models.SetGroupAuthAppCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_group_auth_app_code_with_options_async(request, runtime)
+
     def set_ip_control_apis_with_options(
         self,
         request: cloud_api20160714_models.SetIpControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetIpControlApisResponse:
+        """
+        The ID of the API group.
+        
+        @param request: SetIpControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetIpControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.ip_control_id):
@@ -13524,14 +16353,21 @@
         )
 
     async def set_ip_control_apis_with_options_async(
         self,
         request: cloud_api20160714_models.SetIpControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetIpControlApisResponse:
+        """
+        The ID of the API group.
+        
+        @param request: SetIpControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetIpControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.ip_control_id):
@@ -13559,29 +16395,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_ip_control_apis(
         self,
         request: cloud_api20160714_models.SetIpControlApisRequest,
     ) -> cloud_api20160714_models.SetIpControlApisResponse:
+        """
+        The ID of the API group.
+        
+        @param request: SetIpControlApisRequest
+        @return: SetIpControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_ip_control_apis_with_options(request, runtime)
 
     async def set_ip_control_apis_async(
         self,
         request: cloud_api20160714_models.SetIpControlApisRequest,
     ) -> cloud_api20160714_models.SetIpControlApisResponse:
+        """
+        The ID of the API group.
+        
+        @param request: SetIpControlApisRequest
+        @return: SetIpControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_ip_control_apis_with_options_async(request, runtime)
 
     def set_signature_apis_with_options(
         self,
         request: cloud_api20160714_models.SetSignatureApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: SetSignatureApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetSignatureApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -13610,14 +16465,21 @@
         )
 
     async def set_signature_apis_with_options_async(
         self,
         request: cloud_api20160714_models.SetSignatureApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: SetSignatureApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetSignatureApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -13645,29 +16507,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_signature_apis(
         self,
         request: cloud_api20160714_models.SetSignatureApisRequest,
     ) -> cloud_api20160714_models.SetSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: SetSignatureApisRequest
+        @return: SetSignatureApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_signature_apis_with_options(request, runtime)
 
     async def set_signature_apis_async(
         self,
         request: cloud_api20160714_models.SetSignatureApisRequest,
     ) -> cloud_api20160714_models.SetSignatureApisResponse:
+        """
+        The ID of the signature key.
+        
+        @param request: SetSignatureApisRequest
+        @return: SetSignatureApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_signature_apis_with_options_async(request, runtime)
 
     def set_traffic_control_apis_with_options(
         self,
         request: cloud_api20160714_models.SetTrafficControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs to which you want to bind a specified throttling policy.
+        
+        @param request: SetTrafficControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetTrafficControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -13696,14 +16577,21 @@
         )
 
     async def set_traffic_control_apis_with_options_async(
         self,
         request: cloud_api20160714_models.SetTrafficControlApisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SetTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs to which you want to bind a specified throttling policy.
+        
+        @param request: SetTrafficControlApisRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetTrafficControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -13731,21 +16619,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_traffic_control_apis(
         self,
         request: cloud_api20160714_models.SetTrafficControlApisRequest,
     ) -> cloud_api20160714_models.SetTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs to which you want to bind a specified throttling policy.
+        
+        @param request: SetTrafficControlApisRequest
+        @return: SetTrafficControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_traffic_control_apis_with_options(request, runtime)
 
     async def set_traffic_control_apis_async(
         self,
         request: cloud_api20160714_models.SetTrafficControlApisRequest,
     ) -> cloud_api20160714_models.SetTrafficControlApisResponse:
+        """
+        The ID of the API group containing the APIs to which you want to bind a specified throttling policy.
+        
+        @param request: SetTrafficControlApisRequest
+        @return: SetTrafficControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_traffic_control_apis_with_options_async(request, runtime)
 
     def set_vpc_access_with_options(
         self,
         request: cloud_api20160714_models.SetVpcAccessRequest,
         runtime: util_models.RuntimeOptions,
@@ -13922,14 +16822,21 @@
         return await self.set_wildcard_domain_patterns_with_options_async(request, runtime)
 
     def switch_api_with_options(
         self,
         request: cloud_api20160714_models.SwitchApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SwitchApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: SwitchApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
@@ -13960,14 +16867,21 @@
         )
 
     async def switch_api_with_options_async(
         self,
         request: cloud_api20160714_models.SwitchApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.SwitchApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: SwitchApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
@@ -13997,29 +16911,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def switch_api(
         self,
         request: cloud_api20160714_models.SwitchApiRequest,
     ) -> cloud_api20160714_models.SwitchApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: SwitchApiRequest
+        @return: SwitchApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.switch_api_with_options(request, runtime)
 
     async def switch_api_async(
         self,
         request: cloud_api20160714_models.SwitchApiRequest,
     ) -> cloud_api20160714_models.SwitchApiResponse:
+        """
+        The ID of the API.
+        
+        @param request: SwitchApiRequest
+        @return: SwitchApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.switch_api_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: cloud_api20160714_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.TagResourcesResponse:
+        """
+        The key of tag N.
+        Valid values of N: `1 to 20.`
+        
+        @param request: TagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.security_token):
@@ -14046,14 +16980,22 @@
         )
 
     async def tag_resources_with_options_async(
         self,
         request: cloud_api20160714_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.TagResourcesResponse:
+        """
+        The key of tag N.
+        Valid values of N: `1 to 20.`
+        
+        @param request: TagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.security_token):
@@ -14079,29 +17021,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def tag_resources(
         self,
         request: cloud_api20160714_models.TagResourcesRequest,
     ) -> cloud_api20160714_models.TagResourcesResponse:
+        """
+        The key of tag N.
+        Valid values of N: `1 to 20.`
+        
+        @param request: TagResourcesRequest
+        @return: TagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     async def tag_resources_async(
         self,
         request: cloud_api20160714_models.TagResourcesRequest,
     ) -> cloud_api20160714_models.TagResourcesResponse:
+        """
+        The key of tag N.
+        Valid values of N: `1 to 20.`
+        
+        @param request: TagResourcesRequest
+        @return: TagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.tag_resources_with_options_async(request, runtime)
 
     def untag_resources_with_options(
         self,
         request: cloud_api20160714_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.UntagResourcesResponse:
+        """
+        Specifies whether to delete all tags. This parameter is valid only when the *TagKey.N**parameter is not specified. Default value: false. Valid values:
+        *   **true**\
+        *   **false**\
+        
+        @param request: UntagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UntagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
@@ -14130,14 +17095,23 @@
         )
 
     async def untag_resources_with_options_async(
         self,
         request: cloud_api20160714_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloud_api20160714_models.UntagResourcesResponse:
+        """
+        Specifies whether to delete all tags. This parameter is valid only when the *TagKey.N**parameter is not specified. Default value: false. Valid values:
+        *   **true**\
+        *   **false**\
+        
+        @param request: UntagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UntagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
@@ -14165,16 +17139,110 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def untag_resources(
         self,
         request: cloud_api20160714_models.UntagResourcesRequest,
     ) -> cloud_api20160714_models.UntagResourcesResponse:
+        """
+        Specifies whether to delete all tags. This parameter is valid only when the *TagKey.N**parameter is not specified. Default value: false. Valid values:
+        *   **true**\
+        *   **false**\
+        
+        @param request: UntagResourcesRequest
+        @return: UntagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     async def untag_resources_async(
         self,
         request: cloud_api20160714_models.UntagResourcesRequest,
     ) -> cloud_api20160714_models.UntagResourcesResponse:
+        """
+        Specifies whether to delete all tags. This parameter is valid only when the *TagKey.N**parameter is not specified. Default value: false. Valid values:
+        *   **true**\
+        *   **false**\
+        
+        @param request: UntagResourcesRequest
+        @return: UntagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
+
+    def validate_vpc_connectivity_with_options(
+        self,
+        request: cloud_api20160714_models.ValidateVpcConnectivityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.ValidateVpcConnectivityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.vpc_access_id):
+            query['VpcAccessId'] = request.vpc_access_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ValidateVpcConnectivity',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.ValidateVpcConnectivityResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def validate_vpc_connectivity_with_options_async(
+        self,
+        request: cloud_api20160714_models.ValidateVpcConnectivityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloud_api20160714_models.ValidateVpcConnectivityResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.vpc_access_id):
+            query['VpcAccessId'] = request.vpc_access_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ValidateVpcConnectivity',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.ValidateVpcConnectivityResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def validate_vpc_connectivity(
+        self,
+        request: cloud_api20160714_models.ValidateVpcConnectivityRequest,
+    ) -> cloud_api20160714_models.ValidateVpcConnectivityResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.validate_vpc_connectivity_with_options(request, runtime)
+
+    async def validate_vpc_connectivity_async(
+        self,
+        request: cloud_api20160714_models.ValidateVpcConnectivityRequest,
+    ) -> cloud_api20160714_models.ValidateVpcConnectivityResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.validate_vpc_connectivity_with_options_async(request, runtime)
```

### Comparing `alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714/models.py` & `alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -234,16 +234,19 @@
     def __init__(
         self,
         app_id: str = None,
         cidr_ip: str = None,
         ip_control_id: str = None,
         security_token: str = None,
     ):
+        # The ID of the policy. The ID is unique.
         self.app_id = app_id
+        # The ID of the request.
         self.cidr_ip = cidr_ip
+        # The IP addresses or CIDR blocks involved in the policy. Separate multiple IP addresses or CIDR blocks with semicolons (;). You can specify a maximum of 10 IP addresses or CIDR blocks.
         self.ip_control_id = ip_control_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -277,15 +280,21 @@
 
 class AddIpControlPolicyItemResponseBody(TeaModel):
     def __init__(
         self,
         policy_item_id: str = None,
         request_id: str = None,
     ):
+        # When you call this operation, note that:
+        # 
+        # *   This operation is intended for API providers.
+        # *   An added policy immediately takes effect on all APIs that are bound to the access control list (ACL).
+        # *   A maximum of 100 policies can be added to an ACL.
         self.policy_item_id = policy_item_id
+        # Adds a policy to an existing ACL.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -358,17 +367,23 @@
         security_token: str = None,
         special_key: str = None,
         special_type: str = None,
         traffic_control_id: str = None,
         traffic_value: int = None,
     ):
         self.security_token = security_token
+        # The ID of the request.
         self.special_key = special_key
+        # The special throttling value.
         self.special_type = special_type
+        # The ID of the app or Alibaba Cloud account. Specify this parameter based on the value of the **SpecialType** parameter. You can view your account ID on the [Account Management](https://account.console.aliyun.com/?spm=a2c4g.11186623.2.15.3f053654YpMPwo#/secure) page.
         self.traffic_control_id = traffic_control_id
+        # *   This API is intended for API providers.
+        # *   If the input SpecialKey already exists, the previous configuration is overwritten. Use caution when calling this operation.
+        # *   Special throttling policies must be added to an existing throttling policy, and can take effect on all the APIs to which the throttling policy is bound.
         self.traffic_value = traffic_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -404,14 +419,15 @@
 
 
 class AddTrafficSpecialControlResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Adds a custom special policy to a specified throttling policy.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -767,15 +783,17 @@
 
 class BatchDeployApisRequestApi(TeaModel):
     def __init__(
         self,
         api_uid: str = None,
         group_id: str = None,
     ):
+        # Publishes multiple APIs at a time.
         self.api_uid = api_uid
+        # The APIs that you want to operate.
         self.group_id = group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -802,17 +820,20 @@
     def __init__(
         self,
         api: List[BatchDeployApisRequestApi] = None,
         description: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # b4f5c342b8bc4ef88ccda0332402e0fa
         self.api = api
+        # 2b35dd68345b472f8051647306a16415
         self.description = description
         self.security_token = security_token
+        # The description.
         self.stage_name = stage_name
 
     def validate(self):
         if self.api:
             for k in self.api:
                 if k:
                     k.validate()
@@ -928,48 +949,56 @@
         return self
 
 
 class CreateAccessControlListRequest(TeaModel):
     def __init__(
         self,
         acl_name: str = None,
+        address_ipversion: str = None,
         security_token: str = None,
     ):
+        # The name of the ACL. The name must be 1 to 30 characters in length, and can contain letters, digits, periods (.), hyphens (-), forward slashes (/), and underscores (\_). The name must be unique within the region.
         self.acl_name = acl_name
+        self.address_ipversion = address_ipversion
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.acl_name is not None:
             result['AclName'] = self.acl_name
+        if self.address_ipversion is not None:
+            result['AddressIPVersion'] = self.address_ipversion
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclName') is not None:
             self.acl_name = m.get('AclName')
+        if m.get('AddressIPVersion') is not None:
+            self.address_ipversion = m.get('AddressIPVersion')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class CreateAccessControlListResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1059,40 +1088,83 @@
         service_config: str = None,
         service_parameters: str = None,
         service_parameters_map: str = None,
         system_parameters: str = None,
         visibility: str = None,
         web_socket_api_type: str = None,
     ):
+        # If the **AuthType** is **APP** authentication, you need to pass this value to specify the signature algorithm. If you do not specify this parameter, the default value HmacSHA256 is used. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method
+        # The name of the API that you want to create. The name must be unique within the API group. The name must be 4 to 50 characters in length. It must start with a letter and can contain letters, digits, and underscores (\_).
         self.api_name = api_name
+        # If the **AuthType** parameter is set to **APP**, the valid values are:
+        # 
+        # *   **DEFAULT**: The default value that is used if no other values are passed. This value indicates that the settings of the group are used.
+        # *   **DISABLE**: The authentication is disabled.
+        # *   **HEADER**: AppCode can be placed in the Header parameter for authentication.
+        # *   **HEADER_QUERY**: AppCode can be placed in the Header or Query parameter for authentication.
         self.app_code_auth_type = app_code_auth_type
+        # API安全认证类型，目前可以取值：
+        # 
+        # - **APP**：只允许已授权的APP调用
+        # - **ANONYMOUS**：允许匿名调用，设置为允许匿名调用需要注意：
+        #   任何能够获取该API服务信息的人，都将能够调用该API。网关不会对调用者做身份认证，也无法设置按用户的流量控制，若开放该API请设置好按API的流量控制。
         self.auth_type = auth_type
+        # Specifies whether to enable backend services.
         self.backend_enable = backend_enable
+        # The IDof the backend service
         self.backend_id = backend_id
         self.constant_parameters = constant_parameters
+        # The description of the API. The description can be up to 180 characters in length.
         self.description = description
+        # *   Specifies whether to set **DisableInternet** to **true** to limit API calls to within the VPC.
+        # *   If you set **DisableInternet** to **false**, the limit is lifted. The default value is false when you create an API.
         self.disable_internet = disable_internet
         self.error_code_samples = error_code_samples
         self.fail_result_sample = fail_result_sample
+        # *   Specifies whether to set **ForceNonceCheck** to **true** to force the check of X-Ca-Nonce during the request. This is the unique identifier of the request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent replay attacks.
+        # *   If you set **ForceNonceCheck** to **false**, the check is not performed. The default value is false when you create an API.
         self.force_nonce_check = force_nonce_check
+        # The ID of the API group.
         self.group_id = group_id
+        # The switch status of ACL. Valid values:- **on** and **off**.
         self.open_id_connect_config = open_id_connect_config
+        # The configuration items of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestConfig](~~43985~~).
         self.request_config = request_config
         self.request_parameters = request_parameters
+        # The return description of the API.
         self.result_body_model = result_body_model
         self.result_descriptions = result_descriptions
         self.result_sample = result_sample
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML. Default value: JSON.
         self.result_type = result_type
         self.security_token = security_token
+        # The configuration items of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceConfig](~~43987~~).
         self.service_config = service_config
         self.service_parameters = service_parameters
         self.service_parameters_map = service_parameters_map
         self.system_parameters = system_parameters
+        # Specifies whether to make the API public. Valid values:
+        # 
+        # *   **PUBLIC**: Make the API public. If you set this parameter to PUBLIC, this API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE**: Make the API private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.visibility = visibility
+        # The type of the two-way communication API.
+        # 
+        # *   **COMMON**: common API
+        # *   **REGISTER**: registered API
+        # *   **UNREGISTER**: unregistered API
+        # *   **NOTIFY**: downstream notification API
         self.web_socket_api_type = web_socket_api_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1217,15 +1289,17 @@
 
 class CreateApiResponseBody(TeaModel):
     def __init__(
         self,
         api_id: str = None,
         request_id: str = None,
     ):
+        # The ID of the API.
         self.api_id = api_id
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1680,25 +1754,25 @@
     def __init__(
         self,
         app_code: str = None,
         app_key: str = None,
         app_name: str = None,
         app_secret: str = None,
         description: str = None,
+        extend: str = None,
         security_token: str = None,
-        source: str = None,
         tag: List[CreateAppRequestTag] = None,
     ):
         self.app_code = app_code
         self.app_key = app_key
         self.app_name = app_name
         self.app_secret = app_secret
         self.description = description
+        self.extend = extend
         self.security_token = security_token
-        self.source = source
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -1715,18 +1789,18 @@
             result['AppKey'] = self.app_key
         if self.app_name is not None:
             result['AppName'] = self.app_name
         if self.app_secret is not None:
             result['AppSecret'] = self.app_secret
         if self.description is not None:
             result['Description'] = self.description
+        if self.extend is not None:
+            result['Extend'] = self.extend
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
-        if self.source is not None:
-            result['Source'] = self.source
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
@@ -1737,18 +1811,18 @@
             self.app_key = m.get('AppKey')
         if m.get('AppName') is not None:
             self.app_name = m.get('AppName')
         if m.get('AppSecret') is not None:
             self.app_secret = m.get('AppSecret')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('Extend') is not None:
+            self.extend = m.get('Extend')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
-        if m.get('Source') is not None:
-            self.source = m.get('Source')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = CreateAppRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
@@ -2338,39 +2412,134 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDatasetItemResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateInstanceRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateInstanceRequestZoneVSwitchSecurityGroup(TeaModel):
+    def __init__(
+        self,
+        cidr_block: str = None,
+        security_group_id: str = None,
+        v_switch_id: str = None,
+        zone_id: str = None,
+    ):
+        self.cidr_block = cidr_block
+        self.security_group_id = security_group_id
+        self.v_switch_id = v_switch_id
+        self.zone_id = zone_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cidr_block is not None:
+            result['CidrBlock'] = self.cidr_block
+        if self.security_group_id is not None:
+            result['SecurityGroupId'] = self.security_group_id
+        if self.v_switch_id is not None:
+            result['VSwitchId'] = self.v_switch_id
+        if self.zone_id is not None:
+            result['ZoneId'] = self.zone_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CidrBlock') is not None:
+            self.cidr_block = m.get('CidrBlock')
+        if m.get('SecurityGroupId') is not None:
+            self.security_group_id = m.get('SecurityGroupId')
+        if m.get('VSwitchId') is not None:
+            self.v_switch_id = m.get('VSwitchId')
+        if m.get('ZoneId') is not None:
+            self.zone_id = m.get('ZoneId')
+        return self
+
+
 class CreateInstanceRequest(TeaModel):
     def __init__(
         self,
         auto_pay: bool = None,
         charge_type: str = None,
         duration: int = None,
         https_policy: str = None,
+        instance_cidr: str = None,
         instance_name: str = None,
         instance_spec: str = None,
+        instance_type: str = None,
         pricing_cycle: str = None,
+        tag: List[CreateInstanceRequestTag] = None,
         token: str = None,
+        user_vpc_id: str = None,
         zone_id: str = None,
+        zone_vswitch_security_group: List[CreateInstanceRequestZoneVSwitchSecurityGroup] = None,
     ):
         self.auto_pay = auto_pay
         self.charge_type = charge_type
         self.duration = duration
         self.https_policy = https_policy
+        self.instance_cidr = instance_cidr
         self.instance_name = instance_name
         self.instance_spec = instance_spec
+        self.instance_type = instance_type
         self.pricing_cycle = pricing_cycle
+        self.tag = tag
         self.token = token
+        self.user_vpc_id = user_vpc_id
         self.zone_id = zone_id
+        self.zone_vswitch_security_group = zone_vswitch_security_group
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+        if self.zone_vswitch_security_group:
+            for k in self.zone_vswitch_security_group:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2378,79 +2547,115 @@
             result['AutoPay'] = self.auto_pay
         if self.charge_type is not None:
             result['ChargeType'] = self.charge_type
         if self.duration is not None:
             result['Duration'] = self.duration
         if self.https_policy is not None:
             result['HttpsPolicy'] = self.https_policy
+        if self.instance_cidr is not None:
+            result['InstanceCidr'] = self.instance_cidr
         if self.instance_name is not None:
             result['InstanceName'] = self.instance_name
         if self.instance_spec is not None:
             result['InstanceSpec'] = self.instance_spec
+        if self.instance_type is not None:
+            result['InstanceType'] = self.instance_type
         if self.pricing_cycle is not None:
             result['PricingCycle'] = self.pricing_cycle
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.token is not None:
             result['Token'] = self.token
+        if self.user_vpc_id is not None:
+            result['UserVpcId'] = self.user_vpc_id
         if self.zone_id is not None:
             result['ZoneId'] = self.zone_id
+        result['ZoneVSwitchSecurityGroup'] = []
+        if self.zone_vswitch_security_group is not None:
+            for k in self.zone_vswitch_security_group:
+                result['ZoneVSwitchSecurityGroup'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoPay') is not None:
             self.auto_pay = m.get('AutoPay')
         if m.get('ChargeType') is not None:
             self.charge_type = m.get('ChargeType')
         if m.get('Duration') is not None:
             self.duration = m.get('Duration')
         if m.get('HttpsPolicy') is not None:
             self.https_policy = m.get('HttpsPolicy')
+        if m.get('InstanceCidr') is not None:
+            self.instance_cidr = m.get('InstanceCidr')
         if m.get('InstanceName') is not None:
             self.instance_name = m.get('InstanceName')
         if m.get('InstanceSpec') is not None:
             self.instance_spec = m.get('InstanceSpec')
+        if m.get('InstanceType') is not None:
+            self.instance_type = m.get('InstanceType')
         if m.get('PricingCycle') is not None:
             self.pricing_cycle = m.get('PricingCycle')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateInstanceRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('Token') is not None:
             self.token = m.get('Token')
+        if m.get('UserVpcId') is not None:
+            self.user_vpc_id = m.get('UserVpcId')
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
+        self.zone_vswitch_security_group = []
+        if m.get('ZoneVSwitchSecurityGroup') is not None:
+            for k in m.get('ZoneVSwitchSecurityGroup'):
+                temp_model = CreateInstanceRequestZoneVSwitchSecurityGroup()
+                self.zone_vswitch_security_group.append(temp_model.from_map(k))
         return self
 
 
 class CreateInstanceResponseBody(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         request_id: str = None,
+        tag_status: bool = None,
     ):
         self.instance_id = instance_id
         self.request_id = request_id
+        self.tag_status = tag_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.tag_status is not None:
+            result['TagStatus'] = self.tag_status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('TagStatus') is not None:
+            self.tag_status = m.get('TagStatus')
         return self
 
 
 class CreateInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
@@ -2496,14 +2701,15 @@
 
 class CreateIntranetDomainRequest(TeaModel):
     def __init__(
         self,
         group_id: str = None,
         security_token: str = None,
     ):
+        # The custom domain name.
         self.group_id = group_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2529,15 +2735,17 @@
 
 class CreateIntranetDomainResponseBody(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.domain_name = domain_name
+        # auditing
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2779,14 +2987,15 @@
         log_type: str = None,
         security_token: str = None,
         sls_log_store: str = None,
         sls_project: str = None,
     ):
         self.log_type = log_type
         self.security_token = security_token
+        # slslogstore
         self.sls_log_store = sls_log_store
         self.sls_project = sls_project
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2893,17 +3102,21 @@
     def __init__(
         self,
         description: str = None,
         group_id: str = None,
         model_name: str = None,
         schema: str = None,
     ):
+        # The description of the model definition.
         self.description = description
+        # The ID of the API group to which the model belongs.
         self.group_id = group_id
+        # The name of the model. The name must be unique within the group.
         self.model_name = model_name
+        # The definition of the model in JSON Schema.
         self.schema = schema
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2944,23 +3157,33 @@
         model_name: str = None,
         model_ref: str = None,
         modified_time: str = None,
         region_id: str = None,
         request_id: str = None,
         schema: str = None,
     ):
+        # The time when the model was created.
         self.created_time = created_time
+        # The description of the created model.
         self.description = description
+        # The ID of the API group to which the created model belongs.
         self.group_id = group_id
+        # The ID of the created model.
         self.model_id = model_id
+        # The name of the created model.
         self.model_name = model_name
+        # The URI of the created model.
         self.model_ref = model_ref
+        # The time when the model is last modified.
         self.modified_time = modified_time
+        # The region to which the created model belongs.
         self.region_id = region_id
+        # The ID of the request.
         self.request_id = request_id
+        # The definition of the created model.
         self.schema = schema
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3367,16 +3590,19 @@
         self,
         security_token: str = None,
         signature_key: str = None,
         signature_name: str = None,
         signature_secret: str = None,
     ):
         self.security_token = security_token
+        # The ID of the request.
         self.signature_key = signature_key
+        # The Secret value of the key. The value must be 6 to 30 characters in length and can contain letters, digits, and special characters. Special characters include underscores (\_), at signs (@), number signs (#), exclamation points (!), and asterisks (\*). The value must start with a letter.
         self.signature_name = signature_name
+        # The ID of the back-end signature key.
         self.signature_secret = signature_secret
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3410,16 +3636,22 @@
 class CreateSignatureResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         signature_id: str = None,
         signature_name: str = None,
     ):
+        # The name of the back-end signature key.
         self.request_id = request_id
+        # *   This API is intended for API providers.
+        # *   The API operation only creates a key policy. You must call the binding operation to bind the key to an API.
+        # *   After the key is bound to the API, requests sent from API Gateway to the backend service contain signature strings. You can specify whether your backend service verifies these signature strings.
+        # *   The QPS limit on this operation is 50 per user.
         self.signature_id = signature_id
+        # Creates a backend signature key.
         self.signature_name = signature_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3497,20 +3729,31 @@
         app_default: int = None,
         description: str = None,
         security_token: str = None,
         traffic_control_name: str = None,
         traffic_control_unit: str = None,
         user_default: int = None,
     ):
+        # The default throttling value for each app.
         self.api_default = api_default
+        # ThrottlingTestDescription
         self.app_default = app_default
+        # The ID of the throttling policy.
         self.description = description
         self.security_token = security_token
+        # The unit to be used in the throttling policy. Valid values:
+        # 
+        # *   **SECOND**\
+        # *   **MINUTE**\
+        # *   **HOUR**\
+        # *   **DAY**\
         self.traffic_control_name = traffic_control_name
+        # The default throttling value for each user.
         self.traffic_control_unit = traffic_control_unit
+        # The description of the throttling policy.
         self.user_default = user_default
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3555,15 +3798,19 @@
 
 class CreateTrafficControlResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         traffic_control_id: str = None,
     ):
+        # Creates a custom throttling policy.
         self.request_id = request_id
+        # *   This API is intended for API providers.
+        # *   Throttling policies must be bound to APIs to take effect. After a policy is bound to an API, it goes into effect on that API immediately.
+        # *   The QPS limit on this operation is 50 per user.
         self.traffic_control_id = traffic_control_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3737,14 +3984,15 @@
 class DeleteAllTrafficSpecialControlRequest(TeaModel):
     def __init__(
         self,
         security_token: str = None,
         traffic_control_id: str = None,
     ):
         self.security_token = security_token
+        # *   This API is intended for API providers.
         self.traffic_control_id = traffic_control_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3768,14 +4016,15 @@
 
 
 class DeleteAllTrafficSpecialControlResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Deletes all custom special policies of a specified throttling policy.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4103,17 +4352,20 @@
     def __init__(
         self,
         group_id: str = None,
         security_token: str = None,
         stage_id: str = None,
         variable_name: str = None,
     ):
+        # The name of the variable to be deleted. This parameter is case-sensitive.
         self.group_id = group_id
         self.security_token = security_token
+        # The ID of the request.
         self.stage_id = stage_id
+        # *   This operation is intended for API providers.
         self.variable_name = variable_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4145,14 +4397,15 @@
 
 
 class DeleteApiStageVariableResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Deletes a specified variable in a specified environment.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4809,15 +5062,19 @@
 class DeleteDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         group_id: str = None,
         security_token: str = None,
     ):
+        # *   This operation is intended for API providers.
+        # *   If the specified domain name does not exist, a successful response will still appear.
+        # *   Unbinding a domain name from an API group will affect access to the APIs in the group. Exercise caution when using this operation.
         self.domain_name = domain_name
+        # The ID of the request.
         self.group_id = group_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4846,14 +5103,15 @@
 
 
 class DeleteDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Unbinds a custom domain name from a specified API group.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5179,14 +5437,17 @@
 
 class DeleteIpControlRequest(TeaModel):
     def __init__(
         self,
         ip_control_id: str = None,
         security_token: str = None,
     ):
+        # *   This operation is intended for API providers.
+        # *   If the ACL is bound to an API, you must unbind the ACL from the API before you can delete the ACL. Otherwise, an error is returned.
+        # *   If you call this operation on an ACL that does not exist, a success message is returned.
         self.ip_control_id = ip_control_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5211,14 +5472,15 @@
 
 
 class DeleteIpControlResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Deletes an access control list (ACL).
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5387,15 +5649,17 @@
 
 class DeleteModelRequest(TeaModel):
     def __init__(
         self,
         group_id: str = None,
         model_name: str = None,
     ):
+        # The ID of the request.
         self.group_id = group_id
+        # The ID of the API group to which the model belongs.
         self.model_name = model_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5419,14 +5683,15 @@
 
 
 class DeleteModelResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Deletes a model from Model Management for an API group.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5753,14 +6018,18 @@
 class DeleteSignatureRequest(TeaModel):
     def __init__(
         self,
         security_token: str = None,
         signature_id: str = None,
     ):
         self.security_token = security_token
+        # *   This API is intended for API providers.
+        # *   This API operation deletes an existing backend signature key.
+        # *   You cannot delete a key that is bound to an API. To delete the key, you must unbind it first.
+        # *   The QPS limit on this operation is 50 per user.
         self.signature_id = signature_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5784,14 +6053,15 @@
 
 
 class DeleteSignatureResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Deletes a backend signature key.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5963,16 +6233,20 @@
         self,
         security_token: str = None,
         special_key: str = None,
         special_type: str = None,
         traffic_control_id: str = None,
     ):
         self.security_token = security_token
+        # *   This API is intended for API providers.
+        # *   You can obtain the input parameters required in this operation by calling other APIs.
         self.special_key = special_key
+        # The ID of the request.
         self.special_type = special_type
+        # The ID of the app or Alibaba Cloud account. You can view your account ID on the [Account Management](https://account.console.aliyun.com/?spm=a2c4g.11186623.2.15.343130a8sDi8cO#/secure) page.
         self.traffic_control_id = traffic_control_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6004,14 +6278,15 @@
 
 
 class DeleteTrafficSpecialControlResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Deletes a custom special throttling policy.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6079,18 +6354,28 @@
         self,
         api_id: str = None,
         description: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The publishing remarks.
         self.api_id = api_id
-        self.description = description
+        # *   This operation is intended for API providers. Only the API that you have defined and published to a runtime environment can be called.
+        # *   An API is published to a cluster in less than 5 seconds.
+        # *   The QPS limit on this operation is 50 per user.
+        self.description = description
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **PRE: the pre-release environment**\
+        # *   **TEST: the test environment**\
         self.group_id = group_id
         self.security_token = security_token
+        # The ID of the request.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6126,14 +6411,15 @@
 
 
 class DeployApiResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Publishes an API to a specified environment.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6610,19 +6896,21 @@
         return self
 
 
 class DescribeAccessControlListsRequest(TeaModel):
     def __init__(
         self,
         acl_name: str = None,
+        address_ipversion: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
     ):
         self.acl_name = acl_name
+        self.address_ipversion = address_ipversion
         self.page_number = page_number
         self.page_size = page_size
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -6630,65 +6918,75 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.acl_name is not None:
             result['AclName'] = self.acl_name
+        if self.address_ipversion is not None:
+            result['AddressIPVersion'] = self.address_ipversion
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclName') is not None:
             self.acl_name = m.get('AclName')
+        if m.get('AddressIPVersion') is not None:
+            self.address_ipversion = m.get('AddressIPVersion')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeAccessControlListsResponseBodyAclsAcl(TeaModel):
     def __init__(
         self,
         acl_id: str = None,
         acl_name: str = None,
+        address_ipversion: str = None,
     ):
         self.acl_id = acl_id
         self.acl_name = acl_name
+        self.address_ipversion = address_ipversion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.acl_id is not None:
             result['AclId'] = self.acl_id
         if self.acl_name is not None:
             result['AclName'] = self.acl_name
+        if self.address_ipversion is not None:
+            result['AddressIPVersion'] = self.address_ipversion
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclId') is not None:
             self.acl_id = m.get('AclId')
         if m.get('AclName') is not None:
             self.acl_name = m.get('AclName')
+        if m.get('AddressIPVersion') is not None:
+            self.address_ipversion = m.get('AddressIPVersion')
         return self
 
 
 class DescribeAccessControlListsResponseBodyAcls(TeaModel):
     def __init__(
         self,
         acl: List[DescribeAccessControlListsResponseBodyAclsAcl] = None,
@@ -6823,15 +7121,17 @@
 class DescribeApiRequest(TeaModel):
     def __init__(
         self,
         api_id: str = None,
         group_id: str = None,
         security_token: str = None,
     ):
+        # The ID of the API.
         self.api_id = api_id
+        # The ID of the API.
         self.group_id = group_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6862,16 +7162,19 @@
 class DescribeApiResponseBodyBackendConfig(TeaModel):
     def __init__(
         self,
         backend_id: str = None,
         backend_name: str = None,
         backend_type: str = None,
     ):
+        # Backend service type
         self.backend_id = backend_id
+        # The configuration items of API requests sent by the consumer to API Gateway.
         self.backend_name = backend_name
+        # The name of the backend service.
         self.backend_type = backend_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6902,17 +7205,21 @@
     def __init__(
         self,
         constant_value: str = None,
         description: str = None,
         location: str = None,
         service_parameter_name: str = None,
     ):
+        # The parameters of API requests sent by the consumer to API Gateway.
         self.constant_value = constant_value
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.description = description
+        # The name of the backend service parameter.
         self.location = location
+        # The value of the parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6983,18 +7290,23 @@
         self,
         demo_value: str = None,
         description: str = None,
         location: str = None,
         parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # Description
         self.demo_value = demo_value
+        # Client IP Address
         self.description = description
+        # The name of the corresponding backend parameter.
         self.location = location
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.parameter_name = parameter_name
+        # System parameters sent by API Gateway to the backend service
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7067,16 +7379,19 @@
 class DescribeApiResponseBodyDeployedInfosDeployedInfo(TeaModel):
     def __init__(
         self,
         deployed_status: str = None,
         effective_version: str = None,
         stage_name: str = None,
     ):
+        # auditing
         self.deployed_status = deployed_status
+        # The deployment status. Valid values: DEPLOYED and NONDEPLOYED.
         self.effective_version = effective_version
+        # The effective version.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7142,17 +7457,21 @@
     def __init__(
         self,
         code: str = None,
         description: str = None,
         message: str = None,
         model: str = None,
     ):
+        # Model
         self.code = code
+        # The UserId parameter is missing from the request.
         self.description = description
+        # Description
         self.message = message
+        # Error message
         self.model = model
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7222,17 +7541,21 @@
     def __init__(
         self,
         id_token_param_name: str = None,
         open_id_api_type: str = None,
         public_key: str = None,
         public_key_id: str = None,
     ):
+        # The ID of the public key.
         self.id_token_param_name = id_token_param_name
+        # The name of the parameter that corresponds to the token.
         self.open_id_api_type = open_id_api_type
+        # The sample error codes returned by the backend service.
         self.public_key = public_key
+        # The public key.
         self.public_key_id = public_key_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7270,20 +7593,29 @@
         body_model: str = None,
         post_body_description: str = None,
         request_http_method: str = None,
         request_mode: str = None,
         request_path: str = None,
         request_protocol: str = None,
     ):
+        # The request mode. Valid values: MAPPING and PASSTHROUGH.
         self.body_format = body_format
+        # The API request path. If the complete API URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the API request path is ` /object/add  `.
         self.body_model = body_model
+        # The protocol type supported by the API. Valid values: HTTP and HTTPS. Separate multiple values with commas (,), such as "HTTP,HTTPS".
         self.post_body_description = post_body_description
+        # This parameter takes effect only when the RequestMode parameter is set to MAPPING.********\
+        # 
+        # The server data transmission method used for POST and PUT requests. Valid values: FORM and STREAM. FORM indicates that data in key-value pairs is transmitted as forms. STREAM indicates that data is transmitted as byte streams.
         self.request_http_method = request_http_method
+        # The description of the request body.
         self.request_mode = request_mode
+        # The HTTP method used to make the request. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_path = request_path
+        # The configuration items of API requests sent by API Gateway to the backend service.
         self.request_protocol = request_protocol
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7343,30 +7675,47 @@
         max_value: int = None,
         min_length: int = None,
         min_value: int = None,
         parameter_type: str = None,
         regular_expression: str = None,
         required: str = None,
     ):
+        # The hash values that can be entered when **ParameterType** is set to Int, Long, Float, Double, or String. Separate different values with commas (,), such as 1,2,3,4,9 or A,B,C,E,F.
         self.api_parameter_name = api_parameter_name
+        # The minimum parameter value when **ParameterType** is set to Int, Long, Float, or Double.
         self.array_items_type = array_items_type
+        # The name of the parameter.
         self.default_value = default_value
+        # Indicates whether the parameter is required. Valid values: **REQUIRED** and **OPTIONAL**.
         self.demo_value = demo_value
+        # Age
         self.description = description
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.doc_order = doc_order
+        # The maximum parameter length when **ParameterType** is set to String.
         self.doc_show = doc_show
+        # Examples
         self.enum_value = enum_value
+        # The maximum parameter value when **ParameterType** is set to Int, Long, Float, or Double.
         self.json_scheme = json_scheme
+        # The parameters of API requests sent by API Gateway to the backend service.
         self.location = location
+        # The default value.
         self.max_length = max_length
+        # The type of the array element.
         self.max_value = max_value
+        # The order in the document.
         self.min_length = min_length
+        # Indicates whether the document is public. Valid values: **PUBLIC** and **PRIVATE**.
         self.min_value = min_value
+        # The regular expression used for parameter validation when **ParameterType** is set to String.
         self.parameter_type = parameter_type
+        # The minimum parameter length when **ParameterType** is set to String.
         self.regular_expression = regular_expression
+        # Description
         self.required = required
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7480,129 +7829,29 @@
         if m.get('RequestParameter') is not None:
             for k in m.get('RequestParameter'):
                 temp_model = DescribeApiResponseBodyRequestParametersRequestParameter()
                 self.request_parameter.append(temp_model.from_map(k))
         return self
 
 
-class DescribeApiResponseBodyResultDescriptionsResultDescription(TeaModel):
-    def __init__(
-        self,
-        description: str = None,
-        has_child: bool = None,
-        id: str = None,
-        key: str = None,
-        mandatory: bool = None,
-        name: str = None,
-        pid: str = None,
-        type: str = None,
-    ):
-        self.description = description
-        self.has_child = has_child
-        self.id = id
-        self.key = key
-        self.mandatory = mandatory
-        self.name = name
-        self.pid = pid
-        self.type = type
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.description is not None:
-            result['Description'] = self.description
-        if self.has_child is not None:
-            result['HasChild'] = self.has_child
-        if self.id is not None:
-            result['Id'] = self.id
-        if self.key is not None:
-            result['Key'] = self.key
-        if self.mandatory is not None:
-            result['Mandatory'] = self.mandatory
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.pid is not None:
-            result['Pid'] = self.pid
-        if self.type is not None:
-            result['Type'] = self.type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
-        if m.get('HasChild') is not None:
-            self.has_child = m.get('HasChild')
-        if m.get('Id') is not None:
-            self.id = m.get('Id')
-        if m.get('Key') is not None:
-            self.key = m.get('Key')
-        if m.get('Mandatory') is not None:
-            self.mandatory = m.get('Mandatory')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('Pid') is not None:
-            self.pid = m.get('Pid')
-        if m.get('Type') is not None:
-            self.type = m.get('Type')
-        return self
-
-
-class DescribeApiResponseBodyResultDescriptions(TeaModel):
-    def __init__(
-        self,
-        result_description: List[DescribeApiResponseBodyResultDescriptionsResultDescription] = None,
-    ):
-        self.result_description = result_description
-
-    def validate(self):
-        if self.result_description:
-            for k in self.result_description:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['ResultDescription'] = []
-        if self.result_description is not None:
-            for k in self.result_description:
-                result['ResultDescription'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.result_description = []
-        if m.get('ResultDescription') is not None:
-            for k in m.get('ResultDescription'):
-                temp_model = DescribeApiResponseBodyResultDescriptionsResultDescription()
-                self.result_description.append(temp_model.from_map(k))
-        return self
-
-
 class DescribeApiResponseBodyServiceConfigEventBridgeConfig(TeaModel):
     def __init__(
         self,
         event_bridge_region_id: str = None,
         event_bus: str = None,
         event_source: str = None,
         role_arn: str = None,
     ):
+        # The Arn that is authorized by a RAM user to EventBridge.
         self.event_bridge_region_id = event_bridge_region_id
+        # The event source.
         self.event_bus = event_bus
+        # The ID of the region where the EventBridge instance is located.
         self.event_source = event_source
+        # Configuration items of the third-party OpenID Connect authentication method
         self.role_arn = role_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7645,25 +7894,41 @@
         only_business_path: bool = None,
         path: str = None,
         qualifier: str = None,
         region_id: str = None,
         role_arn: str = None,
         service_name: str = None,
     ):
+        # The API request path.
         self.content_type_catagory = content_type_catagory
+        # The region where the Function Compute instance is located.
         self.content_type_value = content_type_value
+        # The value of the ContentType header when the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.fc_base_url = fc_base_url
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role to be assumed by API Gateway to access Function Compute.
         self.fc_type = fc_type
+        # The ContentType header type used when you call the backend service over HTTP.
+        # 
+        # *   **DEFAULT**: the default header type in API Gateway
+        # *   **CUSTOM**: a custom header type
+        # *   **CLIENT**: the ContentType header type of the client
         self.function_name = function_name
+        # The root path of Function Compute.
         self.method = method
+        # The function name defined in Function Compute.
         self.only_business_path = only_business_path
+        # The service name defined in Function Compute.
         self.path = path
+        # Information when the backend service is OSS
         self.qualifier = qualifier
+        # The backend only receives the service path.
         self.region_id = region_id
+        # The request method.
         self.role_arn = role_arn
+        # The alias of the function.
         self.service_name = service_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7728,15 +7993,17 @@
 
 class DescribeApiResponseBodyServiceConfigMockHeadersMockHeader(TeaModel):
     def __init__(
         self,
         header_name: str = None,
         header_value: str = None,
     ):
+        # Configuration items related to VPC channels
         self.header_name = header_name
+        # The name of the HTTP header.
         self.header_value = header_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7799,16 +8066,18 @@
         self,
         action: str = None,
         bucket_name: str = None,
         key: str = None,
         oss_region_id: str = None,
     ):
         self.action = action
+        # Configuration items of EventBridge
         self.bucket_name = bucket_name
         self.key = key
+        # The OSS bucket.
         self.oss_region_id = oss_region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7844,18 +8113,23 @@
         self,
         instance_id: str = None,
         name: str = None,
         port: int = None,
         vpc_id: str = None,
         vpc_scheme: str = None,
     ):
+        # The port number that corresponds to the instance.
         self.instance_id = instance_id
+        # Backend configuration items when the backend service is Function Compute
         self.name = name
+        # The name of the VPC access authorization.
         self.port = port
+        # The VPC protocol.
         self.vpc_id = vpc_id
+        # The ID of the ECS or SLB instance in the VPC.
         self.vpc_scheme = vpc_scheme
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7907,30 +8181,57 @@
         service_http_method: str = None,
         service_path: str = None,
         service_protocol: str = None,
         service_timeout: int = None,
         service_vpc_enable: str = None,
         vpc_config: DescribeApiResponseBodyServiceConfigVpcConfig = None,
     ):
+        # The status code returned for service mocking.
         self.aone_app_name = aone_app_name
+        # The URL used to call the back-end service. If the complete back-end service URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the value of **ServiceAddress** is `http://api.a.com:8080`.
         self.content_type_catagory = content_type_catagory
+        # The protocol used by the backend service. Valid values: HTTP and HTTPS.
         self.content_type_value = content_type_value
+        # The event bus.
         self.event_bridge_config = event_bridge_config
+        # The type of the Function Compute instance.
         self.function_compute_config = function_compute_config
+        # Specifies whether to enable the VPC channel. Valid values:
+        # 
+        # *   **TRUE**: The VPC channel is enabled. You must create the corresponding VPC access authorization before you can enable a VPC channel.
+        # *   **FALSE**: The VPC channel is not enabled.
         self.mock = mock
+        # The value of the HTTP header.
         self.mock_headers = mock_headers
+        # The HTTP method used to call a backend service. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.mock_result = mock_result
+        # The value of the ContentType header when the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.mock_status_code = mock_status_code
+        # The ID of the region where the OSS instance is located.
         self.oss_config = oss_config
+        # Specifies whether to enable the Mock mode. Valid values:
+        # 
+        # *   **TRUE**: The Mock mode is enabled.
+        # *   **FALSE**: The Mock mode is not enabled.
         self.service_address = service_address
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_http_method = service_http_method
+        # The ContentType header type used when you call the backend service over HTTP.
+        # 
+        # *   **DEFAULT**: the default header type in API Gateway
+        # *   **CUSTOM**: a custom header type
+        # *   **CLIENT**: the ContentType header type of the client
         self.service_path = service_path
+        # The path used to call the back-end service. If the complete back-end service path is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, **ServicePath** is `/object/add`.
         self.service_protocol = service_protocol
+        # The simulated headers.
         self.service_timeout = service_timeout
+        # The result returned when the Mock mode is enabled.
         self.service_vpc_enable = service_vpc_enable
+        # The ID of the VPC.
         self.vpc_config = vpc_config
 
     def validate(self):
         if self.event_bridge_config:
             self.event_bridge_config.validate()
         if self.function_compute_config:
             self.function_compute_config.validate()
@@ -8030,16 +8331,19 @@
 class DescribeApiResponseBodyServiceParametersServiceParameter(TeaModel):
     def __init__(
         self,
         location: str = None,
         parameter_type: str = None,
         service_parameter_name: str = None,
     ):
+        # The data type of the back-end service parameter.
         self.location = location
+        # The name of the backend service parameter.
         self.parameter_type = parameter_type
+        # The mappings between parameters of requests sent by the consumer to API Gateway and parameters of requests sent by API Gateway to the backend service.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8103,15 +8407,17 @@
 
 class DescribeApiResponseBodyServiceParametersMapServiceParameterMap(TeaModel):
     def __init__(
         self,
         request_parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # The name of the backend service parameter.
         self.request_parameter_name = request_parameter_name
+        # The API publishing status.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8174,18 +8480,23 @@
         self,
         demo_value: str = None,
         description: str = None,
         location: str = None,
         parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # Description
         self.demo_value = demo_value
+        # Client IP Address
         self.description = description
+        # The name of the corresponding backend parameter.
         self.location = location
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.parameter_name = parameter_name
+        # Custom system parameters
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8281,59 +8592,129 @@
         modified_time: str = None,
         open_id_connect_config: DescribeApiResponseBodyOpenIdConnectConfig = None,
         region_id: str = None,
         request_config: DescribeApiResponseBodyRequestConfig = None,
         request_id: str = None,
         request_parameters: DescribeApiResponseBodyRequestParameters = None,
         result_body_model: str = None,
-        result_descriptions: DescribeApiResponseBodyResultDescriptions = None,
         result_sample: str = None,
         result_type: str = None,
         service_config: DescribeApiResponseBodyServiceConfig = None,
         service_parameters: DescribeApiResponseBodyServiceParameters = None,
         service_parameters_map: DescribeApiResponseBodyServiceParametersMap = None,
         system_parameters: DescribeApiResponseBodySystemParameters = None,
         visibility: str = None,
         web_socket_api_type: str = None,
     ):
+        # The region ID of the API.
         self.allow_signature_method = allow_signature_method
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML.
         self.api_id = api_id
+        # Specifies whether to enable backend services.
         self.api_name = api_name
+        # If **AuthType** is set to **APP**, this value must be passed to specify the signature algorithm. If you do not specify a value, HmacSHA256 is used by default. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.app_code_auth_type = app_code_auth_type
+        # The last modification time of the API.
         self.auth_type = auth_type
+        # The ID of the backend service.
         self.backend_config = backend_config
+        # Backend configurations
         self.backend_enable = backend_enable
+        # Description
         self.constant_parameters = constant_parameters
+        # The name of the API, which is unique in the group.
         self.created_time = created_time
+        # Examples
         self.custom_system_parameters = custom_system_parameters
+        # The name of the runtime environment. Valid values: RELEASE and TEST.
         self.deployed_infos = deployed_infos
+        # The name of the API group.
         self.description = description
+        # The returned description of the API.
         self.disable_internet = disable_internet
+        # Error codes
         self.error_code_samples = error_code_samples
+        # The security authentication method of the API. Valid values:
+        # 
+        # *   **APP**: Only authorized applications can call the API.
+        # 
+        # *   **ANONYMOUS**: The API can be anonymously called. In this mode, you must take note of the following rules:
+        # 
+        #     *   All users who have obtained the API service information can call this API. API Gateway does not authenticate callers and cannot set user-specific throttling policies. If you make this API public, set API-specific throttling policies.
+        #     *   We recommend that you do not make the API whose security authentication method is ANONYMOUS available in Alibaba Cloud Marketplace because API Gateway cannot meter calls on the caller or limit the number of calls on the API. If you want to make the API group to which the API belongs available in Alibaba Cloud Marketplace, we recommend that you move the API to another group, set its type to PRIVATE, or set its security authentication method to APP.
+        # 
+        # *   **APPOPENID**: The OpenID Connect account authentication method is used. Only applications authorized by OpenID Connect can call the API. If this method is selected, the OpenIdConnectConfig parameter is required.
         self.fail_result_sample = fail_result_sample
+        # Specifies whether to make the API public. Valid values:
+        # 
+        # *   **PUBLIC**: Make the API public. If you set this parameter to PUBLIC, this API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE**: Make the API private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.force_nonce_check = force_nonce_check
+        # Specifies whether to enable the Mock mode. Valid values:
+        # 
+        # *   OPEN: The Mock mode is enabled.
+        # *   CLOSED: The Mock mode is not enabled.
         self.group_id = group_id
+        # The ID of the API group.
         self.group_name = group_name
+        # The result returned for service mocking.
         self.mock = mock
+        # The creation time of the API.
         self.mock_result = mock_result
+        # The ID of the request.
         self.modified_time = modified_time
+        # The OpenID Connect mode. Valid values:
+        # 
+        # *   **IDTOKEN**: indicates the APIs that are called by clients to obtain tokens. If you specify this value, the PublicKeyId parameter and the PublicKey parameter are required.
+        # *   **BUSINESS**: indicates business APIs. Tokens are used to call the business APIs. If you specify this value, the IdTokenParamName parameter is required.
         self.open_id_connect_config = open_id_connect_config
+        # Specifies whether to carry the header : X-Ca-Nonce when calling an API. This is the unique identifier of the request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent reply attacks. Valid values:
+        # 
+        # *   **true**: This field is forcibly checked when an API is requested to prevent replay attacks.
+        # *   **false**: This field is not checked.
         self.region_id = region_id
+        # The body model.
         self.request_config = request_config
+        # The description of the API.
         self.request_id = request_id
+        # The JSON Schema used for JSON validation when **ParameterType** is set to String.
         self.request_parameters = request_parameters
+        # The sample response from the backend service.
         self.result_body_model = result_body_model
-        self.result_descriptions = result_descriptions
+        # If **AuthType** is set to **APP**, the valid values are:
+        # 
+        # *   **DEFAULT**: The default value that is used if no other values are passed. This value means that the setting of the group is used.
+        # *   **DISABLE**: The authentication is disabled.
+        # *   **HEADER**: AppCode can be placed in the Header parameter for authentication.
+        # *   **HEADER_QUERY**: AppCode can be placed in the Header or Query parameter for authentication.
         self.result_sample = result_sample
+        # The type of the two-way communication API. Valid values:
+        # 
+        # *   **COMMON**: general APIs
+        # *   **REGISTER**: registered APIs
+        # *   **UNREGISTER**: unregistered APIs
+        # *   **NOTIFY**: downstream notification
         self.result_type = result_type
+        # The application name in AONE.
         self.service_config = service_config
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.service_parameters = service_parameters
+        # The corresponding frontend parameter name. It must be included in RequestParametersObject and matches ApiParameterName in RequestParameter data.
         self.service_parameters_map = service_parameters_map
+        # Examples
         self.system_parameters = system_parameters
+        # The sample error response from the backend service.
         self.visibility = visibility
+        # Specifies whether to limit API calls to within the VPC. Valid values:
+        # 
+        # *   **true**: Only API calls from the VPC are supported.
+        # *   **false**: API calls from the VPC and Internet are both supported.
         self.web_socket_api_type = web_socket_api_type
 
     def validate(self):
         if self.backend_config:
             self.backend_config.validate()
         if self.constant_parameters:
             self.constant_parameters.validate()
@@ -8345,16 +8726,14 @@
             self.error_code_samples.validate()
         if self.open_id_connect_config:
             self.open_id_connect_config.validate()
         if self.request_config:
             self.request_config.validate()
         if self.request_parameters:
             self.request_parameters.validate()
-        if self.result_descriptions:
-            self.result_descriptions.validate()
         if self.service_config:
             self.service_config.validate()
         if self.service_parameters:
             self.service_parameters.validate()
         if self.service_parameters_map:
             self.service_parameters_map.validate()
         if self.system_parameters:
@@ -8416,16 +8795,14 @@
             result['RequestConfig'] = self.request_config.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.request_parameters is not None:
             result['RequestParameters'] = self.request_parameters.to_map()
         if self.result_body_model is not None:
             result['ResultBodyModel'] = self.result_body_model
-        if self.result_descriptions is not None:
-            result['ResultDescriptions'] = self.result_descriptions.to_map()
         if self.result_sample is not None:
             result['ResultSample'] = self.result_sample
         if self.result_type is not None:
             result['ResultType'] = self.result_type
         if self.service_config is not None:
             result['ServiceConfig'] = self.service_config.to_map()
         if self.service_parameters is not None:
@@ -8500,17 +8877,14 @@
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('RequestParameters') is not None:
             temp_model = DescribeApiResponseBodyRequestParameters()
             self.request_parameters = temp_model.from_map(m['RequestParameters'])
         if m.get('ResultBodyModel') is not None:
             self.result_body_model = m.get('ResultBodyModel')
-        if m.get('ResultDescriptions') is not None:
-            temp_model = DescribeApiResponseBodyResultDescriptions()
-            self.result_descriptions = temp_model.from_map(m['ResultDescriptions'])
         if m.get('ResultSample') is not None:
             self.result_sample = m.get('ResultSample')
         if m.get('ResultType') is not None:
             self.result_type = m.get('ResultType')
         if m.get('ServiceConfig') is not None:
             temp_model = DescribeApiResponseBodyServiceConfig()
             self.service_config = temp_model.from_map(m['ServiceConfig'])
@@ -8775,14 +9149,15 @@
         self.array_items_type = array_items_type
         self.default_value = default_value
         self.demo_value = demo_value
         self.description = description
         self.doc_order = doc_order
         self.doc_show = doc_show
         self.enum_value = enum_value
+        # JSON scheme
         self.json_scheme = json_scheme
         self.location = location
         self.max_length = max_length
         self.max_value = max_value
         self.min_length = min_length
         self.min_value = min_value
         self.parameter_type = parameter_type
@@ -8904,118 +9279,14 @@
         if m.get('RequestParameter') is not None:
             for k in m.get('RequestParameter'):
                 temp_model = DescribeApiDocResponseBodyRequestParametersRequestParameter()
                 self.request_parameter.append(temp_model.from_map(k))
         return self
 
 
-class DescribeApiDocResponseBodyResultDescriptionsResultDescription(TeaModel):
-    def __init__(
-        self,
-        description: str = None,
-        has_child: bool = None,
-        id: str = None,
-        key: str = None,
-        mandatory: bool = None,
-        name: str = None,
-        pid: str = None,
-        type: str = None,
-    ):
-        self.description = description
-        self.has_child = has_child
-        self.id = id
-        self.key = key
-        self.mandatory = mandatory
-        self.name = name
-        self.pid = pid
-        self.type = type
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.description is not None:
-            result['Description'] = self.description
-        if self.has_child is not None:
-            result['HasChild'] = self.has_child
-        if self.id is not None:
-            result['Id'] = self.id
-        if self.key is not None:
-            result['Key'] = self.key
-        if self.mandatory is not None:
-            result['Mandatory'] = self.mandatory
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.pid is not None:
-            result['Pid'] = self.pid
-        if self.type is not None:
-            result['Type'] = self.type
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
-        if m.get('HasChild') is not None:
-            self.has_child = m.get('HasChild')
-        if m.get('Id') is not None:
-            self.id = m.get('Id')
-        if m.get('Key') is not None:
-            self.key = m.get('Key')
-        if m.get('Mandatory') is not None:
-            self.mandatory = m.get('Mandatory')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('Pid') is not None:
-            self.pid = m.get('Pid')
-        if m.get('Type') is not None:
-            self.type = m.get('Type')
-        return self
-
-
-class DescribeApiDocResponseBodyResultDescriptions(TeaModel):
-    def __init__(
-        self,
-        result_description: List[DescribeApiDocResponseBodyResultDescriptionsResultDescription] = None,
-    ):
-        self.result_description = result_description
-
-    def validate(self):
-        if self.result_description:
-            for k in self.result_description:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['ResultDescription'] = []
-        if self.result_description is not None:
-            for k in self.result_description:
-                result['ResultDescription'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        self.result_description = []
-        if m.get('ResultDescription') is not None:
-            for k in m.get('ResultDescription'):
-                temp_model = DescribeApiDocResponseBodyResultDescriptionsResultDescription()
-                self.result_description.append(temp_model.from_map(k))
-        return self
-
-
 class DescribeApiDocResponseBody(TeaModel):
     def __init__(
         self,
         api_id: str = None,
         api_name: str = None,
         auth_type: str = None,
         deployed_time: str = None,
@@ -9026,15 +9297,14 @@
         force_nonce_check: bool = None,
         group_id: str = None,
         group_name: str = None,
         region_id: str = None,
         request_config: DescribeApiDocResponseBodyRequestConfig = None,
         request_id: str = None,
         request_parameters: DescribeApiDocResponseBodyRequestParameters = None,
-        result_descriptions: DescribeApiDocResponseBodyResultDescriptions = None,
         result_sample: str = None,
         result_type: str = None,
         stage_name: str = None,
         visibility: str = None,
     ):
         self.api_id = api_id
         self.api_name = api_name
@@ -9047,29 +9317,26 @@
         self.force_nonce_check = force_nonce_check
         self.group_id = group_id
         self.group_name = group_name
         self.region_id = region_id
         self.request_config = request_config
         self.request_id = request_id
         self.request_parameters = request_parameters
-        self.result_descriptions = result_descriptions
         self.result_sample = result_sample
         self.result_type = result_type
         self.stage_name = stage_name
         self.visibility = visibility
 
     def validate(self):
         if self.error_code_samples:
             self.error_code_samples.validate()
         if self.request_config:
             self.request_config.validate()
         if self.request_parameters:
             self.request_parameters.validate()
-        if self.result_descriptions:
-            self.result_descriptions.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -9099,16 +9366,14 @@
             result['RegionId'] = self.region_id
         if self.request_config is not None:
             result['RequestConfig'] = self.request_config.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.request_parameters is not None:
             result['RequestParameters'] = self.request_parameters.to_map()
-        if self.result_descriptions is not None:
-            result['ResultDescriptions'] = self.result_descriptions.to_map()
         if self.result_sample is not None:
             result['ResultSample'] = self.result_sample
         if self.result_type is not None:
             result['ResultType'] = self.result_type
         if self.stage_name is not None:
             result['StageName'] = self.stage_name
         if self.visibility is not None:
@@ -9146,17 +9411,14 @@
             temp_model = DescribeApiDocResponseBodyRequestConfig()
             self.request_config = temp_model.from_map(m['RequestConfig'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('RequestParameters') is not None:
             temp_model = DescribeApiDocResponseBodyRequestParameters()
             self.request_parameters = temp_model.from_map(m['RequestParameters'])
-        if m.get('ResultDescriptions') is not None:
-            temp_model = DescribeApiDocResponseBodyResultDescriptions()
-            self.result_descriptions = temp_model.from_map(m['ResultDescriptions'])
         if m.get('ResultSample') is not None:
             self.result_sample = m.get('ResultSample')
         if m.get('ResultType') is not None:
             self.result_type = m.get('ResultType')
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         if m.get('Visibility') is not None:
@@ -9210,15 +9472,17 @@
 
 class DescribeApiGroupRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # The key of the tag.
         self.key = key
+        # The value of the tag.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9244,16 +9508,18 @@
 class DescribeApiGroupRequest(TeaModel):
     def __init__(
         self,
         group_id: str = None,
         security_token: str = None,
         tag: List[DescribeApiGroupRequestTag] = None,
     ):
+        # The ID of the API group. This ID is generated by the system and globally unique.
         self.group_id = group_id
         self.security_token = security_token
+        # The object tags that match the lifecycle rule. You can specify multiple tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -9290,38 +9556,61 @@
 
 class DescribeApiGroupResponseBodyCustomDomainsDomainItem(TeaModel):
     def __init__(
         self,
         bind_stage_name: str = None,
         certificate_id: str = None,
         certificate_name: str = None,
+        certificate_valid_end: int = None,
+        certificate_valid_start: int = None,
         custom_domain_type: str = None,
         domain_binding_status: str = None,
         domain_cnamestatus: str = None,
         domain_legal_status: str = None,
         domain_name: str = None,
         domain_remark: str = None,
         domain_web_socket_status: str = None,
         is_http_redirect_to_https: bool = None,
         wildcard_domain_patterns: str = None,
-        wss_enable: str = None,
     ):
+        # The name of the bound runtime environment.
         self.bind_stage_name = bind_stage_name
+        # The unique ID of the SSL certificate, which is automatically generated by the system.
         self.certificate_id = certificate_id
+        # The name of the SSL certificate.
         self.certificate_name = certificate_name
+        self.certificate_valid_end = certificate_valid_end
+        self.certificate_valid_start = certificate_valid_start
+        # The type of the custom domain name.
         self.custom_domain_type = custom_domain_type
+        # The binding status of the custom domain name. Valid values:
+        # 
+        # *   **BINDING**: The domain name is bound.
+        # *   **BOUND**: The domain name is not bound.
         self.domain_binding_status = domain_binding_status
+        # The domain name resolution status. Valid values:
+        # 
+        # *   **RESOLVED**: The domain name has been resolved.
+        # *   **UNRESOLVED**: The domain name has not been resolved.
         self.domain_cnamestatus = domain_cnamestatus
+        # The validity status of the domain name. Valid values:
+        # 
+        # *   **NORMAL**: The domain name is valid.
+        # *   **ABNORMAL**: The domain name is invalid. This status affects API calls and must be resolved as soon as possible.
         self.domain_legal_status = domain_legal_status
+        # The domain name.
         self.domain_name = domain_name
+        # The domain name-related remarks, such as the cause for a domain name exception.
         self.domain_remark = domain_remark
+        # The status of the domain name that uses the WebSocket feature.
         self.domain_web_socket_status = domain_web_socket_status
+        # Indicates whether to redirect HTTP requests to HTTPS.
         self.is_http_redirect_to_https = is_http_redirect_to_https
+        # The wildcard domain name mode.
         self.wildcard_domain_patterns = wildcard_domain_patterns
-        self.wss_enable = wss_enable
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -9330,14 +9619,18 @@
         result = dict()
         if self.bind_stage_name is not None:
             result['BindStageName'] = self.bind_stage_name
         if self.certificate_id is not None:
             result['CertificateId'] = self.certificate_id
         if self.certificate_name is not None:
             result['CertificateName'] = self.certificate_name
+        if self.certificate_valid_end is not None:
+            result['CertificateValidEnd'] = self.certificate_valid_end
+        if self.certificate_valid_start is not None:
+            result['CertificateValidStart'] = self.certificate_valid_start
         if self.custom_domain_type is not None:
             result['CustomDomainType'] = self.custom_domain_type
         if self.domain_binding_status is not None:
             result['DomainBindingStatus'] = self.domain_binding_status
         if self.domain_cnamestatus is not None:
             result['DomainCNAMEStatus'] = self.domain_cnamestatus
         if self.domain_legal_status is not None:
@@ -9348,26 +9641,28 @@
             result['DomainRemark'] = self.domain_remark
         if self.domain_web_socket_status is not None:
             result['DomainWebSocketStatus'] = self.domain_web_socket_status
         if self.is_http_redirect_to_https is not None:
             result['IsHttpRedirectToHttps'] = self.is_http_redirect_to_https
         if self.wildcard_domain_patterns is not None:
             result['WildcardDomainPatterns'] = self.wildcard_domain_patterns
-        if self.wss_enable is not None:
-            result['WssEnable'] = self.wss_enable
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BindStageName') is not None:
             self.bind_stage_name = m.get('BindStageName')
         if m.get('CertificateId') is not None:
             self.certificate_id = m.get('CertificateId')
         if m.get('CertificateName') is not None:
             self.certificate_name = m.get('CertificateName')
+        if m.get('CertificateValidEnd') is not None:
+            self.certificate_valid_end = m.get('CertificateValidEnd')
+        if m.get('CertificateValidStart') is not None:
+            self.certificate_valid_start = m.get('CertificateValidStart')
         if m.get('CustomDomainType') is not None:
             self.custom_domain_type = m.get('CustomDomainType')
         if m.get('DomainBindingStatus') is not None:
             self.domain_binding_status = m.get('DomainBindingStatus')
         if m.get('DomainCNAMEStatus') is not None:
             self.domain_cnamestatus = m.get('DomainCNAMEStatus')
         if m.get('DomainLegalStatus') is not None:
@@ -9378,16 +9673,14 @@
             self.domain_remark = m.get('DomainRemark')
         if m.get('DomainWebSocketStatus') is not None:
             self.domain_web_socket_status = m.get('DomainWebSocketStatus')
         if m.get('IsHttpRedirectToHttps') is not None:
             self.is_http_redirect_to_https = m.get('IsHttpRedirectToHttps')
         if m.get('WildcardDomainPatterns') is not None:
             self.wildcard_domain_patterns = m.get('WildcardDomainPatterns')
-        if m.get('WssEnable') is not None:
-            self.wss_enable = m.get('WssEnable')
         return self
 
 
 class DescribeApiGroupResponseBodyCustomDomains(TeaModel):
     def __init__(
         self,
         domain_item: List[DescribeApiGroupResponseBodyCustomDomainsDomainItem] = None,
@@ -9425,16 +9718,19 @@
 class DescribeApiGroupResponseBodyStageItemsStageInfo(TeaModel):
     def __init__(
         self,
         description: str = None,
         stage_id: str = None,
         stage_name: str = None,
     ):
+        # The description of the runtime environment.
         self.description = description
+        # The ID of the runtime environment.
         self.stage_id = stage_id
+        # The name of the runtime environment.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9497,76 +9793,118 @@
 
 
 class DescribeApiGroupResponseBody(TeaModel):
     def __init__(
         self,
         base_path: str = None,
         billing_status: str = None,
-        classic_vpc_sub_domain: str = None,
         cloud_market_commodity: bool = None,
         cms_monitor_group: str = None,
         compatible_flags: str = None,
         created_time: str = None,
         custom_domains: DescribeApiGroupResponseBodyCustomDomains = None,
         custom_trace_config: str = None,
         customer_configs: str = None,
+        dedicated_instance_type: str = None,
         default_domain: str = None,
         description: str = None,
         group_id: str = None,
         group_name: str = None,
         https_policy: str = None,
         illegal_status: str = None,
         instance_id: str = None,
         instance_type: str = None,
-        instance_vip_list: str = None,
         ipv_6status: str = None,
+        migration_error: str = None,
+        migration_status: str = None,
         modified_time: str = None,
         passthrough_headers: str = None,
         region_id: str = None,
         request_id: str = None,
-        rpc_pattern: str = None,
         stage_items: DescribeApiGroupResponseBodyStageItems = None,
         status: str = None,
         sub_domain: str = None,
         traffic_limit: int = None,
         user_log_config: str = None,
         vpc_domain: str = None,
         vpc_slb_intranet_domain: str = None,
     ):
+        # The root path of the API.
         self.base_path = base_path
+        # The billing status of the API group.
+        # 
+        # *   **NORMAL**: The API group is normal.
+        # *   **LOCKED**: The API group is locked due to overdue payments.
         self.billing_status = billing_status
-        self.classic_vpc_sub_domain = classic_vpc_sub_domain
+        # The products on Alibaba Cloud Marketplace.
         self.cloud_market_commodity = cloud_market_commodity
+        # The CloudMonitor application group.
         self.cms_monitor_group = cms_monitor_group
+        # The list of associated tags. Separate multiple tags with commas (,).
         self.compatible_flags = compatible_flags
+        # The creation time (UTC) of the API group.
         self.created_time = created_time
+        # The custom domain name information.
         self.custom_domains = custom_domains
+        # The custom trace configuration.
         self.custom_trace_config = custom_trace_config
+        # The list of custom configuration items.
         self.customer_configs = customer_configs
+        self.dedicated_instance_type = dedicated_instance_type
+        # The default domain name.
         self.default_domain = default_domain
+        # The description of the API group.
         self.description = description
+        # The ID of the API group. This ID is generated by the system and globally unique.
         self.group_id = group_id
+        # The name of the group to which the API belongs.
         self.group_name = group_name
+        # The HTTPS policy.
         self.https_policy = https_policy
+        # The validity status of the API group. Valid values:
+        # 
+        # *   **NORMAL**: The API group is normal.
+        # *   **LOCKED**: The API group is locked because it is not valid.
         self.illegal_status = illegal_status
+        # The ID of the instance.
         self.instance_id = instance_id
+        # The type of the instance.
+        # 
+        # *   CLASSIC_SHARED: shared instance that uses the classic network configuration
+        # *   VPC_SHARED: shared instance that uses VPC
+        # *   VPC_DEDICATED: dedicated instance that uses VPC
         self.instance_type = instance_type
-        self.instance_vip_list = instance_vip_list
+        # The IPv6 status.
         self.ipv_6status = ipv_6status
+        self.migration_error = migration_error
+        self.migration_status = migration_status
+        # The last modification time (UTC) of the API group.
         self.modified_time = modified_time
+        # Specifies whether to pass headers.
         self.passthrough_headers = passthrough_headers
+        # The region to which the API group belongs.
         self.region_id = region_id
+        # The ID of the request.
         self.request_id = request_id
-        self.rpc_pattern = rpc_pattern
+        # The runtime environment information.
         self.stage_items = stage_items
+        # The status of the API group.
+        # 
+        # *   **NORMAL**: The API group is normal.
+        # *   **DELETE**: The API group is deleted.
         self.status = status
+        # The second-level domain name automatically assigned to the API group.
         self.sub_domain = sub_domain
+        # The upper QPS limit of the API group. The default value is 500. You can increase the upper limit by submitting an application.
         self.traffic_limit = traffic_limit
+        # The user log settings.
         self.user_log_config = user_log_config
+        # The VPC domain name.
         self.vpc_domain = vpc_domain
+        # The VPC SLB domain name.
         self.vpc_slb_intranet_domain = vpc_slb_intranet_domain
 
     def validate(self):
         if self.custom_domains:
             self.custom_domains.validate()
         if self.stage_items:
             self.stage_items.validate()
@@ -9577,30 +9915,30 @@
             return _map
 
         result = dict()
         if self.base_path is not None:
             result['BasePath'] = self.base_path
         if self.billing_status is not None:
             result['BillingStatus'] = self.billing_status
-        if self.classic_vpc_sub_domain is not None:
-            result['ClassicVpcSubDomain'] = self.classic_vpc_sub_domain
         if self.cloud_market_commodity is not None:
             result['CloudMarketCommodity'] = self.cloud_market_commodity
         if self.cms_monitor_group is not None:
             result['CmsMonitorGroup'] = self.cms_monitor_group
         if self.compatible_flags is not None:
             result['CompatibleFlags'] = self.compatible_flags
         if self.created_time is not None:
             result['CreatedTime'] = self.created_time
         if self.custom_domains is not None:
             result['CustomDomains'] = self.custom_domains.to_map()
         if self.custom_trace_config is not None:
             result['CustomTraceConfig'] = self.custom_trace_config
         if self.customer_configs is not None:
             result['CustomerConfigs'] = self.customer_configs
+        if self.dedicated_instance_type is not None:
+            result['DedicatedInstanceType'] = self.dedicated_instance_type
         if self.default_domain is not None:
             result['DefaultDomain'] = self.default_domain
         if self.description is not None:
             result['Description'] = self.description
         if self.group_id is not None:
             result['GroupId'] = self.group_id
         if self.group_name is not None:
@@ -9609,28 +9947,28 @@
             result['HttpsPolicy'] = self.https_policy
         if self.illegal_status is not None:
             result['IllegalStatus'] = self.illegal_status
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.instance_type is not None:
             result['InstanceType'] = self.instance_type
-        if self.instance_vip_list is not None:
-            result['InstanceVipList'] = self.instance_vip_list
         if self.ipv_6status is not None:
             result['Ipv6Status'] = self.ipv_6status
+        if self.migration_error is not None:
+            result['MigrationError'] = self.migration_error
+        if self.migration_status is not None:
+            result['MigrationStatus'] = self.migration_status
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.passthrough_headers is not None:
             result['PassthroughHeaders'] = self.passthrough_headers
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.rpc_pattern is not None:
-            result['RpcPattern'] = self.rpc_pattern
         if self.stage_items is not None:
             result['StageItems'] = self.stage_items.to_map()
         if self.status is not None:
             result['Status'] = self.status
         if self.sub_domain is not None:
             result['SubDomain'] = self.sub_domain
         if self.traffic_limit is not None:
@@ -9645,16 +9983,14 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BasePath') is not None:
             self.base_path = m.get('BasePath')
         if m.get('BillingStatus') is not None:
             self.billing_status = m.get('BillingStatus')
-        if m.get('ClassicVpcSubDomain') is not None:
-            self.classic_vpc_sub_domain = m.get('ClassicVpcSubDomain')
         if m.get('CloudMarketCommodity') is not None:
             self.cloud_market_commodity = m.get('CloudMarketCommodity')
         if m.get('CmsMonitorGroup') is not None:
             self.cms_monitor_group = m.get('CmsMonitorGroup')
         if m.get('CompatibleFlags') is not None:
             self.compatible_flags = m.get('CompatibleFlags')
         if m.get('CreatedTime') is not None:
@@ -9662,14 +9998,16 @@
         if m.get('CustomDomains') is not None:
             temp_model = DescribeApiGroupResponseBodyCustomDomains()
             self.custom_domains = temp_model.from_map(m['CustomDomains'])
         if m.get('CustomTraceConfig') is not None:
             self.custom_trace_config = m.get('CustomTraceConfig')
         if m.get('CustomerConfigs') is not None:
             self.customer_configs = m.get('CustomerConfigs')
+        if m.get('DedicatedInstanceType') is not None:
+            self.dedicated_instance_type = m.get('DedicatedInstanceType')
         if m.get('DefaultDomain') is not None:
             self.default_domain = m.get('DefaultDomain')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('GroupId') is not None:
             self.group_id = m.get('GroupId')
         if m.get('GroupName') is not None:
@@ -9678,28 +10016,28 @@
             self.https_policy = m.get('HttpsPolicy')
         if m.get('IllegalStatus') is not None:
             self.illegal_status = m.get('IllegalStatus')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('InstanceType') is not None:
             self.instance_type = m.get('InstanceType')
-        if m.get('InstanceVipList') is not None:
-            self.instance_vip_list = m.get('InstanceVipList')
         if m.get('Ipv6Status') is not None:
             self.ipv_6status = m.get('Ipv6Status')
+        if m.get('MigrationError') is not None:
+            self.migration_error = m.get('MigrationError')
+        if m.get('MigrationStatus') is not None:
+            self.migration_status = m.get('MigrationStatus')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('PassthroughHeaders') is not None:
             self.passthrough_headers = m.get('PassthroughHeaders')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('RpcPattern') is not None:
-            self.rpc_pattern = m.get('RpcPattern')
         if m.get('StageItems') is not None:
             temp_model = DescribeApiGroupResponseBodyStageItems()
             self.stage_items = temp_model.from_map(m['StageItems'])
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('SubDomain') is not None:
             self.sub_domain = m.get('SubDomain')
@@ -10304,20 +10642,26 @@
         api_name: str = None,
         group_id: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_id = api_id
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.api_name = api_name
+        # The ID of the API.
         self.group_id = group_id
+        # The ID of the request.
         self.page_number = page_number
+        # The page number of the returned page.
         self.page_size = page_size
         self.security_token = security_token
+        # The name of the API. The name is used for fuzzy match.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10370,23 +10714,36 @@
         group_id: str = None,
         group_name: str = None,
         history_version: str = None,
         region_id: str = None,
         stage_name: str = None,
         status: str = None,
     ):
+        # Creates an object
         self.api_id = api_id
+        # The region where the API is located.
         self.api_name = api_name
+        # The historical version of the API.
         self.deployed_time = deployed_time
+        # The name of the group to which an API belongs.
         self.description = description
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST.
         self.group_id = group_id
+        # The publishing time (UTC) of the API.
         self.group_name = group_name
+        # CreateObject
         self.history_version = history_version
+        # Queries the historical versions of a specified API.
         self.region_id = region_id
+        # The name of the API.
         self.stage_name = stage_name
+        # The description of the API.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10481,18 +10838,23 @@
         self,
         api_his_items: DescribeApiHistoriesResponseBodyApiHisItems = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The ID of the API.
         self.api_his_items = api_his_items
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned API information. It is an array consisting of ApiHisItem data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # Indicates whether an API version is effective. Valid values: ONLINE and OFFLINE.
         self.total_count = total_count
 
     def validate(self):
         if self.api_his_items:
             self.api_his_items.validate()
 
     def to_map(self):
@@ -10578,18 +10940,26 @@
         self,
         api_id: str = None,
         group_id: str = None,
         history_version: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The ID of the API.
         self.api_id = api_id
+        # The ID of the API group to which the API belongs. This ID is generated by the system and globally unique.
         self.group_id = group_id
+        # The historical version number of the API.
         self.history_version = history_version
         self.security_token = security_token
+        # The environment to which the API is published. Valid values:
+        # 
+        # *   **RELEASE**: production environment
+        # *   **TEST**: test environment
+        # *   **PRE**: staging environment
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10627,16 +10997,19 @@
 class DescribeApiHistoryResponseBodyBackendConfig(TeaModel):
     def __init__(
         self,
         backend_id: str = None,
         backend_name: str = None,
         backend_type: str = None,
     ):
+        # The ID of the backend service.
         self.backend_id = backend_id
+        # The name of the backend service.
         self.backend_name = backend_name
+        # The type of the backend service.
         self.backend_type = backend_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10667,17 +11040,21 @@
     def __init__(
         self,
         constant_value: str = None,
         description: str = None,
         location: str = None,
         service_parameter_name: str = None,
     ):
+        # The value of the constant parameter.
         self.constant_value = constant_value
+        # The description of the parameter.
         self.description = description
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The name of the backend parameter that corresponds to the constant parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10748,18 +11125,23 @@
         self,
         demo_value: str = None,
         description: str = None,
         location: str = None,
         parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # The sample value of the parameter.
         self.demo_value = demo_value
+        # The description of the parameter.
         self.description = description
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The name of the parameter.
         self.parameter_name = parameter_name
+        # The name of the backend parameter that corresponds to the custom system parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10832,16 +11214,19 @@
 class DescribeApiHistoryResponseBodyErrorCodeSamplesErrorCodeSample(TeaModel):
     def __init__(
         self,
         code: str = None,
         description: str = None,
         message: str = None,
     ):
+        # The error code.
         self.code = code
+        # The description.
         self.description = description
+        # The error message.
         self.message = message
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10907,17 +11292,22 @@
     def __init__(
         self,
         id_token_param_name: str = None,
         open_id_api_type: str = None,
         public_key: str = None,
         public_key_id: str = None,
     ):
+        # The name of the parameter that corresponds to the token.
         self.id_token_param_name = id_token_param_name
+        # *   ****\
+        # *   ****\
         self.open_id_api_type = open_id_api_type
+        # The public key of the API.
         self.public_key = public_key
+        # The ID of the public key.
         self.public_key_id = public_key_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10955,20 +11345,31 @@
         body_model: str = None,
         post_body_description: str = None,
         request_http_method: str = None,
         request_mode: str = None,
         request_path: str = None,
         request_protocol: str = None,
     ):
+        # The format in which data was transmitted to the server for a POST or PUT request. Valid values: FORM and STREAM. FORM indicates that data was transmitted as forms that consist of key-value pairs. STREAM indicates that data was transmitted as byte streams. This parameter takes effect when the RequestMode parameter is set to MAPPING.
         self.body_format = body_format
+        # The body model.
         self.body_model = body_model
+        # The description of the request body.
         self.post_body_description = post_body_description
+        # The HTTP request method. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_http_method = request_http_method
+        # The request mode of the parameters. Valid values:
+        # 
+        # *   MAPPING: Parameters are mapped. Unknown parameters are filtered out.
+        # *   PASSTHROUGH: Parameters are passed through.
+        # *   MAPPING_PASSTHROUGH: Parameters are mapped. Unknown parameters are passed through.
         self.request_mode = request_mode
+        # The request path of the API.
         self.request_path = request_path
+        # The type of the protocol that is supported by the API. Valid values: HTTP, HTTPS, and WebSocket. Separate multiple values with commas (,). Example: "HTTP,HTTPS".
         self.request_protocol = request_protocol
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11028,30 +11429,47 @@
         max_value: int = None,
         min_length: int = None,
         min_value: int = None,
         parameter_type: str = None,
         regular_expression: str = None,
         required: str = None,
     ):
+        # The name of the parameter in the API request.
         self.api_parameter_name = api_parameter_name
+        # The type of the array element.
         self.array_items_type = array_items_type
+        # The default value of the parameter.
         self.default_value = default_value
+        # The sample value of the parameter.
         self.demo_value = demo_value
+        # The description of the parameter.
         self.description = description
+        # The order in which the parameter is sorted in the document.
         self.doc_order = doc_order
+        # Indicates whether the document is public. Valid values: **PUBLIC** and **PRIVATE**.
         self.doc_show = doc_show
+        # The hash values can be specified if the **ParameterType** parameter is set to Int, Long, Float, Double, or String. Separate multiple hash values with commas (,). Examples: 1,2,3,4,9 and A,B,C,E,F.
         self.enum_value = enum_value
+        # The JSON scheme.
         self.json_scheme = json_scheme
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The maximum length of the parameter value if the **ParameterType** parameter is set to String.
         self.max_length = max_length
+        # The maximum value of the parameter if the **ParameterType** parameter is set to Int, Long, Float, or Double.
         self.max_value = max_value
+        # The minimum length of the parameter value if the **ParameterType** parameter is set to String.
         self.min_length = min_length
+        # The minimum value of the parameter if the **ParameterType** parameter is set to Int, Long, Float, or Double.
         self.min_value = min_value
+        # The data type of the parameter. Valid values: String, Int, Long, Float, Double, and Boolean.
         self.parameter_type = parameter_type
+        # The regular expression that is used to validate the parameter if the **ParameterType** parameter is set to String.
         self.regular_expression = regular_expression
+        # Indicates whether the parameter is required. Valid values: **REQUIRED** and **OPTIONAL**.
         self.required = required
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11177,21 +11595,29 @@
         id: str = None,
         key: str = None,
         mandatory: bool = None,
         name: str = None,
         pid: str = None,
         type: str = None,
     ):
+        # The description.
         self.description = description
+        # Indicates whether a subnode exists.
         self.has_child = has_child
+        # The ID of the result.
         self.id = id
+        # The primary key of the result.
         self.key = key
+        # Indicates whether the parameter is required.
         self.mandatory = mandatory
+        # The name of the result.
         self.name = name
+        # The ID of the parent node.
         self.pid = pid
+        # The type of the result.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11277,17 +11703,21 @@
     def __init__(
         self,
         event_bridge_region_id: str = None,
         event_bus: str = None,
         event_source: str = None,
         role_arn: str = None,
     ):
+        # The ID of the region where EventBridge is deployed.
         self.event_bridge_region_id = event_bridge_region_id
+        # The event bus.
         self.event_bus = event_bus
+        # The event source.
         self.event_source = event_source
+        # The ARN of the RAM role that is assigned to EventBridge.
         self.role_arn = role_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11330,25 +11760,41 @@
         only_business_path: bool = None,
         path: str = None,
         qualifier: str = None,
         region_id: str = None,
         role_arn: str = None,
         service_name: str = None,
     ):
+        # The ContentType header that is used if the ServiceProtocol parameter is set to HTTP. Valid values:
+        # 
+        # *   **DEFAULT**: the default header in API Gateway
+        # *   **CUSTOM**: a custom header
+        # *   **CLIENT**: the ContentType header of the client
         self.content_type_catagory = content_type_catagory
+        # The value of the ContentType header if the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value
+        # The root path of the service in Function Compute.
         self.fc_base_url = fc_base_url
+        # The type of the service in Function Compute.
         self.fc_type = fc_type
+        # The function name that is defined in Function Compute.
         self.function_name = function_name
+        # The request method.
         self.method = method
+        # Indicates whether the backend receives only the service path.
         self.only_business_path = only_business_path
+        # The path of the API request.
         self.path = path
+        # The alias of the function.
         self.qualifier = qualifier
+        # The ID of the region.
         self.region_id = region_id
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role that is assumed by API Gateway to access Function Compute.
         self.role_arn = role_arn
+        # The service name that is defined in Function Compute.
         self.service_name = service_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11413,15 +11859,17 @@
 
 class DescribeApiHistoryResponseBodyServiceConfigMockHeadersMockHeader(TeaModel):
     def __init__(
         self,
         header_name: str = None,
         header_value: str = None,
     ):
+        # The name of the HTTP header
         self.header_name = header_name
+        # The value of the HTTP header.
         self.header_value = header_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11484,16 +11932,18 @@
         self,
         action: str = None,
         bucket_name: str = None,
         key: str = None,
         oss_region_id: str = None,
     ):
         self.action = action
+        # The name of the OSS bucket.
         self.bucket_name = bucket_name
         self.key = key
+        # The ID of the region where OSS is deployed.
         self.oss_region_id = oss_region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11529,18 +11979,23 @@
         self,
         instance_id: str = None,
         name: str = None,
         port: int = None,
         vpc_id: str = None,
         vpc_scheme: str = None,
     ):
+        # The ID of the Elastic Compute Service (ECS) or Server Load Balancer (SLB) instance in the VPC.
         self.instance_id = instance_id
+        # The name of the VPC.
         self.name = name
+        # The port number that corresponds to the instance.
         self.port = port
+        # The ID of the VPC.
         self.vpc_id = vpc_id
+        # The protocol of the VPC.
         self.vpc_scheme = vpc_scheme
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11592,30 +12047,59 @@
         service_path: str = None,
         service_protocol: str = None,
         service_timeout: int = None,
         service_vpc_enable: str = None,
         vpc_config: DescribeApiHistoryResponseBodyServiceConfigVpcConfig = None,
         vpc_id: str = None,
     ):
+        # The ContentType header that is used if the ServiceProtocol parameter is set to HTTP. Valid values:
+        # 
+        # *   DEFAULT: the default header in API Gateway
+        # *   CUSTOM: a custom header
+        # *   CLIENT: the ContentType header of the client
         self.content_type_catagory = content_type_catagory
+        # The value of the ContentType header if the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value
+        # The configuration items of EventBridge.
         self.event_bridge_config = event_bridge_config
+        # The configuration items of the backend service whose type is Function Compute.
         self.function_compute_config = function_compute_config
+        # Indicates whether the mock mode is enabled. Valid values:
+        # 
+        # *   TRUE
+        # *   FALSE
         self.mock = mock
+        # The mock headers.
         self.mock_headers = mock_headers
+        # The result that is returned if the Mock parameter is set to TRUE.
         self.mock_result = mock_result
+        # The status code that is returned for service mocking.
         self.mock_status_code = mock_status_code
+        # The configuration items of the backend service whose type is Object Storage Service (OSS).
         self.oss_config = oss_config
+        # The URL that is used to call the backend service.
         self.service_address = service_address
+        # The HTTP request method that is used if the ServiceProtocol parameter is set to HTTP. Valid values: PUT, GET, POST, DELETE, PATCH, HEAD, OPTIONS, and ANY.
         self.service_http_method = service_http_method
+        # The path that is used when the backend service is called.
         self.service_path = service_path
+        # The protocol of the backend service. Only HTTP, HTTPS, and Function Compute are supported.
         self.service_protocol = service_protocol
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_timeout = service_timeout
+        # Indicates whether the VPC channel is enabled. Valid values:
+        # 
+        # *   TRUE
+        # *   FALSE
+        # 
+        # Before you can enable the VPC channel, make sure that a VPC authorization is added.
         self.service_vpc_enable = service_vpc_enable
+        # The configuration items of the VPC channel.
         self.vpc_config = vpc_config
+        # The ID of the virtual private cloud (VPC).
         self.vpc_id = vpc_id
 
     def validate(self):
         if self.event_bridge_config:
             self.event_bridge_config.validate()
         if self.function_compute_config:
             self.function_compute_config.validate()
@@ -11715,16 +12199,19 @@
 class DescribeApiHistoryResponseBodyServiceParametersServiceParameter(TeaModel):
     def __init__(
         self,
         location: str = None,
         parameter_type: str = None,
         service_parameter_name: str = None,
     ):
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The data type of the parameter. Valid values: STRING, NUMBER, and BOOLEAN.
         self.parameter_type = parameter_type
+        # The name of the backend parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11788,15 +12275,17 @@
 
 class DescribeApiHistoryResponseBodyServiceParametersMapServiceParameterMap(TeaModel):
     def __init__(
         self,
         request_parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # The name of the frontend parameter. The name must be included in RequestParametersObject and match ApiParameterName in RequestParameters.
         self.request_parameter_name = request_parameter_name
+        # The name of the backend parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11859,18 +12348,23 @@
         self,
         demo_value: str = None,
         description: str = None,
         location: str = None,
         parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # The sample value of the parameter.
         self.demo_value = demo_value
+        # The description of the parameter.
         self.description = description
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The name of the parameter. Valid values: CaClientIp, CaDomain, CaRequestHandleTime, CaAppId, CaRequestId, CaHttpSchema, and CaProxy.
         self.parameter_name = parameter_name
+        # The name of the backend parameter that corresponds to the system parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11975,48 +12469,120 @@
         service_parameters_map: DescribeApiHistoryResponseBodyServiceParametersMap = None,
         stage_name: str = None,
         status: str = None,
         system_parameters: DescribeApiHistoryResponseBodySystemParameters = None,
         visibility: str = None,
         web_socket_api_type: str = None,
     ):
+        # The signature algorithm that is used if the **AuthType** parameter is set to **APP**. If no value is specified for the AllowSignatureMethod parameter, the default value HmacSHA256 is used. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method
+        # The ID of the API.
         self.api_id = api_id
+        # The name of the API.
         self.api_name = api_name
+        # The type of AppCode authentication. Default value: DEFAULT. Valid values:
+        # 
+        # *   DEFAULT: AppCode authentication is supported after the API is published in Alibaba Cloud Marketplace.
+        # *   DISABLE: AppCode authentication is not supported.
+        # *   HEADER: AppCode authentication is supported only in Header parameters.
+        # *   HEADER_QUERY: AppCode authentication is supported in Header or Query parameters.
         self.app_code_auth_type = app_code_auth_type
+        # The type of the security authentication that is used for the API. Valid values:
+        # 
+        # *   **APP**: The API can be called only by authorized applications.
+        # 
+        # *   **ANONYMOUS**: The API can be anonymously called. Take note of the following information:
+        # 
+        #     *   All users who have obtained the API service information can call this API. API Gateway neither authenticates callers nor sets user-specific throttling policies. If this API is a public one, you must set throttling policies for it.
         self.auth_type = auth_type
+        # The configuration items of the backend service.
         self.backend_config = backend_config
+        # Indicates whether the backend service is enabled.
         self.backend_enable = backend_enable
+        # The constant parameters.
         self.constant_parameters = constant_parameters
+        # The custom system parameters.
         self.custom_system_parameters = custom_system_parameters
+        # The time when the API was published. The time is displayed in UTC.
         self.deployed_time = deployed_time
+        # The description of the API.
         self.description = description
+        # *   If the **DisableInternet** parameter is set to **true**, you call the API only over internal networks.
+        # *   If the **DisableInternet** parameter is set to **false**, no limit is imposed on networks. When you create an API, the default value of this parameter is false.
         self.disable_internet = disable_internet
+        # The sample error codes that are returned from the backend service.
+        # 
+        # For more information, see [ErrorCodeSample](~~44392~~).
         self.error_code_samples = error_code_samples
+        # The sample error response that is returned from the backend service.
         self.fail_result_sample = fail_result_sample
+        # *   Indicates whether to forcefully check X-Ca-Nonce. X-Ca-Nonce is the unique identifier of a request and is generally identified by UUID. If the **ForceNonceCheck** parameter is set to **true**, X-Ca-Nonce is forcefully checked. After API Gateway receives this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps defend against replay attacks.
+        # *   If the **ForceNonceCheck** parameter is set to **false**, X-Ca-Nonce is not checked. When you create an API, the default value of this parameter is false.
         self.force_nonce_check = force_nonce_check
+        # The ID of the API group.
         self.group_id = group_id
+        # The name of the API group.
         self.group_name = group_name
+        # The historical version number of the API.
         self.history_version = history_version
+        # The configuration items of third-party OpenID Connect authentication.
         self.open_id_connect_config = open_id_connect_config
+        # The ID of the region where the API is deployed.
         self.region_id = region_id
+        # The configuration items of API requests that are sent from the consumer to API Gateway.
+        # 
+        # For more information, see [RequestConfig](~~43985~~).
         self.request_config = request_config
+        # The ID of the request.
         self.request_id = request_id
+        # The parameters of API requests that are sent from the consumer to API Gateway.
+        # 
+        # For more information, see [RequestParameter](~~43986~~).
         self.request_parameters = request_parameters
+        # The response of the API.
         self.result_body_model = result_body_model
+        # The descriptions that are returned for the API.
         self.result_descriptions = result_descriptions
+        # The sample response.
         self.result_sample = result_sample
+        # The type of data that is returned.
         self.result_type = result_type
+        # The information about backend service calls.
         self.service_config = service_config
+        # The parameters of API requests that are sent from API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameter](~~43988~~).
         self.service_parameters = service_parameters
+        # The mappings between the parameters of requests sent from the consumer to API Gateway and the parameters of requests sent from API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameterMap](~~43989~~).
         self.service_parameters_map = service_parameters_map
+        # The environment to which the API is published. Valid values:
+        # 
+        # *   **RELEASE**: production environment
+        # *   **PRE**: staging environment
+        # *   **TEST**: test environment
         self.stage_name = stage_name
         self.status = status
+        # The system parameters of the API in the JSON format.
         self.system_parameters = system_parameters
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**: The API is public. If you publish the definition of a public API to the production environment, the definition is displayed on the APIs page for all users.
+        # *   **PRIVATE**: The API is private. If you publish an API group that contains a private API in Alibaba Cloud Marketplace, the API is not displayed in Alibaba Cloud Marketplace.
         self.visibility = visibility
+        # The type of the API that is used in bidirectional communication. Valid values:
+        # 
+        # *   **COMMON**: common API
+        # *   **REGISTER**: registered API
+        # *   **UNREGISTER**: unregistered API
+        # *   **NOTIFY**: downstream notification API
         self.web_socket_api_type = web_socket_api_type
 
     def validate(self):
         if self.backend_config:
             self.backend_config.validate()
         if self.constant_parameters:
             self.constant_parameters.validate()
@@ -12256,19 +12822,24 @@
         api_ids: str = None,
         group_id: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_ids = api_ids
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.group_id = group_id
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the request.
         self.page_size = page_size
         self.security_token = security_token
+        # The IDs of APIs. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12312,18 +12883,26 @@
         self,
         api_id: str = None,
         api_name: str = None,
         bound_time: str = None,
         ip_control_id: str = None,
         ip_control_name: str = None,
     ):
+        # The name of the ACL.
         self.api_id = api_id
+        # Queries the access control lists (ACLs) that are bound to all the APIs in an API group in a specified environment.
         self.api_name = api_name
+        # The ID of the ACL.
         self.bound_time = bound_time
+        # The name of the API.
         self.ip_control_id = ip_control_id
+        # *   This operation is intended for API callers.
+        # *   If an optional parameter is not specified, all results are returned on separate pages.
+        # 
+        # ·
         self.ip_control_name = ip_control_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12398,18 +12977,23 @@
         self,
         api_ip_controls: DescribeApiIpControlsResponseBodyApiIpControls = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The ID of the API.
         self.api_ip_controls = api_ip_controls
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The information about the ACLs. The information is an array of ApiIpControlItem data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The time of binding.
         self.total_count = total_count
 
     def validate(self):
         if self.api_ip_controls:
             self.api_ip_controls.validate()
 
     def to_map(self):
@@ -13109,19 +13693,24 @@
         api_ids: str = None,
         group_id: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_ids = api_ids
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.group_id = group_id
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the request.
         self.page_size = page_size
         self.security_token = security_token
+        # The IDs of the APIs that you want to query. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13165,18 +13754,24 @@
         self,
         api_id: str = None,
         api_name: str = None,
         bound_time: str = None,
         signature_id: str = None,
         signature_name: str = None,
     ):
+        # The name of the backend signature key.
         self.api_id = api_id
+        # Queries the backend signature keys that are bound to the APIs of a specified API group in a specified environment.
         self.api_name = api_name
+        # The ID of the backend signature key.
         self.bound_time = bound_time
+        # The name of the API.
         self.signature_id = signature_id
+        # *   This API is intended for API providers.
+        # *   The ApiIds parameter is optional. If this parameter is not specified, all results in the specified environment of an API group are returned.
         self.signature_name = signature_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13251,18 +13846,23 @@
         self,
         api_signatures: DescribeApiSignaturesResponseBodyApiSignatures = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The ID of the API.
         self.api_signatures = api_signatures
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned signature key information. It is an array consisting of ApiSignatureItem data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The time when the backend signature key was bound.
         self.total_count = total_count
 
     def validate(self):
         if self.api_signatures:
             self.api_signatures.validate()
 
     def to_map(self):
@@ -13349,19 +13949,24 @@
         api_ids: str = None,
         group_id: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_ids = api_ids
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.group_id = group_id
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the request.
         self.page_size = page_size
         self.security_token = security_token
+        # The IDs of APIs that you want to query. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13405,18 +14010,24 @@
         self,
         api_id: str = None,
         api_name: str = None,
         bound_time: str = None,
         traffic_control_id: str = None,
         traffic_control_name: str = None,
     ):
+        # The name of the throttling policy.
         self.api_id = api_id
+        # Queries the throttling policies bound to all members of an API group in a specified environment.
         self.api_name = api_name
+        # The ID of the throttling policy.
         self.bound_time = bound_time
+        # API operation
         self.traffic_control_id = traffic_control_id
+        # *   This API is intended for API providers.
+        # *   The ApiIds parameter is optional. If this parameter is not specified, all results in the specified environment of an API group are returned.
         self.traffic_control_name = traffic_control_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13491,18 +14102,23 @@
         self,
         api_traffic_controls: DescribeApiTrafficControlsResponseBodyApiTrafficControls = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The ID of the API.
         self.api_traffic_controls = api_traffic_controls
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned throttling policy information. It is an array consisting of ApiTrafficControlItem data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The binding time of the throttling policy.
         self.total_count = total_count
 
     def validate(self):
         if self.api_traffic_controls:
             self.api_traffic_controls.validate()
 
     def to_map(self):
@@ -13866,15 +14482,17 @@
 
 class DescribeApisRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # The tag key.
         self.key = key
+        # The tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13906,30 +14524,47 @@
         api_path: str = None,
         catalog_id: str = None,
         enable_tag_auth: bool = None,
         group_id: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
+        stage_name: str = None,
         tag: List[DescribeApisRequestTag] = None,
         un_deployed: bool = None,
         visibility: str = None,
     ):
+        # The API ID.
         self.api_id = api_id
+        # The HTTP method of the API request.
         self.api_method = api_method
+        # The API name. The name is used for fuzzy match.
         self.api_name = api_name
+        # The request path of the API.
         self.api_path = api_path
+        # The category ID.
         self.catalog_id = catalog_id
+        # Specifies whether to enable tag verification.
         self.enable_tag_auth = enable_tag_auth
+        # The API group ID.
         self.group_id = group_id
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page. Default value: 10.
         self.page_size = page_size
         self.security_token = security_token
+        self.stage_name = stage_name
+        # The tags of objects that match the rule.
         self.tag = tag
+        # Specifies whether to filter unpublished APIs.
         self.un_deployed = un_deployed
+        # Specifies whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**: The API is public. If you publish the definition of a public API to the production environment, the definition is displayed on the APIs page for all users.
+        # *   **PRIVATE**: The API is private. If you publish an API group that contains a private API in Alibaba Cloud Marketplace, the API is not displayed in Alibaba Cloud Marketplace.
         self.visibility = visibility
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -13956,14 +14591,16 @@
             result['GroupId'] = self.group_id
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         if self.un_deployed is not None:
             result['UnDeployed'] = self.un_deployed
         if self.visibility is not None:
@@ -13988,55 +14625,231 @@
             self.group_id = m.get('GroupId')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = DescribeApisRequestTag()
                 self.tag.append(temp_model.from_map(k))
         if m.get('UnDeployed') is not None:
             self.un_deployed = m.get('UnDeployed')
         if m.get('Visibility') is not None:
             self.visibility = m.get('Visibility')
         return self
 
 
+class DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfosDeployedInfo(TeaModel):
+    def __init__(
+        self,
+        deployed_status: str = None,
+        effective_version: str = None,
+        stage_name: str = None,
+    ):
+        # The deployment status. Valid values: DEPLOYED and NONDEPLOYED.
+        self.deployed_status = deployed_status
+        # The deployed version.
+        self.effective_version = effective_version
+        # Stage Name:
+        # 
+        # *   **RELEASE**: production environment
+        # *   **PRE**: staging environment
+        # *   **TEST**: test environment
+        self.stage_name = stage_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.deployed_status is not None:
+            result['DeployedStatus'] = self.deployed_status
+        if self.effective_version is not None:
+            result['EffectiveVersion'] = self.effective_version
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DeployedStatus') is not None:
+            self.deployed_status = m.get('DeployedStatus')
+        if m.get('EffectiveVersion') is not None:
+            self.effective_version = m.get('EffectiveVersion')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        return self
+
+
+class DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfos(TeaModel):
+    def __init__(
+        self,
+        deployed_info: List[DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfosDeployedInfo] = None,
+    ):
+        self.deployed_info = deployed_info
+
+    def validate(self):
+        if self.deployed_info:
+            for k in self.deployed_info:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DeployedInfo'] = []
+        if self.deployed_info is not None:
+            for k in self.deployed_info:
+                result['DeployedInfo'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.deployed_info = []
+        if m.get('DeployedInfo') is not None:
+            for k in m.get('DeployedInfo'):
+                temp_model = DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfosDeployedInfo()
+                self.deployed_info.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeApisResponseBodyApiSummarysApiSummaryTagListTag(TeaModel):
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        # The tag key.
+        self.tag_key = tag_key
+        # The tag value.
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
+class DescribeApisResponseBodyApiSummarysApiSummaryTagList(TeaModel):
+    def __init__(
+        self,
+        tag: List[DescribeApisResponseBodyApiSummarysApiSummaryTagListTag] = None,
+    ):
+        self.tag = tag
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = DescribeApisResponseBodyApiSummarysApiSummaryTagListTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
 class DescribeApisResponseBodyApiSummarysApiSummary(TeaModel):
     def __init__(
         self,
         api_id: str = None,
         api_method: str = None,
         api_name: str = None,
         api_path: str = None,
         created_time: str = None,
+        deployed_infos: DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfos = None,
         description: str = None,
         group_id: str = None,
         group_name: str = None,
         modified_time: str = None,
         region_id: str = None,
+        tag_list: DescribeApisResponseBodyApiSummarysApiSummaryTagList = None,
         visibility: str = None,
     ):
+        # The API ID.
         self.api_id = api_id
+        # The HTTP method of the API request.
         self.api_method = api_method
+        # The API name.
         self.api_name = api_name
+        # The request path of the API.
         self.api_path = api_path
+        # The time when the API was created. The time is displayed in UTC.
         self.created_time = created_time
+        # The API publishing statuses.
+        self.deployed_infos = deployed_infos
+        # The API description.
         self.description = description
+        # The API group ID.
         self.group_id = group_id
+        # The name of the API group to which the API belongs.
         self.group_name = group_name
+        # The time when the API was modified. The time is displayed in UTC.
         self.modified_time = modified_time
+        # The ID of the region to which the API belongs.
         self.region_id = region_id
+        # The tags that are added to the APIs.
+        self.tag_list = tag_list
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**: The API is public.
+        # *   **PRIVATE**: The API is private.
         self.visibility = visibility
 
     def validate(self):
-        pass
+        if self.deployed_infos:
+            self.deployed_infos.validate()
+        if self.tag_list:
+            self.tag_list.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -14046,24 +14859,28 @@
             result['ApiMethod'] = self.api_method
         if self.api_name is not None:
             result['ApiName'] = self.api_name
         if self.api_path is not None:
             result['ApiPath'] = self.api_path
         if self.created_time is not None:
             result['CreatedTime'] = self.created_time
+        if self.deployed_infos is not None:
+            result['DeployedInfos'] = self.deployed_infos.to_map()
         if self.description is not None:
             result['Description'] = self.description
         if self.group_id is not None:
             result['GroupId'] = self.group_id
         if self.group_name is not None:
             result['GroupName'] = self.group_name
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.tag_list is not None:
+            result['TagList'] = self.tag_list.to_map()
         if self.visibility is not None:
             result['Visibility'] = self.visibility
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApiId') is not None:
@@ -14072,24 +14889,30 @@
             self.api_method = m.get('ApiMethod')
         if m.get('ApiName') is not None:
             self.api_name = m.get('ApiName')
         if m.get('ApiPath') is not None:
             self.api_path = m.get('ApiPath')
         if m.get('CreatedTime') is not None:
             self.created_time = m.get('CreatedTime')
+        if m.get('DeployedInfos') is not None:
+            temp_model = DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfos()
+            self.deployed_infos = temp_model.from_map(m['DeployedInfos'])
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('GroupId') is not None:
             self.group_id = m.get('GroupId')
         if m.get('GroupName') is not None:
             self.group_name = m.get('GroupName')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('TagList') is not None:
+            temp_model = DescribeApisResponseBodyApiSummarysApiSummaryTagList()
+            self.tag_list = temp_model.from_map(m['TagList'])
         if m.get('Visibility') is not None:
             self.visibility = m.get('Visibility')
         return self
 
 
 class DescribeApisResponseBodyApiSummarys(TeaModel):
     def __init__(
@@ -14131,18 +14954,23 @@
         self,
         api_summarys: DescribeApisResponseBodyApiSummarys = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The queried API definitions.
         self.api_summarys = api_summarys
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The request ID.
         self.request_id = request_id
+        # The total number of returned entries.
         self.total_count = total_count
 
     def validate(self):
         if self.api_summarys:
             self.api_summarys.validate()
 
     def to_map(self):
@@ -14779,16 +15607,19 @@
     def __init__(
         self,
         ip_control_id: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
     ):
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.ip_control_id = ip_control_id
+        # The ID of the request.
         self.page_number = page_number
+        # The page number of the returned page.
         self.page_size = page_size
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -14829,22 +15660,35 @@
         description: str = None,
         group_id: str = None,
         group_name: str = None,
         region_id: str = None,
         stage_name: str = None,
         visibility: str = None,
     ):
+        # Description
         self.api_id = api_id
+        # *   This API is intended for API providers.
+        # *   You can specify PageNumber to obtain the result on the specified page.
         self.api_name = api_name
+        # The ID of the API.
         self.bound_time = bound_time
+        # The name of the API group.
         self.description = description
+        # The API operation.
         self.group_id = group_id
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_name = group_name
+        # Queries the APIs that are bound to an access control list (ACL).
         self.region_id = region_id
+        # The region where the API is located.
         self.stage_name = stage_name
+        # The description of the API.
         self.visibility = visibility
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14935,18 +15779,26 @@
         self,
         api_infos: DescribeApisByIpControlResponseBodyApiInfos = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**\
+        # *   **PRIVATE**\
         self.api_infos = api_infos
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned API information. It is an array consisting of ApiInfo data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The binding time of the API.
         self.total_count = total_count
 
     def validate(self):
         if self.api_infos:
             self.api_infos.validate()
 
     def to_map(self):
@@ -15031,17 +15883,20 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         signature_id: str = None,
     ):
+        # The ID of the request.
         self.page_number = page_number
+        # The page number of the returned page.
         self.page_size = page_size
         self.security_token = security_token
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.signature_id = signature_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15081,22 +15936,35 @@
         description: str = None,
         group_id: str = None,
         group_name: str = None,
         region_id: str = None,
         stage_name: str = None,
         visibility: str = None,
     ):
+        # Description
         self.api_id = api_id
+        # *   This API is intended for API providers.
+        # *   The results are returned on separate pages. You can specify PageNumber to obtain the result on the specified page.
         self.api_name = api_name
+        # The ID of the API.
         self.bound_time = bound_time
+        # The name of the group to which the API belongs.
         self.description = description
+        # The name of the API.
         self.group_id = group_id
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_name = group_name
+        # Queries the APIs to which a specified backend signature key is bound.
         self.region_id = region_id
+        # The region where the API is located.
         self.stage_name = stage_name
+        # The description of the API.
         self.visibility = visibility
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15187,18 +16055,26 @@
         self,
         api_infos: DescribeApisBySignatureResponseBodyApiInfos = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**\
+        # *   **PRIVATE**\
         self.api_infos = api_infos
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned API information. It is an array consisting of ApiInfo data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The binding time of the API.
         self.total_count = total_count
 
     def validate(self):
         if self.api_infos:
             self.api_infos.validate()
 
     def to_map(self):
@@ -15283,17 +16159,20 @@
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         traffic_control_id: str = None,
     ):
+        # The ID of the request.
         self.page_number = page_number
+        # The page number of the returned page.
         self.page_size = page_size
         self.security_token = security_token
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.traffic_control_id = traffic_control_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15333,22 +16212,35 @@
         description: str = None,
         group_id: str = None,
         group_name: str = None,
         region_id: str = None,
         stage_name: str = None,
         visibility: str = None,
     ):
+        # Description
         self.api_id = api_id
+        # *   This API is intended for API providers.
+        # *   You can specify PageNumber to obtain the result on the specified page.
         self.api_name = api_name
+        # The ID of the API.
         self.bound_time = bound_time
+        # The name of the group to which an API belongs.
         self.description = description
+        # The name of the API
         self.group_id = group_id
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_name = group_name
+        # Queries the APIs to which a specified throttling policy is bound.
         self.region_id = region_id
+        # The region where the API is located.
         self.stage_name = stage_name
+        # The description of the API.
         self.visibility = visibility
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15439,18 +16331,26 @@
         self,
         api_infos: DescribeApisByTrafficControlResponseBodyApiInfos = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**\
+        # *   **PRIVATE**\
         self.api_infos = api_infos
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned API information. It is an array consisting of ApiInfo data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The binding time of the API.
         self.total_count = total_count
 
     def validate(self):
         if self.api_infos:
             self.api_infos.validate()
 
     def to_map(self):
@@ -15567,21 +16467,23 @@
 class DescribeAppResponseBody(TeaModel):
     def __init__(
         self,
         app_id: int = None,
         app_name: str = None,
         created_time: str = None,
         description: str = None,
+        extend: str = None,
         modified_time: str = None,
         request_id: str = None,
     ):
         self.app_id = app_id
         self.app_name = app_name
         self.created_time = created_time
         self.description = description
+        self.extend = extend
         self.modified_time = modified_time
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -15594,14 +16496,16 @@
             result['AppId'] = self.app_id
         if self.app_name is not None:
             result['AppName'] = self.app_name
         if self.created_time is not None:
             result['CreatedTime'] = self.created_time
         if self.description is not None:
             result['Description'] = self.description
+        if self.extend is not None:
+            result['Extend'] = self.extend
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         return result
 
     def from_map(self, m: dict = None):
@@ -15610,14 +16514,16 @@
             self.app_id = m.get('AppId')
         if m.get('AppName') is not None:
             self.app_name = m.get('AppName')
         if m.get('CreatedTime') is not None:
             self.created_time = m.get('CreatedTime')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('Extend') is not None:
+            self.extend = m.get('Extend')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         return self
 
 
@@ -15702,25 +16608,27 @@
     def __init__(
         self,
         app_code: str = None,
         app_id: int = None,
         app_key: str = None,
         app_name: str = None,
         enable_tag_auth: bool = None,
+        extend: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         sort: str = None,
         tag: List[DescribeAppAttributesRequestTag] = None,
     ):
         self.app_code = app_code
         self.app_id = app_id
         self.app_key = app_key
         self.app_name = app_name
         self.enable_tag_auth = enable_tag_auth
+        self.extend = extend
         self.page_number = page_number
         self.page_size = page_size
         self.security_token = security_token
         self.sort = sort
         self.tag = tag
 
     def validate(self):
@@ -15741,14 +16649,16 @@
             result['AppId'] = self.app_id
         if self.app_key is not None:
             result['AppKey'] = self.app_key
         if self.app_name is not None:
             result['AppName'] = self.app_name
         if self.enable_tag_auth is not None:
             result['EnableTagAuth'] = self.enable_tag_auth
+        if self.extend is not None:
+            result['Extend'] = self.extend
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         if self.sort is not None:
@@ -15767,14 +16677,16 @@
             self.app_id = m.get('AppId')
         if m.get('AppKey') is not None:
             self.app_key = m.get('AppKey')
         if m.get('AppName') is not None:
             self.app_name = m.get('AppName')
         if m.get('EnableTagAuth') is not None:
             self.enable_tag_auth = m.get('EnableTagAuth')
+        if m.get('Extend') is not None:
+            self.extend = m.get('Extend')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         if m.get('Sort') is not None:
@@ -15858,21 +16770,23 @@
 class DescribeAppAttributesResponseBodyAppsAppAttribute(TeaModel):
     def __init__(
         self,
         app_id: int = None,
         app_name: str = None,
         created_time: str = None,
         description: str = None,
+        extend: str = None,
         modified_time: str = None,
         tags: DescribeAppAttributesResponseBodyAppsAppAttributeTags = None,
     ):
         self.app_id = app_id
         self.app_name = app_name
         self.created_time = created_time
         self.description = description
+        self.extend = extend
         self.modified_time = modified_time
         self.tags = tags
 
     def validate(self):
         if self.tags:
             self.tags.validate()
 
@@ -15886,14 +16800,16 @@
             result['AppId'] = self.app_id
         if self.app_name is not None:
             result['AppName'] = self.app_name
         if self.created_time is not None:
             result['CreatedTime'] = self.created_time
         if self.description is not None:
             result['Description'] = self.description
+        if self.extend is not None:
+            result['Extend'] = self.extend
         if self.modified_time is not None:
             result['ModifiedTime'] = self.modified_time
         if self.tags is not None:
             result['Tags'] = self.tags.to_map()
         return result
 
     def from_map(self, m: dict = None):
@@ -15902,14 +16818,16 @@
             self.app_id = m.get('AppId')
         if m.get('AppName') is not None:
             self.app_name = m.get('AppName')
         if m.get('CreatedTime') is not None:
             self.created_time = m.get('CreatedTime')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('Extend') is not None:
+            self.extend = m.get('Extend')
         if m.get('ModifiedTime') is not None:
             self.modified_time = m.get('ModifiedTime')
         if m.get('Tags') is not None:
             temp_model = DescribeAppAttributesResponseBodyAppsAppAttributeTags()
             self.tags = temp_model.from_map(m['Tags'])
         return self
 
@@ -16232,17 +17150,21 @@
         self,
         app_id: int = None,
         app_owner: int = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
     ):
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.app_id = app_id
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.app_owner = app_owner
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the request.
         self.page_size = page_size
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -16281,16 +17203,21 @@
 class DescribeAppsResponseBodyAppsAppItem(TeaModel):
     def __init__(
         self,
         app_id: int = None,
         app_name: str = None,
         description: str = None,
     ):
+        # Queries the apps. App information is returned only to the app owner.
         self.app_id = app_id
+        # The ID of the app.
         self.app_name = app_name
+        # *   This API is intended for API providers.
+        # *   API providers can use the app IDs or their Apsara Stack tenant accounts to query app information.
+        # *   Each provider can call this operation for a maximum of 200 times every day in a region.
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16357,18 +17284,23 @@
         self,
         apps: DescribeAppsResponseBodyApps = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The description of the app.
         self.apps = apps
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned app information. It is an array consisting of AppItem data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The name of the app.
         self.total_count = total_count
 
     def validate(self):
         if self.apps:
             self.apps.validate()
 
     def to_map(self):
@@ -16453,16 +17385,19 @@
     def __init__(
         self,
         app_id: int = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
     ):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.app_id = app_id
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the request.
         self.page_size = page_size
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -16505,24 +17440,42 @@
         description: str = None,
         group_id: str = None,
         group_name: str = None,
         operator: str = None,
         region_id: str = None,
         stage_name: str = None,
     ):
+        # The expiration time of the authorization in UTC.
         self.api_id = api_id
+        # *   This operation is intended for API callers.
+        # *   The specified application can call all APIs included in the responses.
         self.api_name = api_name
+        # Queries weather based on the region name
         self.auth_vaild_time = auth_vaild_time
+        # The description of the authorization.
         self.authorization_source = authorization_source
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.authorized_time = authorized_time
+        # The name of the API group.
         self.description = description
+        # The authorizer. Valid values:
+        # 
+        # *   **PROVIDER:** the API owner
+        # *   **CONSUMER:** the API caller
         self.group_id = group_id
+        # The authorization time in UTC.
         self.group_name = group_name
+        # The name of the API operation.
         self.operator = operator
+        # Queries the authorized APIs of a specified application.
         self.region_id = region_id
+        # The region to which the API belongs.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16621,18 +17574,26 @@
         self,
         authorized_apis: DescribeAuthorizedApisResponseBodyAuthorizedApis = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The authorization source. Valid values:
+        # 
+        # *   **CONSOLE**\
+        # *   **API**\
         self.authorized_apis = authorized_apis
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The authorized API set.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The unique identifier of the API, which is generated by the system.
         self.total_count = total_count
 
     def validate(self):
         if self.authorized_apis:
             self.authorized_apis.validate()
 
     def to_map(self):
@@ -17018,14 +17979,130 @@
         if m.get('BackendId') is not None:
             self.backend_id = m.get('BackendId')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
+class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfigNacosConfig(TeaModel):
+    def __init__(
+        self,
+        access_key: str = None,
+        auth_type: str = None,
+        clusters: str = None,
+        group_name: str = None,
+        namespace: str = None,
+        password: str = None,
+        secret_key: str = None,
+        server_address: str = None,
+        service_name: str = None,
+        user_name: str = None,
+    ):
+        self.access_key = access_key
+        self.auth_type = auth_type
+        self.clusters = clusters
+        self.group_name = group_name
+        self.namespace = namespace
+        self.password = password
+        self.secret_key = secret_key
+        self.server_address = server_address
+        self.service_name = service_name
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_key is not None:
+            result['AccessKey'] = self.access_key
+        if self.auth_type is not None:
+            result['AuthType'] = self.auth_type
+        if self.clusters is not None:
+            result['Clusters'] = self.clusters
+        if self.group_name is not None:
+            result['GroupName'] = self.group_name
+        if self.namespace is not None:
+            result['Namespace'] = self.namespace
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.secret_key is not None:
+            result['SecretKey'] = self.secret_key
+        if self.server_address is not None:
+            result['ServerAddress'] = self.server_address
+        if self.service_name is not None:
+            result['ServiceName'] = self.service_name
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessKey') is not None:
+            self.access_key = m.get('AccessKey')
+        if m.get('AuthType') is not None:
+            self.auth_type = m.get('AuthType')
+        if m.get('Clusters') is not None:
+            self.clusters = m.get('Clusters')
+        if m.get('GroupName') is not None:
+            self.group_name = m.get('GroupName')
+        if m.get('Namespace') is not None:
+            self.namespace = m.get('Namespace')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('SecretKey') is not None:
+            self.secret_key = m.get('SecretKey')
+        if m.get('ServerAddress') is not None:
+            self.server_address = m.get('ServerAddress')
+        if m.get('ServiceName') is not None:
+            self.service_name = m.get('ServiceName')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        return self
+
+
+class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfig(TeaModel):
+    def __init__(
+        self,
+        nacos_config: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfigNacosConfig = None,
+        rc_type: str = None,
+    ):
+        self.nacos_config = nacos_config
+        self.rc_type = rc_type
+
+    def validate(self):
+        if self.nacos_config:
+            self.nacos_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.nacos_config is not None:
+            result['NacosConfig'] = self.nacos_config.to_map()
+        if self.rc_type is not None:
+            result['RcType'] = self.rc_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NacosConfig') is not None:
+            temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfigNacosConfig()
+            self.nacos_config = temp_model.from_map(m['NacosConfig'])
+        if m.get('RcType') is not None:
+            self.rc_type = m.get('RcType')
+        return self
+
+
 class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigEventBridgeConfig(TeaModel):
     def __init__(
         self,
         event_bridge_region_id: str = None,
         event_bus: str = None,
         event_source: str = None,
         role_arn: str = None,
@@ -17311,31 +18388,37 @@
             self.vpc_target_host_name = m.get('VpcTargetHostName')
         return self
 
 
 class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfig(TeaModel):
     def __init__(
         self,
+        discovery_config: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfig = None,
         event_bridge_config: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigEventBridgeConfig = None,
         function_compute_config: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigFunctionComputeConfig = None,
+        http_target_host_name: str = None,
         mock_config: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfig = None,
         oss_config: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigOssConfig = None,
         service_address: str = None,
         type: str = None,
         vpc_config: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigVpcConfig = None,
     ):
+        self.discovery_config = discovery_config
         self.event_bridge_config = event_bridge_config
         self.function_compute_config = function_compute_config
+        self.http_target_host_name = http_target_host_name
         self.mock_config = mock_config
         self.oss_config = oss_config
         self.service_address = service_address
         self.type = type
         self.vpc_config = vpc_config
 
     def validate(self):
+        if self.discovery_config:
+            self.discovery_config.validate()
         if self.event_bridge_config:
             self.event_bridge_config.validate()
         if self.function_compute_config:
             self.function_compute_config.validate()
         if self.mock_config:
             self.mock_config.validate()
         if self.oss_config:
@@ -17345,38 +18428,47 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.discovery_config is not None:
+            result['DiscoveryConfig'] = self.discovery_config.to_map()
         if self.event_bridge_config is not None:
             result['EventBridgeConfig'] = self.event_bridge_config.to_map()
         if self.function_compute_config is not None:
             result['FunctionComputeConfig'] = self.function_compute_config.to_map()
+        if self.http_target_host_name is not None:
+            result['HttpTargetHostName'] = self.http_target_host_name
         if self.mock_config is not None:
             result['MockConfig'] = self.mock_config.to_map()
         if self.oss_config is not None:
             result['OssConfig'] = self.oss_config.to_map()
         if self.service_address is not None:
             result['ServiceAddress'] = self.service_address
         if self.type is not None:
             result['Type'] = self.type
         if self.vpc_config is not None:
             result['VpcConfig'] = self.vpc_config.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DiscoveryConfig') is not None:
+            temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfig()
+            self.discovery_config = temp_model.from_map(m['DiscoveryConfig'])
         if m.get('EventBridgeConfig') is not None:
             temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigEventBridgeConfig()
             self.event_bridge_config = temp_model.from_map(m['EventBridgeConfig'])
         if m.get('FunctionComputeConfig') is not None:
             temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigFunctionComputeConfig()
             self.function_compute_config = temp_model.from_map(m['FunctionComputeConfig'])
+        if m.get('HttpTargetHostName') is not None:
+            self.http_target_host_name = m.get('HttpTargetHostName')
         if m.get('MockConfig') is not None:
             temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfig()
             self.mock_config = temp_model.from_map(m['MockConfig'])
         if m.get('OssConfig') is not None:
             temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigOssConfig()
             self.oss_config = temp_model.from_map(m['OssConfig'])
         if m.get('ServiceAddress') is not None:
@@ -18783,17 +19875,24 @@
     def __init__(
         self,
         api_id: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The ID of the API.
         self.api_id = api_id
+        # The ID of the API group. An API group ID is generated by the system and is globally unique.
         self.group_id = group_id
         self.security_token = security_token
+        # The environment in which the API runs. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18828,17 +19927,21 @@
     def __init__(
         self,
         constant_value: str = None,
         description: str = None,
         location: str = None,
         service_parameter_name: str = None,
     ):
+        # The constant value.
         self.constant_value = constant_value
+        # The description of the parameter.
         self.description = description
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The name of the backend service parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18909,18 +20012,23 @@
         self,
         demo_value: str = None,
         description: str = None,
         location: str = None,
         parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # The sample value.
         self.demo_value = demo_value
+        # The description of the parameter.
         self.description = description
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The name of the custom system parameter.
         self.parameter_name = parameter_name
+        # The name of the corresponding backend parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18993,16 +20101,19 @@
 class DescribeDeployedApiResponseBodyErrorCodeSamplesErrorCodeSample(TeaModel):
     def __init__(
         self,
         code: str = None,
         description: str = None,
         message: str = None,
     ):
+        # The error code returned if the request failed.
         self.code = code
+        # The description of the error.
         self.description = description
+        # The error message returned if the request failed.
         self.message = message
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19068,17 +20179,24 @@
     def __init__(
         self,
         id_token_param_name: str = None,
         open_id_api_type: str = None,
         public_key: str = None,
         public_key_id: str = None,
     ):
+        # The name of the parameter that corresponds to the token.
         self.id_token_param_name = id_token_param_name
+        # The OpenID Connect mode. Valid values:
+        # 
+        # *   **IDTOKEN:** OpenID Connect calls the authentication API to issue tokens. If the value is specified, the PublicKeyId parameter and the PublicKey parameter are required.
+        # *   **BUSINESS:** OpenID Connect calls the business API to verify identities by using existing tokens. If this value is specified, the IdTokenParamName parameter is required.
         self.open_id_api_type = open_id_api_type
+        # The public key of the API.
         self.public_key = public_key
+        # The ID of the public key.
         self.public_key_id = public_key_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19116,20 +20234,33 @@
         body_model: str = None,
         post_body_description: str = None,
         request_http_method: str = None,
         request_mode: str = None,
         request_path: str = None,
         request_protocol: str = None,
     ):
+        # This parameter takes effect only when the **RequestMode** parameter is set to **MAPPING**.
+        # 
+        # The format in which data is transmitted to the server for POST and PUT requests. Valid values: **FORM** and **STREAM**. FORM indicates that data is transmitted in the key-value pair format. STREAM indicates that data is transmitted as byte streams.
         self.body_format = body_format
+        # The body model.
         self.body_model = body_model
+        # The description of the request body.
         self.post_body_description = post_body_description
+        # The HTTP method that is used to make the request. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_http_method = request_http_method
+        # The request mode. Valid values:
+        # 
+        # *   MAPPING: Parameters are mapped. Unknown parameters are filtered out.
+        # *   PASSTHROUGH: Parameters are passed through.
+        # *   MAPPING_PASSTHROUGH: Parameters are mapped. Unknown parameters are passed through.
         self.request_mode = request_mode
+        # The path of the API request. If the complete API URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, The path of the API request is ` /object/add  `.
         self.request_path = request_path
+        # The protocol type supported by the API. Valid values: HTTP, HTTPS, and WebSocket. Separate multiple values with commas (,). Example: "HTTP,HTTPS".
         self.request_protocol = request_protocol
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19189,30 +20320,47 @@
         max_value: int = None,
         min_length: int = None,
         min_value: int = None,
         parameter_type: str = None,
         regular_expression: str = None,
         required: str = None,
     ):
+        # The name of the API parameter.
         self.api_parameter_name = api_parameter_name
+        # The type of the array element.
         self.array_items_type = array_items_type
+        # The default value.
         self.default_value = default_value
+        # The sample value.
         self.demo_value = demo_value
+        # The parameter description.
         self.description = description
+        # The order in the document.
         self.doc_order = doc_order
+        # Indicates whether the document is public. Valid values: **PUBLIC** and **PRIVATE**.
         self.doc_show = doc_show
+        # The hash values that can be entered when **ParameterType** is set to Int, Long, Float, Double, or String. Separate different values with commas (,). Examples: 1,2,3,4,9 and A,B,C,E,F.
         self.enum_value = enum_value
+        # JSON scheme
         self.json_scheme = json_scheme
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The maximum length of the **ParameterType** parameter when the parameter is set to String.
         self.max_length = max_length
+        # The maximum value of the **ParameterType** parameter when the parameter is set to Int, Long, Float, or Double.
         self.max_value = max_value
+        # The minimum length of the **ParameterType** parameter when the parameter is set to String.
         self.min_length = min_length
+        # The minimum value of the **ParameterType** parameter when the parameter is set to Int, Long, Float, or Double.
         self.min_value = min_value
+        # The type of the parameter. Valid values: String, Int, Long, Float, Double, and Boolean.
         self.parameter_type = parameter_type
+        # The regular expression used for parameter validation when **ParameterType** is set to String.
         self.regular_expression = regular_expression
+        # Indicates whether the parameter is required. Valid values: **REQUIRED** and **OPTIONAL**.
         self.required = required
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19338,18 +20486,20 @@
         id: str = None,
         key: str = None,
         mandatory: bool = None,
         name: str = None,
         pid: str = None,
         type: str = None,
     ):
+        # The description of the parameter.
         self.description = description
         self.has_child = has_child
         self.id = id
         self.key = key
+        # Indicates whether the parameter is required.
         self.mandatory = mandatory
         self.name = name
         self.pid = pid
         self.type = type
 
     def validate(self):
         pass
@@ -19446,25 +20596,41 @@
         only_business_path: bool = None,
         path: str = None,
         qualifier: str = None,
         region_id: str = None,
         role_arn: str = None,
         service_name: str = None,
     ):
+        # The ContentType header used when a backend HTTP service is called. Valid values:
+        # 
+        # *   **DEFAULT:** the default header in API Gateway
+        # *   **CUSTOM:** a custom header
+        # *   **CLIENT:** the ContentType header specified by the client
         self.content_type_catagory = content_type_catagory
+        # The value of the ContentType header when the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value
+        # The root path of Function Compute.
         self.fc_base_url = fc_base_url
+        # The type of the Function Compute instance.
         self.fc_type = fc_type
+        # The function name defined in Function Compute.
         self.function_name = function_name
+        # The request method.
         self.method = method
+        # Indicates whether the backend receives only the service path.
         self.only_business_path = only_business_path
+        # The API request path.
         self.path = path
+        # The alias of the function.
         self.qualifier = qualifier
+        # The region in which the instance resides.
         self.region_id = region_id
+        # The ARN of the RAM role assumed by API Gateway to access Function Compute.
         self.role_arn = role_arn
+        # The service name defined in Function Compute.
         self.service_name = service_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19529,15 +20695,17 @@
 
 class DescribeDeployedApiResponseBodyServiceConfigMockHeadersMockHeader(TeaModel):
     def __init__(
         self,
         header_name: str = None,
         header_value: str = None,
     ):
+        # The name of the HTTP header parameter.
         self.header_name = header_name
+        # The value of the HTTP header parameter.
         self.header_value = header_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19599,17 +20767,21 @@
     def __init__(
         self,
         instance_id: str = None,
         name: str = None,
         port: int = None,
         vpc_id: str = None,
     ):
+        # The ID of the Elastic Compute Service (ECS) or Server Load Balancer (SLB) instance in the VPC.
         self.instance_id = instance_id
+        # The name of the VPC access authorization.
         self.name = name
+        # The port number that corresponds to the instance.
         self.port = port
+        # The ID of the VPC.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19653,26 +20825,45 @@
         service_path: str = None,
         service_protocol: str = None,
         service_timeout: int = None,
         service_vpc_enable: str = None,
         vpc_config: DescribeDeployedApiResponseBodyServiceConfigVpcConfig = None,
         vpc_id: str = None,
     ):
+        # The backend configuration items when the backend service is Function Compute.
         self.function_compute_config = function_compute_config
+        # Indicates whether the Mock mode is enabled. Valid values:
+        # 
+        # *   **TRUE:** The Mock mode is enabled.
+        # *   **FALSE:** The Mock mode is not enabled.
         self.mock = mock
+        # The mock headers.
         self.mock_headers = mock_headers
+        # The result returned when the Mock mode is enabled.
         self.mock_result = mock_result
+        # The status code returned for service mock.
         self.mock_status_code = mock_status_code
+        # The URL that is used to call the backend service. If the complete URL of a backend service is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the value of ServiceAddress is **http://api.a.com:8080**.``
         self.service_address = service_address
+        # The HTTP method that is used to call a backend service. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.service_http_method = service_http_method
+        # The path that is used to call the backend service. If the complete URL of a backend service is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the value of the **ServicePath** parameter is `/object/add`.
         self.service_path = service_path
+        # The backend service protocol. Only HTTP, HTTPS, and Function Compute are supported.
         self.service_protocol = service_protocol
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_timeout = service_timeout
+        # Indicates whether to enable the VPC channel. Valid values:
+        # 
+        # *   **TRUE**: The VPC channel is enabled. You can enable a VPC channel only after you create the corresponding access authorization for the VPC.
+        # *   **FALSE**: The VPC channel is not enabled.
         self.service_vpc_enable = service_vpc_enable
+        # The configuration items of the VPC channel.
         self.vpc_config = vpc_config
+        # The ID of the VPC.
         self.vpc_id = vpc_id
 
     def validate(self):
         if self.function_compute_config:
             self.function_compute_config.validate()
         if self.mock_headers:
             self.mock_headers.validate()
@@ -19750,16 +20941,19 @@
 class DescribeDeployedApiResponseBodyServiceParametersServiceParameter(TeaModel):
     def __init__(
         self,
         location: str = None,
         parameter_type: str = None,
         service_parameter_name: str = None,
     ):
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The data type of the backend service parameter. Valid values: STRING, NUMBER, and BOOLEAN.
         self.parameter_type = parameter_type
+        # The name of the backend service parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19823,15 +21017,17 @@
 
 class DescribeDeployedApiResponseBodyServiceParametersMapServiceParameterMap(TeaModel):
     def __init__(
         self,
         request_parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # The name of the frontend input parameter.
         self.request_parameter_name = request_parameter_name
+        # The name of the backend service parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19894,18 +21090,23 @@
         self,
         demo_value: str = None,
         description: str = None,
         location: str = None,
         parameter_name: str = None,
         service_parameter_name: str = None,
     ):
+        # The example.
         self.demo_value = demo_value
+        # The description of the parameter.
         self.description = description
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location
+        # The name of the system parameter. Valid values: CaClientIp, CaDomain, CaRequestHandleTime, CaAppId, CaRequestId, CaHttpSchema, CaProxy.
         self.parameter_name = parameter_name
+        # The name of the corresponding backend parameter.
         self.service_parameter_name = service_parameter_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20004,42 +21205,103 @@
         service_config: DescribeDeployedApiResponseBodyServiceConfig = None,
         service_parameters: DescribeDeployedApiResponseBodyServiceParameters = None,
         service_parameters_map: DescribeDeployedApiResponseBodyServiceParametersMap = None,
         stage_name: str = None,
         system_parameters: DescribeDeployedApiResponseBodySystemParameters = None,
         visibility: str = None,
     ):
+        # The signature method used by the client. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method
+        # The ID of the API.
         self.api_id = api_id
+        # The name of the API.
         self.api_name = api_name
+        # The authentication method of the API. Valid values:
+        # 
+        # *   **APP:** Only authorized apps are allowed to call the API.
+        # 
+        # *   **ANONYMOUS**: The API can be anonymously called. In this mode, you must take note of the following rules:
+        # 
+        #     *   All users who have obtained the API service information can call this API. API Gateway does not authenticate callers and cannot set user-specific throttling policies. If the API is made public, set API-specific throttling policies.
         self.auth_type = auth_type
+        # The constant parameters.
         self.constant_parameters = constant_parameters
+        # The custom system parameters.
         self.custom_system_parameters = custom_system_parameters
+        # The deployment time. Format: yyyy-mm-ddhh:mm:ss.
         self.deployed_time = deployed_time
+        # The description of the parameter.
         self.description = description
+        # *   Indicates whether to call the API only in an internal network. If this parameter is set to **true**, the API can be called only in an internal network.
+        # *   If this parameter is set to **false**, the API can be called over the Internet and in an internal network.
+        # 
+        # > If you do not configure this parameter when you modify the API, the original value is used.
         self.disable_internet = disable_internet
+        # The sample error codes returned by the backend service.
+        # 
+        # For more information, see [ErrorCodeSample](~~44392~~).
         self.error_code_samples = error_code_samples
+        # The sample error response from the backend service.
         self.fail_result_sample = fail_result_sample
+        # *   Indicates whether to forcibly check X-Ca-Nonce. If the **ForceNonceCheck** parameter is set to **true**, X-Ca-Nonce is forcibly checked. X-Ca-Nonce is the unique identifier of a request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent replay attacks.
+        # *   If the **ForceNonceCheck** parameter is set to **false**, the X-Ca-Nonce is not checked. Default value: false.
         self.force_nonce_check = force_nonce_check
+        # The ID of the API group.
         self.group_id = group_id
+        # The name of the API group.
         self.group_name = group_name
+        # The configuration items of the third-party OpenID Connect authentication method.
         self.open_id_connect_config = open_id_connect_config
+        # The region in which the API group resides.
         self.region_id = region_id
+        # The configuration items of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestConfig](~~43985~~).
         self.request_config = request_config
+        # The ID of the request.
         self.request_id = request_id
+        # The parameters of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestParameter](~~43986~~).
         self.request_parameters = request_parameters
+        # The return description of the API.
         self.result_body_model = result_body_model
+        # The returned description of the API.
         self.result_descriptions = result_descriptions
+        # The sample response from the backend service.
         self.result_sample = result_sample
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML. Default value: JSON.
         self.result_type = result_type
+        # The configuration items of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceConfig](~~43987~~).
         self.service_config = service_config
+        # The parameters of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameter](~~43988~~).
         self.service_parameters = service_parameters
+        # The mappings between parameters of requests sent by the consumer to API Gateway and parameters of requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameterMap](~~43989~~).
         self.service_parameters_map = service_parameters_map
+        # The environment in which the API runs. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
         self.stage_name = stage_name
+        # The system parameters.
         self.system_parameters = system_parameters
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC:** The API is public. If this parameter is set to PUBLIC, the API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE:** The API is private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.visibility = visibility
 
     def validate(self):
         if self.constant_parameters:
             self.constant_parameters.validate()
         if self.custom_system_parameters:
             self.custom_system_parameters.validate()
@@ -20596,15 +21858,17 @@
 class DescribeDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         group_id: str = None,
         security_token: str = None,
     ):
+        # The custom domain name.
         self.domain_name = domain_name
+        # The private key of the SSL certificate.
         self.group_id = group_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -20635,36 +21899,62 @@
 class DescribeDomainResponseBody(TeaModel):
     def __init__(
         self,
         certificate_body: str = None,
         certificate_id: str = None,
         certificate_name: str = None,
         certificate_private_key: str = None,
+        certificate_valid_end: int = None,
+        certificate_valid_start: int = None,
         domain_binding_status: str = None,
         domain_cnamestatus: str = None,
         domain_legal_status: str = None,
         domain_name: str = None,
         domain_remark: str = None,
         domain_web_socket_status: str = None,
         group_id: str = None,
         request_id: str = None,
         sub_domain: str = None,
     ):
+        # The domain name resolution status. Valid values:
+        # 
+        # *   RESOLVED: The domain name has been resolved.
+        # *   UNRESOLVED: The domain name has not been resolved.
         self.certificate_body = certificate_body
+        # The ID of the request.
         self.certificate_id = certificate_id
+        # The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
         self.certificate_name = certificate_name
+        # The binding status of the custom domain name. Valid values:
+        # 
+        # *   BINDING: The domain name has been bound.
+        # *   BOUND: The domain name has not been bound.
         self.certificate_private_key = certificate_private_key
+        self.certificate_valid_end = certificate_valid_end
+        self.certificate_valid_start = certificate_valid_start
+        # The domain name does not have an ICP filing.
         self.domain_binding_status = domain_binding_status
+        # Queries details about a bound custom domain name, including the automatically assigned second-level domain name, custom domain name, and SSL certificate.
         self.domain_cnamestatus = domain_cnamestatus
+        # The content of the certificate.
         self.domain_legal_status = domain_legal_status
+        # Remarks about the domain name, such as the cause of an exception.
         self.domain_name = domain_name
+        # The unique ID of the SSL certificate, which is automatically generated by the system.
         self.domain_remark = domain_remark
+        # The name of the SSL certificate.
         self.domain_web_socket_status = domain_web_socket_status
+        # The second-level domain name that is automatically assigned to the API group.
         self.group_id = group_id
+        # The validity status of the domain name. Valid values:
+        # 
+        # *   NORMAL
+        # *   ABNORMAL: This status affects API calls and must be resolved as soon as possible.
         self.request_id = request_id
+        # *   This operation is intended for API providers.
         self.sub_domain = sub_domain
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20676,14 +21966,18 @@
             result['CertificateBody'] = self.certificate_body
         if self.certificate_id is not None:
             result['CertificateId'] = self.certificate_id
         if self.certificate_name is not None:
             result['CertificateName'] = self.certificate_name
         if self.certificate_private_key is not None:
             result['CertificatePrivateKey'] = self.certificate_private_key
+        if self.certificate_valid_end is not None:
+            result['CertificateValidEnd'] = self.certificate_valid_end
+        if self.certificate_valid_start is not None:
+            result['CertificateValidStart'] = self.certificate_valid_start
         if self.domain_binding_status is not None:
             result['DomainBindingStatus'] = self.domain_binding_status
         if self.domain_cnamestatus is not None:
             result['DomainCNAMEStatus'] = self.domain_cnamestatus
         if self.domain_legal_status is not None:
             result['DomainLegalStatus'] = self.domain_legal_status
         if self.domain_name is not None:
@@ -20706,14 +22000,18 @@
             self.certificate_body = m.get('CertificateBody')
         if m.get('CertificateId') is not None:
             self.certificate_id = m.get('CertificateId')
         if m.get('CertificateName') is not None:
             self.certificate_name = m.get('CertificateName')
         if m.get('CertificatePrivateKey') is not None:
             self.certificate_private_key = m.get('CertificatePrivateKey')
+        if m.get('CertificateValidEnd') is not None:
+            self.certificate_valid_end = m.get('CertificateValidEnd')
+        if m.get('CertificateValidStart') is not None:
+            self.certificate_valid_start = m.get('CertificateValidStart')
         if m.get('DomainBindingStatus') is not None:
             self.domain_binding_status = m.get('DomainBindingStatus')
         if m.get('DomainCNAMEStatus') is not None:
             self.domain_cnamestatus = m.get('DomainCNAMEStatus')
         if m.get('DomainLegalStatus') is not None:
             self.domain_legal_status = m.get('DomainLegalStatus')
         if m.get('DomainName') is not None:
@@ -21047,14 +22345,2272 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeHistoryApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeImportOASTaskRequest(TeaModel):
+    def __init__(
+        self,
+        operation_id: str = None,
+        security_token: str = None,
+    ):
+        self.operation_id = operation_id
+        self.security_token = security_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operation_id is not None:
+            result['OperationId'] = self.operation_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OperationId') is not None:
+            self.operation_id = m.get('OperationId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeImportOASTaskResponseBodyApiResultsApiResult(TeaModel):
+    def __init__(
+        self,
+        api_id: str = None,
+        api_name: str = None,
+        description: str = None,
+        error_message: str = None,
+        group_id: str = None,
+        method: str = None,
+        path: str = None,
+        update_status: str = None,
+    ):
+        self.api_id = api_id
+        self.api_name = api_name
+        self.description = description
+        self.error_message = error_message
+        self.group_id = group_id
+        self.method = method
+        self.path = path
+        self.update_status = update_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_id is not None:
+            result['ApiId'] = self.api_id
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.method is not None:
+            result['Method'] = self.method
+        if self.path is not None:
+            result['Path'] = self.path
+        if self.update_status is not None:
+            result['UpdateStatus'] = self.update_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiId') is not None:
+            self.api_id = m.get('ApiId')
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('Method') is not None:
+            self.method = m.get('Method')
+        if m.get('Path') is not None:
+            self.path = m.get('Path')
+        if m.get('UpdateStatus') is not None:
+            self.update_status = m.get('UpdateStatus')
+        return self
+
+
+class DescribeImportOASTaskResponseBodyApiResults(TeaModel):
+    def __init__(
+        self,
+        api_result: List[DescribeImportOASTaskResponseBodyApiResultsApiResult] = None,
+    ):
+        self.api_result = api_result
+
+    def validate(self):
+        if self.api_result:
+            for k in self.api_result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ApiResult'] = []
+        if self.api_result is not None:
+            for k in self.api_result:
+                result['ApiResult'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.api_result = []
+        if m.get('ApiResult') is not None:
+            for k in m.get('ApiResult'):
+                temp_model = DescribeImportOASTaskResponseBodyApiResultsApiResult()
+                self.api_result.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeImportOASTaskResponseBodyModelResultsModelResult(TeaModel):
+    def __init__(
+        self,
+        error_message: str = None,
+        group_id: str = None,
+        model_id: str = None,
+        model_name: str = None,
+        update_status: str = None,
+    ):
+        self.error_message = error_message
+        self.group_id = group_id
+        self.model_id = model_id
+        self.model_name = model_name
+        self.update_status = update_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.model_id is not None:
+            result['ModelId'] = self.model_id
+        if self.model_name is not None:
+            result['ModelName'] = self.model_name
+        if self.update_status is not None:
+            result['UpdateStatus'] = self.update_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('ModelId') is not None:
+            self.model_id = m.get('ModelId')
+        if m.get('ModelName') is not None:
+            self.model_name = m.get('ModelName')
+        if m.get('UpdateStatus') is not None:
+            self.update_status = m.get('UpdateStatus')
+        return self
+
+
+class DescribeImportOASTaskResponseBodyModelResults(TeaModel):
+    def __init__(
+        self,
+        model_result: List[DescribeImportOASTaskResponseBodyModelResultsModelResult] = None,
+    ):
+        self.model_result = model_result
+
+    def validate(self):
+        if self.model_result:
+            for k in self.model_result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ModelResult'] = []
+        if self.model_result is not None:
+            for k in self.model_result:
+                result['ModelResult'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.model_result = []
+        if m.get('ModelResult') is not None:
+            for k in m.get('ModelResult'):
+                temp_model = DescribeImportOASTaskResponseBodyModelResultsModelResult()
+                self.model_result.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeImportOASTaskResponseBody(TeaModel):
+    def __init__(
+        self,
+        api_results: DescribeImportOASTaskResponseBodyApiResults = None,
+        model_results: DescribeImportOASTaskResponseBodyModelResults = None,
+        request_id: str = None,
+        task_status: str = None,
+    ):
+        self.api_results = api_results
+        self.model_results = model_results
+        self.request_id = request_id
+        self.task_status = task_status
+
+    def validate(self):
+        if self.api_results:
+            self.api_results.validate()
+        if self.model_results:
+            self.model_results.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_results is not None:
+            result['ApiResults'] = self.api_results.to_map()
+        if self.model_results is not None:
+            result['ModelResults'] = self.model_results.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.task_status is not None:
+            result['TaskStatus'] = self.task_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiResults') is not None:
+            temp_model = DescribeImportOASTaskResponseBodyApiResults()
+            self.api_results = temp_model.from_map(m['ApiResults'])
+        if m.get('ModelResults') is not None:
+            temp_model = DescribeImportOASTaskResponseBodyModelResults()
+            self.model_results = temp_model.from_map(m['ModelResults'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TaskStatus') is not None:
+            self.task_status = m.get('TaskStatus')
+        return self
+
+
+class DescribeImportOASTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeImportOASTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeImportOASTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceDropConnectionsRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        sbc_name: str = None,
+        security_token: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the dedicated instance.
+        self.instance_id = instance_id
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name
+        self.security_token = security_token
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sbc_name is not None:
+            result['SbcName'] = self.sbc_name
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SbcName') is not None:
+            self.sbc_name = m.get('SbcName')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceDropConnectionsResponseBodyInstanceDropConnectionsMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The monitoring time. The time follows the ISO 8601 standard. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The number of dropped packets in the instance.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceDropConnectionsResponseBodyInstanceDropConnections(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceDropConnectionsResponseBodyInstanceDropConnectionsMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceDropConnectionsResponseBodyInstanceDropConnectionsMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceDropConnectionsResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_drop_connections: DescribeInstanceDropConnectionsResponseBodyInstanceDropConnections = None,
+        request_id: str = None,
+    ):
+        # The list of dropped connections in the instance.
+        self.instance_drop_connections = instance_drop_connections
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_drop_connections:
+            self.instance_drop_connections.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_drop_connections is not None:
+            result['InstanceDropConnections'] = self.instance_drop_connections.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceDropConnections') is not None:
+            temp_model = DescribeInstanceDropConnectionsResponseBodyInstanceDropConnections()
+            self.instance_drop_connections = temp_model.from_map(m['InstanceDropConnections'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceDropConnectionsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceDropConnectionsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceDropConnectionsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceDropPacketRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        sbc_name: str = None,
+        security_token: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name
+        self.security_token = security_token
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sbc_name is not None:
+            result['SbcName'] = self.sbc_name
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SbcName') is not None:
+            self.sbc_name = m.get('SbcName')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceDropPacketResponseBodyInstanceDropPacketMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item: str = None,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The metric. Valid values:
+        # 
+        # *   InstanceDropPacketRX: the number of inbound packets dropped in the instance per second.
+        # *   InstanceDropPacketTX: the number of outbound packets dropped in the instance per second.
+        self.item = item
+        # The monitoring time. The time follows the ISO 8601 standard. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The number of dropped packets in the instance.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item is not None:
+            result['Item'] = self.item
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Item') is not None:
+            self.item = m.get('Item')
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceDropPacketResponseBodyInstanceDropPacket(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceDropPacketResponseBodyInstanceDropPacketMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceDropPacketResponseBodyInstanceDropPacketMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceDropPacketResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_drop_packet: DescribeInstanceDropPacketResponseBodyInstanceDropPacket = None,
+        request_id: str = None,
+    ):
+        # The list of dropped packets in the instance.
+        self.instance_drop_packet = instance_drop_packet
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_drop_packet:
+            self.instance_drop_packet.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_drop_packet is not None:
+            result['InstanceDropPacket'] = self.instance_drop_packet.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceDropPacket') is not None:
+            temp_model = DescribeInstanceDropPacketResponseBodyInstanceDropPacket()
+            self.instance_drop_packet = temp_model.from_map(m['InstanceDropPacket'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceDropPacketResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceDropPacketResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceDropPacketResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceHttpCodeRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        security_token: str = None,
+        stage_name: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        self.security_token = security_token
+        # The environment in which the API is requested. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
+        self.stage_name = stage_name
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceHttpCodeResponseBodyInstanceHttpCodeMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The HTTP status code.
+        self.item_time = item_time
+        # The number of HTTP status codes returned.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceHttpCodeResponseBodyInstanceHttpCode(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceHttpCodeResponseBodyInstanceHttpCodeMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceHttpCodeResponseBodyInstanceHttpCodeMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceHttpCodeResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_http_code: DescribeInstanceHttpCodeResponseBodyInstanceHttpCode = None,
+        request_id: str = None,
+    ):
+        # The list of HTTP status codes returned.
+        self.instance_http_code = instance_http_code
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_http_code:
+            self.instance_http_code.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_http_code is not None:
+            result['InstanceHttpCode'] = self.instance_http_code.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceHttpCode') is not None:
+            temp_model = DescribeInstanceHttpCodeResponseBodyInstanceHttpCode()
+            self.instance_http_code = temp_model.from_map(m['InstanceHttpCode'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceHttpCodeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceHttpCodeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceHttpCodeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceLatencyRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        security_token: str = None,
+        stage_name: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        self.security_token = security_token
+        # The environment in which the API is requested. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
+        self.stage_name = stage_name
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceLatencyResponseBodyInstanceLatencyMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item: str = None,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The metric. Valid values:
+        # 
+        # *   gatewayLatency API: the processing latency of API Gateway
+        # *   latency: the processing latency of the backend service.
+        self.item = item
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The value of the average latency.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item is not None:
+            result['Item'] = self.item
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Item') is not None:
+            self.item = m.get('Item')
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceLatencyResponseBodyInstanceLatency(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceLatencyResponseBodyInstanceLatencyMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceLatencyResponseBodyInstanceLatencyMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceLatencyResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_latency: DescribeInstanceLatencyResponseBodyInstanceLatency = None,
+        request_id: str = None,
+    ):
+        # The list of average latencies in the instance.
+        self.instance_latency = instance_latency
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_latency:
+            self.instance_latency.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_latency is not None:
+            result['InstanceLatency'] = self.instance_latency.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceLatency') is not None:
+            temp_model = DescribeInstanceLatencyResponseBodyInstanceLatency()
+            self.instance_latency = temp_model.from_map(m['InstanceLatency'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceLatencyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceLatencyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceLatencyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceNewConnectionsRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        sbc_name: str = None,
+        security_token: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name
+        self.security_token = security_token
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sbc_name is not None:
+            result['SbcName'] = self.sbc_name
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SbcName') is not None:
+            self.sbc_name = m.get('SbcName')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceNewConnectionsResponseBodyInstanceNewConnectionsMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The number of new connections in the instance.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceNewConnectionsResponseBodyInstanceNewConnections(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceNewConnectionsResponseBodyInstanceNewConnectionsMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceNewConnectionsResponseBodyInstanceNewConnectionsMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceNewConnectionsResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_new_connections: DescribeInstanceNewConnectionsResponseBodyInstanceNewConnections = None,
+        request_id: str = None,
+    ):
+        # The list of new connections in the instance.
+        self.instance_new_connections = instance_new_connections
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_new_connections:
+            self.instance_new_connections.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_new_connections is not None:
+            result['InstanceNewConnections'] = self.instance_new_connections.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceNewConnections') is not None:
+            temp_model = DescribeInstanceNewConnectionsResponseBodyInstanceNewConnections()
+            self.instance_new_connections = temp_model.from_map(m['InstanceNewConnections'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceNewConnectionsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceNewConnectionsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceNewConnectionsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstancePacketsRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        sbc_name: str = None,
+        security_token: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name
+        self.security_token = security_token
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sbc_name is not None:
+            result['SbcName'] = self.sbc_name
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SbcName') is not None:
+            self.sbc_name = m.get('SbcName')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstancePacketsResponseBodyInstancePacketsMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item: str = None,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The metric. Valid values:
+        # 
+        # *   InstancePacketRX: inbound data packets
+        # *   InstancePacketTX: outbound data packets
+        self.item = item
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The number of inbound and outbound data packets in the instance.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item is not None:
+            result['Item'] = self.item
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Item') is not None:
+            self.item = m.get('Item')
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstancePacketsResponseBodyInstancePackets(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstancePacketsResponseBodyInstancePacketsMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstancePacketsResponseBodyInstancePacketsMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstancePacketsResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_packets: DescribeInstancePacketsResponseBodyInstancePackets = None,
+        request_id: str = None,
+    ):
+        # The list of inbound and outbound data packets in the instance.
+        self.instance_packets = instance_packets
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_packets:
+            self.instance_packets.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_packets is not None:
+            result['InstancePackets'] = self.instance_packets.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstancePackets') is not None:
+            temp_model = DescribeInstancePacketsResponseBodyInstancePackets()
+            self.instance_packets = temp_model.from_map(m['InstancePackets'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstancePacketsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstancePacketsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstancePacketsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceQpsRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        security_token: str = None,
+        stage_name: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        self.security_token = security_token
+        # The environment in which the API is requested. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
+        self.stage_name = stage_name
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceQpsResponseBodyInstanceQpsMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The monitoring time. The time follows the ISO 8601 standard. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The number of requests sent to the APIs in the instance.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceQpsResponseBodyInstanceQps(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceQpsResponseBodyInstanceQpsMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceQpsResponseBodyInstanceQpsMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceQpsResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_qps: DescribeInstanceQpsResponseBodyInstanceQps = None,
+        request_id: str = None,
+    ):
+        # The list of requests sent to the APIs in the instance.
+        self.instance_qps = instance_qps
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_qps:
+            self.instance_qps.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_qps is not None:
+            result['InstanceQps'] = self.instance_qps.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceQps') is not None:
+            temp_model = DescribeInstanceQpsResponseBodyInstanceQps()
+            self.instance_qps = temp_model.from_map(m['InstanceQps'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceQpsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceQpsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceQpsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceSlbConnectRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        sbc_name: str = None,
+        security_token: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name
+        self.security_token = security_token
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sbc_name is not None:
+            result['SbcName'] = self.sbc_name
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SbcName') is not None:
+            self.sbc_name = m.get('SbcName')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceSlbConnectResponseBodyInstanceSlbConnectMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item: str = None,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The metric. Valid values:
+        # 
+        # *   InstanceMaxConnection: the maximum number of connections
+        # *   InstanceInactiveConnection: the number of inactive connections
+        # *   InstanceActiveConnection: the number of active connections
+        self.item = item
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The number of concurrent connections in the instance.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item is not None:
+            result['Item'] = self.item
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Item') is not None:
+            self.item = m.get('Item')
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceSlbConnectResponseBodyInstanceSlbConnect(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceSlbConnectResponseBodyInstanceSlbConnectMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceSlbConnectResponseBodyInstanceSlbConnectMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceSlbConnectResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_slb_connect: DescribeInstanceSlbConnectResponseBodyInstanceSlbConnect = None,
+        request_id: str = None,
+    ):
+        # The list of concurrent connections in the instance.
+        self.instance_slb_connect = instance_slb_connect
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_slb_connect:
+            self.instance_slb_connect.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_slb_connect is not None:
+            result['InstanceSlbConnect'] = self.instance_slb_connect.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceSlbConnect') is not None:
+            temp_model = DescribeInstanceSlbConnectResponseBodyInstanceSlbConnect()
+            self.instance_slb_connect = temp_model.from_map(m['InstanceSlbConnect'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceSlbConnectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceSlbConnectResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceSlbConnectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeInstanceTrafficRequest(TeaModel):
+    def __init__(
+        self,
+        end_time: str = None,
+        instance_id: str = None,
+        security_token: str = None,
+        stage_name: str = None,
+        start_time: str = None,
+    ):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time
+        # The ID of the instance.
+        self.instance_id = instance_id
+        self.security_token = security_token
+        # The environment in which the API runs. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST: the test environment**\
+        self.stage_name = stage_name
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
+class DescribeInstanceTrafficResponseBodyInstanceTrafficMonitorItem(TeaModel):
+    def __init__(
+        self,
+        item: str = None,
+        item_time: str = None,
+        item_value: str = None,
+    ):
+        # The metric. Valid values:
+        # 
+        # *   inbound: traffic consumed by requests
+        # *   outbound: traffic consumed by responses
+        self.item = item
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time
+        # The amount of traffic consumed by the requests and responses in the instance.
+        self.item_value = item_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.item is not None:
+            result['Item'] = self.item
+        if self.item_time is not None:
+            result['ItemTime'] = self.item_time
+        if self.item_value is not None:
+            result['ItemValue'] = self.item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Item') is not None:
+            self.item = m.get('Item')
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceTrafficResponseBodyInstanceTraffic(TeaModel):
+    def __init__(
+        self,
+        monitor_item: List[DescribeInstanceTrafficResponseBodyInstanceTrafficMonitorItem] = None,
+    ):
+        self.monitor_item = monitor_item
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MonitorItem'] = []
+        if self.monitor_item is not None:
+            for k in self.monitor_item:
+                result['MonitorItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.monitor_item = []
+        if m.get('MonitorItem') is not None:
+            for k in m.get('MonitorItem'):
+                temp_model = DescribeInstanceTrafficResponseBodyInstanceTrafficMonitorItem()
+                self.monitor_item.append(temp_model.from_map(k))
+        return self
+
+
+class DescribeInstanceTrafficResponseBody(TeaModel):
+    def __init__(
+        self,
+        instance_traffic: DescribeInstanceTrafficResponseBodyInstanceTraffic = None,
+        request_id: str = None,
+    ):
+        # The traffic consumed by the requests and responses in the instance.
+        self.instance_traffic = instance_traffic
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        if self.instance_traffic:
+            self.instance_traffic.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_traffic is not None:
+            result['InstanceTraffic'] = self.instance_traffic.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceTraffic') is not None:
+            temp_model = DescribeInstanceTrafficResponseBodyInstanceTraffic()
+            self.instance_traffic = temp_model.from_map(m['InstanceTraffic'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeInstanceTrafficResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeInstanceTrafficResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeInstanceTrafficResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeInstancesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         self.key = key
@@ -21207,82 +24763,198 @@
         if m.get('SpecAttribute') is not None:
             for k in m.get('SpecAttribute'):
                 temp_model = DescribeInstancesResponseBodyInstancesInstanceAttributeInstanceSpecAttributesSpecAttribute()
                 self.spec_attribute.append(temp_model.from_map(k))
         return self
 
 
+class DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributesNetworkInterfaceAttribute(TeaModel):
+    def __init__(
+        self,
+        cidr_block: str = None,
+        security_group_id: str = None,
+        vswitch_id: str = None,
+        zone_id: str = None,
+    ):
+        # vSwitch的网段。
+        self.cidr_block = cidr_block
+        # 安全组的ID，同一个安全组内的服务可以互相访问。
+        self.security_group_id = security_group_id
+        # 虚拟交换机ID
+        self.vswitch_id = vswitch_id
+        # 可用区ID
+        self.zone_id = zone_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cidr_block is not None:
+            result['CidrBlock'] = self.cidr_block
+        if self.security_group_id is not None:
+            result['SecurityGroupId'] = self.security_group_id
+        if self.vswitch_id is not None:
+            result['VswitchId'] = self.vswitch_id
+        if self.zone_id is not None:
+            result['ZoneId'] = self.zone_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CidrBlock') is not None:
+            self.cidr_block = m.get('CidrBlock')
+        if m.get('SecurityGroupId') is not None:
+            self.security_group_id = m.get('SecurityGroupId')
+        if m.get('VswitchId') is not None:
+            self.vswitch_id = m.get('VswitchId')
+        if m.get('ZoneId') is not None:
+            self.zone_id = m.get('ZoneId')
+        return self
+
+
+class DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributes(TeaModel):
+    def __init__(
+        self,
+        network_interface_attribute: List[DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributesNetworkInterfaceAttribute] = None,
+    ):
+        self.network_interface_attribute = network_interface_attribute
+
+    def validate(self):
+        if self.network_interface_attribute:
+            for k in self.network_interface_attribute:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['NetworkInterfaceAttribute'] = []
+        if self.network_interface_attribute is not None:
+            for k in self.network_interface_attribute:
+                result['NetworkInterfaceAttribute'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.network_interface_attribute = []
+        if m.get('NetworkInterfaceAttribute') is not None:
+            for k in m.get('NetworkInterfaceAttribute'):
+                temp_model = DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributesNetworkInterfaceAttribute()
+                self.network_interface_attribute.append(temp_model.from_map(k))
+        return self
+
+
 class DescribeInstancesResponseBodyInstancesInstanceAttribute(TeaModel):
     def __init__(
         self,
         acl_id: str = None,
         acl_name: str = None,
         acl_status: str = None,
         acl_type: str = None,
         classic_egress_address: str = None,
+        connect_cidr_blocks: str = None,
+        connect_vpc_id: str = None,
         created_time: str = None,
+        dedicated_instance_type: str = None,
         egress_ipv_6enable: bool = None,
         expired_time: str = None,
         https_policies: str = None,
+        ipv6acl_id: str = None,
+        ipv6acl_name: str = None,
+        ipv6acl_status: str = None,
+        ipv6acl_type: str = None,
         instance_charge_type: str = None,
+        instance_cidr_block: str = None,
+        instance_cluster_id: str = None,
         instance_id: str = None,
         instance_name: str = None,
         instance_rps_limit: int = None,
         instance_spec: str = None,
         instance_spec_attributes: DescribeInstancesResponseBodyInstancesInstanceAttributeInstanceSpecAttributes = None,
         instance_type: str = None,
         internet_egress_address: str = None,
         intranet_segments: str = None,
+        maintain_end_time: str = None,
+        maintain_start_time: str = None,
+        network_interface_attributes: DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributes = None,
         region_id: str = None,
         status: str = None,
         support_ipv_6: bool = None,
         user_vpc_id: str = None,
         user_vswitch_id: str = None,
-        vip_type_list: str = None,
         vpc_egress_address: str = None,
         vpc_intranet_enable: bool = None,
         vpc_owner_id: int = None,
         vpc_slb_intranet_enable: bool = None,
         zone_id: str = None,
         zone_local_name: str = None,
     ):
         self.acl_id = acl_id
         self.acl_name = acl_name
         self.acl_status = acl_status
         self.acl_type = acl_type
         self.classic_egress_address = classic_egress_address
+        self.connect_cidr_blocks = connect_cidr_blocks
+        # VPC融合类型专享实例联通的用户VPC ID
+        self.connect_vpc_id = connect_vpc_id
         self.created_time = created_time
+        # 专享实例类型
+        # - vpc_connect：VPC融合类型专享实例
+        # - normal：传统类型专享实例
+        self.dedicated_instance_type = dedicated_instance_type
         self.egress_ipv_6enable = egress_ipv_6enable
         self.expired_time = expired_time
         self.https_policies = https_policies
+        self.ipv6acl_id = ipv6acl_id
+        self.ipv6acl_name = ipv6acl_name
+        self.ipv6acl_status = ipv6acl_status
+        self.ipv6acl_type = ipv6acl_type
         self.instance_charge_type = instance_charge_type
+        # 专享实例所在网段
+        # - 172.16.0.0/12
+        # - 192.168.0.0/16
+        self.instance_cidr_block = instance_cidr_block
+        self.instance_cluster_id = instance_cluster_id
         self.instance_id = instance_id
         self.instance_name = instance_name
         self.instance_rps_limit = instance_rps_limit
         self.instance_spec = instance_spec
         self.instance_spec_attributes = instance_spec_attributes
         self.instance_type = instance_type
         self.internet_egress_address = internet_egress_address
         self.intranet_segments = intranet_segments
+        self.maintain_end_time = maintain_end_time
+        self.maintain_start_time = maintain_start_time
+        # VPC融合类型专享实例连通的用户VPC内的网络信息
+        self.network_interface_attributes = network_interface_attributes
         self.region_id = region_id
         self.status = status
         self.support_ipv_6 = support_ipv_6
         self.user_vpc_id = user_vpc_id
         self.user_vswitch_id = user_vswitch_id
-        self.vip_type_list = vip_type_list
         self.vpc_egress_address = vpc_egress_address
         self.vpc_intranet_enable = vpc_intranet_enable
         self.vpc_owner_id = vpc_owner_id
         self.vpc_slb_intranet_enable = vpc_slb_intranet_enable
         self.zone_id = zone_id
         self.zone_local_name = zone_local_name
 
     def validate(self):
         if self.instance_spec_attributes:
             self.instance_spec_attributes.validate()
+        if self.network_interface_attributes:
+            self.network_interface_attributes.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -21292,24 +24964,42 @@
             result['AclName'] = self.acl_name
         if self.acl_status is not None:
             result['AclStatus'] = self.acl_status
         if self.acl_type is not None:
             result['AclType'] = self.acl_type
         if self.classic_egress_address is not None:
             result['ClassicEgressAddress'] = self.classic_egress_address
+        if self.connect_cidr_blocks is not None:
+            result['ConnectCidrBlocks'] = self.connect_cidr_blocks
+        if self.connect_vpc_id is not None:
+            result['ConnectVpcId'] = self.connect_vpc_id
         if self.created_time is not None:
             result['CreatedTime'] = self.created_time
+        if self.dedicated_instance_type is not None:
+            result['DedicatedInstanceType'] = self.dedicated_instance_type
         if self.egress_ipv_6enable is not None:
             result['EgressIpv6Enable'] = self.egress_ipv_6enable
         if self.expired_time is not None:
             result['ExpiredTime'] = self.expired_time
         if self.https_policies is not None:
             result['HttpsPolicies'] = self.https_policies
+        if self.ipv6acl_id is not None:
+            result['IPV6AclId'] = self.ipv6acl_id
+        if self.ipv6acl_name is not None:
+            result['IPV6AclName'] = self.ipv6acl_name
+        if self.ipv6acl_status is not None:
+            result['IPV6AclStatus'] = self.ipv6acl_status
+        if self.ipv6acl_type is not None:
+            result['IPV6AclType'] = self.ipv6acl_type
         if self.instance_charge_type is not None:
             result['InstanceChargeType'] = self.instance_charge_type
+        if self.instance_cidr_block is not None:
+            result['InstanceCidrBlock'] = self.instance_cidr_block
+        if self.instance_cluster_id is not None:
+            result['InstanceClusterId'] = self.instance_cluster_id
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.instance_name is not None:
             result['InstanceName'] = self.instance_name
         if self.instance_rps_limit is not None:
             result['InstanceRpsLimit'] = self.instance_rps_limit
         if self.instance_spec is not None:
@@ -21318,26 +25008,30 @@
             result['InstanceSpecAttributes'] = self.instance_spec_attributes.to_map()
         if self.instance_type is not None:
             result['InstanceType'] = self.instance_type
         if self.internet_egress_address is not None:
             result['InternetEgressAddress'] = self.internet_egress_address
         if self.intranet_segments is not None:
             result['IntranetSegments'] = self.intranet_segments
+        if self.maintain_end_time is not None:
+            result['MaintainEndTime'] = self.maintain_end_time
+        if self.maintain_start_time is not None:
+            result['MaintainStartTime'] = self.maintain_start_time
+        if self.network_interface_attributes is not None:
+            result['NetworkInterfaceAttributes'] = self.network_interface_attributes.to_map()
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.status is not None:
             result['Status'] = self.status
         if self.support_ipv_6 is not None:
             result['SupportIpv6'] = self.support_ipv_6
         if self.user_vpc_id is not None:
             result['UserVpcId'] = self.user_vpc_id
         if self.user_vswitch_id is not None:
             result['UserVswitchId'] = self.user_vswitch_id
-        if self.vip_type_list is not None:
-            result['VipTypeList'] = self.vip_type_list
         if self.vpc_egress_address is not None:
             result['VpcEgressAddress'] = self.vpc_egress_address
         if self.vpc_intranet_enable is not None:
             result['VpcIntranetEnable'] = self.vpc_intranet_enable
         if self.vpc_owner_id is not None:
             result['VpcOwnerId'] = self.vpc_owner_id
         if self.vpc_slb_intranet_enable is not None:
@@ -21356,24 +25050,42 @@
             self.acl_name = m.get('AclName')
         if m.get('AclStatus') is not None:
             self.acl_status = m.get('AclStatus')
         if m.get('AclType') is not None:
             self.acl_type = m.get('AclType')
         if m.get('ClassicEgressAddress') is not None:
             self.classic_egress_address = m.get('ClassicEgressAddress')
+        if m.get('ConnectCidrBlocks') is not None:
+            self.connect_cidr_blocks = m.get('ConnectCidrBlocks')
+        if m.get('ConnectVpcId') is not None:
+            self.connect_vpc_id = m.get('ConnectVpcId')
         if m.get('CreatedTime') is not None:
             self.created_time = m.get('CreatedTime')
+        if m.get('DedicatedInstanceType') is not None:
+            self.dedicated_instance_type = m.get('DedicatedInstanceType')
         if m.get('EgressIpv6Enable') is not None:
             self.egress_ipv_6enable = m.get('EgressIpv6Enable')
         if m.get('ExpiredTime') is not None:
             self.expired_time = m.get('ExpiredTime')
         if m.get('HttpsPolicies') is not None:
             self.https_policies = m.get('HttpsPolicies')
+        if m.get('IPV6AclId') is not None:
+            self.ipv6acl_id = m.get('IPV6AclId')
+        if m.get('IPV6AclName') is not None:
+            self.ipv6acl_name = m.get('IPV6AclName')
+        if m.get('IPV6AclStatus') is not None:
+            self.ipv6acl_status = m.get('IPV6AclStatus')
+        if m.get('IPV6AclType') is not None:
+            self.ipv6acl_type = m.get('IPV6AclType')
         if m.get('InstanceChargeType') is not None:
             self.instance_charge_type = m.get('InstanceChargeType')
+        if m.get('InstanceCidrBlock') is not None:
+            self.instance_cidr_block = m.get('InstanceCidrBlock')
+        if m.get('InstanceClusterId') is not None:
+            self.instance_cluster_id = m.get('InstanceClusterId')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('InstanceName') is not None:
             self.instance_name = m.get('InstanceName')
         if m.get('InstanceRpsLimit') is not None:
             self.instance_rps_limit = m.get('InstanceRpsLimit')
         if m.get('InstanceSpec') is not None:
@@ -21383,26 +25095,31 @@
             self.instance_spec_attributes = temp_model.from_map(m['InstanceSpecAttributes'])
         if m.get('InstanceType') is not None:
             self.instance_type = m.get('InstanceType')
         if m.get('InternetEgressAddress') is not None:
             self.internet_egress_address = m.get('InternetEgressAddress')
         if m.get('IntranetSegments') is not None:
             self.intranet_segments = m.get('IntranetSegments')
+        if m.get('MaintainEndTime') is not None:
+            self.maintain_end_time = m.get('MaintainEndTime')
+        if m.get('MaintainStartTime') is not None:
+            self.maintain_start_time = m.get('MaintainStartTime')
+        if m.get('NetworkInterfaceAttributes') is not None:
+            temp_model = DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributes()
+            self.network_interface_attributes = temp_model.from_map(m['NetworkInterfaceAttributes'])
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('SupportIpv6') is not None:
             self.support_ipv_6 = m.get('SupportIpv6')
         if m.get('UserVpcId') is not None:
             self.user_vpc_id = m.get('UserVpcId')
         if m.get('UserVswitchId') is not None:
             self.user_vswitch_id = m.get('UserVswitchId')
-        if m.get('VipTypeList') is not None:
-            self.vip_type_list = m.get('VipTypeList')
         if m.get('VpcEgressAddress') is not None:
             self.vpc_egress_address = m.get('VpcEgressAddress')
         if m.get('VpcIntranetEnable') is not None:
             self.vpc_intranet_enable = m.get('VpcIntranetEnable')
         if m.get('VpcOwnerId') is not None:
             self.vpc_owner_id = m.get('VpcOwnerId')
         if m.get('VpcSlbIntranetEnable') is not None:
@@ -21786,18 +25503,26 @@
         ip_control_id: str = None,
         ip_control_name: str = None,
         ip_control_type: str = None,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
     ):
+        # The ID of the ACL. The ID is unique.
         self.ip_control_id = ip_control_id
+        # The name of the ACL.
         self.ip_control_name = ip_control_name
+        # The type of the ACL. Valid values:
+        # 
+        # *   **ALLOW**: a whitelist
+        # *   **REFUSE**: a blacklist
         self.ip_control_type = ip_control_type
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.page_size = page_size
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -21844,20 +25569,27 @@
         description: str = None,
         ip_control_id: str = None,
         ip_control_name: str = None,
         ip_control_type: str = None,
         modified_time: str = None,
         region_id: str = None,
     ):
+        # The time when the ACL was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The description of the ACL.
         self.description = description
+        # The ID of the ACL.
         self.ip_control_id = ip_control_id
+        # The name of the ACL.
         self.ip_control_name = ip_control_name
+        # The type of the ACL.
         self.ip_control_type = ip_control_type
+        # The time when the ACL was modified. The time is displayed in UTC.
         self.modified_time = modified_time
+        # The ID of the region in which the ACL is deployed.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21940,18 +25672,23 @@
         self,
         ip_control_infos: DescribeIpControlsResponseBodyIpControlInfos = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information about the ACL. The information is an array that consists of IpControlInfo data. The information does not include specific policies.
         self.ip_control_infos = ip_control_infos
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of returned entries.
         self.total_count = total_count
 
     def validate(self):
         if self.ip_control_infos:
             self.ip_control_infos.validate()
 
     def to_map(self):
@@ -22339,18 +26076,23 @@
         self,
         group_id: str = None,
         model_id: str = None,
         model_name: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.group_id = group_id
+        # The ID of the request.
         self.model_id = model_id
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.model_name = model_name
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the model.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22393,21 +26135,29 @@
         group_id: str = None,
         model_id: str = None,
         model_name: str = None,
         model_ref: str = None,
         modified_time: str = None,
         schema: str = None,
     ):
+        # The URI of the model.
         self.created_time = created_time
+        # The name of the model.
         self.description = description
+        # The definition of the model.
         self.group_id = group_id
+        # *   Fuzzy queries are supported.
         self.model_id = model_id
+        # The ID of the model.
         self.model_name = model_name
+        # Obtains the created models of an API group.
         self.model_ref = model_ref
+        # The definition of the model description.
         self.modified_time = modified_time
+        # The time when the model was created.
         self.schema = schema
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22494,18 +26244,23 @@
         self,
         model_details: DescribeModelsResponseBodyModelDetails = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The ID of the API group to which the model belongs.
         self.model_details = model_details
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned information about models. It is an array consisting of ModelDetail data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The last modification time of the model.
         self.total_count = total_count
 
     def validate(self):
         if self.model_details:
             self.model_details.validate()
 
     def to_map(self):
@@ -22582,14 +26337,302 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeModelsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePluginApisRequest(TeaModel):
+    def __init__(
+        self,
+        api_id: str = None,
+        api_name: str = None,
+        description: str = None,
+        group_id: str = None,
+        method: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        path: str = None,
+        plugin_id: str = None,
+        security_token: str = None,
+    ):
+        self.api_id = api_id
+        self.api_name = api_name
+        self.description = description
+        self.group_id = group_id
+        self.method = method
+        self.page_number = page_number
+        self.page_size = page_size
+        self.path = path
+        self.plugin_id = plugin_id
+        self.security_token = security_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_id is not None:
+            result['ApiId'] = self.api_id
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.method is not None:
+            result['Method'] = self.method
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.path is not None:
+            result['Path'] = self.path
+        if self.plugin_id is not None:
+            result['PluginId'] = self.plugin_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiId') is not None:
+            self.api_id = m.get('ApiId')
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('Method') is not None:
+            self.method = m.get('Method')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Path') is not None:
+            self.path = m.get('Path')
+        if m.get('PluginId') is not None:
+            self.plugin_id = m.get('PluginId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribePluginApisResponseBodyApiSummarysApiPluginSummary(TeaModel):
+    def __init__(
+        self,
+        api_id: str = None,
+        api_name: str = None,
+        description: str = None,
+        group_id: str = None,
+        group_name: str = None,
+        method: str = None,
+        path: str = None,
+        region_id: str = None,
+        stage_name: str = None,
+    ):
+        self.api_id = api_id
+        self.api_name = api_name
+        self.description = description
+        self.group_id = group_id
+        self.group_name = group_name
+        self.method = method
+        self.path = path
+        self.region_id = region_id
+        self.stage_name = stage_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_id is not None:
+            result['ApiId'] = self.api_id
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.group_name is not None:
+            result['GroupName'] = self.group_name
+        if self.method is not None:
+            result['Method'] = self.method
+        if self.path is not None:
+            result['Path'] = self.path
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiId') is not None:
+            self.api_id = m.get('ApiId')
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('GroupName') is not None:
+            self.group_name = m.get('GroupName')
+        if m.get('Method') is not None:
+            self.method = m.get('Method')
+        if m.get('Path') is not None:
+            self.path = m.get('Path')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        return self
+
+
+class DescribePluginApisResponseBodyApiSummarys(TeaModel):
+    def __init__(
+        self,
+        api_plugin_summary: List[DescribePluginApisResponseBodyApiSummarysApiPluginSummary] = None,
+    ):
+        self.api_plugin_summary = api_plugin_summary
+
+    def validate(self):
+        if self.api_plugin_summary:
+            for k in self.api_plugin_summary:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ApiPluginSummary'] = []
+        if self.api_plugin_summary is not None:
+            for k in self.api_plugin_summary:
+                result['ApiPluginSummary'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.api_plugin_summary = []
+        if m.get('ApiPluginSummary') is not None:
+            for k in m.get('ApiPluginSummary'):
+                temp_model = DescribePluginApisResponseBodyApiSummarysApiPluginSummary()
+                self.api_plugin_summary.append(temp_model.from_map(k))
+        return self
+
+
+class DescribePluginApisResponseBody(TeaModel):
+    def __init__(
+        self,
+        api_summarys: DescribePluginApisResponseBodyApiSummarys = None,
+        page_number: int = None,
+        page_size: int = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.api_summarys = api_summarys
+        self.page_number = page_number
+        self.page_size = page_size
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.api_summarys:
+            self.api_summarys.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_summarys is not None:
+            result['ApiSummarys'] = self.api_summarys.to_map()
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiSummarys') is not None:
+            temp_model = DescribePluginApisResponseBodyApiSummarys()
+            self.api_summarys = temp_model.from_map(m['ApiSummarys'])
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribePluginApisResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribePluginApisResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribePluginApisResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribePluginSchemasRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         security_token: str = None,
     ):
         self.language = language
@@ -23370,20 +27413,31 @@
 
 
 class DescribePluginsByApiRequest(TeaModel):
     def __init__(
         self,
         api_id: str = None,
         group_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The ID of the API.
         self.api_id = api_id
+        # The ID of the group to which the API belongs.
         self.group_id = group_id
+        self.page_number = page_number
+        self.page_size = page_size
         self.security_token = security_token
+        # The environment in which the API is running. Valid values:
+        # 
+        # *   **RELEASE**: production
+        # *   **PRE**: staging
+        # *   **TEST**: test
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23391,26 +27445,34 @@
             return _map
 
         result = dict()
         if self.api_id is not None:
             result['ApiId'] = self.api_id
         if self.group_id is not None:
             result['GroupId'] = self.group_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         if self.stage_name is not None:
             result['StageName'] = self.stage_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApiId') is not None:
             self.api_id = m.get('ApiId')
         if m.get('GroupId') is not None:
             self.group_id = m.get('GroupId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
@@ -23422,21 +27484,29 @@
         modified_time: str = None,
         plugin_data: str = None,
         plugin_id: str = None,
         plugin_name: str = None,
         plugin_type: str = None,
         region_id: str = None,
     ):
+        # The time when the plug-in was created. The time is displayed in UTC.
         self.created_time = created_time
+        # The description of the plug-in.
         self.description = description
+        # The time when the plug-in was last modified. The time is displayed in UTC.
         self.modified_time = modified_time
+        # The definition statement of the plug-in.
         self.plugin_data = plugin_data
+        # The ID of the plug-in.
         self.plugin_id = plugin_id
+        # The name of the plug-in.
         self.plugin_name = plugin_name
+        # The type of the plug-in.
         self.plugin_type = plugin_type
+        # The region where the plug-in resides.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23523,18 +27593,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         plugins: DescribePluginsByApiResponseBodyPlugins = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The plug-in information. The information is an array that consists of PluginAttribute data.
         self.plugins = plugins
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of returned entries.
         self.total_count = total_count
 
     def validate(self):
         if self.plugins:
             self.plugins.validate()
 
     def to_map(self):
@@ -24556,18 +28631,22 @@
         self,
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         signature_id: str = None,
         signature_name: str = None,
     ):
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the request.
         self.page_size = page_size
         self.security_token = security_token
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.signature_id = signature_id
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.signature_name = signature_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24609,20 +28688,28 @@
         modified_time: str = None,
         region_id: str = None,
         signature_id: str = None,
         signature_key: str = None,
         signature_name: str = None,
         signature_secret: str = None,
     ):
+        # *   This API is intended for API providers.
+        # *   This operation is used to query the backend signature keys in a Region. Region is a system parameter.
         self.created_time = created_time
+        # The Secret value of the backend signature key.
         self.modified_time = modified_time
+        # Queries backend signature keys.
         self.region_id = region_id
+        # The name of the backend signature key.
         self.signature_id = signature_id
+        # The region where the key is located.
         self.signature_key = signature_key
+        # The creation time of the key.
         self.signature_name = signature_name
+        # The Key value of the backend signature key.
         self.signature_secret = signature_secret
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24705,18 +28792,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         signature_infos: DescribeSignaturesResponseBodySignatureInfos = None,
         total_count: int = None,
     ):
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned signature information. It is an array consisting of SignatureInfo data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The ID of the backend signature key.
         self.signature_infos = signature_infos
+        # The last modification time of the key.
         self.total_count = total_count
 
     def validate(self):
         if self.signature_infos:
             self.signature_infos.validate()
 
     def to_map(self):
@@ -24801,17 +28893,23 @@
     def __init__(
         self,
         api_id: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The ID of the request.
         self.api_id = api_id
+        # The runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The returned signature key information. It is an array consisting of SignatureItem data.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24845,16 +28943,19 @@
 class DescribeSignaturesByApiResponseBodySignaturesSignatureItem(TeaModel):
     def __init__(
         self,
         bound_time: str = None,
         signature_id: str = None,
         signature_name: str = None,
     ):
+        # The name of the backend signature key.
         self.bound_time = bound_time
+        # *   This API is intended for API providers.
         self.signature_id = signature_id
+        # Queries the backend signature keys that are bound to a specified API.
         self.signature_name = signature_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24918,15 +29019,17 @@
 
 class DescribeSignaturesByApiResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         signatures: DescribeSignaturesByApiResponseBodySignatures = None,
     ):
+        # The time when the key was bound.
         self.request_id = request_id
+        # The ID of the backend signature key.
         self.signatures = signatures
 
     def validate(self):
         if self.signatures:
             self.signatures.validate()
 
     def to_map(self):
@@ -24991,14 +29094,142 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSignaturesByApiResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeSummaryDataRequest(TeaModel):
+    def __init__(
+        self,
+        security_token: str = None,
+    ):
+        self.security_token = security_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeSummaryDataResponseBody(TeaModel):
+    def __init__(
+        self,
+        expire_instance_num: int = None,
+        region: str = None,
+        request_id: str = None,
+        usage_api_num: int = None,
+        usage_group_num: int = None,
+        usage_instance_num: int = None,
+    ):
+        self.expire_instance_num = expire_instance_num
+        self.region = region
+        self.request_id = request_id
+        self.usage_api_num = usage_api_num
+        self.usage_group_num = usage_group_num
+        self.usage_instance_num = usage_instance_num
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.expire_instance_num is not None:
+            result['ExpireInstanceNum'] = self.expire_instance_num
+        if self.region is not None:
+            result['Region'] = self.region
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.usage_api_num is not None:
+            result['UsageApiNum'] = self.usage_api_num
+        if self.usage_group_num is not None:
+            result['UsageGroupNum'] = self.usage_group_num
+        if self.usage_instance_num is not None:
+            result['UsageInstanceNum'] = self.usage_instance_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExpireInstanceNum') is not None:
+            self.expire_instance_num = m.get('ExpireInstanceNum')
+        if m.get('Region') is not None:
+            self.region = m.get('Region')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('UsageApiNum') is not None:
+            self.usage_api_num = m.get('UsageApiNum')
+        if m.get('UsageGroupNum') is not None:
+            self.usage_group_num = m.get('UsageGroupNum')
+        if m.get('UsageInstanceNum') is not None:
+            self.usage_instance_num = m.get('UsageInstanceNum')
+        return self
+
+
+class DescribeSummaryDataResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeSummaryDataResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeSummaryDataResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeSystemParametersRequest(TeaModel):
     def __init__(
         self,
         security_token: str = None,
     ):
         self.security_token = security_token
 
@@ -25026,17 +29257,22 @@
     def __init__(
         self,
         demo_value: str = None,
         description: str = None,
         param_name: str = None,
         param_type: str = None,
     ):
+        # Client IP Address
         self.demo_value = demo_value
+        # The name of the parameter.
         self.description = description
+        # *   This API is intended for API callers.
+        # *   The response of this API contains the system parameters that are optional in API definitions.
         self.param_name = param_name
+        # Queries the common parameters supported by the system.
         self.param_type = param_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25104,15 +29340,17 @@
 
 class DescribeSystemParametersResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         system_params: DescribeSystemParametersResponseBodySystemParams = None,
     ):
+        # Examples
         self.request_id = request_id
+        # The description of a parameter.
         self.system_params = system_params
 
     def validate(self):
         if self.system_params:
             self.system_params.validate()
 
     def to_map(self):
@@ -25189,21 +29427,31 @@
         page_number: int = None,
         page_size: int = None,
         security_token: str = None,
         stage_name: str = None,
         traffic_control_id: str = None,
         traffic_control_name: str = None,
     ):
+        # The name of the throttling policy.
         self.api_id = api_id
+        # The environment name. This parameter must be specified together with GroupId and ApiId. Valid values:********\
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
+        # The page number of the returned page.
         self.page_number = page_number
+        # The ID of the request.
         self.page_size = page_size
         self.security_token = security_token
+        # ThrottlingTest
         self.stage_name = stage_name
+        # The specified API ID. This parameter must be specified together with GroupId and StageName.
         self.traffic_control_id = traffic_control_id
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.traffic_control_name = traffic_control_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25252,15 +29500,19 @@
 
 class DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicySpecialsSpecial(TeaModel):
     def __init__(
         self,
         special_key: str = None,
         traffic_value: int = None,
     ):
+        # Queries custom throttling policies and their details. Conditional queries are supported.
         self.special_key = special_key
+        # *   This API is intended for API providers.
+        # *   This API can be used to query all existing throttling policies (including special throttling policies) and their details.
+        # *   You can specify query conditions. For example, you can query the throttling policies bound to a specified API or in a specified environment.
         self.traffic_value = traffic_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25320,15 +29572,17 @@
 
 class DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicy(TeaModel):
     def __init__(
         self,
         special_type: str = None,
         specials: DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicySpecials = None,
     ):
+        # The throttling value.
         self.special_type = special_type
+        # The AppId or user account corresponding to SpecialType.
         self.specials = specials
 
     def validate(self):
         if self.specials:
             self.specials.validate()
 
     def to_map(self):
@@ -25398,23 +29652,40 @@
         modified_time: str = None,
         special_policies: DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPolicies = None,
         traffic_control_id: str = None,
         traffic_control_name: str = None,
         traffic_control_unit: str = None,
         user_default: int = None,
     ):
+        # The description of the throttling policy.
         self.api_default = api_default
+        # The creation time (UTC) of the throttling policy.
         self.app_default = app_default
+        # The type of the special throttling policy. Valid values:
+        # 
+        # *   **APP**\
+        # *   **USER**\
         self.created_time = created_time
+        # The name of the throttling policy.
         self.description = description
+        # The unit to be used in the throttling policy. Valid values:
+        # 
+        # *   MINUTE
+        # *   HOUR
+        # *   DAY
         self.modified_time = modified_time
+        # The returned information about a special throttling policy. It is an array consisting of Special data.
         self.special_policies = special_policies
+        # The returned information about a special throttling policy. It is an array consisting of SpecialPolicy data.
         self.traffic_control_id = traffic_control_id
+        # The ID of the throttling policy.
         self.traffic_control_name = traffic_control_name
+        # The default throttling value for each app.
         self.traffic_control_unit = traffic_control_unit
+        # The last modification time (UTC) of the throttling policy.
         self.user_default = user_default
 
     def validate(self):
         if self.special_policies:
             self.special_policies.validate()
 
     def to_map(self):
@@ -25511,18 +29782,23 @@
         self,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
         traffic_controls: DescribeTrafficControlsResponseBodyTrafficControls = None,
     ):
+        # The number of entries returned per page.
         self.page_number = page_number
+        # The returned throttling policy information. It is an array consisting of TrafficControl data.
         self.page_size = page_size
+        # The total number of returned entries.
         self.request_id = request_id
+        # The default throttling value for each user.
         self.total_count = total_count
+        # The default throttling value for each API.
         self.traffic_controls = traffic_controls
 
     def validate(self):
         if self.traffic_controls:
             self.traffic_controls.validate()
 
     def to_map(self):
@@ -25607,17 +29883,23 @@
     def __init__(
         self,
         api_id: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The ID of the request.
         self.api_id = api_id
+        # The runtime environment of the API. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The returned throttling policy information. It is an array consisting of TrafficControlItem data.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25651,16 +29933,19 @@
 class DescribeTrafficControlsByApiResponseBodyTrafficControlItemsTrafficControlItem(TeaModel):
     def __init__(
         self,
         bound_time: str = None,
         traffic_control_item_id: str = None,
         traffic_control_item_name: str = None,
     ):
+        # *   This API is intended for API providers.
         self.bound_time = bound_time
+        # The name of the throttling policy.
         self.traffic_control_item_id = traffic_control_item_id
+        # Queries the throttling policy that is bound to a specific API.
         self.traffic_control_item_name = traffic_control_item_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25724,15 +30009,17 @@
 
 class DescribeTrafficControlsByApiResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         traffic_control_items: DescribeTrafficControlsByApiResponseBodyTrafficControlItems = None,
     ):
+        # The ID of the throttling policy.
         self.request_id = request_id
+        # The binding time of the policy.
         self.traffic_control_items = traffic_control_items
 
     def validate(self):
         if self.traffic_control_items:
             self.traffic_control_items.validate()
 
     def to_map(self):
@@ -26817,42 +31104,48 @@
         return self
 
 
 class DisableInstanceAccessControlRequest(TeaModel):
     def __init__(
         self,
         acl_id: str = None,
+        address_ipversion: str = None,
         instance_id: str = None,
         security_token: str = None,
     ):
         self.acl_id = acl_id
+        self.address_ipversion = address_ipversion
         self.instance_id = instance_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.acl_id is not None:
             result['AclId'] = self.acl_id
+        if self.address_ipversion is not None:
+            result['AddressIPVersion'] = self.address_ipversion
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclId') is not None:
             self.acl_id = m.get('AclId')
+        if m.get('AddressIPVersion') is not None:
+            self.address_ipversion = m.get('AddressIPVersion')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
@@ -27468,19 +31761,21 @@
 
 
 class EnableInstanceAccessControlRequest(TeaModel):
     def __init__(
         self,
         acl_id: str = None,
         acl_type: str = None,
+        address_ipversion: str = None,
         instance_id: str = None,
         security_token: str = None,
     ):
         self.acl_id = acl_id
         self.acl_type = acl_type
+        self.address_ipversion = address_ipversion
         self.instance_id = instance_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -27489,26 +31784,30 @@
             return _map
 
         result = dict()
         if self.acl_id is not None:
             result['AclId'] = self.acl_id
         if self.acl_type is not None:
             result['AclType'] = self.acl_type
+        if self.address_ipversion is not None:
+            result['AddressIPVersion'] = self.address_ipversion
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclId') is not None:
             self.acl_id = m.get('AclId')
         if m.get('AclType') is not None:
             self.acl_type = m.get('AclType')
+        if m.get('AddressIPVersion') is not None:
+            self.address_ipversion = m.get('AddressIPVersion')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
@@ -27579,30 +31878,611 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EnableInstanceAccessControlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ImportOASRequest(TeaModel):
+    def __init__(
+        self,
+        auth_type: str = None,
+        backend_name: str = None,
+        data: str = None,
+        group_id: str = None,
+        ignore_warning: bool = None,
+        oasversion: str = None,
+        overwrite: bool = None,
+        request_mode: str = None,
+        security_token: str = None,
+        skip_dry_run: bool = None,
+    ):
+        # API安全认证类型，目前可以取值：
+        # 
+        # - **APP**：只允许已授权的APP调用
+        # - **ANONYMOUS**：允许匿名调用，设置为允许匿名调用需要注意：
+        #      - 任何能够获取该API服务信息的人，都将能够调用该API。网关不会对调用者做身份认证，也无法设置按用户的流量控制，若开放该API请设置好按API的流量控制。
+        self.auth_type = auth_type
+        self.backend_name = backend_name
+        self.data = data
+        self.group_id = group_id
+        self.ignore_warning = ignore_warning
+        self.oasversion = oasversion
+        self.overwrite = overwrite
+        self.request_mode = request_mode
+        self.security_token = security_token
+        self.skip_dry_run = skip_dry_run
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_type is not None:
+            result['AuthType'] = self.auth_type
+        if self.backend_name is not None:
+            result['BackendName'] = self.backend_name
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.ignore_warning is not None:
+            result['IgnoreWarning'] = self.ignore_warning
+        if self.oasversion is not None:
+            result['OASVersion'] = self.oasversion
+        if self.overwrite is not None:
+            result['Overwrite'] = self.overwrite
+        if self.request_mode is not None:
+            result['RequestMode'] = self.request_mode
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.skip_dry_run is not None:
+            result['SkipDryRun'] = self.skip_dry_run
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthType') is not None:
+            self.auth_type = m.get('AuthType')
+        if m.get('BackendName') is not None:
+            self.backend_name = m.get('BackendName')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('IgnoreWarning') is not None:
+            self.ignore_warning = m.get('IgnoreWarning')
+        if m.get('OASVersion') is not None:
+            self.oasversion = m.get('OASVersion')
+        if m.get('Overwrite') is not None:
+            self.overwrite = m.get('Overwrite')
+        if m.get('RequestMode') is not None:
+            self.request_mode = m.get('RequestMode')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('SkipDryRun') is not None:
+            self.skip_dry_run = m.get('SkipDryRun')
+        return self
+
+
+class ImportOASResponseBodyErrorMessages(TeaModel):
+    def __init__(
+        self,
+        error_message: List[str] = None,
+    ):
+        self.error_message = error_message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        return self
+
+
+class ImportOASResponseBodyFailedApisFailedApi(TeaModel):
+    def __init__(
+        self,
+        error_msg: str = None,
+        http_method: str = None,
+        path: str = None,
+    ):
+        self.error_msg = error_msg
+        self.http_method = http_method
+        self.path = path
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_msg is not None:
+            result['ErrorMsg'] = self.error_msg
+        if self.http_method is not None:
+            result['HttpMethod'] = self.http_method
+        if self.path is not None:
+            result['Path'] = self.path
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorMsg') is not None:
+            self.error_msg = m.get('ErrorMsg')
+        if m.get('HttpMethod') is not None:
+            self.http_method = m.get('HttpMethod')
+        if m.get('Path') is not None:
+            self.path = m.get('Path')
+        return self
+
+
+class ImportOASResponseBodyFailedApis(TeaModel):
+    def __init__(
+        self,
+        failed_api: List[ImportOASResponseBodyFailedApisFailedApi] = None,
+    ):
+        self.failed_api = failed_api
+
+    def validate(self):
+        if self.failed_api:
+            for k in self.failed_api:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['FailedApi'] = []
+        if self.failed_api is not None:
+            for k in self.failed_api:
+                result['FailedApi'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.failed_api = []
+        if m.get('FailedApi') is not None:
+            for k in m.get('FailedApi'):
+                temp_model = ImportOASResponseBodyFailedApisFailedApi()
+                self.failed_api.append(temp_model.from_map(k))
+        return self
+
+
+class ImportOASResponseBodyFailedModelsFailedModel(TeaModel):
+    def __init__(
+        self,
+        error_msg: str = None,
+        group_id: str = None,
+        model_name: str = None,
+    ):
+        self.error_msg = error_msg
+        self.group_id = group_id
+        self.model_name = model_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_msg is not None:
+            result['ErrorMsg'] = self.error_msg
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.model_name is not None:
+            result['ModelName'] = self.model_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorMsg') is not None:
+            self.error_msg = m.get('ErrorMsg')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('ModelName') is not None:
+            self.model_name = m.get('ModelName')
+        return self
+
+
+class ImportOASResponseBodyFailedModels(TeaModel):
+    def __init__(
+        self,
+        failed_model: List[ImportOASResponseBodyFailedModelsFailedModel] = None,
+    ):
+        self.failed_model = failed_model
+
+    def validate(self):
+        if self.failed_model:
+            for k in self.failed_model:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['FailedModel'] = []
+        if self.failed_model is not None:
+            for k in self.failed_model:
+                result['FailedModel'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.failed_model = []
+        if m.get('FailedModel') is not None:
+            for k in m.get('FailedModel'):
+                temp_model = ImportOASResponseBodyFailedModelsFailedModel()
+                self.failed_model.append(temp_model.from_map(k))
+        return self
+
+
+class ImportOASResponseBodySuccessApisSuccessApi(TeaModel):
+    def __init__(
+        self,
+        api_id: str = None,
+        api_operation: str = None,
+        http_method: str = None,
+        path: str = None,
+    ):
+        self.api_id = api_id
+        self.api_operation = api_operation
+        self.http_method = http_method
+        self.path = path
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_id is not None:
+            result['ApiId'] = self.api_id
+        if self.api_operation is not None:
+            result['ApiOperation'] = self.api_operation
+        if self.http_method is not None:
+            result['HttpMethod'] = self.http_method
+        if self.path is not None:
+            result['Path'] = self.path
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiId') is not None:
+            self.api_id = m.get('ApiId')
+        if m.get('ApiOperation') is not None:
+            self.api_operation = m.get('ApiOperation')
+        if m.get('HttpMethod') is not None:
+            self.http_method = m.get('HttpMethod')
+        if m.get('Path') is not None:
+            self.path = m.get('Path')
+        return self
+
+
+class ImportOASResponseBodySuccessApis(TeaModel):
+    def __init__(
+        self,
+        success_api: List[ImportOASResponseBodySuccessApisSuccessApi] = None,
+    ):
+        self.success_api = success_api
+
+    def validate(self):
+        if self.success_api:
+            for k in self.success_api:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['SuccessApi'] = []
+        if self.success_api is not None:
+            for k in self.success_api:
+                result['SuccessApi'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.success_api = []
+        if m.get('SuccessApi') is not None:
+            for k in m.get('SuccessApi'):
+                temp_model = ImportOASResponseBodySuccessApisSuccessApi()
+                self.success_api.append(temp_model.from_map(k))
+        return self
+
+
+class ImportOASResponseBodySuccessModelsSuccessModel(TeaModel):
+    def __init__(
+        self,
+        group_id: str = None,
+        model_name: str = None,
+        model_operation: str = None,
+        model_uid: str = None,
+    ):
+        self.group_id = group_id
+        self.model_name = model_name
+        self.model_operation = model_operation
+        self.model_uid = model_uid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.model_name is not None:
+            result['ModelName'] = self.model_name
+        if self.model_operation is not None:
+            result['ModelOperation'] = self.model_operation
+        if self.model_uid is not None:
+            result['ModelUid'] = self.model_uid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('ModelName') is not None:
+            self.model_name = m.get('ModelName')
+        if m.get('ModelOperation') is not None:
+            self.model_operation = m.get('ModelOperation')
+        if m.get('ModelUid') is not None:
+            self.model_uid = m.get('ModelUid')
+        return self
+
+
+class ImportOASResponseBodySuccessModels(TeaModel):
+    def __init__(
+        self,
+        success_model: List[ImportOASResponseBodySuccessModelsSuccessModel] = None,
+    ):
+        self.success_model = success_model
+
+    def validate(self):
+        if self.success_model:
+            for k in self.success_model:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['SuccessModel'] = []
+        if self.success_model is not None:
+            for k in self.success_model:
+                result['SuccessModel'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.success_model = []
+        if m.get('SuccessModel') is not None:
+            for k in m.get('SuccessModel'):
+                temp_model = ImportOASResponseBodySuccessModelsSuccessModel()
+                self.success_model.append(temp_model.from_map(k))
+        return self
+
+
+class ImportOASResponseBodyWarningMessages(TeaModel):
+    def __init__(
+        self,
+        warning_message: List[str] = None,
+    ):
+        self.warning_message = warning_message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.warning_message is not None:
+            result['WarningMessage'] = self.warning_message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('WarningMessage') is not None:
+            self.warning_message = m.get('WarningMessage')
+        return self
+
+
+class ImportOASResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_messages: ImportOASResponseBodyErrorMessages = None,
+        failed_apis: ImportOASResponseBodyFailedApis = None,
+        failed_models: ImportOASResponseBodyFailedModels = None,
+        operation_id: str = None,
+        request_id: str = None,
+        success_apis: ImportOASResponseBodySuccessApis = None,
+        success_models: ImportOASResponseBodySuccessModels = None,
+        warning_messages: ImportOASResponseBodyWarningMessages = None,
+    ):
+        self.error_messages = error_messages
+        self.failed_apis = failed_apis
+        self.failed_models = failed_models
+        self.operation_id = operation_id
+        self.request_id = request_id
+        self.success_apis = success_apis
+        self.success_models = success_models
+        self.warning_messages = warning_messages
+
+    def validate(self):
+        if self.error_messages:
+            self.error_messages.validate()
+        if self.failed_apis:
+            self.failed_apis.validate()
+        if self.failed_models:
+            self.failed_models.validate()
+        if self.success_apis:
+            self.success_apis.validate()
+        if self.success_models:
+            self.success_models.validate()
+        if self.warning_messages:
+            self.warning_messages.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_messages is not None:
+            result['ErrorMessages'] = self.error_messages.to_map()
+        if self.failed_apis is not None:
+            result['FailedApis'] = self.failed_apis.to_map()
+        if self.failed_models is not None:
+            result['FailedModels'] = self.failed_models.to_map()
+        if self.operation_id is not None:
+            result['OperationId'] = self.operation_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success_apis is not None:
+            result['SuccessApis'] = self.success_apis.to_map()
+        if self.success_models is not None:
+            result['SuccessModels'] = self.success_models.to_map()
+        if self.warning_messages is not None:
+            result['WarningMessages'] = self.warning_messages.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorMessages') is not None:
+            temp_model = ImportOASResponseBodyErrorMessages()
+            self.error_messages = temp_model.from_map(m['ErrorMessages'])
+        if m.get('FailedApis') is not None:
+            temp_model = ImportOASResponseBodyFailedApis()
+            self.failed_apis = temp_model.from_map(m['FailedApis'])
+        if m.get('FailedModels') is not None:
+            temp_model = ImportOASResponseBodyFailedModels()
+            self.failed_models = temp_model.from_map(m['FailedModels'])
+        if m.get('OperationId') is not None:
+            self.operation_id = m.get('OperationId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SuccessApis') is not None:
+            temp_model = ImportOASResponseBodySuccessApis()
+            self.success_apis = temp_model.from_map(m['SuccessApis'])
+        if m.get('SuccessModels') is not None:
+            temp_model = ImportOASResponseBodySuccessModels()
+            self.success_models = temp_model.from_map(m['SuccessModels'])
+        if m.get('WarningMessages') is not None:
+            temp_model = ImportOASResponseBodyWarningMessages()
+            self.warning_messages = temp_model.from_map(m['WarningMessages'])
+        return self
+
+
+class ImportOASResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ImportOASResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ImportOASResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ImportSwaggerRequest(TeaModel):
     def __init__(
         self,
         data: str = None,
         data_format: str = None,
         dry_run: bool = None,
         global_condition: Dict[str, Any] = None,
         group_id: str = None,
         overwrite: bool = None,
         security_token: str = None,
     ):
         self.data = data
+        # 382271
         self.data_format = data_format
         self.dry_run = dry_run
+        # Creates an API by importing Swagger-compliant data.
         self.global_condition = global_condition
         self.group_id = group_id
+        # 8e274ec61cf6468e83b68371956831cb
         self.overwrite = overwrite
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -27654,18 +32534,21 @@
         dry_run: bool = None,
         global_condition_shrink: str = None,
         group_id: str = None,
         overwrite: bool = None,
         security_token: str = None,
     ):
         self.data = data
+        # 382271
         self.data_format = data_format
         self.dry_run = dry_run
+        # Creates an API by importing Swagger-compliant data.
         self.global_condition_shrink = global_condition_shrink
         self.group_id = group_id
+        # 8e274ec61cf6468e83b68371956831cb
         self.overwrite = overwrite
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -28670,49 +33553,131 @@
         service_parameters_map: str = None,
         service_protocol: str = None,
         service_timeout: int = None,
         use_backend_service: bool = None,
         visibility: str = None,
         vpc_config: str = None,
     ):
+        # If the **AuthType** parameter is set to **APP**, you must include this parameter to specify the signature algorithm. If you do not specify a value, HmacSHA256 is used by default. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method
+        # The ID of the API.
         self.api_id = api_id
+        # The name of the API.
         self.api_name = api_name
+        # If the **AuthType** parameter is set to **APP**, the valid values are:
+        # 
+        # *   **DEFAULT**: The default value that is used if no other values are passed. This value indicates that the settings of the group are used.
+        # *   **DISABLE**: The authentication is disabled.
+        # *   **HEADER**: AppCode can be placed in the Header parameter for authentication.
+        # *   **HEADER_QUERY**: AppCode can be placed in the Header or Query parameter for authentication.
         self.app_code_auth_type = app_code_auth_type
+        # API安全认证类型，目前可以取值：
+        # 
+        # - **APP**：只允许已授权的APP调用
+        # - **ANONYMOUS**：允许匿名调用，设置为允许匿名调用需要注意：
+        #      - 任何能够获取该API服务信息的人，都将能够调用该API。网关不会对调用者做身份认证，也无法设置按用户的流量控制，若开放该API请设置好按API的流量控制；
+        #      - AppCodeAuthType的值不会生效。
         self.auth_type = auth_type
+        # The name of the backend service. This parameter takes effect only when the UseBackendService parameter is set to TRUE.
         self.backend_name = backend_name
+        # This parameter takes effect only when the **RequestMode** parameter is set to **MAPPING**.
+        # 
+        # The format in which data is transmitted to the server for POST and PUT requests. Valid values: **FORM** and **STREAM**. FORM indicates that data is transmitted in the key-value pair format. STREAM indicates that data is transmitted as byte streams.
         self.body_format = body_format
+        # The body model.
         self.body_model = body_model
+        # The ContentType configuration of the backend request.
+        # 
+        # *   DEFAULT: the default configuration in API Gateway
+        # *   CUSTOM: a custom configuration
         self.content_type_category = content_type_category
+        # The value of the ContentType header when the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value
+        # The description of the API.
         self.description = description
+        # *   Specifies whether to call the API only in an internal network. If the **DisableInternet** parameter is set to **true**, the API can be called only in an internal network.
+        # *   If the **DisableInternet** parameter is set to **false**, the API can be called over the Internet and in an internal network.
         self.disable_internet = disable_internet
+        # The sample error codes returned by the backend service.
+        # 
+        # For more information, see [ErrorCodeSample](~~44392~~).
         self.error_code_samples = error_code_samples
+        # The sample error response from the backend service. This value is used only to generate documents. It does not affect the returned result.
         self.fail_result_sample = fail_result_sample
+        # *   Specifies whether to forcibly check X-Ca-Nonce. If the **ForceNonceCheck** parameter is set to **true**, X-Ca-Nonce is forcibly checked. X-Ca-Nonce is the unique identifier of the request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent replay attacks.
+        # *   If the **ForceNonceCheck** parameter is set to **false**, X-Ca-Nonce is not checked. If you do not modify this parameter when you modify an API, the original value is used.
         self.force_nonce_check = force_nonce_check
+        # The Function Compute configuration.
         self.function_compute_config = function_compute_config
+        # The HTTP configuration.
         self.http_config = http_config
+        # The Mock configuration.
         self.mock_config = mock_config
+        # The name of the model.
         self.model_name = model_name
+        # The OSS configuration.
         self.oss_config = oss_config
+        # The description of the request body.
         self.post_body_description = post_body_description
+        # The HTTP method used to make the request. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_http_method = request_http_method
+        # The request mode. Valid values:
+        # 
+        # *   MAPPING: Parameters are mapped. Unknown parameters are filtered out.
+        # *   PASSTHROUGH: Parameters are passed through.
+        # *   MAPPING_PASSTHROUGH: Parameters are mapped. Unknown parameters are passed through.
         self.request_mode = request_mode
+        # The parameters of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestParameter](~~43986~~).
         self.request_parameters = request_parameters
+        # The path of the API request. If the complete API URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the path of the API request is `/object/add`.
         self.request_path = request_path
+        # The protocol type supported by the API. Valid values: HTTP and HTTPS. Separate multiple values with commas (,), such as "HTTP,HTTPS".
         self.request_protocol = request_protocol
+        # The sample response from the backend service. This value is used only to generate documents. It does not affect the returned result.
         self.result_sample = result_sample
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML. This value is used only to generate documents. It does not affect the returned result.
         self.result_type = result_type
         self.security_token = security_token
+        # The parameters of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameter](~~43988~~).
         self.service_parameters = service_parameters
+        # The mappings between parameters of requests sent by the consumer to API Gateway and parameters of requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameterMap](~~43989~~).
         self.service_parameters_map = service_parameters_map
+        # The protocol that is used to access backend services. Valid values:
+        # 
+        # *   Http: for backend services that use HTTP or HTTPS
+        # *   Vpc: for backend services that use VPC
+        # *   FC: for Function Compute
+        # *   OSS: for Object Storage Service
+        # *   Mock: for backend services that use the Mock mode
+        # *   EventBridge: for EventBridge
+        # 
+        # You must specify the config value for the corresponding backend service.
         self.service_protocol = service_protocol
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_timeout = service_timeout
+        # Specifies whether to use the information about the created backend service. Valid values:
+        # 
+        # *   TRUE: uses the information about the created backend service.
+        # *   FALSE: uses the information about the custom backend service.
         self.use_backend_service = use_backend_service
+        # Specifies whether to make the API public. Valid values:
+        # 
+        # *   **PUBLIC:** The API is public. If this parameter is set to PUBLIC, the API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE:** The API is private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.visibility = visibility
+        # The VPC configuration.
         self.vpc_config = vpc_config
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28872,14 +33837,15 @@
 
 
 class ModifyApiConfigurationResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28985,28 +33951,30 @@
         default_domain: str = None,
         description: str = None,
         group_id: str = None,
         group_name: str = None,
         passthrough_headers: str = None,
         rpc_pattern: str = None,
         security_token: str = None,
+        support_sse: str = None,
         tag: List[ModifyApiGroupRequestTag] = None,
         user_log_config: str = None,
     ):
         self.base_path = base_path
         self.compatible_flags = compatible_flags
         self.custom_trace_config = custom_trace_config
         self.customer_configs = customer_configs
         self.default_domain = default_domain
         self.description = description
         self.group_id = group_id
         self.group_name = group_name
         self.passthrough_headers = passthrough_headers
         self.rpc_pattern = rpc_pattern
         self.security_token = security_token
+        self.support_sse = support_sse
         self.tag = tag
         self.user_log_config = user_log_config
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -29036,14 +34004,16 @@
             result['GroupName'] = self.group_name
         if self.passthrough_headers is not None:
             result['PassthroughHeaders'] = self.passthrough_headers
         if self.rpc_pattern is not None:
             result['RpcPattern'] = self.rpc_pattern
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
+        if self.support_sse is not None:
+            result['SupportSSE'] = self.support_sse
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         if self.user_log_config is not None:
             result['UserLogConfig'] = self.user_log_config
         return result
@@ -29068,14 +34038,16 @@
             self.group_name = m.get('GroupName')
         if m.get('PassthroughHeaders') is not None:
             self.passthrough_headers = m.get('PassthroughHeaders')
         if m.get('RpcPattern') is not None:
             self.rpc_pattern = m.get('RpcPattern')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
+        if m.get('SupportSSE') is not None:
+            self.support_sse = m.get('SupportSSE')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = ModifyApiGroupRequestTag()
                 self.tag.append(temp_model.from_map(k))
         if m.get('UserLogConfig') is not None:
             self.user_log_config = m.get('UserLogConfig')
@@ -29328,20 +34300,22 @@
 
 class ModifyAppRequest(TeaModel):
     def __init__(
         self,
         app_id: int = None,
         app_name: str = None,
         description: str = None,
+        extend: str = None,
         security_token: str = None,
         tag: List[ModifyAppRequestTag] = None,
     ):
         self.app_id = app_id
         self.app_name = app_name
         self.description = description
+        self.extend = extend
         self.security_token = security_token
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -29355,14 +34329,16 @@
         result = dict()
         if self.app_id is not None:
             result['AppId'] = self.app_id
         if self.app_name is not None:
             result['AppName'] = self.app_name
         if self.description is not None:
             result['Description'] = self.description
+        if self.extend is not None:
+            result['Extend'] = self.extend
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         return result
@@ -29371,14 +34347,16 @@
         m = m or dict()
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
         if m.get('AppName') is not None:
             self.app_name = m.get('AppName')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('Extend') is not None:
+            self.extend = m.get('Extend')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = ModifyAppRequestTag()
                 self.tag.append(temp_model.from_map(k))
@@ -30082,16 +35060,20 @@
     def __init__(
         self,
         description: str = None,
         ip_control_id: str = None,
         ip_control_name: str = None,
         security_token: str = None,
     ):
+        # *   This operation is intended for API providers.
+        # *   This operation allows you to modify only the name and description of an ACL. You cannot modify the type of the ACL.
         self.description = description
+        # The description. The description can be up to 200 characters in length.
         self.ip_control_id = ip_control_id
+        # The ID of the request.
         self.ip_control_name = ip_control_name
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -30124,14 +35106,15 @@
 
 
 class ModifyIpControlResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Modifies an access control list (ACL).
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30199,17 +35182,29 @@
         self,
         app_id: str = None,
         cidr_ip: str = None,
         ip_control_id: str = None,
         policy_item_id: str = None,
         security_token: str = None,
     ):
+        # The ID of the request.
         self.app_id = app_id
+        # *   This operation is intended for API providers.
+        # *   The modification immediately takes effect on all the APIs that are bound to the policy.
+        # *   This operation causes a full modification of the content of a policy.
         self.cidr_ip = cidr_ip
+        # The ID of the application that is restricted by the policy. You can configure the AppId parameter only when the value of the IpControlType parameter is ALLOW.
+        # 
+        # *   You can add only one application ID at a time.
+        # *   If this parameter is empty, no applications are restricted.
+        # *   If this parameter is not empty, not only IP addresses but also applications are restricted.
+        # *   If this parameter is not empty and no security authentication method is specified for the API, all API calls are restricted.
+        # *   If the value of the IpControlType parameter is REFUSE and the AppId parameter is not empty, API Gateway automatically ignores the AppId parameter and restricts only the IP addresses.
         self.ip_control_id = ip_control_id
+        # The IP address or CIDR block that is defined in a policy. Separate multiple IP addresses or CIDR blocks with semicolons (;). You can add a maximum of 10 IP addresses or CIDR blocks.
         self.policy_item_id = policy_item_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -30246,14 +35241,15 @@
 
 
 class ModifyIpControlPolicyItemResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Modifies a policy in an access control list (ACL).
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30437,18 +35433,23 @@
         self,
         description: str = None,
         group_id: str = None,
         model_name: str = None,
         new_model_name: str = None,
         schema: str = None,
     ):
+        # The new definition of the model.
         self.description = description
+        # The new name of the model.
         self.group_id = group_id
+        # The description of the new model definition.
         self.model_name = model_name
+        # The ID of the request.
         self.new_model_name = new_model_name
+        # The ID of the API group to which the model belongs.
         self.schema = schema
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30484,14 +35485,15 @@
 
 
 class ModifyModelResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Updates the model of an API group.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30729,17 +35731,21 @@
         security_token: str = None,
         signature_id: str = None,
         signature_key: str = None,
         signature_name: str = None,
         signature_secret: str = None,
     ):
         self.security_token = security_token
+        # The new Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\_). It must start with a letter.
         self.signature_id = signature_id
+        # The ID of the request.
         self.signature_key = signature_key
+        # The new Secret value of the key. The value must be 6 to 30 characters in length and can contain letters, digits, and special characters. Special characters include underscores (\_), at signs (@), number signs (#), exclamation points (!), and asterisks (\*). The value must start with a letter.
         self.signature_name = signature_name
+        # The ID of the key.
         self.signature_secret = signature_secret
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30777,16 +35783,22 @@
 class ModifySignatureResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         signature_id: str = None,
         signature_name: str = None,
     ):
+        # The name of the key.
         self.request_id = request_id
+        # *   This API is intended for API providers.
+        # *   This API operation modifies the name, Key value, and Secret value of an existing signature key.
+        # *   Note that the modification takes effect immediately. If the key has been bound to an API, you must adjust the backend signature verification based on the new key accordingly.
+        # *   The QPS limit on this operation is 50 per user.
         self.signature_id = signature_id
+        # Modifies a backend signature key.
         self.signature_name = signature_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30865,21 +35877,33 @@
         description: str = None,
         security_token: str = None,
         traffic_control_id: str = None,
         traffic_control_name: str = None,
         traffic_control_unit: str = None,
         user_default: int = None,
     ):
+        # The default throttling value for each app.
         self.api_default = api_default
+        # ThrottlingTestDescription
         self.app_default = app_default
+        # The ID of the request.
         self.description = description
         self.security_token = security_token
+        # ThrottlingTest
         self.traffic_control_id = traffic_control_id
+        # The unit to be used in the throttling policy. Valid values:
+        # 
+        # *   **SECOND**\
+        # *   **MINUTE**\
+        # *   **HOUR**\
+        # *   **DAY**\
         self.traffic_control_name = traffic_control_name
+        # The default throttling value for each user.
         self.traffic_control_unit = traffic_control_unit
+        # The description of the throttling policy.
         self.user_default = user_default
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30927,14 +35951,15 @@
 
 
 class ModifyTrafficControlResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Modifies the settings of a custom throttling policy.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31006,22 +36031,44 @@
         port: int = None,
         refresh: bool = None,
         security_token: str = None,
         token: str = None,
         vpc_id: str = None,
         vpc_target_host_name: str = None,
     ):
+        # The ID of the new instance.
         self.instance_id = instance_id
+        # The name of the VPC authorization.
+        # 
+        # > 
+        # 
+        # *   The name of a VPC authorization cannot be changed. You cannot use this parameter to change the name of a VPC authorization.
+        # 
+        # *   You must set this parameter to the name of the current VPC authorization.
         self.name = name
+        # Specifies whether to update the associated API.
+        # 
+        # **\
+        # 
+        # **Warning:** If you want to update the VPC authorization of a published API, you must set this parameter to true. Otherwise, the update will not be synchronized to the backend service of the API.
         self.need_batch_work = need_batch_work
+        # The new port number.
         self.port = port
+        # Specifies whether to update the VPC authorization.
+        # 
+        # > 
+        # 
+        # *   If the ID of the instance in your VPC is changed but the IP address of the instance remains unchanged, you can set this parameter to true to update the VPC authorization.
         self.refresh = refresh
         self.security_token = security_token
+        # The token of the request.
         self.token = token
+        # The ID of the new VPC.
         self.vpc_id = vpc_id
+        # The hostname of the backend service.
         self.vpc_target_host_name = vpc_target_host_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31074,15 +36121,21 @@
 
 class ModifyVpcAccessAndUpdateApisResponseBody(TeaModel):
     def __init__(
         self,
         operation_id: str = None,
         request_id: str = None,
     ):
+        # The ID of the asynchronous task.
+        # 
+        # > 
+        # 
+        # *   If the associated API is updated, you can use the task ID in the **DescribeUpdateVpcInfoTask** operation to query the update result.
         self.operation_id = operation_id
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31222,22 +36275,497 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = OpenApiGatewayServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryRequestLogsRequest(TeaModel):
+    def __init__(
+        self,
+        request_log_id: str = None,
+        security_token: str = None,
+    ):
+        # The ID of the request log.
+        self.request_log_id = request_log_id
+        self.security_token = security_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_log_id is not None:
+            result['RequestLogId'] = self.request_log_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestLogId') is not None:
+            self.request_log_id = m.get('RequestLogId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class QueryRequestLogsResponseBodyRequestLogsRequestLog(TeaModel):
+    def __init__(
+        self,
+        api_id: str = None,
+        api_name: str = None,
+        app_name: str = None,
+        backend_request_end: int = None,
+        backend_request_start: int = None,
+        backend_response_end: int = None,
+        backend_response_start: int = None,
+        client_ip: str = None,
+        client_nonce: str = None,
+        consumer_app_id: str = None,
+        consumer_app_key: str = None,
+        custom_trace_id: str = None,
+        domain: str = None,
+        error_code: str = None,
+        error_message: str = None,
+        exception: str = None,
+        front_request_end: int = None,
+        front_request_start: int = None,
+        front_response_end: int = None,
+        front_response_start: int = None,
+        group_id: str = None,
+        group_name: str = None,
+        http_method: str = None,
+        http_path: str = None,
+        initial_request_id: str = None,
+        instance_id: str = None,
+        jwt_claims: str = None,
+        region: str = None,
+        request_body: str = None,
+        request_headers: str = None,
+        request_id: str = None,
+        request_protocol: str = None,
+        request_query_string: str = None,
+        request_size: str = None,
+        request_time: str = None,
+        response_body: str = None,
+        response_headers: str = None,
+        response_size: str = None,
+        service_latency: str = None,
+        stage_id: str = None,
+        stage_name: str = None,
+        status_code: str = None,
+        total_latency: str = None,
+        plugin: str = None,
+    ):
+        # The ID of the API.
+        self.api_id = api_id
+        # The name of the API
+        self.api_name = api_name
+        self.app_name = app_name
+        self.backend_request_end = backend_request_end
+        self.backend_request_start = backend_request_start
+        self.backend_response_end = backend_response_end
+        self.backend_response_start = backend_response_start
+        # The IP address of the client that sends the request.
+        self.client_ip = client_ip
+        # The X-Ca-Nonce header included in the request from the client.
+        self.client_nonce = client_nonce
+        # The ID of the application from which an API request is sent.
+        self.consumer_app_id = consumer_app_id
+        # The application key used by the caller.
+        self.consumer_app_key = consumer_app_key
+        # The ID of the custom trace.
+        self.custom_trace_id = custom_trace_id
+        # The domain name of the request.
+        self.domain = domain
+        # The error code returned if the request failed.
+        self.error_code = error_code
+        # The error message returned if the request fails.
+        self.error_message = error_message
+        # The specific error message returned by the backend service.
+        self.exception = exception
+        self.front_request_end = front_request_end
+        self.front_request_start = front_request_start
+        self.front_response_end = front_response_end
+        self.front_response_start = front_response_start
+        # The ID of the API group to which the API belongs.
+        self.group_id = group_id
+        # The name of the API group to which the API belongs.
+        self.group_name = group_name
+        # The HTTP method used to send the request.
+        self.http_method = http_method
+        # The path of the request.
+        self.http_path = http_path
+        # The initial request ID when API Gateway calls an API. For example, if API-1 calls API-2, the initialRequestId parameter in the log of API-2 indicates the ID of the request from API-1.
+        self.initial_request_id = initial_request_id
+        # The ID of the API Gateway instance to which the API belongs.
+        self.instance_id = instance_id
+        # The JSON web token (JWT) claims. The claims can be configured at the group level.
+        self.jwt_claims = jwt_claims
+        # The ID of the region.
+        self.region = region
+        # The request body. A request body cannot exceed 1,024 bytes in size.
+        self.request_body = request_body
+        # The request headers.
+        self.request_headers = request_headers
+        # The ID of the request.
+        self.request_id = request_id
+        # The protocol used by the client to send the request. Valid values: HTTP, HTTPS, and WS.
+        self.request_protocol = request_protocol
+        # The query string for the request.
+        self.request_query_string = request_query_string
+        # The size of the request. Unit: bytes.
+        self.request_size = request_size
+        # The request time, in UTC.
+        self.request_time = request_time
+        # The response body. A response body cannot exceed 1,024 bytes in size.
+        self.response_body = response_body
+        # The headers in the API response.
+        self.response_headers = response_headers
+        # The size of returned data. Unit: bytes.
+        self.response_size = response_size
+        # The total time consumed to access backend resources. The total time includes the time consumed to request a connection to the resources, the time consumed to establish the connection, and the time consumed to call the backend service. Unit: milliseconds.
+        self.service_latency = service_latency
+        # The ID of the API environment.
+        self.stage_id = stage_id
+        # The name of the API environment.
+        self.stage_name = stage_name
+        # The HTTP status code.
+        self.status_code = status_code
+        # The total time consumed by the request. Unit: milliseconds.
+        self.total_latency = total_latency
+        # The list of plug-ins hit by the request and the relevant context.
+        self.plugin = plugin
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.api_id is not None:
+            result['ApiId'] = self.api_id
+        if self.api_name is not None:
+            result['ApiName'] = self.api_name
+        if self.app_name is not None:
+            result['AppName'] = self.app_name
+        if self.backend_request_end is not None:
+            result['BackendRequestEnd'] = self.backend_request_end
+        if self.backend_request_start is not None:
+            result['BackendRequestStart'] = self.backend_request_start
+        if self.backend_response_end is not None:
+            result['BackendResponseEnd'] = self.backend_response_end
+        if self.backend_response_start is not None:
+            result['BackendResponseStart'] = self.backend_response_start
+        if self.client_ip is not None:
+            result['ClientIp'] = self.client_ip
+        if self.client_nonce is not None:
+            result['ClientNonce'] = self.client_nonce
+        if self.consumer_app_id is not None:
+            result['ConsumerAppId'] = self.consumer_app_id
+        if self.consumer_app_key is not None:
+            result['ConsumerAppKey'] = self.consumer_app_key
+        if self.custom_trace_id is not None:
+            result['CustomTraceId'] = self.custom_trace_id
+        if self.domain is not None:
+            result['Domain'] = self.domain
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.exception is not None:
+            result['Exception'] = self.exception
+        if self.front_request_end is not None:
+            result['FrontRequestEnd'] = self.front_request_end
+        if self.front_request_start is not None:
+            result['FrontRequestStart'] = self.front_request_start
+        if self.front_response_end is not None:
+            result['FrontResponseEnd'] = self.front_response_end
+        if self.front_response_start is not None:
+            result['FrontResponseStart'] = self.front_response_start
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.group_name is not None:
+            result['GroupName'] = self.group_name
+        if self.http_method is not None:
+            result['HttpMethod'] = self.http_method
+        if self.http_path is not None:
+            result['HttpPath'] = self.http_path
+        if self.initial_request_id is not None:
+            result['InitialRequestId'] = self.initial_request_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.jwt_claims is not None:
+            result['JwtClaims'] = self.jwt_claims
+        if self.region is not None:
+            result['Region'] = self.region
+        if self.request_body is not None:
+            result['RequestBody'] = self.request_body
+        if self.request_headers is not None:
+            result['RequestHeaders'] = self.request_headers
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.request_protocol is not None:
+            result['RequestProtocol'] = self.request_protocol
+        if self.request_query_string is not None:
+            result['RequestQueryString'] = self.request_query_string
+        if self.request_size is not None:
+            result['RequestSize'] = self.request_size
+        if self.request_time is not None:
+            result['RequestTime'] = self.request_time
+        if self.response_body is not None:
+            result['ResponseBody'] = self.response_body
+        if self.response_headers is not None:
+            result['ResponseHeaders'] = self.response_headers
+        if self.response_size is not None:
+            result['ResponseSize'] = self.response_size
+        if self.service_latency is not None:
+            result['ServiceLatency'] = self.service_latency
+        if self.stage_id is not None:
+            result['StageId'] = self.stage_id
+        if self.stage_name is not None:
+            result['StageName'] = self.stage_name
+        if self.status_code is not None:
+            result['StatusCode'] = self.status_code
+        if self.total_latency is not None:
+            result['TotalLatency'] = self.total_latency
+        if self.plugin is not None:
+            result['plugin'] = self.plugin
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApiId') is not None:
+            self.api_id = m.get('ApiId')
+        if m.get('ApiName') is not None:
+            self.api_name = m.get('ApiName')
+        if m.get('AppName') is not None:
+            self.app_name = m.get('AppName')
+        if m.get('BackendRequestEnd') is not None:
+            self.backend_request_end = m.get('BackendRequestEnd')
+        if m.get('BackendRequestStart') is not None:
+            self.backend_request_start = m.get('BackendRequestStart')
+        if m.get('BackendResponseEnd') is not None:
+            self.backend_response_end = m.get('BackendResponseEnd')
+        if m.get('BackendResponseStart') is not None:
+            self.backend_response_start = m.get('BackendResponseStart')
+        if m.get('ClientIp') is not None:
+            self.client_ip = m.get('ClientIp')
+        if m.get('ClientNonce') is not None:
+            self.client_nonce = m.get('ClientNonce')
+        if m.get('ConsumerAppId') is not None:
+            self.consumer_app_id = m.get('ConsumerAppId')
+        if m.get('ConsumerAppKey') is not None:
+            self.consumer_app_key = m.get('ConsumerAppKey')
+        if m.get('CustomTraceId') is not None:
+            self.custom_trace_id = m.get('CustomTraceId')
+        if m.get('Domain') is not None:
+            self.domain = m.get('Domain')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('Exception') is not None:
+            self.exception = m.get('Exception')
+        if m.get('FrontRequestEnd') is not None:
+            self.front_request_end = m.get('FrontRequestEnd')
+        if m.get('FrontRequestStart') is not None:
+            self.front_request_start = m.get('FrontRequestStart')
+        if m.get('FrontResponseEnd') is not None:
+            self.front_response_end = m.get('FrontResponseEnd')
+        if m.get('FrontResponseStart') is not None:
+            self.front_response_start = m.get('FrontResponseStart')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('GroupName') is not None:
+            self.group_name = m.get('GroupName')
+        if m.get('HttpMethod') is not None:
+            self.http_method = m.get('HttpMethod')
+        if m.get('HttpPath') is not None:
+            self.http_path = m.get('HttpPath')
+        if m.get('InitialRequestId') is not None:
+            self.initial_request_id = m.get('InitialRequestId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('JwtClaims') is not None:
+            self.jwt_claims = m.get('JwtClaims')
+        if m.get('Region') is not None:
+            self.region = m.get('Region')
+        if m.get('RequestBody') is not None:
+            self.request_body = m.get('RequestBody')
+        if m.get('RequestHeaders') is not None:
+            self.request_headers = m.get('RequestHeaders')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RequestProtocol') is not None:
+            self.request_protocol = m.get('RequestProtocol')
+        if m.get('RequestQueryString') is not None:
+            self.request_query_string = m.get('RequestQueryString')
+        if m.get('RequestSize') is not None:
+            self.request_size = m.get('RequestSize')
+        if m.get('RequestTime') is not None:
+            self.request_time = m.get('RequestTime')
+        if m.get('ResponseBody') is not None:
+            self.response_body = m.get('ResponseBody')
+        if m.get('ResponseHeaders') is not None:
+            self.response_headers = m.get('ResponseHeaders')
+        if m.get('ResponseSize') is not None:
+            self.response_size = m.get('ResponseSize')
+        if m.get('ServiceLatency') is not None:
+            self.service_latency = m.get('ServiceLatency')
+        if m.get('StageId') is not None:
+            self.stage_id = m.get('StageId')
+        if m.get('StageName') is not None:
+            self.stage_name = m.get('StageName')
+        if m.get('StatusCode') is not None:
+            self.status_code = m.get('StatusCode')
+        if m.get('TotalLatency') is not None:
+            self.total_latency = m.get('TotalLatency')
+        if m.get('plugin') is not None:
+            self.plugin = m.get('plugin')
+        return self
+
+
+class QueryRequestLogsResponseBodyRequestLogs(TeaModel):
+    def __init__(
+        self,
+        request_log: List[QueryRequestLogsResponseBodyRequestLogsRequestLog] = None,
+    ):
+        self.request_log = request_log
+
+    def validate(self):
+        if self.request_log:
+            for k in self.request_log:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['RequestLog'] = []
+        if self.request_log is not None:
+            for k in self.request_log:
+                result['RequestLog'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.request_log = []
+        if m.get('RequestLog') is not None:
+            for k in m.get('RequestLog'):
+                temp_model = QueryRequestLogsResponseBodyRequestLogsRequestLog()
+                self.request_log.append(temp_model.from_map(k))
+        return self
+
+
+class QueryRequestLogsResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        request_logs: QueryRequestLogsResponseBodyRequestLogs = None,
+    ):
+        # The ID of the request.
+        self.request_id = request_id
+        # The list of request logs.
+        self.request_logs = request_logs
+
+    def validate(self):
+        if self.request_logs:
+            self.request_logs.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.request_logs is not None:
+            result['RequestLogs'] = self.request_logs.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RequestLogs') is not None:
+            temp_model = QueryRequestLogsResponseBodyRequestLogs()
+            self.request_logs = temp_model.from_map(m['RequestLogs'])
+        return self
+
+
+class QueryRequestLogsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryRequestLogsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryRequestLogsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ReactivateDomainRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         group_id: str = None,
         security_token: str = None,
     ):
+        # *   This operation is intended for API providers.
+        # *   You must solve the problem that is mentioned in the domain name exception prompt before you can reactivate the domain name.
+        # *   A typical reason why a custom domain name becomes abnormal is that the domain name does not have an ICP filing or the domain name is included in a blacklist by the administration. When a custom domain name is abnormal, users cannot use it to access APIs.
+        # *   You can call this operation to reactivate the domain name to resume normal access.
         self.domain_name = domain_name
+        # The ID of the request.
         self.group_id = group_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -31266,14 +36794,15 @@
 
 
 class ReactivateDomainResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Reactivates a custom domain name whose validity status is Abnormal.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31452,19 +36981,27 @@
         api_ids: str = None,
         app_id: int = None,
         description: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # Queries weather based on the region name
         self.api_ids = api_ids
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.app_id = app_id
+        # The ID of the request.
         self.description = description
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The description of the authorization.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31504,14 +37041,15 @@
 
 
 class RemoveApisAuthoritiesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Revokes the access permissions on multiple APIs from a specified app.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31579,18 +37117,26 @@
         self,
         api_id: str = None,
         app_ids: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The IDs of applications. Separate multiple application IDs with commas (,). A maximum of 100 applications IDs can be entered.
         self.api_id = api_id
+        # *   This operation is intended for API providers and callers.
+        # *   Before you revoke access permissions, check by whom the permissions were granted. API providers can only revoke permissions granted by a Provider, and API callers can only revoke permissions granted by a Consumer.
         self.app_ids = app_ids
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The ID of the request.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31626,14 +37172,15 @@
 
 
 class RemoveAppsAuthoritiesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Revokes the access permissions on a specified API from multiple applications. In this case, multiple applications map to a single API.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31701,18 +37248,29 @@
         self,
         api_ids: str = None,
         group_id: str = None,
         ip_control_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The ID of the request.
         self.api_ids = api_ids
-        self.group_id = group_id
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
+        self.group_id = group_id
+        # The ID of the API to be managed.
+        # 
+        # *   If this parameter is not specified, all APIs of the API group are unbound in the specified environment by default.
+        # *   The IDs of the APIs that you want to query. Separate multiple IDs with commas (,). A maximum of 100 IDs can be entered.
         self.ip_control_id = ip_control_id
         self.security_token = security_token
+        # *   This API is intended for API providers.
+        # *   The unbinding takes effect immediately. After the API is unbound from the ACL, the corresponding environment does not have any IP address access control in place for the API.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31748,14 +37306,15 @@
 
 
 class RemoveIpControlApisResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Unbinds an API from an access control list (ACL).
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31821,15 +37380,17 @@
 class RemoveIpControlPolicyItemRequest(TeaModel):
     def __init__(
         self,
         ip_control_id: str = None,
         policy_item_ids: str = None,
         security_token: str = None,
     ):
+        # The ID of the request.
         self.ip_control_id = ip_control_id
+        # *   This operation is intended for API providers.
         self.policy_item_ids = policy_item_ids
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -31858,14 +37419,15 @@
 
 
 class RemoveIpControlPolicyItemResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Removes one or more policies from an access control list (ACL).
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31933,18 +37495,29 @@
         self,
         api_ids: str = None,
         group_id: str = None,
         security_token: str = None,
         signature_id: str = None,
         stage_name: str = None,
     ):
+        # The ID of the request.
         self.api_ids = api_ids
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The IDs of the APIs from which you want to unbind the signature key.
+        # 
+        # *   If this parameter is not specified, the signature key is unbound from all the APIs in the specified environment of the API group.
+        # *   The IDs of the APIs that you want to manage. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.signature_id = signature_id
+        # *   This API is intended for API providers.
+        # *   The operation takes effect immediately. The request sent from API Gateway to the backend service does not contain the signature string. The corresponding verification step can be removed from the backend.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31980,14 +37553,15 @@
 
 
 class RemoveSignatureApisResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Unbinds a backend signature key from APIs.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32055,18 +37629,29 @@
         self,
         api_ids: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
         traffic_control_id: str = None,
     ):
+        # The ID of the request.
         self.api_ids = api_ids
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # *   This API is intended for API providers.
+        # *   This API allows you to unbind a specified throttling policy from up to 100 APIs at a time.
         self.stage_name = stage_name
+        # The IDs of the APIs from which you want to unbind a specified throttling policy.
+        # 
+        # *   If this parameter is not specified, the throttling policy is unbound from all the APIs in the specified environment of the API group.
+        # *   Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.traffic_control_id = traffic_control_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32102,14 +37687,15 @@
 
 
 class RemoveTrafficControlApisResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Unbinds a specified throttling policy from APIs.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32226,14 +37812,15 @@
 class RemoveVpcAccessResponseBodyApisApi(TeaModel):
     def __init__(
         self,
         api_id: str = None,
         group_id: str = None,
         stage_id: str = None,
     ):
+        # API Id
         self.api_id = api_id
         self.group_id = group_id
         self.stage_id = stage_id
 
     def validate(self):
         pass
 
@@ -32507,15 +38094,17 @@
 class ResetAppCodeRequest(TeaModel):
     def __init__(
         self,
         app_code: str = None,
         new_app_code: str = None,
         security_token: str = None,
     ):
+        # The current AppCode of the application.
         self.app_code = app_code
+        # The new AppCode of the application.
         self.new_app_code = new_app_code
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -32544,14 +38133,15 @@
 
 
 class ResetAppCodeResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32614,54 +38204,63 @@
         return self
 
 
 class ResetAppSecretRequest(TeaModel):
     def __init__(
         self,
         app_key: str = None,
+        new_app_key: str = None,
         new_app_secret: str = None,
         security_token: str = None,
     ):
+        # The key of the application that is used to make an API call.
         self.app_key = app_key
+        self.new_app_key = new_app_key
+        # The new key of the application. To improve compatibility, we recommend that you use other parameters.
         self.new_app_secret = new_app_secret
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app_key is not None:
             result['AppKey'] = self.app_key
+        if self.new_app_key is not None:
+            result['NewAppKey'] = self.new_app_key
         if self.new_app_secret is not None:
             result['NewAppSecret'] = self.new_app_secret
         if self.security_token is not None:
             result['SecurityToken'] = self.security_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppKey') is not None:
             self.app_key = m.get('AppKey')
+        if m.get('NewAppKey') is not None:
+            self.new_app_key = m.get('NewAppKey')
         if m.get('NewAppSecret') is not None:
             self.new_app_secret = m.get('NewAppSecret')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class ResetAppSecretResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33189,20 +38788,31 @@
         app_id: int = None,
         auth_valid_time: str = None,
         description: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # Queries weather based on the region name
         self.api_ids = api_ids
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.app_id = app_id
+        # *   This operation is intended for API providers and callers.
+        # *   API providers can authorize any apps to call their APIs.
+        # *   API callers can authorize their own apps to call the APIs that they have purchased.
         self.auth_valid_time = auth_valid_time
+        # The time (UTC) when the authorization expires. If this parameter is empty, the authorization does not expire.
         self.description = description
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The description of the authorization.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33246,14 +38856,15 @@
 
 
 class SetApisAuthoritiesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Authorizes a specified app to call multiple APIs.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33323,20 +38934,31 @@
         app_ids: str = None,
         auth_valid_time: str = None,
         description: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.api_id = api_id
+        # Queries weather based on the region name
         self.app_ids = app_ids
+        # *   This operation is intended for API providers and callers.
+        # *   API providers can authorize any apps to call their APIs.
+        # *   API callers can authorize their own apps to call the APIs that they have purchased.
         self.auth_valid_time = auth_valid_time
+        # The time (UTC) when the authorization expires. If this parameter is empty, the authorization does not expire.
         self.description = description
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The description of the authorization.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33380,14 +39002,15 @@
 
 
 class SetAppsAuthoritiesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Grants access permissions on a specified API to multiple apps.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33878,27 +39501,146 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SetDomainWebSocketStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SetGroupAuthAppCodeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_app_code: str = None,
+        group_id: str = None,
+        security_token: str = None,
+    ):
+        self.auth_app_code = auth_app_code
+        self.group_id = group_id
+        self.security_token = security_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_app_code is not None:
+            result['AuthAppCode'] = self.auth_app_code
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthAppCode') is not None:
+            self.auth_app_code = m.get('AuthAppCode')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class SetGroupAuthAppCodeResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetGroupAuthAppCodeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetGroupAuthAppCodeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetGroupAuthAppCodeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SetIpControlApisRequest(TeaModel):
     def __init__(
         self,
         api_ids: str = None,
         group_id: str = None,
         ip_control_id: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The ID of the request.
         self.api_ids = api_ids
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **PRE**\
+        # *   **TEST**\
         self.group_id = group_id
+        # The API IDs. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.ip_control_id = ip_control_id
         self.security_token = security_token
+        # *   This operation is intended for API callers.
+        # *   A maximum of 100 APIs can be bound at a time.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -33934,14 +39676,15 @@
 
 
 class SetIpControlApisResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Creates a binding relationship between specified access control lists (ACLs) and APIs.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34009,18 +39752,27 @@
         self,
         api_ids: str = None,
         group_id: str = None,
         security_token: str = None,
         signature_id: str = None,
         stage_name: str = None,
     ):
+        # The ID of the request.
         self.api_ids = api_ids
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **PRE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.signature_id = signature_id
+        # *   This API is intended for API providers.
+        # *   This operation allows you to bind a signature key to an API. You can bind signature keys for up to 100 APIs at a time.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34056,14 +39808,15 @@
 
 
 class SetSignatureApisResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Binds a signature key to APIs.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34131,18 +39884,26 @@
         self,
         api_ids: str = None,
         group_id: str = None,
         security_token: str = None,
         stage_name: str = None,
         traffic_control_id: str = None,
     ):
+        # The ID of the request.
         self.api_ids = api_ids
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id
         self.security_token = security_token
+        # *   This API is intended for API providers.
+        # *   This API allows you to bind a specific throttling policy to up to 100 APIs at a time.
         self.stage_name = stage_name
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.traffic_control_id = traffic_control_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34178,14 +39939,15 @@
 
 
 class SetTrafficControlApisResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Binds a throttling policy to APIs.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34504,19 +40266,31 @@
         api_id: str = None,
         description: str = None,
         group_id: str = None,
         history_version: str = None,
         security_token: str = None,
         stage_name: str = None,
     ):
+        # The description of the switch operation.
         self.api_id = api_id
+        # The ID of the request.
         self.description = description
-        self.group_id = group_id
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
+        self.group_id = group_id
+        # *   This API is intended for API providers.
+        # *   The historical version can be obtained through the DescribeHistoryApis API.****\
+        # *   Only APIs that have been published more than once have historical versions to switch to.
+        # *   This operation can only be performed on running APIs. Use caution when performing this operation because the operation cannot be undone after it has been completed and takes effect within 5 seconds.
+        # *   The switch operation is in essence a publish operation, and the reason for this operation must be provided.
         self.history_version = history_version
         self.security_token = security_token
+        # The historical version you want to switch to.
         self.stage_name = stage_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34556,14 +40330,15 @@
 
 
 class SwitchApiResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # Switches the definition of an API in a specified runtime environment to a historical version.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34628,15 +40403,17 @@
 
 class TagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # Adds tags to resources.
         self.key = key
+        # TagResources
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34664,14 +40441,15 @@
         self,
         resource_id: List[str] = None,
         resource_type: str = None,
         security_token: str = None,
         tag: List[TagResourcesRequestTag] = None,
     ):
         self.resource_id = resource_id
+        # The operation that you want to perform. Set the value to **TagResources**.
         self.resource_type = resource_type
         self.security_token = security_token
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
@@ -34788,16 +40566,20 @@
         self,
         all: bool = None,
         resource_id: List[str] = None,
         resource_type: str = None,
         security_token: str = None,
         tag_key: List[str] = None,
     ):
+        # The ID of the request.
         self.all = all
         self.resource_id = resource_id
+        # The key of tag N.
+        # 
+        # Valid values of N: `1 to 20.`
         self.resource_type = resource_type
         self.security_token = security_token
         self.tag_key = tag_key
 
     def validate(self):
         pass
 
@@ -34835,14 +40617,15 @@
 
 
 class UntagResourcesResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # UntagResources
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34901,7 +40684,129 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ValidateVpcConnectivityRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        security_token: str = None,
+        vpc_access_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.security_token = security_token
+        self.vpc_access_id = vpc_access_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.vpc_access_id is not None:
+            result['VpcAccessId'] = self.vpc_access_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('VpcAccessId') is not None:
+            self.vpc_access_id = m.get('VpcAccessId')
+        return self
+
+
+class ValidateVpcConnectivityResponseBody(TeaModel):
+    def __init__(
+        self,
+        connected: bool = None,
+        ip_type: str = None,
+        request_id: str = None,
+    ):
+        self.connected = connected
+        self.ip_type = ip_type
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.connected is not None:
+            result['Connected'] = self.connected
+        if self.ip_type is not None:
+            result['IpType'] = self.ip_type
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Connected') is not None:
+            self.connected = m.get('Connected')
+        if m.get('IpType') is not None:
+            self.ip_type = m.get('IpType')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ValidateVpcConnectivityResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ValidateVpcConnectivityResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ValidateVpcConnectivityResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_cloudapi20160714-2.2.9/alibabacloud_cloudapi20160714.egg-info/PKG-INFO` & `alibabacloud_cloudapi20160714-3.0.0/alibabacloud_cloudapi20160714.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudapi20160714
-Version: 2.2.9
+Version: 3.0.0
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714-2.2.9/setup.py` & `alibabacloud_cloudapi20160714-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudapi20160714.
 
-Created on 13/10/2022
+Created on 31/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudapi20160714"
 NAME = "alibabacloud_cloudapi20160714" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CloudAPI (20160714) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

