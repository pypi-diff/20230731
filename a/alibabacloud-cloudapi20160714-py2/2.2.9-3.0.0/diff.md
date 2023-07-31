# Comparing `tmp/alibabacloud_cloudapi20160714_py2-2.2.9.tar.gz` & `tmp/alibabacloud_cloudapi20160714_py2-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudapi20160714_py2-2.2.9.tar", last modified: Thu Oct 13 02:23:29 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cloudapi20160714_py2-3.0.0.tar", last modified: Mon Jul 31 02:28:40 2023, max compression
```

## Comparing `alibabacloud_cloudapi20160714_py2-2.2.9.tar` & `alibabacloud_cloudapi20160714_py2-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/
--rw-r--r--   0 root         (0) root         (0)     1493 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/__init__.py
--rw-r--r--   0 root         (0) root         (0)   241326 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/client.py
--rw-r--r--   0 root         (0) root         (0)  1160625 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:28:40.000000 alibabacloud_cloudapi20160714_py2-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-31 02:28:40.000000 alibabacloud_cloudapi20160714_py2-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:28:40.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   298890 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714/client.py
+-rw-r--r--   0 root         (0) root         (0)  1410157 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:28:40.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 02:28:40.000000 alibabacloud_cloudapi20160714_py2-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-07-31 02:28:39.000000 alibabacloud_cloudapi20160714_py2-3.0.0/setup.py
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/ChangeLog.md` & `alibabacloud_cloudapi20160714_py2-3.0.0/ChangeLog.md`

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

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/LICENSE` & `alibabacloud_cloudapi20160714_py2-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/PKG-INFO` & `alibabacloud_cloudapi20160714_py2-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudapi20160714_py2
-Version: 2.2.9
+Version: 3.0.0
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/README-CN.md` & `alibabacloud_cloudapi20160714_py2-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/README.md` & `alibabacloud_cloudapi20160714_py2-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/client.py` & `alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,14 +119,29 @@
         )
 
     def add_access_control_list_entry(self, request):
         runtime = util_models.RuntimeOptions()
         return self.add_access_control_list_entry_with_options(request, runtime)
 
     def add_ip_control_policy_item_with_options(self, request, runtime):
+        """
+        The restriction policy on app IDs for a specific policy. You can restrict app IDs only for whitelists. The IpControlType values of whitelists are ALLOW.
+        *   You can add only one app ID restriction policy at a time.
+        *   If this parameter is empty, no restriction is imposed on the app IDs.
+        *   If this parameter is not empty, there is restriction not only on IP addresses, but also on apps.
+        *   Please note that if this parameter is not empty and the security authentication method of the API is No Authentication, all API calls are restricted.
+        *   If this parameter is not empty for a blacklist, API Gateway automatically skips this parameter and sets only restriction on IP addresses. The IpControlType value of a blacklist is REFUSE.
+        
+
+        @param request: AddIpControlPolicyItemRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: AddIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cidr_ip):
             query['CidrIp'] = request.cidr_ip
         if not UtilClient.is_unset(request.ip_control_id):
@@ -149,18 +164,43 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.AddIpControlPolicyItemResponse(),
             self.call_api(params, req, runtime)
         )
 
     def add_ip_control_policy_item(self, request):
+        """
+        The restriction policy on app IDs for a specific policy. You can restrict app IDs only for whitelists. The IpControlType values of whitelists are ALLOW.
+        *   You can add only one app ID restriction policy at a time.
+        *   If this parameter is empty, no restriction is imposed on the app IDs.
+        *   If this parameter is not empty, there is restriction not only on IP addresses, but also on apps.
+        *   Please note that if this parameter is not empty and the security authentication method of the API is No Authentication, all API calls are restricted.
+        *   If this parameter is not empty for a blacklist, API Gateway automatically skips this parameter and sets only restriction on IP addresses. The IpControlType value of a blacklist is REFUSE.
+        
+
+        @param request: AddIpControlPolicyItemRequest
+
+        @return: AddIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_ip_control_policy_item_with_options(request, runtime)
 
     def add_traffic_special_control_with_options(self, request, runtime):
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+
+        @param request: AddTrafficSpecialControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: AddTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.special_key):
             query['SpecialKey'] = request.special_key
         if not UtilClient.is_unset(request.special_type):
@@ -185,14 +225,24 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.AddTrafficSpecialControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def add_traffic_special_control(self, request):
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+
+        @param request: AddTrafficSpecialControlRequest
+
+        @return: AddTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_traffic_special_control_with_options(request, runtime)
 
     def attach_plugin_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
@@ -295,14 +345,16 @@
         return self.batch_deploy_apis_with_options(request, runtime)
 
     def create_access_control_list_with_options(self, request, runtime):
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
@@ -321,72 +373,87 @@
         )
 
     def create_access_control_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_access_control_list_with_options(request, runtime)
 
     def create_api_with_options(self, request, runtime):
+        """
+        This operation is intended for API providers.
+        *   The name of each API within the same group must be unique.
+        *   Each request path within the same group must be unique.
+        *   The QPS limit on this operation is 50 per user.
+        
+
+        @param request: CreateApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
@@ -397,14 +464,25 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.CreateApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_api(self, request):
+        """
+        This operation is intended for API providers.
+        *   The name of each API within the same group must be unique.
+        *   Each request path within the same group must be unique.
+        *   The QPS limit on this operation is 50 per user.
+        
+
+        @param request: CreateApiRequest
+
+        @return: CreateApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_api_with_options(request, runtime)
 
     def create_api_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.base_path):
@@ -491,18 +569,18 @@
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
@@ -673,24 +751,34 @@
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
@@ -807,14 +895,25 @@
         )
 
     def create_log_config(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_log_config_with_options(request, runtime)
 
     def create_model_with_options(self, request, runtime):
+        """
+        For more information about the model definition, see [JSON Schema Draft 4](https://tools.ietf.org/html/draft-zyp-json-schema-04?spm=a2c4g.11186623.2.10.2e977ff7p4BpQd).
+        *   JSON Schema supports only element attributes of the Object type.
+        
+
+        @param request: CreateModelRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: CreateModelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.model_name):
@@ -837,14 +936,23 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.CreateModelResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_model(self, request):
+        """
+        For more information about the model definition, see [JSON Schema Draft 4](https://tools.ietf.org/html/draft-zyp-json-schema-04?spm=a2c4g.11186623.2.10.2e977ff7p4BpQd).
+        *   JSON Schema supports only element attributes of the Object type.
+        
+
+        @param request: CreateModelRequest
+
+        @return: CreateModelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_model_with_options(request, runtime)
 
     def create_monitor_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auth):
@@ -913,14 +1021,24 @@
         )
 
     def create_plugin(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_plugin_with_options(request, runtime)
 
     def create_signature_with_options(self, request, runtime):
+        """
+        The Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+
+        @param request: CreateSignatureRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: CreateSignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_key):
             query['SignatureKey'] = request.signature_key
         if not UtilClient.is_unset(request.signature_name):
@@ -943,18 +1061,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.CreateSignatureResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_signature(self, request):
+        """
+        The Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+
+        @param request: CreateSignatureRequest
+
+        @return: CreateSignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_signature_with_options(request, runtime)
 
     def create_traffic_control_with_options(self, request, runtime):
+        """
+        ThrottlingTest
+        
+
+        @param request: CreateTrafficControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: CreateTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_default):
             query['ApiDefault'] = request.api_default
         if not UtilClient.is_unset(request.app_default):
             query['AppDefault'] = request.app_default
         if not UtilClient.is_unset(request.description):
@@ -983,14 +1119,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.CreateTrafficControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_traffic_control(self, request):
+        """
+        ThrottlingTest
+        
+
+        @param request: CreateTrafficControlRequest
+
+        @return: CreateTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_traffic_control_with_options(request, runtime)
 
     def delete_access_control_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_id):
@@ -1017,14 +1161,24 @@
         )
 
     def delete_access_control_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_access_control_list_with_options(request, runtime)
 
     def delete_all_traffic_special_control_with_options(self, request, runtime):
+        """
+        The ID of the request.
+        
+
+        @param request: DeleteAllTrafficSpecialControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteAllTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.traffic_control_id):
             query['TrafficControlId'] = request.traffic_control_id
         req = open_api_models.OpenApiRequest(
@@ -1043,14 +1197,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DeleteAllTrafficSpecialControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_all_traffic_special_control(self, request):
+        """
+        The ID of the request.
+        
+
+        @param request: DeleteAllTrafficSpecialControlRequest
+
+        @return: DeleteAllTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_all_traffic_special_control_with_options(request, runtime)
 
     def delete_api_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
@@ -1303,14 +1465,24 @@
         )
 
     def delete_dataset_item(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_dataset_item_with_options(request, runtime)
 
     def delete_domain_with_options(self, request, runtime):
+        """
+        The custom domain name.
+        
+
+        @param request: DeleteDomainRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -1331,14 +1503,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DeleteDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_domain(self, request):
+        """
+        The custom domain name.
+        
+
+        @param request: DeleteDomainRequest
+
+        @return: DeleteDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_domain_with_options(request, runtime)
 
     def delete_domain_certificate_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.certificate_id):
@@ -1399,14 +1579,24 @@
         )
 
     def delete_instance(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_instance_with_options(request, runtime)
 
     def delete_ip_control_with_options(self, request, runtime):
+        """
+        The ID of the request.
+        
+
+        @param request: DeleteIpControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
@@ -1425,14 +1615,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DeleteIpControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_ip_control(self, request):
+        """
+        The ID of the request.
+        
+
+        @param request: DeleteIpControlRequest
+
+        @return: DeleteIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_ip_control_with_options(request, runtime)
 
     def delete_log_config_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.log_type):
@@ -1553,14 +1751,24 @@
         )
 
     def delete_plugin(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_plugin_with_options(request, runtime)
 
     def delete_signature_with_options(self, request, runtime):
+        """
+        The ID of the request.
+        
+
+        @param request: DeleteSignatureRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteSignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_id):
             query['SignatureId'] = request.signature_id
         req = open_api_models.OpenApiRequest(
@@ -1579,14 +1787,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DeleteSignatureResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_signature(self, request):
+        """
+        The ID of the request.
+        
+
+        @param request: DeleteSignatureRequest
+
+        @return: DeleteSignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_signature_with_options(request, runtime)
 
     def delete_traffic_control_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
@@ -1613,14 +1829,26 @@
         )
 
     def delete_traffic_control(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_traffic_control_with_options(request, runtime)
 
     def delete_traffic_special_control_with_options(self, request, runtime):
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+
+        @param request: DeleteTrafficSpecialControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteTrafficSpecialControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.special_key):
             query['SpecialKey'] = request.special_key
         if not UtilClient.is_unset(request.special_type):
@@ -1643,18 +1871,38 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DeleteTrafficSpecialControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_traffic_special_control(self, request):
+        """
+        The type of the special throttling policy. Valid values:
+        *   **APP**\
+        *   **USER**\
+        
+
+        @param request: DeleteTrafficSpecialControlRequest
+
+        @return: DeleteTrafficSpecialControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_traffic_special_control_with_options(request, runtime)
 
     def deploy_api_with_options(self, request, runtime):
+        """
+        The ID of the API.
+        
+
+        @param request: DeployApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeployApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
@@ -1679,14 +1927,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DeployApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def deploy_api(self, request):
+        """
+        The ID of the API.
+        
+
+        @param request: DeployApiRequest
+
+        @return: DeployApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.deploy_api_with_options(request, runtime)
 
     def describe_abolish_api_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.operation_uid):
@@ -1747,14 +2003,16 @@
         return self.describe_access_control_list_attribute_with_options(request, runtime)
 
     def describe_access_control_lists_with_options(self, request, runtime):
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
@@ -1777,14 +2035,24 @@
         )
 
     def describe_access_control_lists(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_access_control_lists_with_options(request, runtime)
 
     def describe_api_with_options(self, request, runtime):
+        """
+        This operation is intended for API providers.
+        
+
+        @param request: DescribeApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -1805,14 +2073,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_api(self, request):
+        """
+        This operation is intended for API providers.
+        
+
+        @param request: DescribeApiRequest
+
+        @return: DescribeApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_with_options(request, runtime)
 
     def describe_api_doc_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
@@ -1843,14 +2119,24 @@
         )
 
     def describe_api_doc(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_api_doc_with_options(request, runtime)
 
     def describe_api_group_with_options(self, request, runtime):
+        """
+        This operation is intended for API providers.
+        
+
+        @param request: DescribeApiGroupRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApiGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.tag):
@@ -1871,14 +2157,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApiGroupResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_api_group(self, request):
+        """
+        This operation is intended for API providers.
+        
+
+        @param request: DescribeApiGroupRequest
+
+        @return: DescribeApiGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_group_with_options(request, runtime)
 
     def describe_api_group_vpc_whitelist_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
@@ -1949,14 +2243,26 @@
         )
 
     def describe_api_groups(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_api_groups_with_options(request, runtime)
 
     def describe_api_histories_with_options(self, request, runtime):
+        """
+        The name of the runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST: the test environment**\
+        
+
+        @param request: DescribeApiHistoriesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApiHistoriesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_name):
             query['ApiName'] = request.api_name
         if not UtilClient.is_unset(request.group_id):
@@ -1985,18 +2291,40 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApiHistoriesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_api_histories(self, request):
+        """
+        The name of the runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST: the test environment**\
+        
+
+        @param request: DescribeApiHistoriesRequest
+
+        @return: DescribeApiHistoriesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_histories_with_options(request, runtime)
 
     def describe_api_history_with_options(self, request, runtime):
+        """
+        You can call this operation to query the definition of a specified published version of an API.
+        *   This operation is intended for API providers.
+        *   Each time an API is published, API Gateway records the publishing details, such as the time and the API definition. You can use the version number obtained from other API operations to query the details of an API definition that is published on a specific occasion.
+        
+
+        @param request: DescribeApiHistoryRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApiHistoryResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.history_version):
@@ -2021,18 +2349,38 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApiHistoryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_api_history(self, request):
+        """
+        You can call this operation to query the definition of a specified published version of an API.
+        *   This operation is intended for API providers.
+        *   Each time an API is published, API Gateway records the publishing details, such as the time and the API definition. You can use the version number obtained from other API operations to query the details of an API definition that is published on a specific occasion.
+        
+
+        @param request: DescribeApiHistoryRequest
+
+        @return: DescribeApiHistoryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_history_with_options(request, runtime)
 
     def describe_api_ip_controls_with_options(self, request, runtime):
+        """
+        The ID of the API group.
+        
+
+        @param request: DescribeApiIpControlsRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApiIpControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -2059,14 +2407,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApiIpControlsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_api_ip_controls(self, request):
+        """
+        The ID of the API group.
+        
+
+        @param request: DescribeApiIpControlsRequest
+
+        @return: DescribeApiIpControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_ip_controls_with_options(request, runtime)
 
     def describe_api_latency_data_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
@@ -2171,14 +2527,26 @@
         )
 
     def describe_api_qps_data(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_api_qps_data_with_options(request, runtime)
 
     def describe_api_signatures_with_options(self, request, runtime):
+        """
+        The runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST**\
+        
+
+        @param request: DescribeApiSignaturesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApiSignaturesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -2205,18 +2573,40 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApiSignaturesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_api_signatures(self, request):
+        """
+        The runtime environment. Valid values:
+        *   **RELEASE**\
+        *   **TEST**\
+        
+
+        @param request: DescribeApiSignaturesRequest
+
+        @return: DescribeApiSignaturesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_signatures_with_options(request, runtime)
 
     def describe_api_traffic_controls_with_options(self, request, runtime):
+        """
+        The runtime environment of the API. Valid values:
+        *   **RELEASE**\
+        *   **TEST**: the test environment
+        
+
+        @param request: DescribeApiTrafficControlsRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApiTrafficControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -2243,14 +2633,24 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApiTrafficControlsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_api_traffic_controls(self, request):
+        """
+        The runtime environment of the API. Valid values:
+        *   **RELEASE**\
+        *   **TEST**: the test environment
+        
+
+        @param request: DescribeApiTrafficControlsRequest
+
+        @return: DescribeApiTrafficControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_api_traffic_controls_with_options(request, runtime)
 
     def describe_api_traffic_data_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
@@ -2285,14 +2685,26 @@
         )
 
     def describe_api_traffic_data(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_api_traffic_data_with_options(request, runtime)
 
     def describe_apis_with_options(self, request, runtime):
+        """
+        This operation is intended for API callers.
+        *   This operation returns a list of all APIs that are being defined. The basic information about these APIs is also returned in the list.
+        *   This operation returns all APIs that are being edited, regardless of their environments. The returned definitions may be different from the definitions in the environments.
+        
+
+        @param request: DescribeApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_method):
             query['ApiMethod'] = request.api_method
         if not UtilClient.is_unset(request.api_name):
@@ -2307,14 +2719,16 @@
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
@@ -2333,14 +2747,24 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_apis(self, request):
+        """
+        This operation is intended for API callers.
+        *   This operation returns a list of all APIs that are being defined. The basic information about these APIs is also returned in the list.
+        *   This operation returns all APIs that are being edited, regardless of their environments. The returned definitions may be different from the definitions in the environments.
+        
+
+        @param request: DescribeApisRequest
+
+        @return: DescribeApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_with_options(request, runtime)
 
     def describe_apis_by_app_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_name):
@@ -2417,14 +2841,24 @@
         )
 
     def describe_apis_by_backend(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_by_backend_with_options(request, runtime)
 
     def describe_apis_by_ip_control_with_options(self, request, runtime):
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+
+        @param request: DescribeApisByIpControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApisByIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -2447,18 +2881,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApisByIpControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_apis_by_ip_control(self, request):
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+
+        @param request: DescribeApisByIpControlRequest
+
+        @return: DescribeApisByIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_by_ip_control_with_options(request, runtime)
 
     def describe_apis_by_signature_with_options(self, request, runtime):
+        """
+        The ID of the signature key.
+        
+
+        @param request: DescribeApisBySignatureRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApisBySignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -2481,18 +2933,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApisBySignatureResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_apis_by_signature(self, request):
+        """
+        The ID of the signature key.
+        
+
+        @param request: DescribeApisBySignatureRequest
+
+        @return: DescribeApisBySignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_by_signature_with_options(request, runtime)
 
     def describe_apis_by_traffic_control_with_options(self, request, runtime):
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+
+        @param request: DescribeApisByTrafficControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeApisByTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -2515,14 +2985,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeApisByTrafficControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_apis_by_traffic_control(self, request):
+        """
+        The number of entries to return on each page. Maximum value: 100. Default value: 10.
+        
+
+        @param request: DescribeApisByTrafficControlRequest
+
+        @return: DescribeApisByTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apis_by_traffic_control_with_options(request, runtime)
 
     def describe_app_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -2561,14 +3039,16 @@
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
@@ -2627,14 +3107,24 @@
         )
 
     def describe_app_security(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_app_security_with_options(request, runtime)
 
     def describe_apps_with_options(self, request, runtime):
+        """
+        The ID of the app.
+        
+
+        @param request: DescribeAppsRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeAppsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_owner):
             query['AppOwner'] = request.app_owner
         if not UtilClient.is_unset(request.page_number):
@@ -2659,18 +3149,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeAppsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_apps(self, request):
+        """
+        The ID of the app.
+        
+
+        @param request: DescribeAppsRequest
+
+        @return: DescribeAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apps_with_options(request, runtime)
 
     def describe_authorized_apis_with_options(self, request, runtime):
+        """
+        The number of the page to return. Pages start from page 1. Default value: 1.
+        
+
+        @param request: DescribeAuthorizedApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeAuthorizedApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -2693,14 +3201,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeAuthorizedApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_authorized_apis(self, request):
+        """
+        The number of the page to return. Pages start from page 1. Default value: 1.
+        
+
+        @param request: DescribeAuthorizedApisRequest
+
+        @return: DescribeAuthorizedApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_authorized_apis_with_options(request, runtime)
 
     def describe_authorized_apps_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
@@ -3053,14 +3569,24 @@
         )
 
     def describe_deployed_apis(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_deployed_apis_with_options(request, runtime)
 
     def describe_domain_with_options(self, request, runtime):
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+
+        @param request: DescribeDomainRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -3081,14 +3607,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain(self, request):
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+
+        @param request: DescribeDomainRequest
+
+        @return: DescribeDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_with_options(request, runtime)
 
     def describe_history_apis_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
@@ -3124,14 +3658,368 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_history_apis(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_history_apis_with_options(request, runtime)
 
+    def describe_import_oastask_with_options(self, request, runtime):
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
+    def describe_import_oastask(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_import_oastask_with_options(request, runtime)
+
+    def describe_instance_drop_connections_with_options(self, request, runtime):
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
+    def describe_instance_drop_connections(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_drop_connections_with_options(request, runtime)
+
+    def describe_instance_drop_packet_with_options(self, request, runtime):
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
+    def describe_instance_drop_packet(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_drop_packet_with_options(request, runtime)
+
+    def describe_instance_http_code_with_options(self, request, runtime):
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
+    def describe_instance_http_code(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_http_code_with_options(request, runtime)
+
+    def describe_instance_latency_with_options(self, request, runtime):
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
+    def describe_instance_latency(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_latency_with_options(request, runtime)
+
+    def describe_instance_new_connections_with_options(self, request, runtime):
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
+    def describe_instance_new_connections(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_new_connections_with_options(request, runtime)
+
+    def describe_instance_packets_with_options(self, request, runtime):
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
+    def describe_instance_packets(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_packets_with_options(request, runtime)
+
+    def describe_instance_qps_with_options(self, request, runtime):
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
+    def describe_instance_qps(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_qps_with_options(request, runtime)
+
+    def describe_instance_slb_connect_with_options(self, request, runtime):
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
+    def describe_instance_slb_connect(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_slb_connect_with_options(request, runtime)
+
+    def describe_instance_traffic_with_options(self, request, runtime):
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
+    def describe_instance_traffic(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_instance_traffic_with_options(request, runtime)
+
     def describe_instances_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.enable_tag_authorization):
             query['EnableTagAuthorization'] = request.enable_tag_authorization
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -3197,14 +4085,27 @@
         )
 
     def describe_ip_control_policy_items(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_ip_control_policy_items_with_options(request, runtime)
 
     def describe_ip_controls_with_options(self, request, runtime):
+        """
+        This operation is intended for API providers.
+        *   This operation is used to query the ACLs in a region. Region is a system parameter.
+        *   You can filter the query results by ACL ID, name, or type.
+        *   This operation cannot be used to query specific policies. If you want to query specific policies, call the [DescribeIpControlPolicyItems](~~65532~~) operation.
+        
+
+        @param request: DescribeIpControlsRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeIpControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.ip_control_name):
             query['IpControlName'] = request.ip_control_name
         if not UtilClient.is_unset(request.ip_control_type):
@@ -3231,14 +4132,25 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeIpControlsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_ip_controls(self, request):
+        """
+        This operation is intended for API providers.
+        *   This operation is used to query the ACLs in a region. Region is a system parameter.
+        *   You can filter the query results by ACL ID, name, or type.
+        *   This operation cannot be used to query specific policies. If you want to query specific policies, call the [DescribeIpControlPolicyItems](~~65532~~) operation.
+        
+
+        @param request: DescribeIpControlsRequest
+
+        @return: DescribeIpControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_ip_controls_with_options(request, runtime)
 
     def describe_log_config_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.log_type):
@@ -3295,14 +4207,24 @@
         )
 
     def describe_market_remains_quota(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_market_remains_quota_with_options(request, runtime)
 
     def describe_models_with_options(self, request, runtime):
+        """
+        The name of the model.
+        
+
+        @param request: DescribeModelsRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeModelsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.model_id):
             query['ModelId'] = request.model_id
         if not UtilClient.is_unset(request.model_name):
@@ -3327,17 +4249,71 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeModelsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_models(self, request):
+        """
+        The name of the model.
+        
+
+        @param request: DescribeModelsRequest
+
+        @return: DescribeModelsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_models_with_options(request, runtime)
 
+    def describe_plugin_apis_with_options(self, request, runtime):
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
+    def describe_plugin_apis(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_plugin_apis_with_options(request, runtime)
+
     def describe_plugin_schemas_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.language):
             query['Language'] = request.language
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
@@ -3433,20 +4409,35 @@
         )
 
     def describe_plugins(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_plugins_with_options(request, runtime)
 
     def describe_plugins_by_api_with_options(self, request, runtime):
+        """
+        This operation is intended for API callers.
+        *   This operation supports pagination.
+        
+
+        @param request: DescribePluginsByApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
@@ -3463,14 +4454,23 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribePluginsByApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_plugins_by_api(self, request):
+        """
+        This operation is intended for API callers.
+        *   This operation supports pagination.
+        
+
+        @param request: DescribePluginsByApiRequest
+
+        @return: DescribePluginsByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_plugins_by_api_with_options(request, runtime)
 
     def describe_purchased_api_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_id):
@@ -3601,14 +4601,24 @@
         )
 
     def describe_regions(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_regions_with_options(request, runtime)
 
     def describe_signatures_with_options(self, request, runtime):
+        """
+        The IDs of the keys to query.
+        
+
+        @param request: DescribeSignaturesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeSignaturesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.security_token):
@@ -3633,18 +4643,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeSignaturesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_signatures(self, request):
+        """
+        The IDs of the keys to query.
+        
+
+        @param request: DescribeSignaturesRequest
+
+        @return: DescribeSignaturesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_signatures_with_options(request, runtime)
 
     def describe_signatures_by_api_with_options(self, request, runtime):
+        """
+        The ID of the group to which the API belongs.
+        
+
+        @param request: DescribeSignaturesByApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeSignaturesByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -3667,18 +4695,64 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeSignaturesByApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_signatures_by_api(self, request):
+        """
+        The ID of the group to which the API belongs.
+        
+
+        @param request: DescribeSignaturesByApiRequest
+
+        @return: DescribeSignaturesByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_signatures_by_api_with_options(request, runtime)
 
+    def describe_summary_data_with_options(self, request, runtime):
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
+    def describe_summary_data(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_summary_data_with_options(request, runtime)
+
     def describe_system_parameters_with_options(self, request, runtime):
+        """
+        The returned information about system parameters. It is an array that consists of SystemParam data.
+        
+
+        @param request: DescribeSystemParametersRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeSystemParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3695,18 +4769,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeSystemParametersResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_system_parameters(self, request):
+        """
+        The returned information about system parameters. It is an array that consists of SystemParam data.
+        
+
+        @param request: DescribeSystemParametersRequest
+
+        @return: DescribeSystemParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_system_parameters_with_options(request, runtime)
 
     def describe_traffic_controls_with_options(self, request, runtime):
+        """
+        The specified group ID. This parameter must be specified together with ApiId and StageName.
+        
+
+        @param request: DescribeTrafficControlsRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeTrafficControlsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.page_number):
@@ -3737,18 +4829,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeTrafficControlsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_traffic_controls(self, request):
+        """
+        The specified group ID. This parameter must be specified together with ApiId and StageName.
+        
+
+        @param request: DescribeTrafficControlsRequest
+
+        @return: DescribeTrafficControlsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_traffic_controls_with_options(request, runtime)
 
     def describe_traffic_controls_by_api_with_options(self, request, runtime):
+        """
+        The ID of the API.
+        
+
+        @param request: DescribeTrafficControlsByApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeTrafficControlsByApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -3771,14 +4881,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.DescribeTrafficControlsByApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_traffic_controls_by_api(self, request):
+        """
+        The ID of the API.
+        
+
+        @param request: DescribeTrafficControlsByApiRequest
+
+        @return: DescribeTrafficControlsByApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_traffic_controls_by_api_with_options(request, runtime)
 
     def describe_update_backend_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.operation_uid):
@@ -3947,14 +5065,16 @@
         return self.detach_plugin_with_options(request, runtime)
 
     def disable_instance_access_control_with_options(self, request, runtime):
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
@@ -4025,14 +5145,16 @@
     def enable_instance_access_control_with_options(self, request, runtime):
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
@@ -4052,15 +5174,73 @@
             self.call_api(params, req, runtime)
         )
 
     def enable_instance_access_control(self, request):
         runtime = util_models.RuntimeOptions()
         return self.enable_instance_access_control_with_options(request, runtime)
 
+    def import_oaswith_options(self, request, runtime):
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
+    def import_oas(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.import_oaswith_options(request, runtime)
+
     def import_swagger_with_options(self, tmp_req, runtime):
+        """
+        0009db9c828549768a200320714b8930
+        
+
+        @param tmp_req: ImportSwaggerRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ImportSwaggerResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = cloud_api20160714_models.ImportSwaggerShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.global_condition):
             request.global_condition_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.global_condition, 'GlobalCondition', 'json')
         query = {}
         if not UtilClient.is_unset(request.data_format):
@@ -4095,14 +5275,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ImportSwaggerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def import_swagger(self, request):
+        """
+        0009db9c828549768a200320714b8930
+        
+
+        @param request: ImportSwaggerRequest
+
+        @return: ImportSwaggerResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.import_swagger_with_options(request, runtime)
 
     def list_tag_resources_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
@@ -4133,14 +5321,24 @@
         )
 
     def list_tag_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_tag_resources_with_options(request, runtime)
 
     def modify_api_with_options(self, request, runtime):
+        """
+        58928
+        
+
+        @param request: ModifyApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ModifyApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_signature_method):
             query['AllowSignatureMethod'] = request.allow_signature_method
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.api_name):
@@ -4211,14 +5409,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ModifyApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_api(self, request):
+        """
+        58928
+        
+
+        @param request: ModifyApiRequest
+
+        @return: ModifyApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_api_with_options(request, runtime)
 
     def modify_api_configuration_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_signature_method):
@@ -4337,14 +5543,16 @@
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
@@ -4405,14 +5613,16 @@
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
@@ -4615,14 +5825,24 @@
         )
 
     def modify_instance_spec(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_instance_spec_with_options(request, runtime)
 
     def modify_ip_control_with_options(self, request, runtime):
+        """
+        The name of the ACL. The name must be 4 to 50 characters in length, and can contain letters, digits, and underscores (\\_). The name cannot start with an underscore (\\_).
+        
+
+        @param request: ModifyIpControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ModifyIpControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.ip_control_name):
@@ -4645,18 +5865,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ModifyIpControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_ip_control(self, request):
+        """
+        The name of the ACL. The name must be 4 to 50 characters in length, and can contain letters, digits, and underscores (\\_). The name cannot start with an underscore (\\_).
+        
+
+        @param request: ModifyIpControlRequest
+
+        @return: ModifyIpControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_ip_control_with_options(request, runtime)
 
     def modify_ip_control_policy_item_with_options(self, request, runtime):
+        """
+        The ID of the policy.
+        
+
+        @param request: ModifyIpControlPolicyItemRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ModifyIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cidr_ip):
             query['CidrIp'] = request.cidr_ip
         if not UtilClient.is_unset(request.ip_control_id):
@@ -4681,14 +5919,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ModifyIpControlPolicyItemResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_ip_control_policy_item(self, request):
+        """
+        The ID of the policy.
+        
+
+        @param request: ModifyIpControlPolicyItemRequest
+
+        @return: ModifyIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_ip_control_policy_item_with_options(request, runtime)
 
     def modify_log_config_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.log_type):
@@ -4793,14 +6039,24 @@
         )
 
     def modify_plugin(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_plugin_with_options(request, runtime)
 
     def modify_signature_with_options(self, request, runtime):
+        """
+        The new name of the key. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+
+        @param request: ModifySignatureRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ModifySignatureResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
         if not UtilClient.is_unset(request.signature_id):
             query['SignatureId'] = request.signature_id
         if not UtilClient.is_unset(request.signature_key):
@@ -4825,18 +6081,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ModifySignatureResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_signature(self, request):
+        """
+        The new name of the key. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It must start with a letter.
+        
+
+        @param request: ModifySignatureRequest
+
+        @return: ModifySignatureResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_signature_with_options(request, runtime)
 
     def modify_traffic_control_with_options(self, request, runtime):
+        """
+        The throttling policy name. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It cannot start with an underscore.
+        
+
+        @param request: ModifyTrafficControlRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ModifyTrafficControlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_default):
             query['ApiDefault'] = request.api_default
         if not UtilClient.is_unset(request.app_default):
             query['AppDefault'] = request.app_default
         if not UtilClient.is_unset(request.description):
@@ -4867,14 +6141,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ModifyTrafficControlResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_traffic_control(self, request):
+        """
+        The throttling policy name. The name must be 4 to 50 characters in length and can contain letters, digits, and underscores (\\_). It cannot start with an underscore.
+        
+
+        @param request: ModifyTrafficControlRequest
+
+        @return: ModifyTrafficControlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_traffic_control_with_options(request, runtime)
 
     def modify_vpc_access_and_update_apis_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
@@ -4936,15 +6218,55 @@
             self.call_api(params, req, runtime)
         )
 
     def open_api_gateway_service(self):
         runtime = util_models.RuntimeOptions()
         return self.open_api_gateway_service_with_options(runtime)
 
+    def query_request_logs_with_options(self, request, runtime):
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
+    def query_request_logs(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.query_request_logs_with_options(request, runtime)
+
     def reactivate_domain_with_options(self, request, runtime):
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+
+        @param request: ReactivateDomainRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ReactivateDomainResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -4965,14 +6287,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ReactivateDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def reactivate_domain(self, request):
+        """
+        The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
+        
+
+        @param request: ReactivateDomainRequest
+
+        @return: ReactivateDomainResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reactivate_domain_with_options(request, runtime)
 
     def remove_access_control_list_entry_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_entrys):
@@ -5001,14 +6331,24 @@
         )
 
     def remove_access_control_list_entry(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_access_control_list_entry_with_options(request, runtime)
 
     def remove_apis_authorities_with_options(self, request, runtime):
+        """
+        The ID of the app. The ID is generated by the system and globally unique.
+        
+
+        @param request: RemoveApisAuthoritiesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RemoveApisAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.description):
@@ -5035,18 +6375,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.RemoveApisAuthoritiesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_apis_authorities(self, request):
+        """
+        The ID of the app. The ID is generated by the system and globally unique.
+        
+
+        @param request: RemoveApisAuthoritiesRequest
+
+        @return: RemoveApisAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_apis_authorities_with_options(request, runtime)
 
     def remove_apps_authorities_with_options(self, request, runtime):
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+
+        @param request: RemoveAppsAuthoritiesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RemoveAppsAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.app_ids):
             query['AppIds'] = request.app_ids
         if not UtilClient.is_unset(request.group_id):
@@ -5071,18 +6429,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.RemoveAppsAuthoritiesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_apps_authorities(self, request):
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+
+        @param request: RemoveAppsAuthoritiesRequest
+
+        @return: RemoveAppsAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_apps_authorities_with_options(request, runtime)
 
     def remove_ip_control_apis_with_options(self, request, runtime):
+        """
+        The ID of the API group containing the API to be managed.
+        
+
+        @param request: RemoveIpControlApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RemoveIpControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.ip_control_id):
@@ -5107,18 +6483,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.RemoveIpControlApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_ip_control_apis(self, request):
+        """
+        The ID of the API group containing the API to be managed.
+        
+
+        @param request: RemoveIpControlApisRequest
+
+        @return: RemoveIpControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_ip_control_apis_with_options(request, runtime)
 
     def remove_ip_control_policy_item_with_options(self, request, runtime):
+        """
+        The ID of a policy. Separate multiple IDs with semicolons (;). A maximum of 100 IDs can be entered.
+        
+
+        @param request: RemoveIpControlPolicyItemRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RemoveIpControlPolicyItemResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ip_control_id):
             query['IpControlId'] = request.ip_control_id
         if not UtilClient.is_unset(request.policy_item_ids):
             query['PolicyItemIds'] = request.policy_item_ids
         if not UtilClient.is_unset(request.security_token):
@@ -5139,18 +6533,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.RemoveIpControlPolicyItemResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_ip_control_policy_item(self, request):
+        """
+        The ID of a policy. Separate multiple IDs with semicolons (;). A maximum of 100 IDs can be entered.
+        
+
+        @param request: RemoveIpControlPolicyItemRequest
+
+        @return: RemoveIpControlPolicyItemResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_ip_control_policy_item_with_options(request, runtime)
 
     def remove_signature_apis_with_options(self, request, runtime):
+        """
+        The ID of the signature key.
+        
+
+        @param request: RemoveSignatureApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RemoveSignatureApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -5175,18 +6587,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.RemoveSignatureApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_signature_apis(self, request):
+        """
+        The ID of the signature key.
+        
+
+        @param request: RemoveSignatureApisRequest
+
+        @return: RemoveSignatureApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_signature_apis_with_options(request, runtime)
 
     def remove_traffic_control_apis_with_options(self, request, runtime):
+        """
+        The ID of the API group containing the APIs from which you want to unbind a specified throttling policy.
+        
+
+        @param request: RemoveTrafficControlApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RemoveTrafficControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -5211,14 +6641,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.RemoveTrafficControlApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def remove_traffic_control_apis(self, request):
+        """
+        The ID of the API group containing the APIs from which you want to unbind a specified throttling policy.
+        
+
+        @param request: RemoveTrafficControlApisRequest
+
+        @return: RemoveTrafficControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_traffic_control_apis_with_options(request, runtime)
 
     def remove_vpc_access_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
@@ -5287,14 +6725,24 @@
         )
 
     def remove_vpc_access_and_abolish_apis(self, request):
         runtime = util_models.RuntimeOptions()
         return self.remove_vpc_access_and_abolish_apis_with_options(request, runtime)
 
     def reset_app_code_with_options(self, request, runtime):
+        """
+        The new AppCode takes effect about 2 seconds after you call this operation.
+        
+
+        @param request: ResetAppCodeRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: ResetAppCodeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_code):
             query['AppCode'] = request.app_code
         if not UtilClient.is_unset(request.new_app_code):
             query['NewAppCode'] = request.new_app_code
         if not UtilClient.is_unset(request.security_token):
@@ -5315,22 +6763,44 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ResetAppCodeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def reset_app_code(self, request):
+        """
+        The new AppCode takes effect about 2 seconds after you call this operation.
+        
+
+        @param request: ResetAppCodeRequest
+
+        @return: ResetAppCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reset_app_code_with_options(request, runtime)
 
     def reset_app_secret_with_options(self, request, runtime):
+        """
+        This operation is intended for API callers.
+        *   A new secret is automatically generated after you have called this operation. This secret cannot be customized.
+        *   The results returned by this operation do not contain the application secret. You can obtain the secret by calling DescribeAppSecurity.
+        
+
+        @param request: ResetAppSecretRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
@@ -5347,14 +6817,24 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.ResetAppSecretResponse(),
             self.call_api(params, req, runtime)
         )
 
     def reset_app_secret(self, request):
+        """
+        This operation is intended for API callers.
+        *   A new secret is automatically generated after you have called this operation. This secret cannot be customized.
+        *   The results returned by this operation do not contain the application secret. You can obtain the secret by calling DescribeAppSecurity.
+        
+
+        @param request: ResetAppSecretRequest
+
+        @return: ResetAppSecretResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reset_app_secret_with_options(request, runtime)
 
     def sdk_generate_by_app_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -5479,14 +6959,24 @@
         )
 
     def set_access_control_list_attribute(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_access_control_list_attribute_with_options(request, runtime)
 
     def set_apis_authorities_with_options(self, request, runtime):
+        """
+        The ID of the app. This ID is generated by the system and globally unique.
+        
+
+        @param request: SetApisAuthoritiesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: SetApisAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.auth_valid_time):
@@ -5515,18 +7005,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.SetApisAuthoritiesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_apis_authorities(self, request):
+        """
+        The ID of the app. This ID is generated by the system and globally unique.
+        
+
+        @param request: SetApisAuthoritiesRequest
+
+        @return: SetApisAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_apis_authorities_with_options(request, runtime)
 
     def set_apps_authorities_with_options(self, request, runtime):
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+
+        @param request: SetAppsAuthoritiesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: SetAppsAuthoritiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.app_ids):
             query['AppIds'] = request.app_ids
         if not UtilClient.is_unset(request.auth_valid_time):
@@ -5555,14 +7063,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.SetAppsAuthoritiesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_apps_authorities(self, request):
+        """
+        The ID of the API. This ID is generated by the system and globally unique.
+        
+
+        @param request: SetAppsAuthoritiesRequest
+
+        @return: SetAppsAuthoritiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_apps_authorities_with_options(request, runtime)
 
     def set_domain_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.bind_stage_name):
@@ -5597,14 +7113,24 @@
         )
 
     def set_domain(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_domain_with_options(request, runtime)
 
     def set_domain_certificate_with_options(self, request, runtime):
+        """
+        382271
+        
+
+        @param request: SetDomainCertificateRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: SetDomainCertificateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ca_certificate_body):
             query['CaCertificateBody'] = request.ca_certificate_body
         if not UtilClient.is_unset(request.certificate_body):
             query['CertificateBody'] = request.certificate_body
         if not UtilClient.is_unset(request.certificate_name):
@@ -5635,14 +7161,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.SetDomainCertificateResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_domain_certificate(self, request):
+        """
+        382271
+        
+
+        @param request: SetDomainCertificateRequest
+
+        @return: SetDomainCertificateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_domain_certificate_with_options(request, runtime)
 
     def set_domain_web_socket_status_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.action_value):
@@ -5674,15 +7208,57 @@
             self.call_api(params, req, runtime)
         )
 
     def set_domain_web_socket_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_domain_web_socket_status_with_options(request, runtime)
 
+    def set_group_auth_app_code_with_options(self, request, runtime):
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
+    def set_group_auth_app_code(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_group_auth_app_code_with_options(request, runtime)
+
     def set_ip_control_apis_with_options(self, request, runtime):
+        """
+        The ID of the API group.
+        
+
+        @param request: SetIpControlApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: SetIpControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.ip_control_id):
@@ -5707,18 +7283,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.SetIpControlApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_ip_control_apis(self, request):
+        """
+        The ID of the API group.
+        
+
+        @param request: SetIpControlApisRequest
+
+        @return: SetIpControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_ip_control_apis_with_options(request, runtime)
 
     def set_signature_apis_with_options(self, request, runtime):
+        """
+        The ID of the signature key.
+        
+
+        @param request: SetSignatureApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: SetSignatureApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -5743,18 +7337,36 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.SetSignatureApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_signature_apis(self, request):
+        """
+        The ID of the signature key.
+        
+
+        @param request: SetSignatureApisRequest
+
+        @return: SetSignatureApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_signature_apis_with_options(request, runtime)
 
     def set_traffic_control_apis_with_options(self, request, runtime):
+        """
+        The ID of the API group containing the APIs to which you want to bind a specified throttling policy.
+        
+
+        @param request: SetTrafficControlApisRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: SetTrafficControlApisResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_ids):
             query['ApiIds'] = request.api_ids
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.security_token):
@@ -5779,14 +7391,22 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.SetTrafficControlApisResponse(),
             self.call_api(params, req, runtime)
         )
 
     def set_traffic_control_apis(self, request):
+        """
+        The ID of the API group containing the APIs to which you want to bind a specified throttling policy.
+        
+
+        @param request: SetTrafficControlApisRequest
+
+        @return: SetTrafficControlApisResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_traffic_control_apis_with_options(request, runtime)
 
     def set_vpc_access_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.description):
@@ -5857,14 +7477,24 @@
         )
 
     def set_wildcard_domain_patterns(self, request):
         runtime = util_models.RuntimeOptions()
         return self.set_wildcard_domain_patterns_with_options(request, runtime)
 
     def switch_api_with_options(self, request, runtime):
+        """
+        The ID of the API.
+        
+
+        @param request: SwitchApiRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: SwitchApiResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_id):
             query['ApiId'] = request.api_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.group_id):
@@ -5891,18 +7521,37 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.SwitchApiResponse(),
             self.call_api(params, req, runtime)
         )
 
     def switch_api(self, request):
+        """
+        The ID of the API.
+        
+
+        @param request: SwitchApiRequest
+
+        @return: SwitchApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.switch_api_with_options(request, runtime)
 
     def tag_resources_with_options(self, request, runtime):
+        """
+        The key of tag N.
+        Valid values of N: `1 to 20.`
+        
+
+        @param request: TagResourcesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: TagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
             query['ResourceType'] = request.resource_type
         if not UtilClient.is_unset(request.security_token):
@@ -5925,18 +7574,39 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.TagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def tag_resources(self, request):
+        """
+        The key of tag N.
+        Valid values of N: `1 to 20.`
+        
+
+        @param request: TagResourcesRequest
+
+        @return: TagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     def untag_resources_with_options(self, request, runtime):
+        """
+        Specifies whether to delete all tags. This parameter is valid only when the *TagKey.N**parameter is not specified. Default value: false. Valid values:
+        *   **true**\
+        *   **false**\
+        
+
+        @param request: UntagResourcesRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: UntagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
         if not UtilClient.is_unset(request.resource_type):
@@ -5961,9 +7631,51 @@
         )
         return TeaCore.from_map(
             cloud_api20160714_models.UntagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def untag_resources(self, request):
+        """
+        Specifies whether to delete all tags. This parameter is valid only when the *TagKey.N**parameter is not specified. Default value: false. Valid values:
+        *   **true**\
+        *   **false**\
+        
+
+        @param request: UntagResourcesRequest
+
+        @return: UntagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
+
+    def validate_vpc_connectivity_with_options(self, request, runtime):
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
+    def validate_vpc_connectivity(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.validate_vpc_connectivity_with_options(request, runtime)
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/models.py` & `alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -200,16 +200,19 @@
             temp_model = AddAccessControlListEntryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddIpControlPolicyItemRequest(TeaModel):
     def __init__(self, app_id=None, cidr_ip=None, ip_control_id=None, security_token=None):
+        # The ID of the policy. The ID is unique.
         self.app_id = app_id  # type: str
+        # The ID of the request.
         self.cidr_ip = cidr_ip  # type: str
+        # The IP addresses or CIDR blocks involved in the policy. Separate multiple IP addresses or CIDR blocks with semicolons (;). You can specify a maximum of 10 IP addresses or CIDR blocks.
         self.ip_control_id = ip_control_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -239,15 +242,21 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class AddIpControlPolicyItemResponseBody(TeaModel):
     def __init__(self, policy_item_id=None, request_id=None):
+        # When you call this operation, note that:
+        # 
+        # *   This operation is intended for API providers.
+        # *   An added policy immediately takes effect on all APIs that are bound to the access control list (ACL).
+        # *   A maximum of 100 policies can be added to an ACL.
         self.policy_item_id = policy_item_id  # type: str
+        # Adds a policy to an existing ACL.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddIpControlPolicyItemResponseBody, self).to_map()
@@ -309,17 +318,23 @@
         return self
 
 
 class AddTrafficSpecialControlRequest(TeaModel):
     def __init__(self, security_token=None, special_key=None, special_type=None, traffic_control_id=None,
                  traffic_value=None):
         self.security_token = security_token  # type: str
+        # The ID of the request.
         self.special_key = special_key  # type: str
+        # The special throttling value.
         self.special_type = special_type  # type: str
+        # The ID of the app or Alibaba Cloud account. Specify this parameter based on the value of the **SpecialType** parameter. You can view your account ID on the [Account Management](https://account.console.aliyun.com/?spm=a2c4g.11186623.2.15.3f053654YpMPwo#/secure) page.
         self.traffic_control_id = traffic_control_id  # type: str
+        # *   This API is intended for API providers.
+        # *   If the input SpecialKey already exists, the previous configuration is overwritten. Use caution when calling this operation.
+        # *   Special throttling policies must be added to an existing throttling policy, and can take effect on all the APIs to which the throttling policy is bound.
         self.traffic_value = traffic_value  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddTrafficSpecialControlRequest, self).to_map()
@@ -352,14 +367,15 @@
         if m.get('TrafficValue') is not None:
             self.traffic_value = m.get('TrafficValue')
         return self
 
 
 class AddTrafficSpecialControlResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Adds a custom special policy to a specified throttling policy.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddTrafficSpecialControlResponseBody, self).to_map()
@@ -672,15 +688,17 @@
             temp_model = BatchAbolishApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchDeployApisRequestApi(TeaModel):
     def __init__(self, api_uid=None, group_id=None):
+        # Publishes multiple APIs at a time.
         self.api_uid = api_uid  # type: str
+        # The APIs that you want to operate.
         self.group_id = group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BatchDeployApisRequestApi, self).to_map()
@@ -701,17 +719,20 @@
         if m.get('GroupId') is not None:
             self.group_id = m.get('GroupId')
         return self
 
 
 class BatchDeployApisRequest(TeaModel):
     def __init__(self, api=None, description=None, security_token=None, stage_name=None):
+        # b4f5c342b8bc4ef88ccda0332402e0fa
         self.api = api  # type: list[BatchDeployApisRequestApi]
+        # 2b35dd68345b472f8051647306a16415
         self.description = description  # type: str
         self.security_token = security_token  # type: str
+        # The description.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         if self.api:
             for k in self.api:
                 if k:
                     k.validate()
@@ -815,44 +836,51 @@
         if m.get('body') is not None:
             temp_model = BatchDeployApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateAccessControlListRequest(TeaModel):
-    def __init__(self, acl_name=None, security_token=None):
+    def __init__(self, acl_name=None, address_ipversion=None, security_token=None):
+        # The name of the ACL. The name must be 1 to 30 characters in length, and can contain letters, digits, periods (.), hyphens (-), forward slashes (/), and underscores (\_). The name must be unique within the region.
         self.acl_name = acl_name  # type: str
+        self.address_ipversion = address_ipversion  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateAccessControlListRequest, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AclName') is not None:
             self.acl_name = m.get('AclName')
+        if m.get('AddressIPVersion') is not None:
+            self.address_ipversion = m.get('AddressIPVersion')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class CreateAccessControlListResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateAccessControlListResponseBody, self).to_map()
@@ -913,40 +941,83 @@
 class CreateApiRequest(TeaModel):
     def __init__(self, allow_signature_method=None, api_name=None, app_code_auth_type=None, auth_type=None,
                  backend_enable=None, backend_id=None, constant_parameters=None, description=None, disable_internet=None,
                  error_code_samples=None, fail_result_sample=None, force_nonce_check=None, group_id=None, open_id_connect_config=None,
                  request_config=None, request_parameters=None, result_body_model=None, result_descriptions=None,
                  result_sample=None, result_type=None, security_token=None, service_config=None, service_parameters=None,
                  service_parameters_map=None, system_parameters=None, visibility=None, web_socket_api_type=None):
+        # If the **AuthType** is **APP** authentication, you need to pass this value to specify the signature algorithm. If you do not specify this parameter, the default value HmacSHA256 is used. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method  # type: str
+        # The name of the API that you want to create. The name must be unique within the API group. The name must be 4 to 50 characters in length. It must start with a letter and can contain letters, digits, and underscores (\_).
         self.api_name = api_name  # type: str
+        # If the **AuthType** parameter is set to **APP**, the valid values are:
+        # 
+        # *   **DEFAULT**: The default value that is used if no other values are passed. This value indicates that the settings of the group are used.
+        # *   **DISABLE**: The authentication is disabled.
+        # *   **HEADER**: AppCode can be placed in the Header parameter for authentication.
+        # *   **HEADER_QUERY**: AppCode can be placed in the Header or Query parameter for authentication.
         self.app_code_auth_type = app_code_auth_type  # type: str
+        # API安全认证类型，目前可以取值：
+        # 
+        # - **APP**：只允许已授权的APP调用
+        # - **ANONYMOUS**：允许匿名调用，设置为允许匿名调用需要注意：
+        #   任何能够获取该API服务信息的人，都将能够调用该API。网关不会对调用者做身份认证，也无法设置按用户的流量控制，若开放该API请设置好按API的流量控制。
         self.auth_type = auth_type  # type: str
+        # Specifies whether to enable backend services.
         self.backend_enable = backend_enable  # type: bool
+        # The IDof the backend service
         self.backend_id = backend_id  # type: str
         self.constant_parameters = constant_parameters  # type: str
+        # The description of the API. The description can be up to 180 characters in length.
         self.description = description  # type: str
+        # *   Specifies whether to set **DisableInternet** to **true** to limit API calls to within the VPC.
+        # *   If you set **DisableInternet** to **false**, the limit is lifted. The default value is false when you create an API.
         self.disable_internet = disable_internet  # type: bool
         self.error_code_samples = error_code_samples  # type: str
         self.fail_result_sample = fail_result_sample  # type: str
+        # *   Specifies whether to set **ForceNonceCheck** to **true** to force the check of X-Ca-Nonce during the request. This is the unique identifier of the request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent replay attacks.
+        # *   If you set **ForceNonceCheck** to **false**, the check is not performed. The default value is false when you create an API.
         self.force_nonce_check = force_nonce_check  # type: bool
+        # The ID of the API group.
         self.group_id = group_id  # type: str
+        # The switch status of ACL. Valid values:- **on** and **off**.
         self.open_id_connect_config = open_id_connect_config  # type: str
+        # The configuration items of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestConfig](~~43985~~).
         self.request_config = request_config  # type: str
         self.request_parameters = request_parameters  # type: str
+        # The return description of the API.
         self.result_body_model = result_body_model  # type: str
         self.result_descriptions = result_descriptions  # type: str
         self.result_sample = result_sample  # type: str
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML. Default value: JSON.
         self.result_type = result_type  # type: str
         self.security_token = security_token  # type: str
+        # The configuration items of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceConfig](~~43987~~).
         self.service_config = service_config  # type: str
         self.service_parameters = service_parameters  # type: str
         self.service_parameters_map = service_parameters_map  # type: str
         self.system_parameters = system_parameters  # type: str
+        # Specifies whether to make the API public. Valid values:
+        # 
+        # *   **PUBLIC**: Make the API public. If you set this parameter to PUBLIC, this API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE**: Make the API private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.visibility = visibility  # type: str
+        # The type of the two-way communication API.
+        # 
+        # *   **COMMON**: common API
+        # *   **REGISTER**: registered API
+        # *   **UNREGISTER**: unregistered API
+        # *   **NOTIFY**: downstream notification API
         self.web_socket_api_type = web_socket_api_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateApiRequest, self).to_map()
@@ -1067,15 +1138,17 @@
         if m.get('WebSocketApiType') is not None:
             self.web_socket_api_type = m.get('WebSocketApiType')
         return self
 
 
 class CreateApiResponseBody(TeaModel):
     def __init__(self, api_id=None, request_id=None):
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateApiResponseBody, self).to_map()
@@ -1472,23 +1545,23 @@
             self.key = m.get('Key')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class CreateAppRequest(TeaModel):
-    def __init__(self, app_code=None, app_key=None, app_name=None, app_secret=None, description=None,
-                 security_token=None, source=None, tag=None):
+    def __init__(self, app_code=None, app_key=None, app_name=None, app_secret=None, description=None, extend=None,
+                 security_token=None, tag=None):
         self.app_code = app_code  # type: str
         self.app_key = app_key  # type: str
         self.app_name = app_name  # type: str
         self.app_secret = app_secret  # type: str
         self.description = description  # type: str
+        self.extend = extend  # type: str
         self.security_token = security_token  # type: str
-        self.source = source  # type: str
         self.tag = tag  # type: list[CreateAppRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -1505,18 +1578,18 @@
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
 
     def from_map(self, m=None):
@@ -1527,18 +1600,18 @@
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
 
@@ -2057,29 +2130,110 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDatasetItemResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateInstanceRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateInstanceRequestTag, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateInstanceRequestZoneVSwitchSecurityGroup(TeaModel):
+    def __init__(self, cidr_block=None, security_group_id=None, v_switch_id=None, zone_id=None):
+        self.cidr_block = cidr_block  # type: str
+        self.security_group_id = security_group_id  # type: str
+        self.v_switch_id = v_switch_id  # type: str
+        self.zone_id = zone_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateInstanceRequestZoneVSwitchSecurityGroup, self).to_map()
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
+    def from_map(self, m=None):
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
-    def __init__(self, auto_pay=None, charge_type=None, duration=None, https_policy=None, instance_name=None,
-                 instance_spec=None, pricing_cycle=None, token=None, zone_id=None):
+    def __init__(self, auto_pay=None, charge_type=None, duration=None, https_policy=None, instance_cidr=None,
+                 instance_name=None, instance_spec=None, instance_type=None, pricing_cycle=None, tag=None, token=None,
+                 user_vpc_id=None, zone_id=None, zone_vswitch_security_group=None):
         self.auto_pay = auto_pay  # type: bool
         self.charge_type = charge_type  # type: str
         self.duration = duration  # type: int
         self.https_policy = https_policy  # type: str
+        self.instance_cidr = instance_cidr  # type: str
         self.instance_name = instance_name  # type: str
         self.instance_spec = instance_spec  # type: str
+        self.instance_type = instance_type  # type: str
         self.pricing_cycle = pricing_cycle  # type: str
+        self.tag = tag  # type: list[CreateInstanceRequestTag]
         self.token = token  # type: str
+        self.user_vpc_id = user_vpc_id  # type: str
         self.zone_id = zone_id  # type: str
+        self.zone_vswitch_security_group = zone_vswitch_security_group  # type: list[CreateInstanceRequestZoneVSwitchSecurityGroup]
 
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
         _map = super(CreateInstanceRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2087,75 +2241,110 @@
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
 
     def from_map(self, m=None):
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
-    def __init__(self, instance_id=None, request_id=None):
+    def __init__(self, instance_id=None, request_id=None, tag_status=None):
         self.instance_id = instance_id  # type: str
         self.request_id = request_id  # type: str
+        self.tag_status = tag_status  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateInstanceResponseBody, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('TagStatus') is not None:
+            self.tag_status = m.get('TagStatus')
         return self
 
 
 class CreateInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
@@ -2192,14 +2381,15 @@
             temp_model = CreateInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateIntranetDomainRequest(TeaModel):
     def __init__(self, group_id=None, security_token=None):
+        # The custom domain name.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2221,15 +2411,17 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class CreateIntranetDomainResponseBody(TeaModel):
     def __init__(self, domain_name=None, request_id=None):
+        # The ID of the request.
         self.domain_name = domain_name  # type: str
+        # auditing
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateIntranetDomainResponseBody, self).to_map()
@@ -2441,14 +2633,15 @@
         return self
 
 
 class CreateLogConfigRequest(TeaModel):
     def __init__(self, log_type=None, security_token=None, sls_log_store=None, sls_project=None):
         self.log_type = log_type  # type: str
         self.security_token = security_token  # type: str
+        # slslogstore
         self.sls_log_store = sls_log_store  # type: str
         self.sls_project = sls_project  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2541,17 +2734,21 @@
             temp_model = CreateLogConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateModelRequest(TeaModel):
     def __init__(self, description=None, group_id=None, model_name=None, schema=None):
+        # The description of the model definition.
         self.description = description  # type: str
+        # The ID of the API group to which the model belongs.
         self.group_id = group_id  # type: str
+        # The name of the model. The name must be unique within the group.
         self.model_name = model_name  # type: str
+        # The definition of the model in JSON Schema.
         self.schema = schema  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateModelRequest, self).to_map()
@@ -2581,23 +2778,33 @@
             self.schema = m.get('Schema')
         return self
 
 
 class CreateModelResponseBody(TeaModel):
     def __init__(self, created_time=None, description=None, group_id=None, model_id=None, model_name=None,
                  model_ref=None, modified_time=None, region_id=None, request_id=None, schema=None):
+        # The time when the model was created.
         self.created_time = created_time  # type: str
+        # The description of the created model.
         self.description = description  # type: str
+        # The ID of the API group to which the created model belongs.
         self.group_id = group_id  # type: str
+        # The ID of the created model.
         self.model_id = model_id  # type: str
+        # The name of the created model.
         self.model_name = model_name  # type: str
+        # The URI of the created model.
         self.model_ref = model_ref  # type: str
+        # The time when the model is last modified.
         self.modified_time = modified_time  # type: str
+        # The region to which the created model belongs.
         self.region_id = region_id  # type: str
+        # The ID of the request.
         self.request_id = request_id  # type: str
+        # The definition of the created model.
         self.schema = schema  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateModelResponseBody, self).to_map()
@@ -2957,16 +3164,19 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateSignatureRequest(TeaModel):
     def __init__(self, security_token=None, signature_key=None, signature_name=None, signature_secret=None):
         self.security_token = security_token  # type: str
+        # The ID of the request.
         self.signature_key = signature_key  # type: str
+        # The Secret value of the key. The value must be 6 to 30 characters in length and can contain letters, digits, and special characters. Special characters include underscores (\_), at signs (@), number signs (#), exclamation points (!), and asterisks (\*). The value must start with a letter.
         self.signature_name = signature_name  # type: str
+        # The ID of the back-end signature key.
         self.signature_secret = signature_secret  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateSignatureRequest, self).to_map()
@@ -2995,16 +3205,22 @@
         if m.get('SignatureSecret') is not None:
             self.signature_secret = m.get('SignatureSecret')
         return self
 
 
 class CreateSignatureResponseBody(TeaModel):
     def __init__(self, request_id=None, signature_id=None, signature_name=None):
+        # The name of the back-end signature key.
         self.request_id = request_id  # type: str
+        # *   This API is intended for API providers.
+        # *   The API operation only creates a key policy. You must call the binding operation to bind the key to an API.
+        # *   After the key is bound to the API, requests sent from API Gateway to the backend service contain signature strings. You can specify whether your backend service verifies these signature strings.
+        # *   The QPS limit on this operation is 50 per user.
         self.signature_id = signature_id  # type: str
+        # Creates a backend signature key.
         self.signature_name = signature_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateSignatureResponseBody, self).to_map()
@@ -3069,20 +3285,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateTrafficControlRequest(TeaModel):
     def __init__(self, api_default=None, app_default=None, description=None, security_token=None,
                  traffic_control_name=None, traffic_control_unit=None, user_default=None):
+        # The default throttling value for each app.
         self.api_default = api_default  # type: int
+        # ThrottlingTestDescription
         self.app_default = app_default  # type: int
+        # The ID of the throttling policy.
         self.description = description  # type: str
         self.security_token = security_token  # type: str
+        # The unit to be used in the throttling policy. Valid values:
+        # 
+        # *   **SECOND**\
+        # *   **MINUTE**\
+        # *   **HOUR**\
+        # *   **DAY**\
         self.traffic_control_name = traffic_control_name  # type: str
+        # The default throttling value for each user.
         self.traffic_control_unit = traffic_control_unit  # type: str
+        # The description of the throttling policy.
         self.user_default = user_default  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTrafficControlRequest, self).to_map()
@@ -3123,15 +3350,19 @@
         if m.get('UserDefault') is not None:
             self.user_default = m.get('UserDefault')
         return self
 
 
 class CreateTrafficControlResponseBody(TeaModel):
     def __init__(self, request_id=None, traffic_control_id=None):
+        # Creates a custom throttling policy.
         self.request_id = request_id  # type: str
+        # *   This API is intended for API providers.
+        # *   Throttling policies must be bound to APIs to take effect. After a policy is bound to an API, it goes into effect on that API immediately.
+        # *   The QPS limit on this operation is 50 per user.
         self.traffic_control_id = traffic_control_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTrafficControlResponseBody, self).to_map()
@@ -3284,14 +3515,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteAllTrafficSpecialControlRequest(TeaModel):
     def __init__(self, security_token=None, traffic_control_id=None):
         self.security_token = security_token  # type: str
+        # *   This API is intended for API providers.
         self.traffic_control_id = traffic_control_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteAllTrafficSpecialControlRequest, self).to_map()
@@ -3312,14 +3544,15 @@
         if m.get('TrafficControlId') is not None:
             self.traffic_control_id = m.get('TrafficControlId')
         return self
 
 
 class DeleteAllTrafficSpecialControlResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Deletes all custom special policies of a specified throttling policy.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteAllTrafficSpecialControlResponseBody, self).to_map()
@@ -3606,17 +3839,20 @@
             temp_model = DeleteApiGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteApiStageVariableRequest(TeaModel):
     def __init__(self, group_id=None, security_token=None, stage_id=None, variable_name=None):
+        # The name of the variable to be deleted. This parameter is case-sensitive.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The ID of the request.
         self.stage_id = stage_id  # type: str
+        # *   This operation is intended for API providers.
         self.variable_name = variable_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteApiStageVariableRequest, self).to_map()
@@ -3645,14 +3881,15 @@
         if m.get('VariableName') is not None:
             self.variable_name = m.get('VariableName')
         return self
 
 
 class DeleteApiStageVariableResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Deletes a specified variable in a specified environment.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteApiStageVariableResponseBody, self).to_map()
@@ -4230,15 +4467,19 @@
             temp_model = DeleteDatasetItemResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteDomainRequest(TeaModel):
     def __init__(self, domain_name=None, group_id=None, security_token=None):
+        # *   This operation is intended for API providers.
+        # *   If the specified domain name does not exist, a successful response will still appear.
+        # *   Unbinding a domain name from an API group will affect access to the APIs in the group. Exercise caution when using this operation.
         self.domain_name = domain_name  # type: str
+        # The ID of the request.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4264,14 +4505,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DeleteDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Unbinds a custom domain name from a specified API group.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteDomainResponseBody, self).to_map()
@@ -4558,14 +4800,17 @@
             temp_model = DeleteInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteIpControlRequest(TeaModel):
     def __init__(self, ip_control_id=None, security_token=None):
+        # *   This operation is intended for API providers.
+        # *   If the ACL is bound to an API, you must unbind the ACL from the API before you can delete the ACL. Otherwise, an error is returned.
+        # *   If you call this operation on an ACL that does not exist, a success message is returned.
         self.ip_control_id = ip_control_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4587,14 +4832,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DeleteIpControlResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Deletes an access control list (ACL).
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteIpControlResponseBody, self).to_map()
@@ -4742,15 +4988,17 @@
             temp_model = DeleteLogConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteModelRequest(TeaModel):
     def __init__(self, group_id=None, model_name=None):
+        # The ID of the request.
         self.group_id = group_id  # type: str
+        # The ID of the API group to which the model belongs.
         self.model_name = model_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteModelRequest, self).to_map()
@@ -4771,14 +5019,15 @@
         if m.get('ModelName') is not None:
             self.model_name = m.get('ModelName')
         return self
 
 
 class DeleteModelResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Deletes a model from Model Management for an API group.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteModelResponseBody, self).to_map()
@@ -5066,14 +5315,18 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteSignatureRequest(TeaModel):
     def __init__(self, security_token=None, signature_id=None):
         self.security_token = security_token  # type: str
+        # *   This API is intended for API providers.
+        # *   This API operation deletes an existing backend signature key.
+        # *   You cannot delete a key that is bound to an API. To delete the key, you must unbind it first.
+        # *   The QPS limit on this operation is 50 per user.
         self.signature_id = signature_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteSignatureRequest, self).to_map()
@@ -5094,14 +5347,15 @@
         if m.get('SignatureId') is not None:
             self.signature_id = m.get('SignatureId')
         return self
 
 
 class DeleteSignatureResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Deletes a backend signature key.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteSignatureResponseBody, self).to_map()
@@ -5250,16 +5504,20 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteTrafficSpecialControlRequest(TeaModel):
     def __init__(self, security_token=None, special_key=None, special_type=None, traffic_control_id=None):
         self.security_token = security_token  # type: str
+        # *   This API is intended for API providers.
+        # *   You can obtain the input parameters required in this operation by calling other APIs.
         self.special_key = special_key  # type: str
+        # The ID of the request.
         self.special_type = special_type  # type: str
+        # The ID of the app or Alibaba Cloud account. You can view your account ID on the [Account Management](https://account.console.aliyun.com/?spm=a2c4g.11186623.2.15.343130a8sDi8cO#/secure) page.
         self.traffic_control_id = traffic_control_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTrafficSpecialControlRequest, self).to_map()
@@ -5288,14 +5546,15 @@
         if m.get('TrafficControlId') is not None:
             self.traffic_control_id = m.get('TrafficControlId')
         return self
 
 
 class DeleteTrafficSpecialControlResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Deletes a custom special throttling policy.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTrafficSpecialControlResponseBody, self).to_map()
@@ -5351,18 +5610,28 @@
             temp_model = DeleteTrafficSpecialControlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeployApiRequest(TeaModel):
     def __init__(self, api_id=None, description=None, group_id=None, security_token=None, stage_name=None):
+        # The publishing remarks.
         self.api_id = api_id  # type: str
-        self.description = description  # type: str
+        # *   This operation is intended for API providers. Only the API that you have defined and published to a runtime environment can be called.
+        # *   An API is published to a cluster in less than 5 seconds.
+        # *   The QPS limit on this operation is 50 per user.
+        self.description = description  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **PRE: the pre-release environment**\
+        # *   **TEST: the test environment**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The ID of the request.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeployApiRequest, self).to_map()
@@ -5395,14 +5664,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class DeployApiResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Publishes an API to a specified environment.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeployApiResponseBody, self).to_map()
@@ -5823,16 +6093,17 @@
         if m.get('body') is not None:
             temp_model = DescribeAccessControlListAttributeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAccessControlListsRequest(TeaModel):
-    def __init__(self, acl_name=None, page_number=None, page_size=None, security_token=None):
+    def __init__(self, acl_name=None, address_ipversion=None, page_number=None, page_size=None, security_token=None):
         self.acl_name = acl_name  # type: str
+        self.address_ipversion = address_ipversion  # type: str
         self.page_number = page_number  # type: int
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -5840,61 +6111,70 @@
         _map = super(DescribeAccessControlListsRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
-    def __init__(self, acl_id=None, acl_name=None):
+    def __init__(self, acl_id=None, acl_name=None, address_ipversion=None):
         self.acl_id = acl_id  # type: str
         self.acl_name = acl_name  # type: str
+        self.address_ipversion = address_ipversion  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAccessControlListsResponseBodyAclsAcl, self).to_map()
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AclId') is not None:
             self.acl_id = m.get('AclId')
         if m.get('AclName') is not None:
             self.acl_name = m.get('AclName')
+        if m.get('AddressIPVersion') is not None:
+            self.address_ipversion = m.get('AddressIPVersion')
         return self
 
 
 class DescribeAccessControlListsResponseBodyAcls(TeaModel):
     def __init__(self, acl=None):
         self.acl = acl  # type: list[DescribeAccessControlListsResponseBodyAclsAcl]
 
@@ -6009,15 +6289,17 @@
             temp_model = DescribeAccessControlListsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApiRequest(TeaModel):
     def __init__(self, api_id=None, group_id=None, security_token=None):
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The ID of the API.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6043,16 +6325,19 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeApiResponseBodyBackendConfig(TeaModel):
     def __init__(self, backend_id=None, backend_name=None, backend_type=None):
+        # Backend service type
         self.backend_id = backend_id  # type: str
+        # The configuration items of API requests sent by the consumer to API Gateway.
         self.backend_name = backend_name  # type: str
+        # The name of the backend service.
         self.backend_type = backend_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyBackendConfig, self).to_map()
@@ -6077,17 +6362,21 @@
         if m.get('BackendType') is not None:
             self.backend_type = m.get('BackendType')
         return self
 
 
 class DescribeApiResponseBodyConstantParametersConstantParameter(TeaModel):
     def __init__(self, constant_value=None, description=None, location=None, service_parameter_name=None):
+        # The parameters of API requests sent by the consumer to API Gateway.
         self.constant_value = constant_value  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.description = description  # type: str
+        # The name of the backend service parameter.
         self.location = location  # type: str
+        # The value of the parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyConstantParametersConstantParameter, self).to_map()
@@ -6149,18 +6438,23 @@
                 self.constant_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiResponseBodyCustomSystemParametersCustomSystemParameter(TeaModel):
     def __init__(self, demo_value=None, description=None, location=None, parameter_name=None,
                  service_parameter_name=None):
+        # Description
         self.demo_value = demo_value  # type: str
+        # Client IP Address
         self.description = description  # type: str
+        # The name of the corresponding backend parameter.
         self.location = location  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.parameter_name = parameter_name  # type: str
+        # System parameters sent by API Gateway to the backend service
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyCustomSystemParametersCustomSystemParameter, self).to_map()
@@ -6225,16 +6519,19 @@
                 temp_model = DescribeApiResponseBodyCustomSystemParametersCustomSystemParameter()
                 self.custom_system_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiResponseBodyDeployedInfosDeployedInfo(TeaModel):
     def __init__(self, deployed_status=None, effective_version=None, stage_name=None):
+        # auditing
         self.deployed_status = deployed_status  # type: str
+        # The deployment status. Valid values: DEPLOYED and NONDEPLOYED.
         self.effective_version = effective_version  # type: str
+        # The effective version.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyDeployedInfosDeployedInfo, self).to_map()
@@ -6291,17 +6588,21 @@
                 temp_model = DescribeApiResponseBodyDeployedInfosDeployedInfo()
                 self.deployed_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiResponseBodyErrorCodeSamplesErrorCodeSample(TeaModel):
     def __init__(self, code=None, description=None, message=None, model=None):
+        # Model
         self.code = code  # type: str
+        # The UserId parameter is missing from the request.
         self.description = description  # type: str
+        # Description
         self.message = message  # type: str
+        # Error message
         self.model = model  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyErrorCodeSamplesErrorCodeSample, self).to_map()
@@ -6362,17 +6663,21 @@
                 temp_model = DescribeApiResponseBodyErrorCodeSamplesErrorCodeSample()
                 self.error_code_sample.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiResponseBodyOpenIdConnectConfig(TeaModel):
     def __init__(self, id_token_param_name=None, open_id_api_type=None, public_key=None, public_key_id=None):
+        # The ID of the public key.
         self.id_token_param_name = id_token_param_name  # type: str
+        # The name of the parameter that corresponds to the token.
         self.open_id_api_type = open_id_api_type  # type: str
+        # The sample error codes returned by the backend service.
         self.public_key = public_key  # type: str
+        # The public key.
         self.public_key_id = public_key_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyOpenIdConnectConfig, self).to_map()
@@ -6402,20 +6707,29 @@
             self.public_key_id = m.get('PublicKeyId')
         return self
 
 
 class DescribeApiResponseBodyRequestConfig(TeaModel):
     def __init__(self, body_format=None, body_model=None, post_body_description=None, request_http_method=None,
                  request_mode=None, request_path=None, request_protocol=None):
+        # The request mode. Valid values: MAPPING and PASSTHROUGH.
         self.body_format = body_format  # type: str
+        # The API request path. If the complete API URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the API request path is ` /object/add  `.
         self.body_model = body_model  # type: str
+        # The protocol type supported by the API. Valid values: HTTP and HTTPS. Separate multiple values with commas (,), such as "HTTP,HTTPS".
         self.post_body_description = post_body_description  # type: str
+        # This parameter takes effect only when the RequestMode parameter is set to MAPPING.********\
+        # 
+        # The server data transmission method used for POST and PUT requests. Valid values: FORM and STREAM. FORM indicates that data in key-value pairs is transmitted as forms. STREAM indicates that data is transmitted as byte streams.
         self.request_http_method = request_http_method  # type: str
+        # The description of the request body.
         self.request_mode = request_mode  # type: str
+        # The HTTP method used to make the request. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_path = request_path  # type: str
+        # The configuration items of API requests sent by API Gateway to the backend service.
         self.request_protocol = request_protocol  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyRequestConfig, self).to_map()
@@ -6459,30 +6773,47 @@
 
 
 class DescribeApiResponseBodyRequestParametersRequestParameter(TeaModel):
     def __init__(self, api_parameter_name=None, array_items_type=None, default_value=None, demo_value=None,
                  description=None, doc_order=None, doc_show=None, enum_value=None, json_scheme=None, location=None,
                  max_length=None, max_value=None, min_length=None, min_value=None, parameter_type=None,
                  regular_expression=None, required=None):
+        # The hash values that can be entered when **ParameterType** is set to Int, Long, Float, Double, or String. Separate different values with commas (,), such as 1,2,3,4,9 or A,B,C,E,F.
         self.api_parameter_name = api_parameter_name  # type: str
+        # The minimum parameter value when **ParameterType** is set to Int, Long, Float, or Double.
         self.array_items_type = array_items_type  # type: str
+        # The name of the parameter.
         self.default_value = default_value  # type: str
+        # Indicates whether the parameter is required. Valid values: **REQUIRED** and **OPTIONAL**.
         self.demo_value = demo_value  # type: str
+        # Age
         self.description = description  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.doc_order = doc_order  # type: int
+        # The maximum parameter length when **ParameterType** is set to String.
         self.doc_show = doc_show  # type: str
+        # Examples
         self.enum_value = enum_value  # type: str
+        # The maximum parameter value when **ParameterType** is set to Int, Long, Float, or Double.
         self.json_scheme = json_scheme  # type: str
+        # The parameters of API requests sent by API Gateway to the backend service.
         self.location = location  # type: str
+        # The default value.
         self.max_length = max_length  # type: long
+        # The type of the array element.
         self.max_value = max_value  # type: long
+        # The order in the document.
         self.min_length = min_length  # type: long
+        # Indicates whether the document is public. Valid values: **PUBLIC** and **PRIVATE**.
         self.min_value = min_value  # type: long
+        # The regular expression used for parameter validation when **ParameterType** is set to String.
         self.parameter_type = parameter_type  # type: str
+        # The minimum parameter length when **ParameterType** is set to String.
         self.regular_expression = regular_expression  # type: str
+        # Description
         self.required = required  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyRequestParametersRequestParameter, self).to_map()
@@ -6593,111 +6924,23 @@
         if m.get('RequestParameter') is not None:
             for k in m.get('RequestParameter'):
                 temp_model = DescribeApiResponseBodyRequestParametersRequestParameter()
                 self.request_parameter.append(temp_model.from_map(k))
         return self
 
 
-class DescribeApiResponseBodyResultDescriptionsResultDescription(TeaModel):
-    def __init__(self, description=None, has_child=None, id=None, key=None, mandatory=None, name=None, pid=None,
-                 type=None):
-        self.description = description  # type: str
-        self.has_child = has_child  # type: bool
-        self.id = id  # type: str
-        self.key = key  # type: str
-        self.mandatory = mandatory  # type: bool
-        self.name = name  # type: str
-        self.pid = pid  # type: str
-        self.type = type  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeApiResponseBodyResultDescriptionsResultDescription, self).to_map()
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
-    def from_map(self, m=None):
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
-    def __init__(self, result_description=None):
-        self.result_description = result_description  # type: list[DescribeApiResponseBodyResultDescriptionsResultDescription]
-
-    def validate(self):
-        if self.result_description:
-            for k in self.result_description:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeApiResponseBodyResultDescriptions, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, event_bridge_region_id=None, event_bus=None, event_source=None, role_arn=None):
+        # The Arn that is authorized by a RAM user to EventBridge.
         self.event_bridge_region_id = event_bridge_region_id  # type: str
+        # The event source.
         self.event_bus = event_bus  # type: str
+        # The ID of the region where the EventBridge instance is located.
         self.event_source = event_source  # type: str
+        # Configuration items of the third-party OpenID Connect authentication method
         self.role_arn = role_arn  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyServiceConfigEventBridgeConfig, self).to_map()
@@ -6728,25 +6971,41 @@
         return self
 
 
 class DescribeApiResponseBodyServiceConfigFunctionComputeConfig(TeaModel):
     def __init__(self, content_type_catagory=None, content_type_value=None, fc_base_url=None, fc_type=None,
                  function_name=None, method=None, only_business_path=None, path=None, qualifier=None, region_id=None,
                  role_arn=None, service_name=None):
+        # The API request path.
         self.content_type_catagory = content_type_catagory  # type: str
+        # The region where the Function Compute instance is located.
         self.content_type_value = content_type_value  # type: str
+        # The value of the ContentType header when the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.fc_base_url = fc_base_url  # type: str
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role to be assumed by API Gateway to access Function Compute.
         self.fc_type = fc_type  # type: str
+        # The ContentType header type used when you call the backend service over HTTP.
+        # 
+        # *   **DEFAULT**: the default header type in API Gateway
+        # *   **CUSTOM**: a custom header type
+        # *   **CLIENT**: the ContentType header type of the client
         self.function_name = function_name  # type: str
+        # The root path of Function Compute.
         self.method = method  # type: str
+        # The function name defined in Function Compute.
         self.only_business_path = only_business_path  # type: bool
+        # The service name defined in Function Compute.
         self.path = path  # type: str
+        # Information when the backend service is OSS
         self.qualifier = qualifier  # type: str
+        # The backend only receives the service path.
         self.region_id = region_id  # type: str
+        # The request method.
         self.role_arn = role_arn  # type: str
+        # The alias of the function.
         self.service_name = service_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyServiceConfigFunctionComputeConfig, self).to_map()
@@ -6807,15 +7066,17 @@
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
         return self
 
 
 class DescribeApiResponseBodyServiceConfigMockHeadersMockHeader(TeaModel):
     def __init__(self, header_name=None, header_value=None):
+        # Configuration items related to VPC channels
         self.header_name = header_name  # type: str
+        # The name of the HTTP header.
         self.header_value = header_value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyServiceConfigMockHeadersMockHeader, self).to_map()
@@ -6869,16 +7130,18 @@
                 self.mock_header.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiResponseBodyServiceConfigOssConfig(TeaModel):
     def __init__(self, action=None, bucket_name=None, key=None, oss_region_id=None):
         self.action = action  # type: str
+        # Configuration items of EventBridge
         self.bucket_name = bucket_name  # type: str
         self.key = key  # type: str
+        # The OSS bucket.
         self.oss_region_id = oss_region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyServiceConfigOssConfig, self).to_map()
@@ -6907,18 +7170,23 @@
         if m.get('OssRegionId') is not None:
             self.oss_region_id = m.get('OssRegionId')
         return self
 
 
 class DescribeApiResponseBodyServiceConfigVpcConfig(TeaModel):
     def __init__(self, instance_id=None, name=None, port=None, vpc_id=None, vpc_scheme=None):
+        # The port number that corresponds to the instance.
         self.instance_id = instance_id  # type: str
+        # Backend configuration items when the backend service is Function Compute
         self.name = name  # type: str
+        # The name of the VPC access authorization.
         self.port = port  # type: int
+        # The VPC protocol.
         self.vpc_id = vpc_id  # type: str
+        # The ID of the ECS or SLB instance in the VPC.
         self.vpc_scheme = vpc_scheme  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyServiceConfigVpcConfig, self).to_map()
@@ -6954,30 +7222,57 @@
 
 
 class DescribeApiResponseBodyServiceConfig(TeaModel):
     def __init__(self, aone_app_name=None, content_type_catagory=None, content_type_value=None,
                  event_bridge_config=None, function_compute_config=None, mock=None, mock_headers=None, mock_result=None,
                  mock_status_code=None, oss_config=None, service_address=None, service_http_method=None, service_path=None,
                  service_protocol=None, service_timeout=None, service_vpc_enable=None, vpc_config=None):
+        # The status code returned for service mocking.
         self.aone_app_name = aone_app_name  # type: str
+        # The URL used to call the back-end service. If the complete back-end service URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the value of **ServiceAddress** is `http://api.a.com:8080`.
         self.content_type_catagory = content_type_catagory  # type: str
+        # The protocol used by the backend service. Valid values: HTTP and HTTPS.
         self.content_type_value = content_type_value  # type: str
+        # The event bus.
         self.event_bridge_config = event_bridge_config  # type: DescribeApiResponseBodyServiceConfigEventBridgeConfig
+        # The type of the Function Compute instance.
         self.function_compute_config = function_compute_config  # type: DescribeApiResponseBodyServiceConfigFunctionComputeConfig
+        # Specifies whether to enable the VPC channel. Valid values:
+        # 
+        # *   **TRUE**: The VPC channel is enabled. You must create the corresponding VPC access authorization before you can enable a VPC channel.
+        # *   **FALSE**: The VPC channel is not enabled.
         self.mock = mock  # type: str
+        # The value of the HTTP header.
         self.mock_headers = mock_headers  # type: DescribeApiResponseBodyServiceConfigMockHeaders
+        # The HTTP method used to call a backend service. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.mock_result = mock_result  # type: str
+        # The value of the ContentType header when the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.mock_status_code = mock_status_code  # type: int
+        # The ID of the region where the OSS instance is located.
         self.oss_config = oss_config  # type: DescribeApiResponseBodyServiceConfigOssConfig
+        # Specifies whether to enable the Mock mode. Valid values:
+        # 
+        # *   **TRUE**: The Mock mode is enabled.
+        # *   **FALSE**: The Mock mode is not enabled.
         self.service_address = service_address  # type: str
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_http_method = service_http_method  # type: str
+        # The ContentType header type used when you call the backend service over HTTP.
+        # 
+        # *   **DEFAULT**: the default header type in API Gateway
+        # *   **CUSTOM**: a custom header type
+        # *   **CLIENT**: the ContentType header type of the client
         self.service_path = service_path  # type: str
+        # The path used to call the back-end service. If the complete back-end service path is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, **ServicePath** is `/object/add`.
         self.service_protocol = service_protocol  # type: str
+        # The simulated headers.
         self.service_timeout = service_timeout  # type: int
+        # The result returned when the Mock mode is enabled.
         self.service_vpc_enable = service_vpc_enable  # type: str
+        # The ID of the VPC.
         self.vpc_config = vpc_config  # type: DescribeApiResponseBodyServiceConfigVpcConfig
 
     def validate(self):
         if self.event_bridge_config:
             self.event_bridge_config.validate()
         if self.function_compute_config:
             self.function_compute_config.validate()
@@ -7072,16 +7367,19 @@
             temp_model = DescribeApiResponseBodyServiceConfigVpcConfig()
             self.vpc_config = temp_model.from_map(m['VpcConfig'])
         return self
 
 
 class DescribeApiResponseBodyServiceParametersServiceParameter(TeaModel):
     def __init__(self, location=None, parameter_type=None, service_parameter_name=None):
+        # The data type of the back-end service parameter.
         self.location = location  # type: str
+        # The name of the backend service parameter.
         self.parameter_type = parameter_type  # type: str
+        # The mappings between parameters of requests sent by the consumer to API Gateway and parameters of requests sent by API Gateway to the backend service.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyServiceParametersServiceParameter, self).to_map()
@@ -7138,15 +7436,17 @@
                 temp_model = DescribeApiResponseBodyServiceParametersServiceParameter()
                 self.service_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiResponseBodyServiceParametersMapServiceParameterMap(TeaModel):
     def __init__(self, request_parameter_name=None, service_parameter_name=None):
+        # The name of the backend service parameter.
         self.request_parameter_name = request_parameter_name  # type: str
+        # The API publishing status.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodyServiceParametersMapServiceParameterMap, self).to_map()
@@ -7200,18 +7500,23 @@
                 self.service_parameter_map.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiResponseBodySystemParametersSystemParameter(TeaModel):
     def __init__(self, demo_value=None, description=None, location=None, parameter_name=None,
                  service_parameter_name=None):
+        # Description
         self.demo_value = demo_value  # type: str
+        # Client IP Address
         self.description = description  # type: str
+        # The name of the corresponding backend parameter.
         self.location = location  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.parameter_name = parameter_name  # type: str
+        # Custom system parameters
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiResponseBodySystemParametersSystemParameter, self).to_map()
@@ -7280,52 +7585,123 @@
 
 class DescribeApiResponseBody(TeaModel):
     def __init__(self, allow_signature_method=None, api_id=None, api_name=None, app_code_auth_type=None,
                  auth_type=None, backend_config=None, backend_enable=None, constant_parameters=None, created_time=None,
                  custom_system_parameters=None, deployed_infos=None, description=None, disable_internet=None, error_code_samples=None,
                  fail_result_sample=None, force_nonce_check=None, group_id=None, group_name=None, mock=None, mock_result=None,
                  modified_time=None, open_id_connect_config=None, region_id=None, request_config=None, request_id=None,
-                 request_parameters=None, result_body_model=None, result_descriptions=None, result_sample=None, result_type=None,
-                 service_config=None, service_parameters=None, service_parameters_map=None, system_parameters=None,
-                 visibility=None, web_socket_api_type=None):
+                 request_parameters=None, result_body_model=None, result_sample=None, result_type=None, service_config=None,
+                 service_parameters=None, service_parameters_map=None, system_parameters=None, visibility=None,
+                 web_socket_api_type=None):
+        # The region ID of the API.
         self.allow_signature_method = allow_signature_method  # type: str
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML.
         self.api_id = api_id  # type: str
+        # Specifies whether to enable backend services.
         self.api_name = api_name  # type: str
+        # If **AuthType** is set to **APP**, this value must be passed to specify the signature algorithm. If you do not specify a value, HmacSHA256 is used by default. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.app_code_auth_type = app_code_auth_type  # type: str
+        # The last modification time of the API.
         self.auth_type = auth_type  # type: str
+        # The ID of the backend service.
         self.backend_config = backend_config  # type: DescribeApiResponseBodyBackendConfig
+        # Backend configurations
         self.backend_enable = backend_enable  # type: bool
+        # Description
         self.constant_parameters = constant_parameters  # type: DescribeApiResponseBodyConstantParameters
+        # The name of the API, which is unique in the group.
         self.created_time = created_time  # type: str
+        # Examples
         self.custom_system_parameters = custom_system_parameters  # type: DescribeApiResponseBodyCustomSystemParameters
+        # The name of the runtime environment. Valid values: RELEASE and TEST.
         self.deployed_infos = deployed_infos  # type: DescribeApiResponseBodyDeployedInfos
+        # The name of the API group.
         self.description = description  # type: str
+        # The returned description of the API.
         self.disable_internet = disable_internet  # type: bool
+        # Error codes
         self.error_code_samples = error_code_samples  # type: DescribeApiResponseBodyErrorCodeSamples
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
         self.fail_result_sample = fail_result_sample  # type: str
+        # Specifies whether to make the API public. Valid values:
+        # 
+        # *   **PUBLIC**: Make the API public. If you set this parameter to PUBLIC, this API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE**: Make the API private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.force_nonce_check = force_nonce_check  # type: bool
+        # Specifies whether to enable the Mock mode. Valid values:
+        # 
+        # *   OPEN: The Mock mode is enabled.
+        # *   CLOSED: The Mock mode is not enabled.
         self.group_id = group_id  # type: str
+        # The ID of the API group.
         self.group_name = group_name  # type: str
+        # The result returned for service mocking.
         self.mock = mock  # type: str
+        # The creation time of the API.
         self.mock_result = mock_result  # type: str
+        # The ID of the request.
         self.modified_time = modified_time  # type: str
+        # The OpenID Connect mode. Valid values:
+        # 
+        # *   **IDTOKEN**: indicates the APIs that are called by clients to obtain tokens. If you specify this value, the PublicKeyId parameter and the PublicKey parameter are required.
+        # *   **BUSINESS**: indicates business APIs. Tokens are used to call the business APIs. If you specify this value, the IdTokenParamName parameter is required.
         self.open_id_connect_config = open_id_connect_config  # type: DescribeApiResponseBodyOpenIdConnectConfig
+        # Specifies whether to carry the header : X-Ca-Nonce when calling an API. This is the unique identifier of the request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent reply attacks. Valid values:
+        # 
+        # *   **true**: This field is forcibly checked when an API is requested to prevent replay attacks.
+        # *   **false**: This field is not checked.
         self.region_id = region_id  # type: str
+        # The body model.
         self.request_config = request_config  # type: DescribeApiResponseBodyRequestConfig
+        # The description of the API.
         self.request_id = request_id  # type: str
+        # The JSON Schema used for JSON validation when **ParameterType** is set to String.
         self.request_parameters = request_parameters  # type: DescribeApiResponseBodyRequestParameters
+        # The sample response from the backend service.
         self.result_body_model = result_body_model  # type: str
-        self.result_descriptions = result_descriptions  # type: DescribeApiResponseBodyResultDescriptions
+        # If **AuthType** is set to **APP**, the valid values are:
+        # 
+        # *   **DEFAULT**: The default value that is used if no other values are passed. This value means that the setting of the group is used.
+        # *   **DISABLE**: The authentication is disabled.
+        # *   **HEADER**: AppCode can be placed in the Header parameter for authentication.
+        # *   **HEADER_QUERY**: AppCode can be placed in the Header or Query parameter for authentication.
         self.result_sample = result_sample  # type: str
+        # The type of the two-way communication API. Valid values:
+        # 
+        # *   **COMMON**: general APIs
+        # *   **REGISTER**: registered APIs
+        # *   **UNREGISTER**: unregistered APIs
+        # *   **NOTIFY**: downstream notification
         self.result_type = result_type  # type: str
+        # The application name in AONE.
         self.service_config = service_config  # type: DescribeApiResponseBodyServiceConfig
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.service_parameters = service_parameters  # type: DescribeApiResponseBodyServiceParameters
+        # The corresponding frontend parameter name. It must be included in RequestParametersObject and matches ApiParameterName in RequestParameter data.
         self.service_parameters_map = service_parameters_map  # type: DescribeApiResponseBodyServiceParametersMap
+        # Examples
         self.system_parameters = system_parameters  # type: DescribeApiResponseBodySystemParameters
+        # The sample error response from the backend service.
         self.visibility = visibility  # type: str
+        # Specifies whether to limit API calls to within the VPC. Valid values:
+        # 
+        # *   **true**: Only API calls from the VPC are supported.
+        # *   **false**: API calls from the VPC and Internet are both supported.
         self.web_socket_api_type = web_socket_api_type  # type: str
 
     def validate(self):
         if self.backend_config:
             self.backend_config.validate()
         if self.constant_parameters:
             self.constant_parameters.validate()
@@ -7337,16 +7713,14 @@
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
@@ -7408,16 +7782,14 @@
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
@@ -7492,17 +7864,14 @@
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
@@ -7725,14 +8094,15 @@
         self.array_items_type = array_items_type  # type: str
         self.default_value = default_value  # type: str
         self.demo_value = demo_value  # type: str
         self.description = description  # type: str
         self.doc_order = doc_order  # type: int
         self.doc_show = doc_show  # type: str
         self.enum_value = enum_value  # type: str
+        # JSON scheme
         self.json_scheme = json_scheme  # type: str
         self.location = location  # type: str
         self.max_length = max_length  # type: long
         self.max_value = max_value  # type: long
         self.min_length = min_length  # type: long
         self.min_value = min_value  # type: long
         self.parameter_type = parameter_type  # type: str
@@ -7851,111 +8221,19 @@
         if m.get('RequestParameter') is not None:
             for k in m.get('RequestParameter'):
                 temp_model = DescribeApiDocResponseBodyRequestParametersRequestParameter()
                 self.request_parameter.append(temp_model.from_map(k))
         return self
 
 
-class DescribeApiDocResponseBodyResultDescriptionsResultDescription(TeaModel):
-    def __init__(self, description=None, has_child=None, id=None, key=None, mandatory=None, name=None, pid=None,
-                 type=None):
-        self.description = description  # type: str
-        self.has_child = has_child  # type: bool
-        self.id = id  # type: str
-        self.key = key  # type: str
-        self.mandatory = mandatory  # type: bool
-        self.name = name  # type: str
-        self.pid = pid  # type: str
-        self.type = type  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeApiDocResponseBodyResultDescriptionsResultDescription, self).to_map()
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
-    def from_map(self, m=None):
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
-    def __init__(self, result_description=None):
-        self.result_description = result_description  # type: list[DescribeApiDocResponseBodyResultDescriptionsResultDescription]
-
-    def validate(self):
-        if self.result_description:
-            for k in self.result_description:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super(DescribeApiDocResponseBodyResultDescriptions, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, api_id=None, api_name=None, auth_type=None, deployed_time=None, description=None,
                  disable_internet=None, error_code_samples=None, fail_result_sample=None, force_nonce_check=None, group_id=None,
                  group_name=None, region_id=None, request_config=None, request_id=None, request_parameters=None,
-                 result_descriptions=None, result_sample=None, result_type=None, stage_name=None, visibility=None):
+                 result_sample=None, result_type=None, stage_name=None, visibility=None):
         self.api_id = api_id  # type: str
         self.api_name = api_name  # type: str
         self.auth_type = auth_type  # type: str
         self.deployed_time = deployed_time  # type: str
         self.description = description  # type: str
         self.disable_internet = disable_internet  # type: bool
         self.error_code_samples = error_code_samples  # type: DescribeApiDocResponseBodyErrorCodeSamples
@@ -7963,29 +8241,26 @@
         self.force_nonce_check = force_nonce_check  # type: bool
         self.group_id = group_id  # type: str
         self.group_name = group_name  # type: str
         self.region_id = region_id  # type: str
         self.request_config = request_config  # type: DescribeApiDocResponseBodyRequestConfig
         self.request_id = request_id  # type: str
         self.request_parameters = request_parameters  # type: DescribeApiDocResponseBodyRequestParameters
-        self.result_descriptions = result_descriptions  # type: DescribeApiDocResponseBodyResultDescriptions
         self.result_sample = result_sample  # type: str
         self.result_type = result_type  # type: str
         self.stage_name = stage_name  # type: str
         self.visibility = visibility  # type: str
 
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
         _map = super(DescribeApiDocResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -8015,16 +8290,14 @@
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
@@ -8062,17 +8335,14 @@
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
@@ -8117,15 +8387,17 @@
             temp_model = DescribeApiDocResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApiGroupRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
+        # The key of the tag.
         self.key = key  # type: str
+        # The value of the tag.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiGroupRequestTag, self).to_map()
@@ -8146,16 +8418,18 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeApiGroupRequest(TeaModel):
     def __init__(self, group_id=None, security_token=None, tag=None):
+        # The ID of the API group. This ID is generated by the system and globally unique.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The object tags that match the lifecycle rule. You can specify multiple tags.
         self.tag = tag  # type: list[DescribeApiGroupRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -8187,30 +8461,53 @@
             for k in m.get('Tag'):
                 temp_model = DescribeApiGroupRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiGroupResponseBodyCustomDomainsDomainItem(TeaModel):
-    def __init__(self, bind_stage_name=None, certificate_id=None, certificate_name=None, custom_domain_type=None,
-                 domain_binding_status=None, domain_cnamestatus=None, domain_legal_status=None, domain_name=None, domain_remark=None,
-                 domain_web_socket_status=None, is_http_redirect_to_https=None, wildcard_domain_patterns=None, wss_enable=None):
+    def __init__(self, bind_stage_name=None, certificate_id=None, certificate_name=None,
+                 certificate_valid_end=None, certificate_valid_start=None, custom_domain_type=None, domain_binding_status=None,
+                 domain_cnamestatus=None, domain_legal_status=None, domain_name=None, domain_remark=None,
+                 domain_web_socket_status=None, is_http_redirect_to_https=None, wildcard_domain_patterns=None):
+        # The name of the bound runtime environment.
         self.bind_stage_name = bind_stage_name  # type: str
+        # The unique ID of the SSL certificate, which is automatically generated by the system.
         self.certificate_id = certificate_id  # type: str
+        # The name of the SSL certificate.
         self.certificate_name = certificate_name  # type: str
+        self.certificate_valid_end = certificate_valid_end  # type: long
+        self.certificate_valid_start = certificate_valid_start  # type: long
+        # The type of the custom domain name.
         self.custom_domain_type = custom_domain_type  # type: str
+        # The binding status of the custom domain name. Valid values:
+        # 
+        # *   **BINDING**: The domain name is bound.
+        # *   **BOUND**: The domain name is not bound.
         self.domain_binding_status = domain_binding_status  # type: str
+        # The domain name resolution status. Valid values:
+        # 
+        # *   **RESOLVED**: The domain name has been resolved.
+        # *   **UNRESOLVED**: The domain name has not been resolved.
         self.domain_cnamestatus = domain_cnamestatus  # type: str
+        # The validity status of the domain name. Valid values:
+        # 
+        # *   **NORMAL**: The domain name is valid.
+        # *   **ABNORMAL**: The domain name is invalid. This status affects API calls and must be resolved as soon as possible.
         self.domain_legal_status = domain_legal_status  # type: str
+        # The domain name.
         self.domain_name = domain_name  # type: str
+        # The domain name-related remarks, such as the cause for a domain name exception.
         self.domain_remark = domain_remark  # type: str
+        # The status of the domain name that uses the WebSocket feature.
         self.domain_web_socket_status = domain_web_socket_status  # type: str
+        # Indicates whether to redirect HTTP requests to HTTPS.
         self.is_http_redirect_to_https = is_http_redirect_to_https  # type: bool
+        # The wildcard domain name mode.
         self.wildcard_domain_patterns = wildcard_domain_patterns  # type: str
-        self.wss_enable = wss_enable  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiGroupResponseBodyCustomDomainsDomainItem, self).to_map()
         if _map is not None:
@@ -8219,14 +8516,18 @@
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
@@ -8237,26 +8538,28 @@
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
 
     def from_map(self, m=None):
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
@@ -8267,16 +8570,14 @@
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
     def __init__(self, domain_item=None):
         self.domain_item = domain_item  # type: list[DescribeApiGroupResponseBodyCustomDomainsDomainItem]
 
@@ -8306,16 +8607,19 @@
                 temp_model = DescribeApiGroupResponseBodyCustomDomainsDomainItem()
                 self.domain_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiGroupResponseBodyStageItemsStageInfo(TeaModel):
     def __init__(self, description=None, stage_id=None, stage_name=None):
+        # The description of the runtime environment.
         self.description = description  # type: str
+        # The ID of the runtime environment.
         self.stage_id = stage_id  # type: str
+        # The name of the runtime environment.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiGroupResponseBodyStageItemsStageInfo, self).to_map()
@@ -8371,52 +8675,94 @@
             for k in m.get('StageInfo'):
                 temp_model = DescribeApiGroupResponseBodyStageItemsStageInfo()
                 self.stage_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiGroupResponseBody(TeaModel):
-    def __init__(self, base_path=None, billing_status=None, classic_vpc_sub_domain=None,
-                 cloud_market_commodity=None, cms_monitor_group=None, compatible_flags=None, created_time=None, custom_domains=None,
-                 custom_trace_config=None, customer_configs=None, default_domain=None, description=None, group_id=None, group_name=None,
-                 https_policy=None, illegal_status=None, instance_id=None, instance_type=None, instance_vip_list=None,
-                 ipv_6status=None, modified_time=None, passthrough_headers=None, region_id=None, request_id=None,
-                 rpc_pattern=None, stage_items=None, status=None, sub_domain=None, traffic_limit=None, user_log_config=None,
-                 vpc_domain=None, vpc_slb_intranet_domain=None):
+    def __init__(self, base_path=None, billing_status=None, cloud_market_commodity=None, cms_monitor_group=None,
+                 compatible_flags=None, created_time=None, custom_domains=None, custom_trace_config=None, customer_configs=None,
+                 dedicated_instance_type=None, default_domain=None, description=None, group_id=None, group_name=None, https_policy=None,
+                 illegal_status=None, instance_id=None, instance_type=None, ipv_6status=None, migration_error=None,
+                 migration_status=None, modified_time=None, passthrough_headers=None, region_id=None, request_id=None,
+                 stage_items=None, status=None, sub_domain=None, traffic_limit=None, user_log_config=None, vpc_domain=None,
+                 vpc_slb_intranet_domain=None):
+        # The root path of the API.
         self.base_path = base_path  # type: str
+        # The billing status of the API group.
+        # 
+        # *   **NORMAL**: The API group is normal.
+        # *   **LOCKED**: The API group is locked due to overdue payments.
         self.billing_status = billing_status  # type: str
-        self.classic_vpc_sub_domain = classic_vpc_sub_domain  # type: str
+        # The products on Alibaba Cloud Marketplace.
         self.cloud_market_commodity = cloud_market_commodity  # type: bool
+        # The CloudMonitor application group.
         self.cms_monitor_group = cms_monitor_group  # type: str
+        # The list of associated tags. Separate multiple tags with commas (,).
         self.compatible_flags = compatible_flags  # type: str
+        # The creation time (UTC) of the API group.
         self.created_time = created_time  # type: str
+        # The custom domain name information.
         self.custom_domains = custom_domains  # type: DescribeApiGroupResponseBodyCustomDomains
+        # The custom trace configuration.
         self.custom_trace_config = custom_trace_config  # type: str
+        # The list of custom configuration items.
         self.customer_configs = customer_configs  # type: str
+        self.dedicated_instance_type = dedicated_instance_type  # type: str
+        # The default domain name.
         self.default_domain = default_domain  # type: str
+        # The description of the API group.
         self.description = description  # type: str
+        # The ID of the API group. This ID is generated by the system and globally unique.
         self.group_id = group_id  # type: str
+        # The name of the group to which the API belongs.
         self.group_name = group_name  # type: str
+        # The HTTPS policy.
         self.https_policy = https_policy  # type: str
+        # The validity status of the API group. Valid values:
+        # 
+        # *   **NORMAL**: The API group is normal.
+        # *   **LOCKED**: The API group is locked because it is not valid.
         self.illegal_status = illegal_status  # type: str
+        # The ID of the instance.
         self.instance_id = instance_id  # type: str
+        # The type of the instance.
+        # 
+        # *   CLASSIC_SHARED: shared instance that uses the classic network configuration
+        # *   VPC_SHARED: shared instance that uses VPC
+        # *   VPC_DEDICATED: dedicated instance that uses VPC
         self.instance_type = instance_type  # type: str
-        self.instance_vip_list = instance_vip_list  # type: str
+        # The IPv6 status.
         self.ipv_6status = ipv_6status  # type: str
+        self.migration_error = migration_error  # type: str
+        self.migration_status = migration_status  # type: str
+        # The last modification time (UTC) of the API group.
         self.modified_time = modified_time  # type: str
+        # Specifies whether to pass headers.
         self.passthrough_headers = passthrough_headers  # type: str
+        # The region to which the API group belongs.
         self.region_id = region_id  # type: str
+        # The ID of the request.
         self.request_id = request_id  # type: str
-        self.rpc_pattern = rpc_pattern  # type: str
+        # The runtime environment information.
         self.stage_items = stage_items  # type: DescribeApiGroupResponseBodyStageItems
+        # The status of the API group.
+        # 
+        # *   **NORMAL**: The API group is normal.
+        # *   **DELETE**: The API group is deleted.
         self.status = status  # type: str
+        # The second-level domain name automatically assigned to the API group.
         self.sub_domain = sub_domain  # type: str
+        # The upper QPS limit of the API group. The default value is 500. You can increase the upper limit by submitting an application.
         self.traffic_limit = traffic_limit  # type: int
+        # The user log settings.
         self.user_log_config = user_log_config  # type: str
+        # The VPC domain name.
         self.vpc_domain = vpc_domain  # type: str
+        # The VPC SLB domain name.
         self.vpc_slb_intranet_domain = vpc_slb_intranet_domain  # type: str
 
     def validate(self):
         if self.custom_domains:
             self.custom_domains.validate()
         if self.stage_items:
             self.stage_items.validate()
@@ -8427,30 +8773,30 @@
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
@@ -8459,28 +8805,28 @@
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
@@ -8495,16 +8841,14 @@
 
     def from_map(self, m=None):
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
@@ -8512,14 +8856,16 @@
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
@@ -8528,28 +8874,28 @@
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
@@ -9078,20 +9424,26 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApiHistoriesRequest(TeaModel):
     def __init__(self, api_id=None, api_name=None, group_id=None, page_number=None, page_size=None,
                  security_token=None, stage_name=None):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_id = api_id  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.api_name = api_name  # type: str
+        # The ID of the API.
         self.group_id = group_id  # type: str
+        # The ID of the request.
         self.page_number = page_number  # type: int
+        # The page number of the returned page.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The name of the API. The name is used for fuzzy match.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoriesRequest, self).to_map()
@@ -9133,23 +9485,36 @@
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeApiHistoriesResponseBodyApiHisItemsApiHisItem(TeaModel):
     def __init__(self, api_id=None, api_name=None, deployed_time=None, description=None, group_id=None,
                  group_name=None, history_version=None, region_id=None, stage_name=None, status=None):
+        # Creates an object
         self.api_id = api_id  # type: str
+        # The region where the API is located.
         self.api_name = api_name  # type: str
+        # The historical version of the API.
         self.deployed_time = deployed_time  # type: str
+        # The name of the group to which an API belongs.
         self.description = description  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST.
         self.group_id = group_id  # type: str
+        # The publishing time (UTC) of the API.
         self.group_name = group_name  # type: str
+        # CreateObject
         self.history_version = history_version  # type: str
+        # Queries the historical versions of a specified API.
         self.region_id = region_id  # type: str
+        # The name of the API.
         self.stage_name = stage_name  # type: str
+        # The description of the API.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoriesResponseBodyApiHisItemsApiHisItem, self).to_map()
@@ -9234,18 +9599,23 @@
                 temp_model = DescribeApiHistoriesResponseBodyApiHisItemsApiHisItem()
                 self.api_his_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoriesResponseBody(TeaModel):
     def __init__(self, api_his_items=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The ID of the API.
         self.api_his_items = api_his_items  # type: DescribeApiHistoriesResponseBodyApiHisItems
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned API information. It is an array consisting of ApiHisItem data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # Indicates whether an API version is effective. Valid values: ONLINE and OFFLINE.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_his_items:
             self.api_his_items.validate()
 
     def to_map(self):
@@ -9319,18 +9689,26 @@
             temp_model = DescribeApiHistoriesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApiHistoryRequest(TeaModel):
     def __init__(self, api_id=None, group_id=None, history_version=None, security_token=None, stage_name=None):
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The ID of the API group to which the API belongs. This ID is generated by the system and globally unique.
         self.group_id = group_id  # type: str
+        # The historical version number of the API.
         self.history_version = history_version  # type: str
         self.security_token = security_token  # type: str
+        # The environment to which the API is published. Valid values:
+        # 
+        # *   **RELEASE**: production environment
+        # *   **TEST**: test environment
+        # *   **PRE**: staging environment
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryRequest, self).to_map()
@@ -9363,16 +9741,19 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeApiHistoryResponseBodyBackendConfig(TeaModel):
     def __init__(self, backend_id=None, backend_name=None, backend_type=None):
+        # The ID of the backend service.
         self.backend_id = backend_id  # type: str
+        # The name of the backend service.
         self.backend_name = backend_name  # type: str
+        # The type of the backend service.
         self.backend_type = backend_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyBackendConfig, self).to_map()
@@ -9397,17 +9778,21 @@
         if m.get('BackendType') is not None:
             self.backend_type = m.get('BackendType')
         return self
 
 
 class DescribeApiHistoryResponseBodyConstantParametersConstantParameter(TeaModel):
     def __init__(self, constant_value=None, description=None, location=None, service_parameter_name=None):
+        # The value of the constant parameter.
         self.constant_value = constant_value  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The name of the backend parameter that corresponds to the constant parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyConstantParametersConstantParameter, self).to_map()
@@ -9469,18 +9854,23 @@
                 self.constant_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodyCustomSystemParametersCustomSystemParameter(TeaModel):
     def __init__(self, demo_value=None, description=None, location=None, parameter_name=None,
                  service_parameter_name=None):
+        # The sample value of the parameter.
         self.demo_value = demo_value  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The name of the parameter.
         self.parameter_name = parameter_name  # type: str
+        # The name of the backend parameter that corresponds to the custom system parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyCustomSystemParametersCustomSystemParameter, self).to_map()
@@ -9545,16 +9935,19 @@
                 temp_model = DescribeApiHistoryResponseBodyCustomSystemParametersCustomSystemParameter()
                 self.custom_system_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodyErrorCodeSamplesErrorCodeSample(TeaModel):
     def __init__(self, code=None, description=None, message=None):
+        # The error code.
         self.code = code  # type: str
+        # The description.
         self.description = description  # type: str
+        # The error message.
         self.message = message  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyErrorCodeSamplesErrorCodeSample, self).to_map()
@@ -9611,17 +10004,22 @@
                 temp_model = DescribeApiHistoryResponseBodyErrorCodeSamplesErrorCodeSample()
                 self.error_code_sample.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodyOpenIdConnectConfig(TeaModel):
     def __init__(self, id_token_param_name=None, open_id_api_type=None, public_key=None, public_key_id=None):
+        # The name of the parameter that corresponds to the token.
         self.id_token_param_name = id_token_param_name  # type: str
+        # *   ****\
+        # *   ****\
         self.open_id_api_type = open_id_api_type  # type: str
+        # The public key of the API.
         self.public_key = public_key  # type: str
+        # The ID of the public key.
         self.public_key_id = public_key_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyOpenIdConnectConfig, self).to_map()
@@ -9651,20 +10049,31 @@
             self.public_key_id = m.get('PublicKeyId')
         return self
 
 
 class DescribeApiHistoryResponseBodyRequestConfig(TeaModel):
     def __init__(self, body_format=None, body_model=None, post_body_description=None, request_http_method=None,
                  request_mode=None, request_path=None, request_protocol=None):
+        # The format in which data was transmitted to the server for a POST or PUT request. Valid values: FORM and STREAM. FORM indicates that data was transmitted as forms that consist of key-value pairs. STREAM indicates that data was transmitted as byte streams. This parameter takes effect when the RequestMode parameter is set to MAPPING.
         self.body_format = body_format  # type: str
+        # The body model.
         self.body_model = body_model  # type: str
+        # The description of the request body.
         self.post_body_description = post_body_description  # type: str
+        # The HTTP request method. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_http_method = request_http_method  # type: str
+        # The request mode of the parameters. Valid values:
+        # 
+        # *   MAPPING: Parameters are mapped. Unknown parameters are filtered out.
+        # *   PASSTHROUGH: Parameters are passed through.
+        # *   MAPPING_PASSTHROUGH: Parameters are mapped. Unknown parameters are passed through.
         self.request_mode = request_mode  # type: str
+        # The request path of the API.
         self.request_path = request_path  # type: str
+        # The type of the protocol that is supported by the API. Valid values: HTTP, HTTPS, and WebSocket. Separate multiple values with commas (,). Example: "HTTP,HTTPS".
         self.request_protocol = request_protocol  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyRequestConfig, self).to_map()
@@ -9708,30 +10117,47 @@
 
 
 class DescribeApiHistoryResponseBodyRequestParametersRequestParameter(TeaModel):
     def __init__(self, api_parameter_name=None, array_items_type=None, default_value=None, demo_value=None,
                  description=None, doc_order=None, doc_show=None, enum_value=None, json_scheme=None, location=None,
                  max_length=None, max_value=None, min_length=None, min_value=None, parameter_type=None,
                  regular_expression=None, required=None):
+        # The name of the parameter in the API request.
         self.api_parameter_name = api_parameter_name  # type: str
+        # The type of the array element.
         self.array_items_type = array_items_type  # type: str
+        # The default value of the parameter.
         self.default_value = default_value  # type: str
+        # The sample value of the parameter.
         self.demo_value = demo_value  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # The order in which the parameter is sorted in the document.
         self.doc_order = doc_order  # type: int
+        # Indicates whether the document is public. Valid values: **PUBLIC** and **PRIVATE**.
         self.doc_show = doc_show  # type: str
+        # The hash values can be specified if the **ParameterType** parameter is set to Int, Long, Float, Double, or String. Separate multiple hash values with commas (,). Examples: 1,2,3,4,9 and A,B,C,E,F.
         self.enum_value = enum_value  # type: str
+        # The JSON scheme.
         self.json_scheme = json_scheme  # type: str
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The maximum length of the parameter value if the **ParameterType** parameter is set to String.
         self.max_length = max_length  # type: long
+        # The maximum value of the parameter if the **ParameterType** parameter is set to Int, Long, Float, or Double.
         self.max_value = max_value  # type: long
+        # The minimum length of the parameter value if the **ParameterType** parameter is set to String.
         self.min_length = min_length  # type: long
+        # The minimum value of the parameter if the **ParameterType** parameter is set to Int, Long, Float, or Double.
         self.min_value = min_value  # type: long
+        # The data type of the parameter. Valid values: String, Int, Long, Float, Double, and Boolean.
         self.parameter_type = parameter_type  # type: str
+        # The regular expression that is used to validate the parameter if the **ParameterType** parameter is set to String.
         self.regular_expression = regular_expression  # type: str
+        # Indicates whether the parameter is required. Valid values: **REQUIRED** and **OPTIONAL**.
         self.required = required  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyRequestParametersRequestParameter, self).to_map()
@@ -9845,21 +10271,29 @@
                 self.request_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodyResultDescriptionsResultDescription(TeaModel):
     def __init__(self, description=None, has_child=None, id=None, key=None, mandatory=None, name=None, pid=None,
                  type=None):
+        # The description.
         self.description = description  # type: str
+        # Indicates whether a subnode exists.
         self.has_child = has_child  # type: bool
+        # The ID of the result.
         self.id = id  # type: str
+        # The primary key of the result.
         self.key = key  # type: str
+        # Indicates whether the parameter is required.
         self.mandatory = mandatory  # type: bool
+        # The name of the result.
         self.name = name  # type: str
+        # The ID of the parent node.
         self.pid = pid  # type: str
+        # The type of the result.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyResultDescriptionsResultDescription, self).to_map()
@@ -9936,17 +10370,21 @@
                 temp_model = DescribeApiHistoryResponseBodyResultDescriptionsResultDescription()
                 self.result_description.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodyServiceConfigEventBridgeConfig(TeaModel):
     def __init__(self, event_bridge_region_id=None, event_bus=None, event_source=None, role_arn=None):
+        # The ID of the region where EventBridge is deployed.
         self.event_bridge_region_id = event_bridge_region_id  # type: str
+        # The event bus.
         self.event_bus = event_bus  # type: str
+        # The event source.
         self.event_source = event_source  # type: str
+        # The ARN of the RAM role that is assigned to EventBridge.
         self.role_arn = role_arn  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyServiceConfigEventBridgeConfig, self).to_map()
@@ -9977,25 +10415,41 @@
         return self
 
 
 class DescribeApiHistoryResponseBodyServiceConfigFunctionComputeConfig(TeaModel):
     def __init__(self, content_type_catagory=None, content_type_value=None, fc_base_url=None, fc_type=None,
                  function_name=None, method=None, only_business_path=None, path=None, qualifier=None, region_id=None,
                  role_arn=None, service_name=None):
+        # The ContentType header that is used if the ServiceProtocol parameter is set to HTTP. Valid values:
+        # 
+        # *   **DEFAULT**: the default header in API Gateway
+        # *   **CUSTOM**: a custom header
+        # *   **CLIENT**: the ContentType header of the client
         self.content_type_catagory = content_type_catagory  # type: str
+        # The value of the ContentType header if the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value  # type: str
+        # The root path of the service in Function Compute.
         self.fc_base_url = fc_base_url  # type: str
+        # The type of the service in Function Compute.
         self.fc_type = fc_type  # type: str
+        # The function name that is defined in Function Compute.
         self.function_name = function_name  # type: str
+        # The request method.
         self.method = method  # type: str
+        # Indicates whether the backend receives only the service path.
         self.only_business_path = only_business_path  # type: bool
+        # The path of the API request.
         self.path = path  # type: str
+        # The alias of the function.
         self.qualifier = qualifier  # type: str
+        # The ID of the region.
         self.region_id = region_id  # type: str
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role that is assumed by API Gateway to access Function Compute.
         self.role_arn = role_arn  # type: str
+        # The service name that is defined in Function Compute.
         self.service_name = service_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyServiceConfigFunctionComputeConfig, self).to_map()
@@ -10056,15 +10510,17 @@
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
         return self
 
 
 class DescribeApiHistoryResponseBodyServiceConfigMockHeadersMockHeader(TeaModel):
     def __init__(self, header_name=None, header_value=None):
+        # The name of the HTTP header
         self.header_name = header_name  # type: str
+        # The value of the HTTP header.
         self.header_value = header_value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyServiceConfigMockHeadersMockHeader, self).to_map()
@@ -10118,16 +10574,18 @@
                 self.mock_header.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodyServiceConfigOssConfig(TeaModel):
     def __init__(self, action=None, bucket_name=None, key=None, oss_region_id=None):
         self.action = action  # type: str
+        # The name of the OSS bucket.
         self.bucket_name = bucket_name  # type: str
         self.key = key  # type: str
+        # The ID of the region where OSS is deployed.
         self.oss_region_id = oss_region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyServiceConfigOssConfig, self).to_map()
@@ -10156,18 +10614,23 @@
         if m.get('OssRegionId') is not None:
             self.oss_region_id = m.get('OssRegionId')
         return self
 
 
 class DescribeApiHistoryResponseBodyServiceConfigVpcConfig(TeaModel):
     def __init__(self, instance_id=None, name=None, port=None, vpc_id=None, vpc_scheme=None):
+        # The ID of the Elastic Compute Service (ECS) or Server Load Balancer (SLB) instance in the VPC.
         self.instance_id = instance_id  # type: str
+        # The name of the VPC.
         self.name = name  # type: str
+        # The port number that corresponds to the instance.
         self.port = port  # type: int
+        # The ID of the VPC.
         self.vpc_id = vpc_id  # type: str
+        # The protocol of the VPC.
         self.vpc_scheme = vpc_scheme  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyServiceConfigVpcConfig, self).to_map()
@@ -10203,30 +10666,59 @@
 
 
 class DescribeApiHistoryResponseBodyServiceConfig(TeaModel):
     def __init__(self, content_type_catagory=None, content_type_value=None, event_bridge_config=None,
                  function_compute_config=None, mock=None, mock_headers=None, mock_result=None, mock_status_code=None, oss_config=None,
                  service_address=None, service_http_method=None, service_path=None, service_protocol=None, service_timeout=None,
                  service_vpc_enable=None, vpc_config=None, vpc_id=None):
+        # The ContentType header that is used if the ServiceProtocol parameter is set to HTTP. Valid values:
+        # 
+        # *   DEFAULT: the default header in API Gateway
+        # *   CUSTOM: a custom header
+        # *   CLIENT: the ContentType header of the client
         self.content_type_catagory = content_type_catagory  # type: str
+        # The value of the ContentType header if the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value  # type: str
+        # The configuration items of EventBridge.
         self.event_bridge_config = event_bridge_config  # type: DescribeApiHistoryResponseBodyServiceConfigEventBridgeConfig
+        # The configuration items of the backend service whose type is Function Compute.
         self.function_compute_config = function_compute_config  # type: DescribeApiHistoryResponseBodyServiceConfigFunctionComputeConfig
+        # Indicates whether the mock mode is enabled. Valid values:
+        # 
+        # *   TRUE
+        # *   FALSE
         self.mock = mock  # type: str
+        # The mock headers.
         self.mock_headers = mock_headers  # type: DescribeApiHistoryResponseBodyServiceConfigMockHeaders
+        # The result that is returned if the Mock parameter is set to TRUE.
         self.mock_result = mock_result  # type: str
+        # The status code that is returned for service mocking.
         self.mock_status_code = mock_status_code  # type: int
+        # The configuration items of the backend service whose type is Object Storage Service (OSS).
         self.oss_config = oss_config  # type: DescribeApiHistoryResponseBodyServiceConfigOssConfig
+        # The URL that is used to call the backend service.
         self.service_address = service_address  # type: str
+        # The HTTP request method that is used if the ServiceProtocol parameter is set to HTTP. Valid values: PUT, GET, POST, DELETE, PATCH, HEAD, OPTIONS, and ANY.
         self.service_http_method = service_http_method  # type: str
+        # The path that is used when the backend service is called.
         self.service_path = service_path  # type: str
+        # The protocol of the backend service. Only HTTP, HTTPS, and Function Compute are supported.
         self.service_protocol = service_protocol  # type: str
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_timeout = service_timeout  # type: int
+        # Indicates whether the VPC channel is enabled. Valid values:
+        # 
+        # *   TRUE
+        # *   FALSE
+        # 
+        # Before you can enable the VPC channel, make sure that a VPC authorization is added.
         self.service_vpc_enable = service_vpc_enable  # type: str
+        # The configuration items of the VPC channel.
         self.vpc_config = vpc_config  # type: DescribeApiHistoryResponseBodyServiceConfigVpcConfig
+        # The ID of the virtual private cloud (VPC).
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         if self.event_bridge_config:
             self.event_bridge_config.validate()
         if self.function_compute_config:
             self.function_compute_config.validate()
@@ -10321,16 +10813,19 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeApiHistoryResponseBodyServiceParametersServiceParameter(TeaModel):
     def __init__(self, location=None, parameter_type=None, service_parameter_name=None):
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The data type of the parameter. Valid values: STRING, NUMBER, and BOOLEAN.
         self.parameter_type = parameter_type  # type: str
+        # The name of the backend parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyServiceParametersServiceParameter, self).to_map()
@@ -10387,15 +10882,17 @@
                 temp_model = DescribeApiHistoryResponseBodyServiceParametersServiceParameter()
                 self.service_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodyServiceParametersMapServiceParameterMap(TeaModel):
     def __init__(self, request_parameter_name=None, service_parameter_name=None):
+        # The name of the frontend parameter. The name must be included in RequestParametersObject and match ApiParameterName in RequestParameters.
         self.request_parameter_name = request_parameter_name  # type: str
+        # The name of the backend parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodyServiceParametersMapServiceParameterMap, self).to_map()
@@ -10449,18 +10946,23 @@
                 self.service_parameter_map.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiHistoryResponseBodySystemParametersSystemParameter(TeaModel):
     def __init__(self, demo_value=None, description=None, location=None, parameter_name=None,
                  service_parameter_name=None):
+        # The sample value of the parameter.
         self.demo_value = demo_value  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # The location of the parameter. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The name of the parameter. Valid values: CaClientIp, CaDomain, CaRequestHandleTime, CaAppId, CaRequestId, CaHttpSchema, and CaProxy.
         self.parameter_name = parameter_name  # type: str
+        # The name of the backend parameter that corresponds to the system parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiHistoryResponseBodySystemParametersSystemParameter, self).to_map()
@@ -10532,48 +11034,120 @@
                  auth_type=None, backend_config=None, backend_enable=None, constant_parameters=None,
                  custom_system_parameters=None, deployed_time=None, description=None, disable_internet=None, error_code_samples=None,
                  fail_result_sample=None, force_nonce_check=None, group_id=None, group_name=None, history_version=None,
                  open_id_connect_config=None, region_id=None, request_config=None, request_id=None, request_parameters=None,
                  result_body_model=None, result_descriptions=None, result_sample=None, result_type=None, service_config=None,
                  service_parameters=None, service_parameters_map=None, stage_name=None, status=None, system_parameters=None,
                  visibility=None, web_socket_api_type=None):
+        # The signature algorithm that is used if the **AuthType** parameter is set to **APP**. If no value is specified for the AllowSignatureMethod parameter, the default value HmacSHA256 is used. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method  # type: str
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The name of the API.
         self.api_name = api_name  # type: str
+        # The type of AppCode authentication. Default value: DEFAULT. Valid values:
+        # 
+        # *   DEFAULT: AppCode authentication is supported after the API is published in Alibaba Cloud Marketplace.
+        # *   DISABLE: AppCode authentication is not supported.
+        # *   HEADER: AppCode authentication is supported only in Header parameters.
+        # *   HEADER_QUERY: AppCode authentication is supported in Header or Query parameters.
         self.app_code_auth_type = app_code_auth_type  # type: str
+        # The type of the security authentication that is used for the API. Valid values:
+        # 
+        # *   **APP**: The API can be called only by authorized applications.
+        # 
+        # *   **ANONYMOUS**: The API can be anonymously called. Take note of the following information:
+        # 
+        #     *   All users who have obtained the API service information can call this API. API Gateway neither authenticates callers nor sets user-specific throttling policies. If this API is a public one, you must set throttling policies for it.
         self.auth_type = auth_type  # type: str
+        # The configuration items of the backend service.
         self.backend_config = backend_config  # type: DescribeApiHistoryResponseBodyBackendConfig
+        # Indicates whether the backend service is enabled.
         self.backend_enable = backend_enable  # type: bool
+        # The constant parameters.
         self.constant_parameters = constant_parameters  # type: DescribeApiHistoryResponseBodyConstantParameters
+        # The custom system parameters.
         self.custom_system_parameters = custom_system_parameters  # type: DescribeApiHistoryResponseBodyCustomSystemParameters
+        # The time when the API was published. The time is displayed in UTC.
         self.deployed_time = deployed_time  # type: str
+        # The description of the API.
         self.description = description  # type: str
+        # *   If the **DisableInternet** parameter is set to **true**, you call the API only over internal networks.
+        # *   If the **DisableInternet** parameter is set to **false**, no limit is imposed on networks. When you create an API, the default value of this parameter is false.
         self.disable_internet = disable_internet  # type: bool
+        # The sample error codes that are returned from the backend service.
+        # 
+        # For more information, see [ErrorCodeSample](~~44392~~).
         self.error_code_samples = error_code_samples  # type: DescribeApiHistoryResponseBodyErrorCodeSamples
+        # The sample error response that is returned from the backend service.
         self.fail_result_sample = fail_result_sample  # type: str
+        # *   Indicates whether to forcefully check X-Ca-Nonce. X-Ca-Nonce is the unique identifier of a request and is generally identified by UUID. If the **ForceNonceCheck** parameter is set to **true**, X-Ca-Nonce is forcefully checked. After API Gateway receives this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps defend against replay attacks.
+        # *   If the **ForceNonceCheck** parameter is set to **false**, X-Ca-Nonce is not checked. When you create an API, the default value of this parameter is false.
         self.force_nonce_check = force_nonce_check  # type: bool
+        # The ID of the API group.
         self.group_id = group_id  # type: str
+        # The name of the API group.
         self.group_name = group_name  # type: str
+        # The historical version number of the API.
         self.history_version = history_version  # type: str
+        # The configuration items of third-party OpenID Connect authentication.
         self.open_id_connect_config = open_id_connect_config  # type: DescribeApiHistoryResponseBodyOpenIdConnectConfig
+        # The ID of the region where the API is deployed.
         self.region_id = region_id  # type: str
+        # The configuration items of API requests that are sent from the consumer to API Gateway.
+        # 
+        # For more information, see [RequestConfig](~~43985~~).
         self.request_config = request_config  # type: DescribeApiHistoryResponseBodyRequestConfig
+        # The ID of the request.
         self.request_id = request_id  # type: str
+        # The parameters of API requests that are sent from the consumer to API Gateway.
+        # 
+        # For more information, see [RequestParameter](~~43986~~).
         self.request_parameters = request_parameters  # type: DescribeApiHistoryResponseBodyRequestParameters
+        # The response of the API.
         self.result_body_model = result_body_model  # type: str
+        # The descriptions that are returned for the API.
         self.result_descriptions = result_descriptions  # type: DescribeApiHistoryResponseBodyResultDescriptions
+        # The sample response.
         self.result_sample = result_sample  # type: str
+        # The type of data that is returned.
         self.result_type = result_type  # type: str
+        # The information about backend service calls.
         self.service_config = service_config  # type: DescribeApiHistoryResponseBodyServiceConfig
+        # The parameters of API requests that are sent from API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameter](~~43988~~).
         self.service_parameters = service_parameters  # type: DescribeApiHistoryResponseBodyServiceParameters
+        # The mappings between the parameters of requests sent from the consumer to API Gateway and the parameters of requests sent from API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameterMap](~~43989~~).
         self.service_parameters_map = service_parameters_map  # type: DescribeApiHistoryResponseBodyServiceParametersMap
+        # The environment to which the API is published. Valid values:
+        # 
+        # *   **RELEASE**: production environment
+        # *   **PRE**: staging environment
+        # *   **TEST**: test environment
         self.stage_name = stage_name  # type: str
         self.status = status  # type: str
+        # The system parameters of the API in the JSON format.
         self.system_parameters = system_parameters  # type: DescribeApiHistoryResponseBodySystemParameters
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**: The API is public. If you publish the definition of a public API to the production environment, the definition is displayed on the APIs page for all users.
+        # *   **PRIVATE**: The API is private. If you publish an API group that contains a private API in Alibaba Cloud Marketplace, the API is not displayed in Alibaba Cloud Marketplace.
         self.visibility = visibility  # type: str
+        # The type of the API that is used in bidirectional communication. Valid values:
+        # 
+        # *   **COMMON**: common API
+        # *   **REGISTER**: registered API
+        # *   **UNREGISTER**: unregistered API
+        # *   **NOTIFY**: downstream notification API
         self.web_socket_api_type = web_socket_api_type  # type: str
 
     def validate(self):
         if self.backend_config:
             self.backend_config.validate()
         if self.constant_parameters:
             self.constant_parameters.validate()
@@ -10801,19 +11375,24 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApiIpControlsRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, page_number=None, page_size=None, security_token=None,
                  stage_name=None):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_ids = api_ids  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.group_id = group_id  # type: str
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the request.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The IDs of APIs. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiIpControlsRequest, self).to_map()
@@ -10850,18 +11429,26 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeApiIpControlsResponseBodyApiIpControlsApiIpControlItem(TeaModel):
     def __init__(self, api_id=None, api_name=None, bound_time=None, ip_control_id=None, ip_control_name=None):
+        # The name of the ACL.
         self.api_id = api_id  # type: str
+        # Queries the access control lists (ACLs) that are bound to all the APIs in an API group in a specified environment.
         self.api_name = api_name  # type: str
+        # The ID of the ACL.
         self.bound_time = bound_time  # type: str
+        # The name of the API.
         self.ip_control_id = ip_control_id  # type: str
+        # *   This operation is intended for API callers.
+        # *   If an optional parameter is not specified, all results are returned on separate pages.
+        # 
+        # ·
         self.ip_control_name = ip_control_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiIpControlsResponseBodyApiIpControlsApiIpControlItem, self).to_map()
@@ -10926,18 +11513,23 @@
                 temp_model = DescribeApiIpControlsResponseBodyApiIpControlsApiIpControlItem()
                 self.api_ip_control_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiIpControlsResponseBody(TeaModel):
     def __init__(self, api_ip_controls=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The ID of the API.
         self.api_ip_controls = api_ip_controls  # type: DescribeApiIpControlsResponseBodyApiIpControls
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The information about the ACLs. The information is an array of ApiIpControlItem data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The time of binding.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_ip_controls:
             self.api_ip_controls.validate()
 
     def to_map(self):
@@ -11555,19 +12147,24 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApiSignaturesRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, page_number=None, page_size=None, security_token=None,
                  stage_name=None):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_ids = api_ids  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.group_id = group_id  # type: str
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the request.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The IDs of the APIs that you want to query. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiSignaturesRequest, self).to_map()
@@ -11604,18 +12201,24 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeApiSignaturesResponseBodyApiSignaturesApiSignatureItem(TeaModel):
     def __init__(self, api_id=None, api_name=None, bound_time=None, signature_id=None, signature_name=None):
+        # The name of the backend signature key.
         self.api_id = api_id  # type: str
+        # Queries the backend signature keys that are bound to the APIs of a specified API group in a specified environment.
         self.api_name = api_name  # type: str
+        # The ID of the backend signature key.
         self.bound_time = bound_time  # type: str
+        # The name of the API.
         self.signature_id = signature_id  # type: str
+        # *   This API is intended for API providers.
+        # *   The ApiIds parameter is optional. If this parameter is not specified, all results in the specified environment of an API group are returned.
         self.signature_name = signature_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiSignaturesResponseBodyApiSignaturesApiSignatureItem, self).to_map()
@@ -11680,18 +12283,23 @@
                 temp_model = DescribeApiSignaturesResponseBodyApiSignaturesApiSignatureItem()
                 self.api_signature_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiSignaturesResponseBody(TeaModel):
     def __init__(self, api_signatures=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The ID of the API.
         self.api_signatures = api_signatures  # type: DescribeApiSignaturesResponseBodyApiSignatures
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned signature key information. It is an array consisting of ApiSignatureItem data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The time when the backend signature key was bound.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_signatures:
             self.api_signatures.validate()
 
     def to_map(self):
@@ -11766,19 +12374,24 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApiTrafficControlsRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, page_number=None, page_size=None, security_token=None,
                  stage_name=None):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.api_ids = api_ids  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.group_id = group_id  # type: str
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the request.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The IDs of APIs that you want to query. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiTrafficControlsRequest, self).to_map()
@@ -11816,18 +12429,24 @@
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeApiTrafficControlsResponseBodyApiTrafficControlsApiTrafficControlItem(TeaModel):
     def __init__(self, api_id=None, api_name=None, bound_time=None, traffic_control_id=None,
                  traffic_control_name=None):
+        # The name of the throttling policy.
         self.api_id = api_id  # type: str
+        # Queries the throttling policies bound to all members of an API group in a specified environment.
         self.api_name = api_name  # type: str
+        # The ID of the throttling policy.
         self.bound_time = bound_time  # type: str
+        # API operation
         self.traffic_control_id = traffic_control_id  # type: str
+        # *   This API is intended for API providers.
+        # *   The ApiIds parameter is optional. If this parameter is not specified, all results in the specified environment of an API group are returned.
         self.traffic_control_name = traffic_control_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiTrafficControlsResponseBodyApiTrafficControlsApiTrafficControlItem, self).to_map()
@@ -11893,18 +12512,23 @@
                 self.api_traffic_control_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiTrafficControlsResponseBody(TeaModel):
     def __init__(self, api_traffic_controls=None, page_number=None, page_size=None, request_id=None,
                  total_count=None):
+        # The ID of the API.
         self.api_traffic_controls = api_traffic_controls  # type: DescribeApiTrafficControlsResponseBodyApiTrafficControls
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned throttling policy information. It is an array consisting of ApiTrafficControlItem data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The binding time of the throttling policy.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_traffic_controls:
             self.api_traffic_controls.validate()
 
     def to_map(self):
@@ -12228,15 +12852,17 @@
             temp_model = DescribeApiTrafficDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApisRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
+        # The tag key.
         self.key = key  # type: str
+        # The tag value.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApisRequestTag, self).to_map()
@@ -12257,28 +12883,44 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeApisRequest(TeaModel):
     def __init__(self, api_id=None, api_method=None, api_name=None, api_path=None, catalog_id=None,
-                 enable_tag_auth=None, group_id=None, page_number=None, page_size=None, security_token=None, tag=None,
-                 un_deployed=None, visibility=None):
+                 enable_tag_auth=None, group_id=None, page_number=None, page_size=None, security_token=None, stage_name=None,
+                 tag=None, un_deployed=None, visibility=None):
+        # The API ID.
         self.api_id = api_id  # type: str
+        # The HTTP method of the API request.
         self.api_method = api_method  # type: str
+        # The API name. The name is used for fuzzy match.
         self.api_name = api_name  # type: str
+        # The request path of the API.
         self.api_path = api_path  # type: str
+        # The category ID.
         self.catalog_id = catalog_id  # type: str
+        # Specifies whether to enable tag verification.
         self.enable_tag_auth = enable_tag_auth  # type: bool
+        # The API group ID.
         self.group_id = group_id  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.page_number = page_number  # type: int
+        # The number of entries to return on each page. Default value: 10.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        self.stage_name = stage_name  # type: str
+        # The tags of objects that match the rule.
         self.tag = tag  # type: list[DescribeApisRequestTag]
+        # Specifies whether to filter unpublished APIs.
         self.un_deployed = un_deployed  # type: bool
+        # Specifies whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**: The API is public. If you publish the definition of a public API to the production environment, the definition is displayed on the APIs page for all users.
+        # *   **PRIVATE**: The API is private. If you publish an API group that contains a private API in Alibaba Cloud Marketplace, the API is not displayed in Alibaba Cloud Marketplace.
         self.visibility = visibility  # type: str
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -12305,14 +12947,16 @@
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
@@ -12337,43 +12981,203 @@
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
+    def __init__(self, deployed_status=None, effective_version=None, stage_name=None):
+        # The deployment status. Valid values: DEPLOYED and NONDEPLOYED.
+        self.deployed_status = deployed_status  # type: str
+        # The deployed version.
+        self.effective_version = effective_version  # type: str
+        # Stage Name:
+        # 
+        # *   **RELEASE**: production environment
+        # *   **PRE**: staging environment
+        # *   **TEST**: test environment
+        self.stage_name = stage_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfosDeployedInfo, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, deployed_info=None):
+        self.deployed_info = deployed_info  # type: list[DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfosDeployedInfo]
+
+    def validate(self):
+        if self.deployed_info:
+            for k in self.deployed_info:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfos, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, tag_key=None, tag_value=None):
+        # The tag key.
+        self.tag_key = tag_key  # type: str
+        # The tag value.
+        self.tag_value = tag_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeApisResponseBodyApiSummarysApiSummaryTagListTag, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
+class DescribeApisResponseBodyApiSummarysApiSummaryTagList(TeaModel):
+    def __init__(self, tag=None):
+        self.tag = tag  # type: list[DescribeApisResponseBodyApiSummarysApiSummaryTagListTag]
+
+    def validate(self):
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeApisResponseBodyApiSummarysApiSummaryTagList, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, api_id=None, api_method=None, api_name=None, api_path=None, created_time=None,
-                 description=None, group_id=None, group_name=None, modified_time=None, region_id=None, visibility=None):
+                 deployed_infos=None, description=None, group_id=None, group_name=None, modified_time=None, region_id=None,
+                 tag_list=None, visibility=None):
+        # The API ID.
         self.api_id = api_id  # type: str
+        # The HTTP method of the API request.
         self.api_method = api_method  # type: str
+        # The API name.
         self.api_name = api_name  # type: str
+        # The request path of the API.
         self.api_path = api_path  # type: str
+        # The time when the API was created. The time is displayed in UTC.
         self.created_time = created_time  # type: str
+        # The API publishing statuses.
+        self.deployed_infos = deployed_infos  # type: DescribeApisResponseBodyApiSummarysApiSummaryDeployedInfos
+        # The API description.
         self.description = description  # type: str
+        # The API group ID.
         self.group_id = group_id  # type: str
+        # The name of the API group to which the API belongs.
         self.group_name = group_name  # type: str
+        # The time when the API was modified. The time is displayed in UTC.
         self.modified_time = modified_time  # type: str
+        # The ID of the region to which the API belongs.
         self.region_id = region_id  # type: str
+        # The tags that are added to the APIs.
+        self.tag_list = tag_list  # type: DescribeApisResponseBodyApiSummarysApiSummaryTagList
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**: The API is public.
+        # *   **PRIVATE**: The API is private.
         self.visibility = visibility  # type: str
 
     def validate(self):
-        pass
+        if self.deployed_infos:
+            self.deployed_infos.validate()
+        if self.tag_list:
+            self.tag_list.validate()
 
     def to_map(self):
         _map = super(DescribeApisResponseBodyApiSummarysApiSummary, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -12383,24 +13187,28 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ApiId') is not None:
@@ -12409,24 +13217,30 @@
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
     def __init__(self, api_summary=None):
@@ -12458,18 +13272,23 @@
                 temp_model = DescribeApisResponseBodyApiSummarysApiSummary()
                 self.api_summary.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApisResponseBody(TeaModel):
     def __init__(self, api_summarys=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The queried API definitions.
         self.api_summarys = api_summarys  # type: DescribeApisResponseBodyApiSummarys
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The number of entries returned per page.
         self.page_size = page_size  # type: int
+        # The request ID.
         self.request_id = request_id  # type: str
+        # The total number of returned entries.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_summarys:
             self.api_summarys.validate()
 
     def to_map(self):
@@ -13028,16 +13847,19 @@
             temp_model = DescribeApisByBackendResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApisByIpControlRequest(TeaModel):
     def __init__(self, ip_control_id=None, page_number=None, page_size=None, security_token=None):
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.ip_control_id = ip_control_id  # type: str
+        # The ID of the request.
         self.page_number = page_number  # type: int
+        # The page number of the returned page.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -13068,22 +13890,35 @@
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeApisByIpControlResponseBodyApiInfosApiInfo(TeaModel):
     def __init__(self, api_id=None, api_name=None, bound_time=None, description=None, group_id=None, group_name=None,
                  region_id=None, stage_name=None, visibility=None):
+        # Description
         self.api_id = api_id  # type: str
+        # *   This API is intended for API providers.
+        # *   You can specify PageNumber to obtain the result on the specified page.
         self.api_name = api_name  # type: str
+        # The ID of the API.
         self.bound_time = bound_time  # type: str
+        # The name of the API group.
         self.description = description  # type: str
+        # The API operation.
         self.group_id = group_id  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_name = group_name  # type: str
+        # Queries the APIs that are bound to an access control list (ACL).
         self.region_id = region_id  # type: str
+        # The region where the API is located.
         self.stage_name = stage_name  # type: str
+        # The description of the API.
         self.visibility = visibility  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApisByIpControlResponseBodyApiInfosApiInfo, self).to_map()
@@ -13164,18 +13999,26 @@
                 temp_model = DescribeApisByIpControlResponseBodyApiInfosApiInfo()
                 self.api_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApisByIpControlResponseBody(TeaModel):
     def __init__(self, api_infos=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**\
+        # *   **PRIVATE**\
         self.api_infos = api_infos  # type: DescribeApisByIpControlResponseBodyApiInfos
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned API information. It is an array consisting of ApiInfo data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The binding time of the API.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_infos:
             self.api_infos.validate()
 
     def to_map(self):
@@ -13249,17 +14092,20 @@
             temp_model = DescribeApisByIpControlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApisBySignatureRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, security_token=None, signature_id=None):
+        # The ID of the request.
         self.page_number = page_number  # type: int
+        # The page number of the returned page.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.signature_id = signature_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApisBySignatureRequest, self).to_map()
@@ -13289,22 +14135,35 @@
             self.signature_id = m.get('SignatureId')
         return self
 
 
 class DescribeApisBySignatureResponseBodyApiInfosApiInfo(TeaModel):
     def __init__(self, api_id=None, api_name=None, bound_time=None, description=None, group_id=None, group_name=None,
                  region_id=None, stage_name=None, visibility=None):
+        # Description
         self.api_id = api_id  # type: str
+        # *   This API is intended for API providers.
+        # *   The results are returned on separate pages. You can specify PageNumber to obtain the result on the specified page.
         self.api_name = api_name  # type: str
+        # The ID of the API.
         self.bound_time = bound_time  # type: str
+        # The name of the group to which the API belongs.
         self.description = description  # type: str
+        # The name of the API.
         self.group_id = group_id  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_name = group_name  # type: str
+        # Queries the APIs to which a specified backend signature key is bound.
         self.region_id = region_id  # type: str
+        # The region where the API is located.
         self.stage_name = stage_name  # type: str
+        # The description of the API.
         self.visibility = visibility  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApisBySignatureResponseBodyApiInfosApiInfo, self).to_map()
@@ -13385,18 +14244,26 @@
                 temp_model = DescribeApisBySignatureResponseBodyApiInfosApiInfo()
                 self.api_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApisBySignatureResponseBody(TeaModel):
     def __init__(self, api_infos=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**\
+        # *   **PRIVATE**\
         self.api_infos = api_infos  # type: DescribeApisBySignatureResponseBodyApiInfos
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned API information. It is an array consisting of ApiInfo data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The binding time of the API.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_infos:
             self.api_infos.validate()
 
     def to_map(self):
@@ -13470,17 +14337,20 @@
             temp_model = DescribeApisBySignatureResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeApisByTrafficControlRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, security_token=None, traffic_control_id=None):
+        # The ID of the request.
         self.page_number = page_number  # type: int
+        # The page number of the returned page.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.traffic_control_id = traffic_control_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApisByTrafficControlRequest, self).to_map()
@@ -13510,22 +14380,35 @@
             self.traffic_control_id = m.get('TrafficControlId')
         return self
 
 
 class DescribeApisByTrafficControlResponseBodyApiInfosApiInfo(TeaModel):
     def __init__(self, api_id=None, api_name=None, bound_time=None, description=None, group_id=None, group_name=None,
                  region_id=None, stage_name=None, visibility=None):
+        # Description
         self.api_id = api_id  # type: str
+        # *   This API is intended for API providers.
+        # *   You can specify PageNumber to obtain the result on the specified page.
         self.api_name = api_name  # type: str
+        # The ID of the API.
         self.bound_time = bound_time  # type: str
+        # The name of the group to which an API belongs.
         self.description = description  # type: str
+        # The name of the API
         self.group_id = group_id  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_name = group_name  # type: str
+        # Queries the APIs to which a specified throttling policy is bound.
         self.region_id = region_id  # type: str
+        # The region where the API is located.
         self.stage_name = stage_name  # type: str
+        # The description of the API.
         self.visibility = visibility  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApisByTrafficControlResponseBodyApiInfosApiInfo, self).to_map()
@@ -13606,18 +14489,26 @@
                 temp_model = DescribeApisByTrafficControlResponseBodyApiInfosApiInfo()
                 self.api_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApisByTrafficControlResponseBody(TeaModel):
     def __init__(self, api_infos=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC**\
+        # *   **PRIVATE**\
         self.api_infos = api_infos  # type: DescribeApisByTrafficControlResponseBodyApiInfos
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned API information. It is an array consisting of ApiInfo data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The binding time of the API.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.api_infos:
             self.api_infos.validate()
 
     def to_map(self):
@@ -13719,20 +14610,21 @@
             self.app_id = m.get('AppId')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeAppResponseBody(TeaModel):
-    def __init__(self, app_id=None, app_name=None, created_time=None, description=None, modified_time=None,
-                 request_id=None):
+    def __init__(self, app_id=None, app_name=None, created_time=None, description=None, extend=None,
+                 modified_time=None, request_id=None):
         self.app_id = app_id  # type: long
         self.app_name = app_name  # type: str
         self.created_time = created_time  # type: str
         self.description = description  # type: str
+        self.extend = extend  # type: str
         self.modified_time = modified_time  # type: str
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -13745,14 +14637,16 @@
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
 
     def from_map(self, m=None):
@@ -13761,14 +14655,16 @@
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
 
 
@@ -13837,21 +14733,22 @@
             self.key = m.get('Key')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class DescribeAppAttributesRequest(TeaModel):
-    def __init__(self, app_code=None, app_id=None, app_key=None, app_name=None, enable_tag_auth=None,
+    def __init__(self, app_code=None, app_id=None, app_key=None, app_name=None, enable_tag_auth=None, extend=None,
                  page_number=None, page_size=None, security_token=None, sort=None, tag=None):
         self.app_code = app_code  # type: str
         self.app_id = app_id  # type: long
         self.app_key = app_key  # type: str
         self.app_name = app_name  # type: str
         self.enable_tag_auth = enable_tag_auth  # type: bool
+        self.extend = extend  # type: str
         self.page_number = page_number  # type: int
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
         self.sort = sort  # type: str
         self.tag = tag  # type: list[DescribeAppAttributesRequestTag]
 
     def validate(self):
@@ -13872,14 +14769,16 @@
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
@@ -13898,14 +14797,16 @@
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
@@ -13976,20 +14877,21 @@
             for k in m.get('TagInfo'):
                 temp_model = DescribeAppAttributesResponseBodyAppsAppAttributeTagsTagInfo()
                 self.tag_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeAppAttributesResponseBodyAppsAppAttribute(TeaModel):
-    def __init__(self, app_id=None, app_name=None, created_time=None, description=None, modified_time=None,
-                 tags=None):
+    def __init__(self, app_id=None, app_name=None, created_time=None, description=None, extend=None,
+                 modified_time=None, tags=None):
         self.app_id = app_id  # type: long
         self.app_name = app_name  # type: str
         self.created_time = created_time  # type: str
         self.description = description  # type: str
+        self.extend = extend  # type: str
         self.modified_time = modified_time  # type: str
         self.tags = tags  # type: DescribeAppAttributesResponseBodyAppsAppAttributeTags
 
     def validate(self):
         if self.tags:
             self.tags.validate()
 
@@ -14003,14 +14905,16 @@
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
 
     def from_map(self, m=None):
@@ -14019,14 +14923,16 @@
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
 
@@ -14306,17 +15212,21 @@
             temp_model = DescribeAppSecurityResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAppsRequest(TeaModel):
     def __init__(self, app_id=None, app_owner=None, page_number=None, page_size=None, security_token=None):
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.app_id = app_id  # type: long
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.app_owner = app_owner  # type: long
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the request.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -14350,16 +15260,21 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeAppsResponseBodyAppsAppItem(TeaModel):
     def __init__(self, app_id=None, app_name=None, description=None):
+        # Queries the apps. App information is returned only to the app owner.
         self.app_id = app_id  # type: long
+        # The ID of the app.
         self.app_name = app_name  # type: str
+        # *   This API is intended for API providers.
+        # *   API providers can use the app IDs or their Apsara Stack tenant accounts to query app information.
+        # *   Each provider can call this operation for a maximum of 200 times every day in a region.
         self.description = description  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAppsResponseBodyAppsAppItem, self).to_map()
@@ -14416,18 +15331,23 @@
                 temp_model = DescribeAppsResponseBodyAppsAppItem()
                 self.app_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeAppsResponseBody(TeaModel):
     def __init__(self, apps=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The description of the app.
         self.apps = apps  # type: DescribeAppsResponseBodyApps
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned app information. It is an array consisting of AppItem data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The name of the app.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.apps:
             self.apps.validate()
 
     def to_map(self):
@@ -14501,16 +15421,19 @@
             temp_model = DescribeAppsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAuthorizedApisRequest(TeaModel):
     def __init__(self, app_id=None, page_number=None, page_size=None, security_token=None):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.app_id = app_id  # type: long
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the request.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -14542,24 +15465,42 @@
         return self
 
 
 class DescribeAuthorizedApisResponseBodyAuthorizedApisAuthorizedApi(TeaModel):
     def __init__(self, api_id=None, api_name=None, auth_vaild_time=None, authorization_source=None,
                  authorized_time=None, description=None, group_id=None, group_name=None, operator=None, region_id=None,
                  stage_name=None):
+        # The expiration time of the authorization in UTC.
         self.api_id = api_id  # type: str
+        # *   This operation is intended for API callers.
+        # *   The specified application can call all APIs included in the responses.
         self.api_name = api_name  # type: str
+        # Queries weather based on the region name
         self.auth_vaild_time = auth_vaild_time  # type: str
+        # The description of the authorization.
         self.authorization_source = authorization_source  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.authorized_time = authorized_time  # type: str
+        # The name of the API group.
         self.description = description  # type: str
+        # The authorizer. Valid values:
+        # 
+        # *   **PROVIDER:** the API owner
+        # *   **CONSUMER:** the API caller
         self.group_id = group_id  # type: str
+        # The authorization time in UTC.
         self.group_name = group_name  # type: str
+        # The name of the API operation.
         self.operator = operator  # type: str
+        # Queries the authorized APIs of a specified application.
         self.region_id = region_id  # type: str
+        # The region to which the API belongs.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeAuthorizedApisResponseBodyAuthorizedApisAuthorizedApi, self).to_map()
@@ -14648,18 +15589,26 @@
                 temp_model = DescribeAuthorizedApisResponseBodyAuthorizedApisAuthorizedApi()
                 self.authorized_api.append(temp_model.from_map(k))
         return self
 
 
 class DescribeAuthorizedApisResponseBody(TeaModel):
     def __init__(self, authorized_apis=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The authorization source. Valid values:
+        # 
+        # *   **CONSOLE**\
+        # *   **API**\
         self.authorized_apis = authorized_apis  # type: DescribeAuthorizedApisResponseBodyAuthorizedApis
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The authorized API set.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The unique identifier of the API, which is generated by the system.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.authorized_apis:
             self.authorized_apis.validate()
 
     def to_map(self):
@@ -15002,14 +15951,115 @@
         if m.get('BackendId') is not None:
             self.backend_id = m.get('BackendId')
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
+class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfigNacosConfig(TeaModel):
+    def __init__(self, access_key=None, auth_type=None, clusters=None, group_name=None, namespace=None,
+                 password=None, secret_key=None, server_address=None, service_name=None, user_name=None):
+        self.access_key = access_key  # type: str
+        self.auth_type = auth_type  # type: str
+        self.clusters = clusters  # type: str
+        self.group_name = group_name  # type: str
+        self.namespace = namespace  # type: str
+        self.password = password  # type: str
+        self.secret_key = secret_key  # type: str
+        self.server_address = server_address  # type: str
+        self.service_name = service_name  # type: str
+        self.user_name = user_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfigNacosConfig, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, nacos_config=None, rc_type=None):
+        self.nacos_config = nacos_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfigNacosConfig
+        self.rc_type = rc_type  # type: str
+
+    def validate(self):
+        if self.nacos_config:
+            self.nacos_config.validate()
+
+    def to_map(self):
+        _map = super(DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfig, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, event_bridge_region_id=None, event_bus=None, event_source=None, role_arn=None):
         self.event_bridge_region_id = event_bridge_region_id  # type: str
         self.event_bus = event_bus  # type: str
         self.event_source = event_source  # type: str
         self.role_arn = role_arn  # type: str
 
@@ -15257,25 +16307,29 @@
             self.vpc_scheme = m.get('VpcScheme')
         if m.get('VpcTargetHostName') is not None:
             self.vpc_target_host_name = m.get('VpcTargetHostName')
         return self
 
 
 class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfig(TeaModel):
-    def __init__(self, event_bridge_config=None, function_compute_config=None, mock_config=None, oss_config=None,
-                 service_address=None, type=None, vpc_config=None):
+    def __init__(self, discovery_config=None, event_bridge_config=None, function_compute_config=None,
+                 http_target_host_name=None, mock_config=None, oss_config=None, service_address=None, type=None, vpc_config=None):
+        self.discovery_config = discovery_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigDiscoveryConfig
         self.event_bridge_config = event_bridge_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigEventBridgeConfig
         self.function_compute_config = function_compute_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigFunctionComputeConfig
+        self.http_target_host_name = http_target_host_name  # type: str
         self.mock_config = mock_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfig
         self.oss_config = oss_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigOssConfig
         self.service_address = service_address  # type: str
         self.type = type  # type: str
         self.vpc_config = vpc_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigVpcConfig
 
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
@@ -15285,38 +16339,47 @@
 
     def to_map(self):
         _map = super(DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfig, self).to_map()
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
 
     def from_map(self, m=None):
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
@@ -16550,17 +17613,24 @@
             temp_model = DescribeDeployApiTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDeployedApiRequest(TeaModel):
     def __init__(self, api_id=None, group_id=None, security_token=None, stage_name=None):
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The ID of the API group. An API group ID is generated by the system and is globally unique.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The environment in which the API runs. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiRequest, self).to_map()
@@ -16589,17 +17659,21 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeDeployedApiResponseBodyConstantParametersConstantParameter(TeaModel):
     def __init__(self, constant_value=None, description=None, location=None, service_parameter_name=None):
+        # The constant value.
         self.constant_value = constant_value  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The name of the backend service parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyConstantParametersConstantParameter, self).to_map()
@@ -16661,18 +17735,23 @@
                 self.constant_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDeployedApiResponseBodyCustomSystemParametersCustomSystemParameter(TeaModel):
     def __init__(self, demo_value=None, description=None, location=None, parameter_name=None,
                  service_parameter_name=None):
+        # The sample value.
         self.demo_value = demo_value  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The name of the custom system parameter.
         self.parameter_name = parameter_name  # type: str
+        # The name of the corresponding backend parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyCustomSystemParametersCustomSystemParameter, self).to_map()
@@ -16737,16 +17816,19 @@
                 temp_model = DescribeDeployedApiResponseBodyCustomSystemParametersCustomSystemParameter()
                 self.custom_system_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDeployedApiResponseBodyErrorCodeSamplesErrorCodeSample(TeaModel):
     def __init__(self, code=None, description=None, message=None):
+        # The error code returned if the request failed.
         self.code = code  # type: str
+        # The description of the error.
         self.description = description  # type: str
+        # The error message returned if the request failed.
         self.message = message  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyErrorCodeSamplesErrorCodeSample, self).to_map()
@@ -16803,17 +17885,24 @@
                 temp_model = DescribeDeployedApiResponseBodyErrorCodeSamplesErrorCodeSample()
                 self.error_code_sample.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDeployedApiResponseBodyOpenIdConnectConfig(TeaModel):
     def __init__(self, id_token_param_name=None, open_id_api_type=None, public_key=None, public_key_id=None):
+        # The name of the parameter that corresponds to the token.
         self.id_token_param_name = id_token_param_name  # type: str
+        # The OpenID Connect mode. Valid values:
+        # 
+        # *   **IDTOKEN:** OpenID Connect calls the authentication API to issue tokens. If the value is specified, the PublicKeyId parameter and the PublicKey parameter are required.
+        # *   **BUSINESS:** OpenID Connect calls the business API to verify identities by using existing tokens. If this value is specified, the IdTokenParamName parameter is required.
         self.open_id_api_type = open_id_api_type  # type: str
+        # The public key of the API.
         self.public_key = public_key  # type: str
+        # The ID of the public key.
         self.public_key_id = public_key_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyOpenIdConnectConfig, self).to_map()
@@ -16843,20 +17932,33 @@
             self.public_key_id = m.get('PublicKeyId')
         return self
 
 
 class DescribeDeployedApiResponseBodyRequestConfig(TeaModel):
     def __init__(self, body_format=None, body_model=None, post_body_description=None, request_http_method=None,
                  request_mode=None, request_path=None, request_protocol=None):
+        # This parameter takes effect only when the **RequestMode** parameter is set to **MAPPING**.
+        # 
+        # The format in which data is transmitted to the server for POST and PUT requests. Valid values: **FORM** and **STREAM**. FORM indicates that data is transmitted in the key-value pair format. STREAM indicates that data is transmitted as byte streams.
         self.body_format = body_format  # type: str
+        # The body model.
         self.body_model = body_model  # type: str
+        # The description of the request body.
         self.post_body_description = post_body_description  # type: str
+        # The HTTP method that is used to make the request. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_http_method = request_http_method  # type: str
+        # The request mode. Valid values:
+        # 
+        # *   MAPPING: Parameters are mapped. Unknown parameters are filtered out.
+        # *   PASSTHROUGH: Parameters are passed through.
+        # *   MAPPING_PASSTHROUGH: Parameters are mapped. Unknown parameters are passed through.
         self.request_mode = request_mode  # type: str
+        # The path of the API request. If the complete API URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, The path of the API request is ` /object/add  `.
         self.request_path = request_path  # type: str
+        # The protocol type supported by the API. Valid values: HTTP, HTTPS, and WebSocket. Separate multiple values with commas (,). Example: "HTTP,HTTPS".
         self.request_protocol = request_protocol  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyRequestConfig, self).to_map()
@@ -16900,30 +18002,47 @@
 
 
 class DescribeDeployedApiResponseBodyRequestParametersRequestParameter(TeaModel):
     def __init__(self, api_parameter_name=None, array_items_type=None, default_value=None, demo_value=None,
                  description=None, doc_order=None, doc_show=None, enum_value=None, json_scheme=None, location=None,
                  max_length=None, max_value=None, min_length=None, min_value=None, parameter_type=None,
                  regular_expression=None, required=None):
+        # The name of the API parameter.
         self.api_parameter_name = api_parameter_name  # type: str
+        # The type of the array element.
         self.array_items_type = array_items_type  # type: str
+        # The default value.
         self.default_value = default_value  # type: str
+        # The sample value.
         self.demo_value = demo_value  # type: str
+        # The parameter description.
         self.description = description  # type: str
+        # The order in the document.
         self.doc_order = doc_order  # type: int
+        # Indicates whether the document is public. Valid values: **PUBLIC** and **PRIVATE**.
         self.doc_show = doc_show  # type: str
+        # The hash values that can be entered when **ParameterType** is set to Int, Long, Float, Double, or String. Separate different values with commas (,). Examples: 1,2,3,4,9 and A,B,C,E,F.
         self.enum_value = enum_value  # type: str
+        # JSON scheme
         self.json_scheme = json_scheme  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The maximum length of the **ParameterType** parameter when the parameter is set to String.
         self.max_length = max_length  # type: long
+        # The maximum value of the **ParameterType** parameter when the parameter is set to Int, Long, Float, or Double.
         self.max_value = max_value  # type: long
+        # The minimum length of the **ParameterType** parameter when the parameter is set to String.
         self.min_length = min_length  # type: long
+        # The minimum value of the **ParameterType** parameter when the parameter is set to Int, Long, Float, or Double.
         self.min_value = min_value  # type: long
+        # The type of the parameter. Valid values: String, Int, Long, Float, Double, and Boolean.
         self.parameter_type = parameter_type  # type: str
+        # The regular expression used for parameter validation when **ParameterType** is set to String.
         self.regular_expression = regular_expression  # type: str
+        # Indicates whether the parameter is required. Valid values: **REQUIRED** and **OPTIONAL**.
         self.required = required  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyRequestParametersRequestParameter, self).to_map()
@@ -17037,18 +18156,20 @@
                 self.request_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDeployedApiResponseBodyResultDescriptionsResultDescription(TeaModel):
     def __init__(self, description=None, has_child=None, id=None, key=None, mandatory=None, name=None, pid=None,
                  type=None):
+        # The description of the parameter.
         self.description = description  # type: str
         self.has_child = has_child  # type: bool
         self.id = id  # type: str
         self.key = key  # type: str
+        # Indicates whether the parameter is required.
         self.mandatory = mandatory  # type: bool
         self.name = name  # type: str
         self.pid = pid  # type: str
         self.type = type  # type: str
 
     def validate(self):
         pass
@@ -17130,25 +18251,41 @@
         return self
 
 
 class DescribeDeployedApiResponseBodyServiceConfigFunctionComputeConfig(TeaModel):
     def __init__(self, content_type_catagory=None, content_type_value=None, fc_base_url=None, fc_type=None,
                  function_name=None, method=None, only_business_path=None, path=None, qualifier=None, region_id=None,
                  role_arn=None, service_name=None):
+        # The ContentType header used when a backend HTTP service is called. Valid values:
+        # 
+        # *   **DEFAULT:** the default header in API Gateway
+        # *   **CUSTOM:** a custom header
+        # *   **CLIENT:** the ContentType header specified by the client
         self.content_type_catagory = content_type_catagory  # type: str
+        # The value of the ContentType header when the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value  # type: str
+        # The root path of Function Compute.
         self.fc_base_url = fc_base_url  # type: str
+        # The type of the Function Compute instance.
         self.fc_type = fc_type  # type: str
+        # The function name defined in Function Compute.
         self.function_name = function_name  # type: str
+        # The request method.
         self.method = method  # type: str
+        # Indicates whether the backend receives only the service path.
         self.only_business_path = only_business_path  # type: bool
+        # The API request path.
         self.path = path  # type: str
+        # The alias of the function.
         self.qualifier = qualifier  # type: str
+        # The region in which the instance resides.
         self.region_id = region_id  # type: str
+        # The ARN of the RAM role assumed by API Gateway to access Function Compute.
         self.role_arn = role_arn  # type: str
+        # The service name defined in Function Compute.
         self.service_name = service_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyServiceConfigFunctionComputeConfig, self).to_map()
@@ -17209,15 +18346,17 @@
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
         return self
 
 
 class DescribeDeployedApiResponseBodyServiceConfigMockHeadersMockHeader(TeaModel):
     def __init__(self, header_name=None, header_value=None):
+        # The name of the HTTP header parameter.
         self.header_name = header_name  # type: str
+        # The value of the HTTP header parameter.
         self.header_value = header_value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyServiceConfigMockHeadersMockHeader, self).to_map()
@@ -17270,17 +18409,21 @@
                 temp_model = DescribeDeployedApiResponseBodyServiceConfigMockHeadersMockHeader()
                 self.mock_header.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDeployedApiResponseBodyServiceConfigVpcConfig(TeaModel):
     def __init__(self, instance_id=None, name=None, port=None, vpc_id=None):
+        # The ID of the Elastic Compute Service (ECS) or Server Load Balancer (SLB) instance in the VPC.
         self.instance_id = instance_id  # type: str
+        # The name of the VPC access authorization.
         self.name = name  # type: str
+        # The port number that corresponds to the instance.
         self.port = port  # type: int
+        # The ID of the VPC.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyServiceConfigVpcConfig, self).to_map()
@@ -17311,26 +18454,45 @@
         return self
 
 
 class DescribeDeployedApiResponseBodyServiceConfig(TeaModel):
     def __init__(self, function_compute_config=None, mock=None, mock_headers=None, mock_result=None,
                  mock_status_code=None, service_address=None, service_http_method=None, service_path=None, service_protocol=None,
                  service_timeout=None, service_vpc_enable=None, vpc_config=None, vpc_id=None):
+        # The backend configuration items when the backend service is Function Compute.
         self.function_compute_config = function_compute_config  # type: DescribeDeployedApiResponseBodyServiceConfigFunctionComputeConfig
+        # Indicates whether the Mock mode is enabled. Valid values:
+        # 
+        # *   **TRUE:** The Mock mode is enabled.
+        # *   **FALSE:** The Mock mode is not enabled.
         self.mock = mock  # type: str
+        # The mock headers.
         self.mock_headers = mock_headers  # type: DescribeDeployedApiResponseBodyServiceConfigMockHeaders
+        # The result returned when the Mock mode is enabled.
         self.mock_result = mock_result  # type: str
+        # The status code returned for service mock.
         self.mock_status_code = mock_status_code  # type: int
+        # The URL that is used to call the backend service. If the complete URL of a backend service is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the value of ServiceAddress is **http://api.a.com:8080**.``
         self.service_address = service_address  # type: str
+        # The HTTP method that is used to call a backend service. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.service_http_method = service_http_method  # type: str
+        # The path that is used to call the backend service. If the complete URL of a backend service is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the value of the **ServicePath** parameter is `/object/add`.
         self.service_path = service_path  # type: str
+        # The backend service protocol. Only HTTP, HTTPS, and Function Compute are supported.
         self.service_protocol = service_protocol  # type: str
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_timeout = service_timeout  # type: int
+        # Indicates whether to enable the VPC channel. Valid values:
+        # 
+        # *   **TRUE**: The VPC channel is enabled. You can enable a VPC channel only after you create the corresponding access authorization for the VPC.
+        # *   **FALSE**: The VPC channel is not enabled.
         self.service_vpc_enable = service_vpc_enable  # type: str
+        # The configuration items of the VPC channel.
         self.vpc_config = vpc_config  # type: DescribeDeployedApiResponseBodyServiceConfigVpcConfig
+        # The ID of the VPC.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         if self.function_compute_config:
             self.function_compute_config.validate()
         if self.mock_headers:
             self.mock_headers.validate()
@@ -17403,16 +18565,19 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeDeployedApiResponseBodyServiceParametersServiceParameter(TeaModel):
     def __init__(self, location=None, parameter_type=None, service_parameter_name=None):
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The data type of the backend service parameter. Valid values: STRING, NUMBER, and BOOLEAN.
         self.parameter_type = parameter_type  # type: str
+        # The name of the backend service parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyServiceParametersServiceParameter, self).to_map()
@@ -17469,15 +18634,17 @@
                 temp_model = DescribeDeployedApiResponseBodyServiceParametersServiceParameter()
                 self.service_parameter.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDeployedApiResponseBodyServiceParametersMapServiceParameterMap(TeaModel):
     def __init__(self, request_parameter_name=None, service_parameter_name=None):
+        # The name of the frontend input parameter.
         self.request_parameter_name = request_parameter_name  # type: str
+        # The name of the backend service parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodyServiceParametersMapServiceParameterMap, self).to_map()
@@ -17531,18 +18698,23 @@
                 self.service_parameter_map.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDeployedApiResponseBodySystemParametersSystemParameter(TeaModel):
     def __init__(self, demo_value=None, description=None, location=None, parameter_name=None,
                  service_parameter_name=None):
+        # The example.
         self.demo_value = demo_value  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # The parameter location. Valid values: BODY, HEAD, QUERY, and PATH.
         self.location = location  # type: str
+        # The name of the system parameter. Valid values: CaClientIp, CaDomain, CaRequestHandleTime, CaAppId, CaRequestId, CaHttpSchema, CaProxy.
         self.parameter_name = parameter_name  # type: str
+        # The name of the corresponding backend parameter.
         self.service_parameter_name = service_parameter_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDeployedApiResponseBodySystemParametersSystemParameter, self).to_map()
@@ -17612,42 +18784,103 @@
 class DescribeDeployedApiResponseBody(TeaModel):
     def __init__(self, allow_signature_method=None, api_id=None, api_name=None, auth_type=None,
                  constant_parameters=None, custom_system_parameters=None, deployed_time=None, description=None, disable_internet=None,
                  error_code_samples=None, fail_result_sample=None, force_nonce_check=None, group_id=None, group_name=None,
                  open_id_connect_config=None, region_id=None, request_config=None, request_id=None, request_parameters=None,
                  result_body_model=None, result_descriptions=None, result_sample=None, result_type=None, service_config=None,
                  service_parameters=None, service_parameters_map=None, stage_name=None, system_parameters=None, visibility=None):
+        # The signature method used by the client. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method  # type: str
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The name of the API.
         self.api_name = api_name  # type: str
+        # The authentication method of the API. Valid values:
+        # 
+        # *   **APP:** Only authorized apps are allowed to call the API.
+        # 
+        # *   **ANONYMOUS**: The API can be anonymously called. In this mode, you must take note of the following rules:
+        # 
+        #     *   All users who have obtained the API service information can call this API. API Gateway does not authenticate callers and cannot set user-specific throttling policies. If the API is made public, set API-specific throttling policies.
         self.auth_type = auth_type  # type: str
+        # The constant parameters.
         self.constant_parameters = constant_parameters  # type: DescribeDeployedApiResponseBodyConstantParameters
+        # The custom system parameters.
         self.custom_system_parameters = custom_system_parameters  # type: DescribeDeployedApiResponseBodyCustomSystemParameters
+        # The deployment time. Format: yyyy-mm-ddhh:mm:ss.
         self.deployed_time = deployed_time  # type: str
+        # The description of the parameter.
         self.description = description  # type: str
+        # *   Indicates whether to call the API only in an internal network. If this parameter is set to **true**, the API can be called only in an internal network.
+        # *   If this parameter is set to **false**, the API can be called over the Internet and in an internal network.
+        # 
+        # > If you do not configure this parameter when you modify the API, the original value is used.
         self.disable_internet = disable_internet  # type: bool
+        # The sample error codes returned by the backend service.
+        # 
+        # For more information, see [ErrorCodeSample](~~44392~~).
         self.error_code_samples = error_code_samples  # type: DescribeDeployedApiResponseBodyErrorCodeSamples
+        # The sample error response from the backend service.
         self.fail_result_sample = fail_result_sample  # type: str
+        # *   Indicates whether to forcibly check X-Ca-Nonce. If the **ForceNonceCheck** parameter is set to **true**, X-Ca-Nonce is forcibly checked. X-Ca-Nonce is the unique identifier of a request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent replay attacks.
+        # *   If the **ForceNonceCheck** parameter is set to **false**, the X-Ca-Nonce is not checked. Default value: false.
         self.force_nonce_check = force_nonce_check  # type: bool
+        # The ID of the API group.
         self.group_id = group_id  # type: str
+        # The name of the API group.
         self.group_name = group_name  # type: str
+        # The configuration items of the third-party OpenID Connect authentication method.
         self.open_id_connect_config = open_id_connect_config  # type: DescribeDeployedApiResponseBodyOpenIdConnectConfig
+        # The region in which the API group resides.
         self.region_id = region_id  # type: str
+        # The configuration items of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestConfig](~~43985~~).
         self.request_config = request_config  # type: DescribeDeployedApiResponseBodyRequestConfig
+        # The ID of the request.
         self.request_id = request_id  # type: str
+        # The parameters of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestParameter](~~43986~~).
         self.request_parameters = request_parameters  # type: DescribeDeployedApiResponseBodyRequestParameters
+        # The return description of the API.
         self.result_body_model = result_body_model  # type: str
+        # The returned description of the API.
         self.result_descriptions = result_descriptions  # type: DescribeDeployedApiResponseBodyResultDescriptions
+        # The sample response from the backend service.
         self.result_sample = result_sample  # type: str
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML. Default value: JSON.
         self.result_type = result_type  # type: str
+        # The configuration items of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceConfig](~~43987~~).
         self.service_config = service_config  # type: DescribeDeployedApiResponseBodyServiceConfig
+        # The parameters of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameter](~~43988~~).
         self.service_parameters = service_parameters  # type: DescribeDeployedApiResponseBodyServiceParameters
+        # The mappings between parameters of requests sent by the consumer to API Gateway and parameters of requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameterMap](~~43989~~).
         self.service_parameters_map = service_parameters_map  # type: DescribeDeployedApiResponseBodyServiceParametersMap
+        # The environment in which the API runs. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
         self.stage_name = stage_name  # type: str
+        # The system parameters.
         self.system_parameters = system_parameters  # type: DescribeDeployedApiResponseBodySystemParameters
+        # Indicates whether the API is public. Valid values:
+        # 
+        # *   **PUBLIC:** The API is public. If this parameter is set to PUBLIC, the API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE:** The API is private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.visibility = visibility  # type: str
 
     def validate(self):
         if self.constant_parameters:
             self.constant_parameters.validate()
         if self.custom_system_parameters:
             self.custom_system_parameters.validate()
@@ -18151,15 +19384,17 @@
             temp_model = DescribeDeployedApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRequest(TeaModel):
     def __init__(self, domain_name=None, group_id=None, security_token=None):
+        # The custom domain name.
         self.domain_name = domain_name  # type: str
+        # The private key of the SSL certificate.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -18185,29 +19420,53 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeDomainResponseBody(TeaModel):
     def __init__(self, certificate_body=None, certificate_id=None, certificate_name=None,
-                 certificate_private_key=None, domain_binding_status=None, domain_cnamestatus=None, domain_legal_status=None,
-                 domain_name=None, domain_remark=None, domain_web_socket_status=None, group_id=None, request_id=None,
-                 sub_domain=None):
+                 certificate_private_key=None, certificate_valid_end=None, certificate_valid_start=None, domain_binding_status=None,
+                 domain_cnamestatus=None, domain_legal_status=None, domain_name=None, domain_remark=None,
+                 domain_web_socket_status=None, group_id=None, request_id=None, sub_domain=None):
+        # The domain name resolution status. Valid values:
+        # 
+        # *   RESOLVED: The domain name has been resolved.
+        # *   UNRESOLVED: The domain name has not been resolved.
         self.certificate_body = certificate_body  # type: str
+        # The ID of the request.
         self.certificate_id = certificate_id  # type: str
+        # The ID of the API group to which the domain name is bound. This ID is generated by the system and globally unique.
         self.certificate_name = certificate_name  # type: str
+        # The binding status of the custom domain name. Valid values:
+        # 
+        # *   BINDING: The domain name has been bound.
+        # *   BOUND: The domain name has not been bound.
         self.certificate_private_key = certificate_private_key  # type: str
+        self.certificate_valid_end = certificate_valid_end  # type: long
+        self.certificate_valid_start = certificate_valid_start  # type: long
+        # The domain name does not have an ICP filing.
         self.domain_binding_status = domain_binding_status  # type: str
+        # Queries details about a bound custom domain name, including the automatically assigned second-level domain name, custom domain name, and SSL certificate.
         self.domain_cnamestatus = domain_cnamestatus  # type: str
+        # The content of the certificate.
         self.domain_legal_status = domain_legal_status  # type: str
+        # Remarks about the domain name, such as the cause of an exception.
         self.domain_name = domain_name  # type: str
+        # The unique ID of the SSL certificate, which is automatically generated by the system.
         self.domain_remark = domain_remark  # type: str
+        # The name of the SSL certificate.
         self.domain_web_socket_status = domain_web_socket_status  # type: str
+        # The second-level domain name that is automatically assigned to the API group.
         self.group_id = group_id  # type: str
+        # The validity status of the domain name. Valid values:
+        # 
+        # *   NORMAL
+        # *   ABNORMAL: This status affects API calls and must be resolved as soon as possible.
         self.request_id = request_id  # type: str
+        # *   This operation is intended for API providers.
         self.sub_domain = sub_domain  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainResponseBody, self).to_map()
@@ -18219,14 +19478,18 @@
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
@@ -18249,14 +19512,18 @@
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
@@ -18551,14 +19818,2023 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeHistoryApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeImportOASTaskRequest(TeaModel):
+    def __init__(self, operation_id=None, security_token=None):
+        self.operation_id = operation_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeImportOASTaskRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OperationId') is not None:
+            self.operation_id = m.get('OperationId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeImportOASTaskResponseBodyApiResultsApiResult(TeaModel):
+    def __init__(self, api_id=None, api_name=None, description=None, error_message=None, group_id=None, method=None,
+                 path=None, update_status=None):
+        self.api_id = api_id  # type: str
+        self.api_name = api_name  # type: str
+        self.description = description  # type: str
+        self.error_message = error_message  # type: str
+        self.group_id = group_id  # type: str
+        self.method = method  # type: str
+        self.path = path  # type: str
+        self.update_status = update_status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeImportOASTaskResponseBodyApiResultsApiResult, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, api_result=None):
+        self.api_result = api_result  # type: list[DescribeImportOASTaskResponseBodyApiResultsApiResult]
+
+    def validate(self):
+        if self.api_result:
+            for k in self.api_result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeImportOASTaskResponseBodyApiResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, error_message=None, group_id=None, model_id=None, model_name=None, update_status=None):
+        self.error_message = error_message  # type: str
+        self.group_id = group_id  # type: str
+        self.model_id = model_id  # type: str
+        self.model_name = model_name  # type: str
+        self.update_status = update_status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeImportOASTaskResponseBodyModelResultsModelResult, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, model_result=None):
+        self.model_result = model_result  # type: list[DescribeImportOASTaskResponseBodyModelResultsModelResult]
+
+    def validate(self):
+        if self.model_result:
+            for k in self.model_result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeImportOASTaskResponseBodyModelResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, api_results=None, model_results=None, request_id=None, task_status=None):
+        self.api_results = api_results  # type: DescribeImportOASTaskResponseBodyApiResults
+        self.model_results = model_results  # type: DescribeImportOASTaskResponseBodyModelResults
+        self.request_id = request_id  # type: str
+        self.task_status = task_status  # type: str
+
+    def validate(self):
+        if self.api_results:
+            self.api_results.validate()
+        if self.model_results:
+            self.model_results.validate()
+
+    def to_map(self):
+        _map = super(DescribeImportOASTaskResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeImportOASTaskResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeImportOASTaskResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, sbc_name=None, security_token=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the dedicated instance.
+        self.instance_id = instance_id  # type: str
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name  # type: str
+        self.security_token = security_token  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropConnectionsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item_time=None, item_value=None):
+        # The monitoring time. The time follows the ISO 8601 standard. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The number of dropped packets in the instance.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropConnectionsResponseBodyInstanceDropConnectionsMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceDropConnectionsResponseBodyInstanceDropConnections(TeaModel):
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceDropConnectionsResponseBodyInstanceDropConnectionsMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropConnectionsResponseBodyInstanceDropConnections, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_drop_connections=None, request_id=None):
+        # The list of dropped connections in the instance.
+        self.instance_drop_connections = instance_drop_connections  # type: DescribeInstanceDropConnectionsResponseBodyInstanceDropConnections
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_drop_connections:
+            self.instance_drop_connections.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropConnectionsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceDropConnectionsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropConnectionsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, sbc_name=None, security_token=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name  # type: str
+        self.security_token = security_token  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropPacketRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item=None, item_time=None, item_value=None):
+        # The metric. Valid values:
+        # 
+        # *   InstanceDropPacketRX: the number of inbound packets dropped in the instance per second.
+        # *   InstanceDropPacketTX: the number of outbound packets dropped in the instance per second.
+        self.item = item  # type: str
+        # The monitoring time. The time follows the ISO 8601 standard. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The number of dropped packets in the instance.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropPacketResponseBodyInstanceDropPacketMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceDropPacketResponseBodyInstanceDropPacketMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropPacketResponseBodyInstanceDropPacket, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_drop_packet=None, request_id=None):
+        # The list of dropped packets in the instance.
+        self.instance_drop_packet = instance_drop_packet  # type: DescribeInstanceDropPacketResponseBodyInstanceDropPacket
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_drop_packet:
+            self.instance_drop_packet.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropPacketResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceDropPacketResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceDropPacketResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, security_token=None, stage_name=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        self.security_token = security_token  # type: str
+        # The environment in which the API is requested. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
+        self.stage_name = stage_name  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceHttpCodeRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item_time=None, item_value=None):
+        # The HTTP status code.
+        self.item_time = item_time  # type: str
+        # The number of HTTP status codes returned.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceHttpCodeResponseBodyInstanceHttpCodeMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceHttpCodeResponseBodyInstanceHttpCode(TeaModel):
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceHttpCodeResponseBodyInstanceHttpCodeMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceHttpCodeResponseBodyInstanceHttpCode, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_http_code=None, request_id=None):
+        # The list of HTTP status codes returned.
+        self.instance_http_code = instance_http_code  # type: DescribeInstanceHttpCodeResponseBodyInstanceHttpCode
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_http_code:
+            self.instance_http_code.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceHttpCodeResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceHttpCodeResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceHttpCodeResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, security_token=None, stage_name=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        self.security_token = security_token  # type: str
+        # The environment in which the API is requested. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
+        self.stage_name = stage_name  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceLatencyRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item=None, item_time=None, item_value=None):
+        # The metric. Valid values:
+        # 
+        # *   gatewayLatency API: the processing latency of API Gateway
+        # *   latency: the processing latency of the backend service.
+        self.item = item  # type: str
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The value of the average latency.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceLatencyResponseBodyInstanceLatencyMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceLatencyResponseBodyInstanceLatencyMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceLatencyResponseBodyInstanceLatency, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_latency=None, request_id=None):
+        # The list of average latencies in the instance.
+        self.instance_latency = instance_latency  # type: DescribeInstanceLatencyResponseBodyInstanceLatency
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_latency:
+            self.instance_latency.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceLatencyResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceLatencyResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceLatencyResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, sbc_name=None, security_token=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name  # type: str
+        self.security_token = security_token  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceNewConnectionsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item_time=None, item_value=None):
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The number of new connections in the instance.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceNewConnectionsResponseBodyInstanceNewConnectionsMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceNewConnectionsResponseBodyInstanceNewConnections(TeaModel):
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceNewConnectionsResponseBodyInstanceNewConnectionsMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceNewConnectionsResponseBodyInstanceNewConnections, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_new_connections=None, request_id=None):
+        # The list of new connections in the instance.
+        self.instance_new_connections = instance_new_connections  # type: DescribeInstanceNewConnectionsResponseBodyInstanceNewConnections
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_new_connections:
+            self.instance_new_connections.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceNewConnectionsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceNewConnectionsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceNewConnectionsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, sbc_name=None, security_token=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name  # type: str
+        self.security_token = security_token  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstancePacketsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item=None, item_time=None, item_value=None):
+        # The metric. Valid values:
+        # 
+        # *   InstancePacketRX: inbound data packets
+        # *   InstancePacketTX: outbound data packets
+        self.item = item  # type: str
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The number of inbound and outbound data packets in the instance.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstancePacketsResponseBodyInstancePacketsMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstancePacketsResponseBodyInstancePacketsMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstancePacketsResponseBodyInstancePackets, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_packets=None, request_id=None):
+        # The list of inbound and outbound data packets in the instance.
+        self.instance_packets = instance_packets  # type: DescribeInstancePacketsResponseBodyInstancePackets
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_packets:
+            self.instance_packets.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstancePacketsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstancePacketsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstancePacketsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, security_token=None, stage_name=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        self.security_token = security_token  # type: str
+        # The environment in which the API is requested. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST**: the test environment
+        self.stage_name = stage_name  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceQpsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item_time=None, item_value=None):
+        # The monitoring time. The time follows the ISO 8601 standard. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The number of requests sent to the APIs in the instance.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceQpsResponseBodyInstanceQpsMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ItemTime') is not None:
+            self.item_time = m.get('ItemTime')
+        if m.get('ItemValue') is not None:
+            self.item_value = m.get('ItemValue')
+        return self
+
+
+class DescribeInstanceQpsResponseBodyInstanceQps(TeaModel):
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceQpsResponseBodyInstanceQpsMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceQpsResponseBodyInstanceQps, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_qps=None, request_id=None):
+        # The list of requests sent to the APIs in the instance.
+        self.instance_qps = instance_qps  # type: DescribeInstanceQpsResponseBodyInstanceQps
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_qps:
+            self.instance_qps.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceQpsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceQpsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceQpsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, sbc_name=None, security_token=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        # The statistical metric. Valid values:
+        # 
+        # *   Maximum
+        # *   Minimum
+        # *   Average
+        self.sbc_name = sbc_name  # type: str
+        self.security_token = security_token  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceSlbConnectRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item=None, item_time=None, item_value=None):
+        # The metric. Valid values:
+        # 
+        # *   InstanceMaxConnection: the maximum number of connections
+        # *   InstanceInactiveConnection: the number of inactive connections
+        # *   InstanceActiveConnection: the number of active connections
+        self.item = item  # type: str
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The number of concurrent connections in the instance.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceSlbConnectResponseBodyInstanceSlbConnectMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceSlbConnectResponseBodyInstanceSlbConnectMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceSlbConnectResponseBodyInstanceSlbConnect, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_slb_connect=None, request_id=None):
+        # The list of concurrent connections in the instance.
+        self.instance_slb_connect = instance_slb_connect  # type: DescribeInstanceSlbConnectResponseBodyInstanceSlbConnect
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_slb_connect:
+            self.instance_slb_connect.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceSlbConnectResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceSlbConnectResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceSlbConnectResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, end_time=None, instance_id=None, security_token=None, stage_name=None, start_time=None):
+        # The end time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.end_time = end_time  # type: str
+        # The ID of the instance.
+        self.instance_id = instance_id  # type: str
+        self.security_token = security_token  # type: str
+        # The environment in which the API runs. Valid values:
+        # 
+        # *   **RELEASE**: the production environment
+        # *   **PRE**: the pre-release environment
+        # *   **TEST: the test environment**\
+        self.stage_name = stage_name  # type: str
+        # The start time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceTrafficRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, item=None, item_time=None, item_value=None):
+        # The metric. Valid values:
+        # 
+        # *   inbound: traffic consumed by requests
+        # *   outbound: traffic consumed by responses
+        self.item = item  # type: str
+        # The monitoring time. The time follows the ISO 8601 standard and UTC time is used. Format: YYYY-MM-DDThh:mm:ssZ
+        self.item_time = item_time  # type: str
+        # The amount of traffic consumed by the requests and responses in the instance.
+        self.item_value = item_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstanceTrafficResponseBodyInstanceTrafficMonitorItem, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, monitor_item=None):
+        self.monitor_item = monitor_item  # type: list[DescribeInstanceTrafficResponseBodyInstanceTrafficMonitorItem]
+
+    def validate(self):
+        if self.monitor_item:
+            for k in self.monitor_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceTrafficResponseBodyInstanceTraffic, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_traffic=None, request_id=None):
+        # The traffic consumed by the requests and responses in the instance.
+        self.instance_traffic = instance_traffic  # type: DescribeInstanceTrafficResponseBodyInstanceTraffic
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.instance_traffic:
+            self.instance_traffic.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceTrafficResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeInstanceTrafficResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstanceTrafficResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, key=None, value=None):
         self.key = key  # type: str
         self.value = value  # type: str
 
     def validate(self):
         pass
@@ -18694,56 +21970,154 @@
         if m.get('SpecAttribute') is not None:
             for k in m.get('SpecAttribute'):
                 temp_model = DescribeInstancesResponseBodyInstancesInstanceAttributeInstanceSpecAttributesSpecAttribute()
                 self.spec_attribute.append(temp_model.from_map(k))
         return self
 
 
+class DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributesNetworkInterfaceAttribute(TeaModel):
+    def __init__(self, cidr_block=None, security_group_id=None, vswitch_id=None, zone_id=None):
+        # vSwitch的网段。
+        self.cidr_block = cidr_block  # type: str
+        # 安全组的ID，同一个安全组内的服务可以互相访问。
+        self.security_group_id = security_group_id  # type: str
+        # 虚拟交换机ID
+        self.vswitch_id = vswitch_id  # type: str
+        # 可用区ID
+        self.zone_id = zone_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributesNetworkInterfaceAttribute, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, network_interface_attribute=None):
+        self.network_interface_attribute = network_interface_attribute  # type: list[DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributesNetworkInterfaceAttribute]
+
+    def validate(self):
+        if self.network_interface_attribute:
+            for k in self.network_interface_attribute:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributes, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, acl_id=None, acl_name=None, acl_status=None, acl_type=None, classic_egress_address=None,
-                 created_time=None, egress_ipv_6enable=None, expired_time=None, https_policies=None, instance_charge_type=None,
-                 instance_id=None, instance_name=None, instance_rps_limit=None, instance_spec=None,
-                 instance_spec_attributes=None, instance_type=None, internet_egress_address=None, intranet_segments=None, region_id=None,
-                 status=None, support_ipv_6=None, user_vpc_id=None, user_vswitch_id=None, vip_type_list=None,
-                 vpc_egress_address=None, vpc_intranet_enable=None, vpc_owner_id=None, vpc_slb_intranet_enable=None, zone_id=None,
-                 zone_local_name=None):
+                 connect_cidr_blocks=None, connect_vpc_id=None, created_time=None, dedicated_instance_type=None,
+                 egress_ipv_6enable=None, expired_time=None, https_policies=None, ipv6acl_id=None, ipv6acl_name=None,
+                 ipv6acl_status=None, ipv6acl_type=None, instance_charge_type=None, instance_cidr_block=None,
+                 instance_cluster_id=None, instance_id=None, instance_name=None, instance_rps_limit=None, instance_spec=None,
+                 instance_spec_attributes=None, instance_type=None, internet_egress_address=None, intranet_segments=None,
+                 maintain_end_time=None, maintain_start_time=None, network_interface_attributes=None, region_id=None, status=None,
+                 support_ipv_6=None, user_vpc_id=None, user_vswitch_id=None, vpc_egress_address=None, vpc_intranet_enable=None,
+                 vpc_owner_id=None, vpc_slb_intranet_enable=None, zone_id=None, zone_local_name=None):
         self.acl_id = acl_id  # type: str
         self.acl_name = acl_name  # type: str
         self.acl_status = acl_status  # type: str
         self.acl_type = acl_type  # type: str
         self.classic_egress_address = classic_egress_address  # type: str
+        self.connect_cidr_blocks = connect_cidr_blocks  # type: str
+        # VPC融合类型专享实例联通的用户VPC ID
+        self.connect_vpc_id = connect_vpc_id  # type: str
         self.created_time = created_time  # type: str
+        # 专享实例类型
+        # - vpc_connect：VPC融合类型专享实例
+        # - normal：传统类型专享实例
+        self.dedicated_instance_type = dedicated_instance_type  # type: str
         self.egress_ipv_6enable = egress_ipv_6enable  # type: bool
         self.expired_time = expired_time  # type: str
         self.https_policies = https_policies  # type: str
+        self.ipv6acl_id = ipv6acl_id  # type: str
+        self.ipv6acl_name = ipv6acl_name  # type: str
+        self.ipv6acl_status = ipv6acl_status  # type: str
+        self.ipv6acl_type = ipv6acl_type  # type: str
         self.instance_charge_type = instance_charge_type  # type: str
+        # 专享实例所在网段
+        # - 172.16.0.0/12
+        # - 192.168.0.0/16
+        self.instance_cidr_block = instance_cidr_block  # type: str
+        self.instance_cluster_id = instance_cluster_id  # type: str
         self.instance_id = instance_id  # type: str
         self.instance_name = instance_name  # type: str
         self.instance_rps_limit = instance_rps_limit  # type: int
         self.instance_spec = instance_spec  # type: str
         self.instance_spec_attributes = instance_spec_attributes  # type: DescribeInstancesResponseBodyInstancesInstanceAttributeInstanceSpecAttributes
         self.instance_type = instance_type  # type: str
         self.internet_egress_address = internet_egress_address  # type: str
         self.intranet_segments = intranet_segments  # type: str
+        self.maintain_end_time = maintain_end_time  # type: str
+        self.maintain_start_time = maintain_start_time  # type: str
+        # VPC融合类型专享实例连通的用户VPC内的网络信息
+        self.network_interface_attributes = network_interface_attributes  # type: DescribeInstancesResponseBodyInstancesInstanceAttributeNetworkInterfaceAttributes
         self.region_id = region_id  # type: str
         self.status = status  # type: str
         self.support_ipv_6 = support_ipv_6  # type: bool
         self.user_vpc_id = user_vpc_id  # type: str
         self.user_vswitch_id = user_vswitch_id  # type: str
-        self.vip_type_list = vip_type_list  # type: str
         self.vpc_egress_address = vpc_egress_address  # type: str
         self.vpc_intranet_enable = vpc_intranet_enable  # type: bool
         self.vpc_owner_id = vpc_owner_id  # type: long
         self.vpc_slb_intranet_enable = vpc_slb_intranet_enable  # type: bool
         self.zone_id = zone_id  # type: str
         self.zone_local_name = zone_local_name  # type: str
 
     def validate(self):
         if self.instance_spec_attributes:
             self.instance_spec_attributes.validate()
+        if self.network_interface_attributes:
+            self.network_interface_attributes.validate()
 
     def to_map(self):
         _map = super(DescribeInstancesResponseBodyInstancesInstanceAttribute, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -18753,24 +22127,42 @@
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
@@ -18779,26 +22171,30 @@
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
@@ -18817,24 +22213,42 @@
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
@@ -18844,26 +22258,31 @@
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
@@ -19198,18 +22617,26 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeIpControlsRequest(TeaModel):
     def __init__(self, ip_control_id=None, ip_control_name=None, ip_control_type=None, page_number=None,
                  page_size=None, security_token=None):
+        # The ID of the ACL. The ID is unique.
         self.ip_control_id = ip_control_id  # type: str
+        # The name of the ACL.
         self.ip_control_name = ip_control_name  # type: str
+        # The type of the ACL. Valid values:
+        # 
+        # *   **ALLOW**: a whitelist
+        # *   **REFUSE**: a blacklist
         self.ip_control_type = ip_control_type  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.page_number = page_number  # type: int
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -19248,20 +22675,27 @@
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeIpControlsResponseBodyIpControlInfosIpControlInfo(TeaModel):
     def __init__(self, create_time=None, description=None, ip_control_id=None, ip_control_name=None,
                  ip_control_type=None, modified_time=None, region_id=None):
+        # The time when the ACL was created. The time is displayed in UTC.
         self.create_time = create_time  # type: str
+        # The description of the ACL.
         self.description = description  # type: str
+        # The ID of the ACL.
         self.ip_control_id = ip_control_id  # type: str
+        # The name of the ACL.
         self.ip_control_name = ip_control_name  # type: str
+        # The type of the ACL.
         self.ip_control_type = ip_control_type  # type: str
+        # The time when the ACL was modified. The time is displayed in UTC.
         self.modified_time = modified_time  # type: str
+        # The ID of the region in which the ACL is deployed.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeIpControlsResponseBodyIpControlInfosIpControlInfo, self).to_map()
@@ -19334,18 +22768,23 @@
                 temp_model = DescribeIpControlsResponseBodyIpControlInfosIpControlInfo()
                 self.ip_control_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeIpControlsResponseBody(TeaModel):
     def __init__(self, ip_control_infos=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The information about the ACL. The information is an array that consists of IpControlInfo data. The information does not include specific policies.
         self.ip_control_infos = ip_control_infos  # type: DescribeIpControlsResponseBodyIpControlInfos
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The number of entries returned per page.
         self.page_size = page_size  # type: int
+        # The ID of the request.
         self.request_id = request_id  # type: str
+        # The total number of returned entries.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.ip_control_infos:
             self.ip_control_infos.validate()
 
     def to_map(self):
@@ -19686,18 +23125,23 @@
             temp_model = DescribeMarketRemainsQuotaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeModelsRequest(TeaModel):
     def __init__(self, group_id=None, model_id=None, model_name=None, page_number=None, page_size=None):
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.group_id = group_id  # type: str
+        # The ID of the request.
         self.model_id = model_id  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.model_name = model_name  # type: str
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the model.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeModelsRequest, self).to_map()
@@ -19731,21 +23175,29 @@
             self.page_size = m.get('PageSize')
         return self
 
 
 class DescribeModelsResponseBodyModelDetailsModelDetail(TeaModel):
     def __init__(self, created_time=None, description=None, group_id=None, model_id=None, model_name=None,
                  model_ref=None, modified_time=None, schema=None):
+        # The URI of the model.
         self.created_time = created_time  # type: str
+        # The name of the model.
         self.description = description  # type: str
+        # The definition of the model.
         self.group_id = group_id  # type: str
+        # *   Fuzzy queries are supported.
         self.model_id = model_id  # type: str
+        # The ID of the model.
         self.model_name = model_name  # type: str
+        # Obtains the created models of an API group.
         self.model_ref = model_ref  # type: str
+        # The definition of the model description.
         self.modified_time = modified_time  # type: str
+        # The time when the model was created.
         self.schema = schema  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeModelsResponseBodyModelDetailsModelDetail, self).to_map()
@@ -19822,18 +23274,23 @@
                 temp_model = DescribeModelsResponseBodyModelDetailsModelDetail()
                 self.model_detail.append(temp_model.from_map(k))
         return self
 
 
 class DescribeModelsResponseBody(TeaModel):
     def __init__(self, model_details=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The ID of the API group to which the model belongs.
         self.model_details = model_details  # type: DescribeModelsResponseBodyModelDetails
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned information about models. It is an array consisting of ModelDetail data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The last modification time of the model.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.model_details:
             self.model_details.validate()
 
     def to_map(self):
@@ -19905,14 +23362,266 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeModelsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePluginApisRequest(TeaModel):
+    def __init__(self, api_id=None, api_name=None, description=None, group_id=None, method=None, page_number=None,
+                 page_size=None, path=None, plugin_id=None, security_token=None):
+        self.api_id = api_id  # type: str
+        self.api_name = api_name  # type: str
+        self.description = description  # type: str
+        self.group_id = group_id  # type: str
+        self.method = method  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.path = path  # type: str
+        self.plugin_id = plugin_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePluginApisRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, api_id=None, api_name=None, description=None, group_id=None, group_name=None, method=None,
+                 path=None, region_id=None, stage_name=None):
+        self.api_id = api_id  # type: str
+        self.api_name = api_name  # type: str
+        self.description = description  # type: str
+        self.group_id = group_id  # type: str
+        self.group_name = group_name  # type: str
+        self.method = method  # type: str
+        self.path = path  # type: str
+        self.region_id = region_id  # type: str
+        self.stage_name = stage_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribePluginApisResponseBodyApiSummarysApiPluginSummary, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, api_plugin_summary=None):
+        self.api_plugin_summary = api_plugin_summary  # type: list[DescribePluginApisResponseBodyApiSummarysApiPluginSummary]
+
+    def validate(self):
+        if self.api_plugin_summary:
+            for k in self.api_plugin_summary:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribePluginApisResponseBodyApiSummarys, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, api_summarys=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        self.api_summarys = api_summarys  # type: DescribePluginApisResponseBodyApiSummarys
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.api_summarys:
+            self.api_summarys.validate()
+
+    def to_map(self):
+        _map = super(DescribePluginApisResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribePluginApisResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribePluginApisResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, language=None, security_token=None):
         self.language = language  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
@@ -20598,18 +24307,28 @@
         if m.get('body') is not None:
             temp_model = DescribePluginsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribePluginsByApiRequest(TeaModel):
-    def __init__(self, api_id=None, group_id=None, security_token=None, stage_name=None):
+    def __init__(self, api_id=None, group_id=None, page_number=None, page_size=None, security_token=None,
+                 stage_name=None):
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The ID of the group to which the API belongs.
         self.group_id = group_id  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The environment in which the API is running. Valid values:
+        # 
+        # *   **RELEASE**: production
+        # *   **PRE**: staging
+        # *   **TEST**: test
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribePluginsByApiRequest, self).to_map()
@@ -20617,43 +24336,59 @@
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
 
     def from_map(self, m=None):
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
 
 
 class DescribePluginsByApiResponseBodyPluginsPluginAttribute(TeaModel):
     def __init__(self, created_time=None, description=None, modified_time=None, plugin_data=None, plugin_id=None,
                  plugin_name=None, plugin_type=None, region_id=None):
+        # The time when the plug-in was created. The time is displayed in UTC.
         self.created_time = created_time  # type: str
+        # The description of the plug-in.
         self.description = description  # type: str
+        # The time when the plug-in was last modified. The time is displayed in UTC.
         self.modified_time = modified_time  # type: str
+        # The definition statement of the plug-in.
         self.plugin_data = plugin_data  # type: str
+        # The ID of the plug-in.
         self.plugin_id = plugin_id  # type: str
+        # The name of the plug-in.
         self.plugin_name = plugin_name  # type: str
+        # The type of the plug-in.
         self.plugin_type = plugin_type  # type: str
+        # The region where the plug-in resides.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribePluginsByApiResponseBodyPluginsPluginAttribute, self).to_map()
@@ -20730,18 +24465,23 @@
                 temp_model = DescribePluginsByApiResponseBodyPluginsPluginAttribute()
                 self.plugin_attribute.append(temp_model.from_map(k))
         return self
 
 
 class DescribePluginsByApiResponseBody(TeaModel):
     def __init__(self, page_number=None, page_size=None, plugins=None, request_id=None, total_count=None):
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The number of entries returned per page.
         self.page_size = page_size  # type: int
+        # The plug-in information. The information is an array that consists of PluginAttribute data.
         self.plugins = plugins  # type: DescribePluginsByApiResponseBodyPlugins
+        # The ID of the request.
         self.request_id = request_id  # type: str
+        # The total number of returned entries.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.plugins:
             self.plugins.validate()
 
     def to_map(self):
@@ -21641,18 +25381,22 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSignaturesRequest(TeaModel):
     def __init__(self, page_number=None, page_size=None, security_token=None, signature_id=None,
                  signature_name=None):
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the request.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.signature_id = signature_id  # type: str
+        # The number of entries to return on each page. Maximum value: 100. Default value: 10.
         self.signature_name = signature_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSignaturesRequest, self).to_map()
@@ -21686,20 +25430,28 @@
             self.signature_name = m.get('SignatureName')
         return self
 
 
 class DescribeSignaturesResponseBodySignatureInfosSignatureInfo(TeaModel):
     def __init__(self, created_time=None, modified_time=None, region_id=None, signature_id=None, signature_key=None,
                  signature_name=None, signature_secret=None):
+        # *   This API is intended for API providers.
+        # *   This operation is used to query the backend signature keys in a Region. Region is a system parameter.
         self.created_time = created_time  # type: str
+        # The Secret value of the backend signature key.
         self.modified_time = modified_time  # type: str
+        # Queries backend signature keys.
         self.region_id = region_id  # type: str
+        # The name of the backend signature key.
         self.signature_id = signature_id  # type: str
+        # The region where the key is located.
         self.signature_key = signature_key  # type: str
+        # The creation time of the key.
         self.signature_name = signature_name  # type: str
+        # The Key value of the backend signature key.
         self.signature_secret = signature_secret  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSignaturesResponseBodySignatureInfosSignatureInfo, self).to_map()
@@ -21772,18 +25524,23 @@
                 temp_model = DescribeSignaturesResponseBodySignatureInfosSignatureInfo()
                 self.signature_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeSignaturesResponseBody(TeaModel):
     def __init__(self, page_number=None, page_size=None, request_id=None, signature_infos=None, total_count=None):
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned signature information. It is an array consisting of SignatureInfo data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The ID of the backend signature key.
         self.signature_infos = signature_infos  # type: DescribeSignaturesResponseBodySignatureInfos
+        # The last modification time of the key.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.signature_infos:
             self.signature_infos.validate()
 
     def to_map(self):
@@ -21857,17 +25614,23 @@
             temp_model = DescribeSignaturesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeSignaturesByApiRequest(TeaModel):
     def __init__(self, api_id=None, group_id=None, security_token=None, stage_name=None):
+        # The ID of the request.
         self.api_id = api_id  # type: str
+        # The runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The returned signature key information. It is an array consisting of SignatureItem data.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSignaturesByApiRequest, self).to_map()
@@ -21896,16 +25659,19 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeSignaturesByApiResponseBodySignaturesSignatureItem(TeaModel):
     def __init__(self, bound_time=None, signature_id=None, signature_name=None):
+        # The name of the backend signature key.
         self.bound_time = bound_time  # type: str
+        # *   This API is intended for API providers.
         self.signature_id = signature_id  # type: str
+        # Queries the backend signature keys that are bound to a specified API.
         self.signature_name = signature_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSignaturesByApiResponseBodySignaturesSignatureItem, self).to_map()
@@ -21962,15 +25728,17 @@
                 temp_model = DescribeSignaturesByApiResponseBodySignaturesSignatureItem()
                 self.signature_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeSignaturesByApiResponseBody(TeaModel):
     def __init__(self, request_id=None, signatures=None):
+        # The time when the key was bound.
         self.request_id = request_id  # type: str
+        # The ID of the backend signature key.
         self.signatures = signatures  # type: DescribeSignaturesByApiResponseBodySignatures
 
     def validate(self):
         if self.signatures:
             self.signatures.validate()
 
     def to_map(self):
@@ -22030,14 +25798,127 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSignaturesByApiResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeSummaryDataRequest(TeaModel):
+    def __init__(self, security_token=None):
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeSummaryDataRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeSummaryDataResponseBody(TeaModel):
+    def __init__(self, expire_instance_num=None, region=None, request_id=None, usage_api_num=None,
+                 usage_group_num=None, usage_instance_num=None):
+        self.expire_instance_num = expire_instance_num  # type: int
+        self.region = region  # type: str
+        self.request_id = request_id  # type: str
+        self.usage_api_num = usage_api_num  # type: int
+        self.usage_group_num = usage_group_num  # type: int
+        self.usage_instance_num = usage_instance_num  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeSummaryDataResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeSummaryDataResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeSummaryDataResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, security_token=None):
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -22056,17 +25937,22 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class DescribeSystemParametersResponseBodySystemParamsSystemParamItem(TeaModel):
     def __init__(self, demo_value=None, description=None, param_name=None, param_type=None):
+        # Client IP Address
         self.demo_value = demo_value  # type: str
+        # The name of the parameter.
         self.description = description  # type: str
+        # *   This API is intended for API callers.
+        # *   The response of this API contains the system parameters that are optional in API definitions.
         self.param_name = param_name  # type: str
+        # Queries the common parameters supported by the system.
         self.param_type = param_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeSystemParametersResponseBodySystemParamsSystemParamItem, self).to_map()
@@ -22127,15 +26013,17 @@
                 temp_model = DescribeSystemParametersResponseBodySystemParamsSystemParamItem()
                 self.system_param_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeSystemParametersResponseBody(TeaModel):
     def __init__(self, request_id=None, system_params=None):
+        # Examples
         self.request_id = request_id  # type: str
+        # The description of a parameter.
         self.system_params = system_params  # type: DescribeSystemParametersResponseBodySystemParams
 
     def validate(self):
         if self.system_params:
             self.system_params.validate()
 
     def to_map(self):
@@ -22198,21 +26086,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTrafficControlsRequest(TeaModel):
     def __init__(self, api_id=None, group_id=None, page_number=None, page_size=None, security_token=None,
                  stage_name=None, traffic_control_id=None, traffic_control_name=None):
+        # The name of the throttling policy.
         self.api_id = api_id  # type: str
+        # The environment name. This parameter must be specified together with GroupId and ApiId. Valid values:********\
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The ID of the request.
         self.page_size = page_size  # type: int
         self.security_token = security_token  # type: str
+        # ThrottlingTest
         self.stage_name = stage_name  # type: str
+        # The specified API ID. This parameter must be specified together with GroupId and StageName.
         self.traffic_control_id = traffic_control_id  # type: str
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.traffic_control_name = traffic_control_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTrafficControlsRequest, self).to_map()
@@ -22257,15 +26155,19 @@
         if m.get('TrafficControlName') is not None:
             self.traffic_control_name = m.get('TrafficControlName')
         return self
 
 
 class DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicySpecialsSpecial(TeaModel):
     def __init__(self, special_key=None, traffic_value=None):
+        # Queries custom throttling policies and their details. Conditional queries are supported.
         self.special_key = special_key  # type: str
+        # *   This API is intended for API providers.
+        # *   This API can be used to query all existing throttling policies (including special throttling policies) and their details.
+        # *   You can specify query conditions. For example, you can query the throttling policies bound to a specified API or in a specified environment.
         self.traffic_value = traffic_value  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicySpecialsSpecial, self).to_map()
@@ -22318,15 +26220,17 @@
                 temp_model = DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicySpecialsSpecial()
                 self.special.append(temp_model.from_map(k))
         return self
 
 
 class DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicy(TeaModel):
     def __init__(self, special_type=None, specials=None):
+        # The throttling value.
         self.special_type = special_type  # type: str
+        # The AppId or user account corresponding to SpecialType.
         self.specials = specials  # type: DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPoliciesSpecialPolicySpecials
 
     def validate(self):
         if self.specials:
             self.specials.validate()
 
     def to_map(self):
@@ -22383,23 +26287,40 @@
         return self
 
 
 class DescribeTrafficControlsResponseBodyTrafficControlsTrafficControl(TeaModel):
     def __init__(self, api_default=None, app_default=None, created_time=None, description=None, modified_time=None,
                  special_policies=None, traffic_control_id=None, traffic_control_name=None, traffic_control_unit=None,
                  user_default=None):
+        # The description of the throttling policy.
         self.api_default = api_default  # type: int
+        # The creation time (UTC) of the throttling policy.
         self.app_default = app_default  # type: int
+        # The type of the special throttling policy. Valid values:
+        # 
+        # *   **APP**\
+        # *   **USER**\
         self.created_time = created_time  # type: str
+        # The name of the throttling policy.
         self.description = description  # type: str
+        # The unit to be used in the throttling policy. Valid values:
+        # 
+        # *   MINUTE
+        # *   HOUR
+        # *   DAY
         self.modified_time = modified_time  # type: str
+        # The returned information about a special throttling policy. It is an array consisting of Special data.
         self.special_policies = special_policies  # type: DescribeTrafficControlsResponseBodyTrafficControlsTrafficControlSpecialPolicies
+        # The returned information about a special throttling policy. It is an array consisting of SpecialPolicy data.
         self.traffic_control_id = traffic_control_id  # type: str
+        # The ID of the throttling policy.
         self.traffic_control_name = traffic_control_name  # type: str
+        # The default throttling value for each app.
         self.traffic_control_unit = traffic_control_unit  # type: str
+        # The last modification time (UTC) of the throttling policy.
         self.user_default = user_default  # type: int
 
     def validate(self):
         if self.special_policies:
             self.special_policies.validate()
 
     def to_map(self):
@@ -22486,18 +26407,23 @@
                 temp_model = DescribeTrafficControlsResponseBodyTrafficControlsTrafficControl()
                 self.traffic_control.append(temp_model.from_map(k))
         return self
 
 
 class DescribeTrafficControlsResponseBody(TeaModel):
     def __init__(self, page_number=None, page_size=None, request_id=None, total_count=None, traffic_controls=None):
+        # The number of entries returned per page.
         self.page_number = page_number  # type: int
+        # The returned throttling policy information. It is an array consisting of TrafficControl data.
         self.page_size = page_size  # type: int
+        # The total number of returned entries.
         self.request_id = request_id  # type: str
+        # The default throttling value for each user.
         self.total_count = total_count  # type: int
+        # The default throttling value for each API.
         self.traffic_controls = traffic_controls  # type: DescribeTrafficControlsResponseBodyTrafficControls
 
     def validate(self):
         if self.traffic_controls:
             self.traffic_controls.validate()
 
     def to_map(self):
@@ -22571,17 +26497,23 @@
             temp_model = DescribeTrafficControlsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeTrafficControlsByApiRequest(TeaModel):
     def __init__(self, api_id=None, group_id=None, security_token=None, stage_name=None):
+        # The ID of the request.
         self.api_id = api_id  # type: str
+        # The runtime environment of the API. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The returned throttling policy information. It is an array consisting of TrafficControlItem data.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTrafficControlsByApiRequest, self).to_map()
@@ -22610,16 +26542,19 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class DescribeTrafficControlsByApiResponseBodyTrafficControlItemsTrafficControlItem(TeaModel):
     def __init__(self, bound_time=None, traffic_control_item_id=None, traffic_control_item_name=None):
+        # *   This API is intended for API providers.
         self.bound_time = bound_time  # type: str
+        # The name of the throttling policy.
         self.traffic_control_item_id = traffic_control_item_id  # type: str
+        # Queries the throttling policy that is bound to a specific API.
         self.traffic_control_item_name = traffic_control_item_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeTrafficControlsByApiResponseBodyTrafficControlItemsTrafficControlItem, self).to_map()
@@ -22676,15 +26611,17 @@
                 temp_model = DescribeTrafficControlsByApiResponseBodyTrafficControlItemsTrafficControlItem()
                 self.traffic_control_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeTrafficControlsByApiResponseBody(TeaModel):
     def __init__(self, request_id=None, traffic_control_items=None):
+        # The ID of the throttling policy.
         self.request_id = request_id  # type: str
+        # The binding time of the policy.
         self.traffic_control_items = traffic_control_items  # type: DescribeTrafficControlsByApiResponseBodyTrafficControlItems
 
     def validate(self):
         if self.traffic_control_items:
             self.traffic_control_items.validate()
 
     def to_map(self):
@@ -23642,40 +27579,45 @@
         if m.get('body') is not None:
             temp_model = DetachPluginResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DisableInstanceAccessControlRequest(TeaModel):
-    def __init__(self, acl_id=None, instance_id=None, security_token=None):
+    def __init__(self, acl_id=None, address_ipversion=None, instance_id=None, security_token=None):
         self.acl_id = acl_id  # type: str
+        self.address_ipversion = address_ipversion  # type: str
         self.instance_id = instance_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DisableInstanceAccessControlRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
 
 
@@ -24218,17 +28160,18 @@
         if m.get('body') is not None:
             temp_model = DryRunSwaggerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableInstanceAccessControlRequest(TeaModel):
-    def __init__(self, acl_id=None, acl_type=None, instance_id=None, security_token=None):
+    def __init__(self, acl_id=None, acl_type=None, address_ipversion=None, instance_id=None, security_token=None):
         self.acl_id = acl_id  # type: str
         self.acl_type = acl_type  # type: str
+        self.address_ipversion = address_ipversion  # type: str
         self.instance_id = instance_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -24237,26 +28180,30 @@
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
 
     def from_map(self, m=None):
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
 
 
@@ -24319,22 +28266,538 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EnableInstanceAccessControlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ImportOASRequest(TeaModel):
+    def __init__(self, auth_type=None, backend_name=None, data=None, group_id=None, ignore_warning=None,
+                 oasversion=None, overwrite=None, request_mode=None, security_token=None, skip_dry_run=None):
+        # API安全认证类型，目前可以取值：
+        # 
+        # - **APP**：只允许已授权的APP调用
+        # - **ANONYMOUS**：允许匿名调用，设置为允许匿名调用需要注意：
+        #      - 任何能够获取该API服务信息的人，都将能够调用该API。网关不会对调用者做身份认证，也无法设置按用户的流量控制，若开放该API请设置好按API的流量控制。
+        self.auth_type = auth_type  # type: str
+        self.backend_name = backend_name  # type: str
+        self.data = data  # type: str
+        self.group_id = group_id  # type: str
+        self.ignore_warning = ignore_warning  # type: bool
+        self.oasversion = oasversion  # type: str
+        self.overwrite = overwrite  # type: bool
+        self.request_mode = request_mode  # type: str
+        self.security_token = security_token  # type: str
+        self.skip_dry_run = skip_dry_run  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImportOASRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, error_message=None):
+        self.error_message = error_message  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodyErrorMessages, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        return self
+
+
+class ImportOASResponseBodyFailedApisFailedApi(TeaModel):
+    def __init__(self, error_msg=None, http_method=None, path=None):
+        self.error_msg = error_msg  # type: str
+        self.http_method = http_method  # type: str
+        self.path = path  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodyFailedApisFailedApi, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, failed_api=None):
+        self.failed_api = failed_api  # type: list[ImportOASResponseBodyFailedApisFailedApi]
+
+    def validate(self):
+        if self.failed_api:
+            for k in self.failed_api:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodyFailedApis, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, error_msg=None, group_id=None, model_name=None):
+        self.error_msg = error_msg  # type: str
+        self.group_id = group_id  # type: str
+        self.model_name = model_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodyFailedModelsFailedModel, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, failed_model=None):
+        self.failed_model = failed_model  # type: list[ImportOASResponseBodyFailedModelsFailedModel]
+
+    def validate(self):
+        if self.failed_model:
+            for k in self.failed_model:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodyFailedModels, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, api_id=None, api_operation=None, http_method=None, path=None):
+        self.api_id = api_id  # type: str
+        self.api_operation = api_operation  # type: str
+        self.http_method = http_method  # type: str
+        self.path = path  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodySuccessApisSuccessApi, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, success_api=None):
+        self.success_api = success_api  # type: list[ImportOASResponseBodySuccessApisSuccessApi]
+
+    def validate(self):
+        if self.success_api:
+            for k in self.success_api:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodySuccessApis, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, group_id=None, model_name=None, model_operation=None, model_uid=None):
+        self.group_id = group_id  # type: str
+        self.model_name = model_name  # type: str
+        self.model_operation = model_operation  # type: str
+        self.model_uid = model_uid  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodySuccessModelsSuccessModel, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, success_model=None):
+        self.success_model = success_model  # type: list[ImportOASResponseBodySuccessModelsSuccessModel]
+
+    def validate(self):
+        if self.success_model:
+            for k in self.success_model:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodySuccessModels, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, warning_message=None):
+        self.warning_message = warning_message  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ImportOASResponseBodyWarningMessages, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.warning_message is not None:
+            result['WarningMessage'] = self.warning_message
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('WarningMessage') is not None:
+            self.warning_message = m.get('WarningMessage')
+        return self
+
+
+class ImportOASResponseBody(TeaModel):
+    def __init__(self, error_messages=None, failed_apis=None, failed_models=None, operation_id=None,
+                 request_id=None, success_apis=None, success_models=None, warning_messages=None):
+        self.error_messages = error_messages  # type: ImportOASResponseBodyErrorMessages
+        self.failed_apis = failed_apis  # type: ImportOASResponseBodyFailedApis
+        self.failed_models = failed_models  # type: ImportOASResponseBodyFailedModels
+        self.operation_id = operation_id  # type: str
+        self.request_id = request_id  # type: str
+        self.success_apis = success_apis  # type: ImportOASResponseBodySuccessApis
+        self.success_models = success_models  # type: ImportOASResponseBodySuccessModels
+        self.warning_messages = warning_messages  # type: ImportOASResponseBodyWarningMessages
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
+        _map = super(ImportOASResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ImportOASResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ImportOASResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, data=None, data_format=None, dry_run=None, global_condition=None, group_id=None,
                  overwrite=None, security_token=None):
         self.data = data  # type: str
+        # 382271
         self.data_format = data_format  # type: str
         self.dry_run = dry_run  # type: bool
+        # Creates an API by importing Swagger-compliant data.
         self.global_condition = global_condition  # type: dict[str, any]
         self.group_id = group_id  # type: str
+        # 8e274ec61cf6468e83b68371956831cb
         self.overwrite = overwrite  # type: bool
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -24378,18 +28841,21 @@
         return self
 
 
 class ImportSwaggerShrinkRequest(TeaModel):
     def __init__(self, data=None, data_format=None, dry_run=None, global_condition_shrink=None, group_id=None,
                  overwrite=None, security_token=None):
         self.data = data  # type: str
+        # 382271
         self.data_format = data_format  # type: str
         self.dry_run = dry_run  # type: bool
+        # Creates an API by importing Swagger-compliant data.
         self.global_condition_shrink = global_condition_shrink  # type: str
         self.group_id = group_id  # type: str
+        # 8e274ec61cf6468e83b68371956831cb
         self.overwrite = overwrite  # type: bool
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -25256,49 +29722,131 @@
                  auth_type=None, backend_name=None, body_format=None, body_model=None, content_type_category=None,
                  content_type_value=None, description=None, disable_internet=None, error_code_samples=None, fail_result_sample=None,
                  force_nonce_check=None, function_compute_config=None, http_config=None, mock_config=None, model_name=None,
                  oss_config=None, post_body_description=None, request_http_method=None, request_mode=None,
                  request_parameters=None, request_path=None, request_protocol=None, result_sample=None, result_type=None,
                  security_token=None, service_parameters=None, service_parameters_map=None, service_protocol=None,
                  service_timeout=None, use_backend_service=None, visibility=None, vpc_config=None):
+        # If the **AuthType** parameter is set to **APP**, you must include this parameter to specify the signature algorithm. If you do not specify a value, HmacSHA256 is used by default. Valid values:
+        # 
+        # *   HmacSHA256
+        # *   HmacSHA1,HmacSHA256
         self.allow_signature_method = allow_signature_method  # type: str
+        # The ID of the API.
         self.api_id = api_id  # type: str
+        # The name of the API.
         self.api_name = api_name  # type: str
+        # If the **AuthType** parameter is set to **APP**, the valid values are:
+        # 
+        # *   **DEFAULT**: The default value that is used if no other values are passed. This value indicates that the settings of the group are used.
+        # *   **DISABLE**: The authentication is disabled.
+        # *   **HEADER**: AppCode can be placed in the Header parameter for authentication.
+        # *   **HEADER_QUERY**: AppCode can be placed in the Header or Query parameter for authentication.
         self.app_code_auth_type = app_code_auth_type  # type: str
+        # API安全认证类型，目前可以取值：
+        # 
+        # - **APP**：只允许已授权的APP调用
+        # - **ANONYMOUS**：允许匿名调用，设置为允许匿名调用需要注意：
+        #      - 任何能够获取该API服务信息的人，都将能够调用该API。网关不会对调用者做身份认证，也无法设置按用户的流量控制，若开放该API请设置好按API的流量控制；
+        #      - AppCodeAuthType的值不会生效。
         self.auth_type = auth_type  # type: str
+        # The name of the backend service. This parameter takes effect only when the UseBackendService parameter is set to TRUE.
         self.backend_name = backend_name  # type: str
+        # This parameter takes effect only when the **RequestMode** parameter is set to **MAPPING**.
+        # 
+        # The format in which data is transmitted to the server for POST and PUT requests. Valid values: **FORM** and **STREAM**. FORM indicates that data is transmitted in the key-value pair format. STREAM indicates that data is transmitted as byte streams.
         self.body_format = body_format  # type: str
+        # The body model.
         self.body_model = body_model  # type: str
+        # The ContentType configuration of the backend request.
+        # 
+        # *   DEFAULT: the default configuration in API Gateway
+        # *   CUSTOM: a custom configuration
         self.content_type_category = content_type_category  # type: str
+        # The value of the ContentType header when the ServiceProtocol parameter is set to HTTP and the ContentTypeCatagory parameter is set to DEFAULT or CUSTOM.
         self.content_type_value = content_type_value  # type: str
+        # The description of the API.
         self.description = description  # type: str
+        # *   Specifies whether to call the API only in an internal network. If the **DisableInternet** parameter is set to **true**, the API can be called only in an internal network.
+        # *   If the **DisableInternet** parameter is set to **false**, the API can be called over the Internet and in an internal network.
         self.disable_internet = disable_internet  # type: bool
+        # The sample error codes returned by the backend service.
+        # 
+        # For more information, see [ErrorCodeSample](~~44392~~).
         self.error_code_samples = error_code_samples  # type: str
+        # The sample error response from the backend service. This value is used only to generate documents. It does not affect the returned result.
         self.fail_result_sample = fail_result_sample  # type: str
+        # *   Specifies whether to forcibly check X-Ca-Nonce. If the **ForceNonceCheck** parameter is set to **true**, X-Ca-Nonce is forcibly checked. X-Ca-Nonce is the unique identifier of the request and is generally identified by UUID. After receiving this parameter, API Gateway verifies the validity of this parameter. The same value can be used only once within 15 minutes. This helps prevent replay attacks.
+        # *   If the **ForceNonceCheck** parameter is set to **false**, X-Ca-Nonce is not checked. If you do not modify this parameter when you modify an API, the original value is used.
         self.force_nonce_check = force_nonce_check  # type: bool
+        # The Function Compute configuration.
         self.function_compute_config = function_compute_config  # type: str
+        # The HTTP configuration.
         self.http_config = http_config  # type: str
+        # The Mock configuration.
         self.mock_config = mock_config  # type: str
+        # The name of the model.
         self.model_name = model_name  # type: str
+        # The OSS configuration.
         self.oss_config = oss_config  # type: str
+        # The description of the request body.
         self.post_body_description = post_body_description  # type: str
+        # The HTTP method used to make the request. Valid values: GET, POST, DELETE, PUT, HEADER, TRACE, PATCH, CONNECT, and OPTIONS.
         self.request_http_method = request_http_method  # type: str
+        # The request mode. Valid values:
+        # 
+        # *   MAPPING: Parameters are mapped. Unknown parameters are filtered out.
+        # *   PASSTHROUGH: Parameters are passed through.
+        # *   MAPPING_PASSTHROUGH: Parameters are mapped. Unknown parameters are passed through.
         self.request_mode = request_mode  # type: str
+        # The parameters of API requests sent by the consumer to API Gateway.
+        # 
+        # For more information, see [RequestParameter](~~43986~~).
         self.request_parameters = request_parameters  # type: str
+        # The path of the API request. If the complete API URL is `http://api.a.com:8080/object/add?key1=value1&key2=value2`, the path of the API request is `/object/add`.
         self.request_path = request_path  # type: str
+        # The protocol type supported by the API. Valid values: HTTP and HTTPS. Separate multiple values with commas (,), such as "HTTP,HTTPS".
         self.request_protocol = request_protocol  # type: str
+        # The sample response from the backend service. This value is used only to generate documents. It does not affect the returned result.
         self.result_sample = result_sample  # type: str
+        # The format of the response from the backend service. Valid values: JSON, TEXT, BINARY, XML, and HTML. This value is used only to generate documents. It does not affect the returned result.
         self.result_type = result_type  # type: str
         self.security_token = security_token  # type: str
+        # The parameters of API requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameter](~~43988~~).
         self.service_parameters = service_parameters  # type: str
+        # The mappings between parameters of requests sent by the consumer to API Gateway and parameters of requests sent by API Gateway to the backend service.
+        # 
+        # For more information, see [ServiceParameterMap](~~43989~~).
         self.service_parameters_map = service_parameters_map  # type: str
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
         self.service_protocol = service_protocol  # type: str
+        # The timeout period of the backend service. Unit: milliseconds.
         self.service_timeout = service_timeout  # type: int
+        # Specifies whether to use the information about the created backend service. Valid values:
+        # 
+        # *   TRUE: uses the information about the created backend service.
+        # *   FALSE: uses the information about the custom backend service.
         self.use_backend_service = use_backend_service  # type: bool
+        # Specifies whether to make the API public. Valid values:
+        # 
+        # *   **PUBLIC:** The API is public. If this parameter is set to PUBLIC, the API is displayed on the APIs page for all users after the API is published to the production environment.
+        # *   **PRIVATE:** The API is private. Private APIs are not displayed in the Alibaba Cloud Marketplace after the API group to which they belong is made available.
         self.visibility = visibility  # type: str
+        # The VPC configuration.
         self.vpc_config = vpc_config  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyApiConfigurationRequest, self).to_map()
@@ -25455,14 +30003,15 @@
         if m.get('VpcConfig') is not None:
             self.vpc_config = m.get('VpcConfig')
         return self
 
 
 class ModifyApiConfigurationResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyApiConfigurationResponseBody, self).to_map()
@@ -25548,26 +30097,27 @@
             self.value = m.get('Value')
         return self
 
 
 class ModifyApiGroupRequest(TeaModel):
     def __init__(self, base_path=None, compatible_flags=None, custom_trace_config=None, customer_configs=None,
                  default_domain=None, description=None, group_id=None, group_name=None, passthrough_headers=None, rpc_pattern=None,
-                 security_token=None, tag=None, user_log_config=None):
+                 security_token=None, support_sse=None, tag=None, user_log_config=None):
         self.base_path = base_path  # type: str
         self.compatible_flags = compatible_flags  # type: str
         self.custom_trace_config = custom_trace_config  # type: str
         self.customer_configs = customer_configs  # type: str
         self.default_domain = default_domain  # type: str
         self.description = description  # type: str
         self.group_id = group_id  # type: str
         self.group_name = group_name  # type: str
         self.passthrough_headers = passthrough_headers  # type: str
         self.rpc_pattern = rpc_pattern  # type: str
         self.security_token = security_token  # type: str
+        self.support_sse = support_sse  # type: str
         self.tag = tag  # type: list[ModifyApiGroupRequestTag]
         self.user_log_config = user_log_config  # type: str
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -25597,14 +30147,16 @@
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
@@ -25629,14 +30181,16 @@
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
@@ -25855,18 +30409,19 @@
             self.key = m.get('Key')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class ModifyAppRequest(TeaModel):
-    def __init__(self, app_id=None, app_name=None, description=None, security_token=None, tag=None):
+    def __init__(self, app_id=None, app_name=None, description=None, extend=None, security_token=None, tag=None):
         self.app_id = app_id  # type: long
         self.app_name = app_name  # type: str
         self.description = description  # type: str
+        self.extend = extend  # type: str
         self.security_token = security_token  # type: str
         self.tag = tag  # type: list[ModifyAppRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -25880,14 +30435,16 @@
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
@@ -25896,14 +30453,16 @@
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
@@ -26519,16 +31078,20 @@
             temp_model = ModifyInstanceSpecResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyIpControlRequest(TeaModel):
     def __init__(self, description=None, ip_control_id=None, ip_control_name=None, security_token=None):
+        # *   This operation is intended for API providers.
+        # *   This operation allows you to modify only the name and description of an ACL. You cannot modify the type of the ACL.
         self.description = description  # type: str
+        # The description. The description can be up to 200 characters in length.
         self.ip_control_id = ip_control_id  # type: str
+        # The ID of the request.
         self.ip_control_name = ip_control_name  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -26558,14 +31121,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class ModifyIpControlResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Modifies an access control list (ACL).
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyIpControlResponseBody, self).to_map()
@@ -26621,17 +31185,29 @@
             temp_model = ModifyIpControlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyIpControlPolicyItemRequest(TeaModel):
     def __init__(self, app_id=None, cidr_ip=None, ip_control_id=None, policy_item_id=None, security_token=None):
+        # The ID of the request.
         self.app_id = app_id  # type: str
+        # *   This operation is intended for API providers.
+        # *   The modification immediately takes effect on all the APIs that are bound to the policy.
+        # *   This operation causes a full modification of the content of a policy.
         self.cidr_ip = cidr_ip  # type: str
+        # The ID of the application that is restricted by the policy. You can configure the AppId parameter only when the value of the IpControlType parameter is ALLOW.
+        # 
+        # *   You can add only one application ID at a time.
+        # *   If this parameter is empty, no applications are restricted.
+        # *   If this parameter is not empty, not only IP addresses but also applications are restricted.
+        # *   If this parameter is not empty and no security authentication method is specified for the API, all API calls are restricted.
+        # *   If the value of the IpControlType parameter is REFUSE and the AppId parameter is not empty, API Gateway automatically ignores the AppId parameter and restricts only the IP addresses.
         self.ip_control_id = ip_control_id  # type: str
+        # The IP address or CIDR block that is defined in a policy. Separate multiple IP addresses or CIDR blocks with semicolons (;). You can add a maximum of 10 IP addresses or CIDR blocks.
         self.policy_item_id = policy_item_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -26665,14 +31241,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class ModifyIpControlPolicyItemResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Modifies a policy in an access control list (ACL).
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyIpControlPolicyItemResponseBody, self).to_map()
@@ -26830,18 +31407,23 @@
             temp_model = ModifyLogConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyModelRequest(TeaModel):
     def __init__(self, description=None, group_id=None, model_name=None, new_model_name=None, schema=None):
+        # The new definition of the model.
         self.description = description  # type: str
+        # The new name of the model.
         self.group_id = group_id  # type: str
+        # The description of the new model definition.
         self.model_name = model_name  # type: str
+        # The ID of the request.
         self.new_model_name = new_model_name  # type: str
+        # The ID of the API group to which the model belongs.
         self.schema = schema  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyModelRequest, self).to_map()
@@ -26874,14 +31456,15 @@
         if m.get('Schema') is not None:
             self.schema = m.get('Schema')
         return self
 
 
 class ModifyModelResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Updates the model of an API group.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyModelResponseBody, self).to_map()
@@ -27089,17 +31672,21 @@
         return self
 
 
 class ModifySignatureRequest(TeaModel):
     def __init__(self, security_token=None, signature_id=None, signature_key=None, signature_name=None,
                  signature_secret=None):
         self.security_token = security_token  # type: str
+        # The new Key value of the key. The value must be 6 to 20 characters in length and can contain letters, digits, and underscores (\_). It must start with a letter.
         self.signature_id = signature_id  # type: str
+        # The ID of the request.
         self.signature_key = signature_key  # type: str
+        # The new Secret value of the key. The value must be 6 to 30 characters in length and can contain letters, digits, and special characters. Special characters include underscores (\_), at signs (@), number signs (#), exclamation points (!), and asterisks (\*). The value must start with a letter.
         self.signature_name = signature_name  # type: str
+        # The ID of the key.
         self.signature_secret = signature_secret  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifySignatureRequest, self).to_map()
@@ -27132,16 +31719,22 @@
         if m.get('SignatureSecret') is not None:
             self.signature_secret = m.get('SignatureSecret')
         return self
 
 
 class ModifySignatureResponseBody(TeaModel):
     def __init__(self, request_id=None, signature_id=None, signature_name=None):
+        # The name of the key.
         self.request_id = request_id  # type: str
+        # *   This API is intended for API providers.
+        # *   This API operation modifies the name, Key value, and Secret value of an existing signature key.
+        # *   Note that the modification takes effect immediately. If the key has been bound to an API, you must adjust the backend signature verification based on the new key accordingly.
+        # *   The QPS limit on this operation is 50 per user.
         self.signature_id = signature_id  # type: str
+        # Modifies a backend signature key.
         self.signature_name = signature_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifySignatureResponseBody, self).to_map()
@@ -27206,21 +31799,33 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyTrafficControlRequest(TeaModel):
     def __init__(self, api_default=None, app_default=None, description=None, security_token=None,
                  traffic_control_id=None, traffic_control_name=None, traffic_control_unit=None, user_default=None):
+        # The default throttling value for each app.
         self.api_default = api_default  # type: int
+        # ThrottlingTestDescription
         self.app_default = app_default  # type: int
+        # The ID of the request.
         self.description = description  # type: str
         self.security_token = security_token  # type: str
+        # ThrottlingTest
         self.traffic_control_id = traffic_control_id  # type: str
+        # The unit to be used in the throttling policy. Valid values:
+        # 
+        # *   **SECOND**\
+        # *   **MINUTE**\
+        # *   **HOUR**\
+        # *   **DAY**\
         self.traffic_control_name = traffic_control_name  # type: str
+        # The default throttling value for each user.
         self.traffic_control_unit = traffic_control_unit  # type: str
+        # The description of the throttling policy.
         self.user_default = user_default  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTrafficControlRequest, self).to_map()
@@ -27265,14 +31870,15 @@
         if m.get('UserDefault') is not None:
             self.user_default = m.get('UserDefault')
         return self
 
 
 class ModifyTrafficControlResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Modifies the settings of a custom throttling policy.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyTrafficControlResponseBody, self).to_map()
@@ -27329,22 +31935,44 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyVpcAccessAndUpdateApisRequest(TeaModel):
     def __init__(self, instance_id=None, name=None, need_batch_work=None, port=None, refresh=None,
                  security_token=None, token=None, vpc_id=None, vpc_target_host_name=None):
+        # The ID of the new instance.
         self.instance_id = instance_id  # type: str
+        # The name of the VPC authorization.
+        # 
+        # > 
+        # 
+        # *   The name of a VPC authorization cannot be changed. You cannot use this parameter to change the name of a VPC authorization.
+        # 
+        # *   You must set this parameter to the name of the current VPC authorization.
         self.name = name  # type: str
+        # Specifies whether to update the associated API.
+        # 
+        # **\
+        # 
+        # **Warning:** If you want to update the VPC authorization of a published API, you must set this parameter to true. Otherwise, the update will not be synchronized to the backend service of the API.
         self.need_batch_work = need_batch_work  # type: bool
+        # The new port number.
         self.port = port  # type: int
+        # Specifies whether to update the VPC authorization.
+        # 
+        # > 
+        # 
+        # *   If the ID of the instance in your VPC is changed but the IP address of the instance remains unchanged, you can set this parameter to true to update the VPC authorization.
         self.refresh = refresh  # type: bool
         self.security_token = security_token  # type: str
+        # The token of the request.
         self.token = token  # type: str
+        # The ID of the new VPC.
         self.vpc_id = vpc_id  # type: str
+        # The hostname of the backend service.
         self.vpc_target_host_name = vpc_target_host_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyVpcAccessAndUpdateApisRequest, self).to_map()
@@ -27393,15 +32021,21 @@
         if m.get('VpcTargetHostName') is not None:
             self.vpc_target_host_name = m.get('VpcTargetHostName')
         return self
 
 
 class ModifyVpcAccessAndUpdateApisResponseBody(TeaModel):
     def __init__(self, operation_id=None, request_id=None):
+        # The ID of the asynchronous task.
+        # 
+        # > 
+        # 
+        # *   If the associated API is updated, you can use the task ID in the **DescribeUpdateVpcInfoTask** operation to query the update result.
         self.operation_id = operation_id  # type: str
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyVpcAccessAndUpdateApisResponseBody, self).to_map()
@@ -27527,17 +32161,438 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = OpenApiGatewayServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryRequestLogsRequest(TeaModel):
+    def __init__(self, request_log_id=None, security_token=None):
+        # The ID of the request log.
+        self.request_log_id = request_log_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryRequestLogsRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestLogId') is not None:
+            self.request_log_id = m.get('RequestLogId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class QueryRequestLogsResponseBodyRequestLogsRequestLog(TeaModel):
+    def __init__(self, api_id=None, api_name=None, app_name=None, backend_request_end=None,
+                 backend_request_start=None, backend_response_end=None, backend_response_start=None, client_ip=None, client_nonce=None,
+                 consumer_app_id=None, consumer_app_key=None, custom_trace_id=None, domain=None, error_code=None,
+                 error_message=None, exception=None, front_request_end=None, front_request_start=None, front_response_end=None,
+                 front_response_start=None, group_id=None, group_name=None, http_method=None, http_path=None, initial_request_id=None,
+                 instance_id=None, jwt_claims=None, region=None, request_body=None, request_headers=None, request_id=None,
+                 request_protocol=None, request_query_string=None, request_size=None, request_time=None, response_body=None,
+                 response_headers=None, response_size=None, service_latency=None, stage_id=None, stage_name=None, status_code=None,
+                 total_latency=None, plugin=None):
+        # The ID of the API.
+        self.api_id = api_id  # type: str
+        # The name of the API
+        self.api_name = api_name  # type: str
+        self.app_name = app_name  # type: str
+        self.backend_request_end = backend_request_end  # type: long
+        self.backend_request_start = backend_request_start  # type: long
+        self.backend_response_end = backend_response_end  # type: long
+        self.backend_response_start = backend_response_start  # type: long
+        # The IP address of the client that sends the request.
+        self.client_ip = client_ip  # type: str
+        # The X-Ca-Nonce header included in the request from the client.
+        self.client_nonce = client_nonce  # type: str
+        # The ID of the application from which an API request is sent.
+        self.consumer_app_id = consumer_app_id  # type: str
+        # The application key used by the caller.
+        self.consumer_app_key = consumer_app_key  # type: str
+        # The ID of the custom trace.
+        self.custom_trace_id = custom_trace_id  # type: str
+        # The domain name of the request.
+        self.domain = domain  # type: str
+        # The error code returned if the request failed.
+        self.error_code = error_code  # type: str
+        # The error message returned if the request fails.
+        self.error_message = error_message  # type: str
+        # The specific error message returned by the backend service.
+        self.exception = exception  # type: str
+        self.front_request_end = front_request_end  # type: long
+        self.front_request_start = front_request_start  # type: long
+        self.front_response_end = front_response_end  # type: long
+        self.front_response_start = front_response_start  # type: long
+        # The ID of the API group to which the API belongs.
+        self.group_id = group_id  # type: str
+        # The name of the API group to which the API belongs.
+        self.group_name = group_name  # type: str
+        # The HTTP method used to send the request.
+        self.http_method = http_method  # type: str
+        # The path of the request.
+        self.http_path = http_path  # type: str
+        # The initial request ID when API Gateway calls an API. For example, if API-1 calls API-2, the initialRequestId parameter in the log of API-2 indicates the ID of the request from API-1.
+        self.initial_request_id = initial_request_id  # type: str
+        # The ID of the API Gateway instance to which the API belongs.
+        self.instance_id = instance_id  # type: str
+        # The JSON web token (JWT) claims. The claims can be configured at the group level.
+        self.jwt_claims = jwt_claims  # type: str
+        # The ID of the region.
+        self.region = region  # type: str
+        # The request body. A request body cannot exceed 1,024 bytes in size.
+        self.request_body = request_body  # type: str
+        # The request headers.
+        self.request_headers = request_headers  # type: str
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+        # The protocol used by the client to send the request. Valid values: HTTP, HTTPS, and WS.
+        self.request_protocol = request_protocol  # type: str
+        # The query string for the request.
+        self.request_query_string = request_query_string  # type: str
+        # The size of the request. Unit: bytes.
+        self.request_size = request_size  # type: str
+        # The request time, in UTC.
+        self.request_time = request_time  # type: str
+        # The response body. A response body cannot exceed 1,024 bytes in size.
+        self.response_body = response_body  # type: str
+        # The headers in the API response.
+        self.response_headers = response_headers  # type: str
+        # The size of returned data. Unit: bytes.
+        self.response_size = response_size  # type: str
+        # The total time consumed to access backend resources. The total time includes the time consumed to request a connection to the resources, the time consumed to establish the connection, and the time consumed to call the backend service. Unit: milliseconds.
+        self.service_latency = service_latency  # type: str
+        # The ID of the API environment.
+        self.stage_id = stage_id  # type: str
+        # The name of the API environment.
+        self.stage_name = stage_name  # type: str
+        # The HTTP status code.
+        self.status_code = status_code  # type: str
+        # The total time consumed by the request. Unit: milliseconds.
+        self.total_latency = total_latency  # type: str
+        # The list of plug-ins hit by the request and the relevant context.
+        self.plugin = plugin  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryRequestLogsResponseBodyRequestLogsRequestLog, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_log=None):
+        self.request_log = request_log  # type: list[QueryRequestLogsResponseBodyRequestLogsRequestLog]
+
+    def validate(self):
+        if self.request_log:
+            for k in self.request_log:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(QueryRequestLogsResponseBodyRequestLogs, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, request_logs=None):
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+        # The list of request logs.
+        self.request_logs = request_logs  # type: QueryRequestLogsResponseBodyRequestLogs
+
+    def validate(self):
+        if self.request_logs:
+            self.request_logs.validate()
+
+    def to_map(self):
+        _map = super(QueryRequestLogsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: QueryRequestLogsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(QueryRequestLogsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, domain_name=None, group_id=None, security_token=None):
+        # *   This operation is intended for API providers.
+        # *   You must solve the problem that is mentioned in the domain name exception prompt before you can reactivate the domain name.
+        # *   A typical reason why a custom domain name becomes abnormal is that the domain name does not have an ICP filing or the domain name is included in a blacklist by the administration. When a custom domain name is abnormal, users cannot use it to access APIs.
+        # *   You can call this operation to reactivate the domain name to resume normal access.
         self.domain_name = domain_name  # type: str
+        # The ID of the request.
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -27563,14 +32618,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class ReactivateDomainResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Reactivates a custom domain name whose validity status is Abnormal.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ReactivateDomainResponseBody, self).to_map()
@@ -27724,19 +32780,27 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveApisAuthoritiesRequest(TeaModel):
     def __init__(self, api_ids=None, app_id=None, description=None, group_id=None, security_token=None,
                  stage_name=None):
+        # Queries weather based on the region name
         self.api_ids = api_ids  # type: str
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.app_id = app_id  # type: long
+        # The ID of the request.
         self.description = description  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The description of the authorization.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveApisAuthoritiesRequest, self).to_map()
@@ -27773,14 +32837,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class RemoveApisAuthoritiesResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Revokes the access permissions on multiple APIs from a specified app.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveApisAuthoritiesResponseBody, self).to_map()
@@ -27836,18 +32901,26 @@
             temp_model = RemoveApisAuthoritiesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveAppsAuthoritiesRequest(TeaModel):
     def __init__(self, api_id=None, app_ids=None, group_id=None, security_token=None, stage_name=None):
+        # The IDs of applications. Separate multiple application IDs with commas (,). A maximum of 100 applications IDs can be entered.
         self.api_id = api_id  # type: str
+        # *   This operation is intended for API providers and callers.
+        # *   Before you revoke access permissions, check by whom the permissions were granted. API providers can only revoke permissions granted by a Provider, and API callers can only revoke permissions granted by a Consumer.
         self.app_ids = app_ids  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The ID of the request.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveAppsAuthoritiesRequest, self).to_map()
@@ -27880,14 +32953,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class RemoveAppsAuthoritiesResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Revokes the access permissions on a specified API from multiple applications. In this case, multiple applications map to a single API.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveAppsAuthoritiesResponseBody, self).to_map()
@@ -27943,18 +33017,29 @@
             temp_model = RemoveAppsAuthoritiesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveIpControlApisRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, ip_control_id=None, security_token=None, stage_name=None):
+        # The ID of the request.
         self.api_ids = api_ids  # type: str
-        self.group_id = group_id  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
+        self.group_id = group_id  # type: str
+        # The ID of the API to be managed.
+        # 
+        # *   If this parameter is not specified, all APIs of the API group are unbound in the specified environment by default.
+        # *   The IDs of the APIs that you want to query. Separate multiple IDs with commas (,). A maximum of 100 IDs can be entered.
         self.ip_control_id = ip_control_id  # type: str
         self.security_token = security_token  # type: str
+        # *   This API is intended for API providers.
+        # *   The unbinding takes effect immediately. After the API is unbound from the ACL, the corresponding environment does not have any IP address access control in place for the API.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveIpControlApisRequest, self).to_map()
@@ -27987,14 +33072,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class RemoveIpControlApisResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Unbinds an API from an access control list (ACL).
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveIpControlApisResponseBody, self).to_map()
@@ -28050,15 +33136,17 @@
             temp_model = RemoveIpControlApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveIpControlPolicyItemRequest(TeaModel):
     def __init__(self, ip_control_id=None, policy_item_ids=None, security_token=None):
+        # The ID of the request.
         self.ip_control_id = ip_control_id  # type: str
+        # *   This operation is intended for API providers.
         self.policy_item_ids = policy_item_ids  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -28084,14 +33172,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class RemoveIpControlPolicyItemResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Removes one or more policies from an access control list (ACL).
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveIpControlPolicyItemResponseBody, self).to_map()
@@ -28147,18 +33236,29 @@
             temp_model = RemoveIpControlPolicyItemResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveSignatureApisRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, security_token=None, signature_id=None, stage_name=None):
+        # The ID of the request.
         self.api_ids = api_ids  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The IDs of the APIs from which you want to unbind the signature key.
+        # 
+        # *   If this parameter is not specified, the signature key is unbound from all the APIs in the specified environment of the API group.
+        # *   The IDs of the APIs that you want to manage. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.signature_id = signature_id  # type: str
+        # *   This API is intended for API providers.
+        # *   The operation takes effect immediately. The request sent from API Gateway to the backend service does not contain the signature string. The corresponding verification step can be removed from the backend.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveSignatureApisRequest, self).to_map()
@@ -28191,14 +33291,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class RemoveSignatureApisResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Unbinds a backend signature key from APIs.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveSignatureApisResponseBody, self).to_map()
@@ -28254,18 +33355,29 @@
             temp_model = RemoveSignatureApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveTrafficControlApisRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, security_token=None, stage_name=None, traffic_control_id=None):
+        # The ID of the request.
         self.api_ids = api_ids  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # *   This API is intended for API providers.
+        # *   This API allows you to unbind a specified throttling policy from up to 100 APIs at a time.
         self.stage_name = stage_name  # type: str
+        # The IDs of the APIs from which you want to unbind a specified throttling policy.
+        # 
+        # *   If this parameter is not specified, the throttling policy is unbound from all the APIs in the specified environment of the API group.
+        # *   Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.traffic_control_id = traffic_control_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveTrafficControlApisRequest, self).to_map()
@@ -28298,14 +33410,15 @@
         if m.get('TrafficControlId') is not None:
             self.traffic_control_id = m.get('TrafficControlId')
         return self
 
 
 class RemoveTrafficControlApisResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Unbinds a specified throttling policy from APIs.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RemoveTrafficControlApisResponseBody, self).to_map()
@@ -28405,14 +33518,15 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class RemoveVpcAccessResponseBodyApisApi(TeaModel):
     def __init__(self, api_id=None, group_id=None, stage_id=None):
+        # API Id
         self.api_id = api_id  # type: str
         self.group_id = group_id  # type: str
         self.stage_id = stage_id  # type: str
 
     def validate(self):
         pass
 
@@ -28653,15 +33767,17 @@
             temp_model = RemoveVpcAccessAndAbolishApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResetAppCodeRequest(TeaModel):
     def __init__(self, app_code=None, new_app_code=None, security_token=None):
+        # The current AppCode of the application.
         self.app_code = app_code  # type: str
+        # The new AppCode of the application.
         self.new_app_code = new_app_code  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -28687,14 +33803,15 @@
         if m.get('SecurityToken') is not None:
             self.security_token = m.get('SecurityToken')
         return self
 
 
 class ResetAppCodeResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ResetAppCodeResponseBody, self).to_map()
@@ -28749,49 +33866,57 @@
         if m.get('body') is not None:
             temp_model = ResetAppCodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ResetAppSecretRequest(TeaModel):
-    def __init__(self, app_key=None, new_app_secret=None, security_token=None):
+    def __init__(self, app_key=None, new_app_key=None, new_app_secret=None, security_token=None):
+        # The key of the application that is used to make an API call.
         self.app_key = app_key  # type: str
+        self.new_app_key = new_app_key  # type: str
+        # The new key of the application. To improve compatibility, we recommend that you use other parameters.
         self.new_app_secret = new_app_secret  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ResetAppSecretRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ResetAppSecretResponseBody, self).to_map()
@@ -29251,20 +34376,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetApisAuthoritiesRequest(TeaModel):
     def __init__(self, api_ids=None, app_id=None, auth_valid_time=None, description=None, group_id=None,
                  security_token=None, stage_name=None):
+        # Queries weather based on the region name
         self.api_ids = api_ids  # type: str
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.app_id = app_id  # type: long
+        # *   This operation is intended for API providers and callers.
+        # *   API providers can authorize any apps to call their APIs.
+        # *   API callers can authorize their own apps to call the APIs that they have purchased.
         self.auth_valid_time = auth_valid_time  # type: str
+        # The time (UTC) when the authorization expires. If this parameter is empty, the authorization does not expire.
         self.description = description  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The description of the authorization.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetApisAuthoritiesRequest, self).to_map()
@@ -29305,14 +34441,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class SetApisAuthoritiesResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Authorizes a specified app to call multiple APIs.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetApisAuthoritiesResponseBody, self).to_map()
@@ -29369,20 +34506,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetAppsAuthoritiesRequest(TeaModel):
     def __init__(self, api_id=None, app_ids=None, auth_valid_time=None, description=None, group_id=None,
                  security_token=None, stage_name=None):
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.api_id = api_id  # type: str
+        # Queries weather based on the region name
         self.app_ids = app_ids  # type: str
+        # *   This operation is intended for API providers and callers.
+        # *   API providers can authorize any apps to call their APIs.
+        # *   API callers can authorize their own apps to call the APIs that they have purchased.
         self.auth_valid_time = auth_valid_time  # type: str
+        # The time (UTC) when the authorization expires. If this parameter is empty, the authorization does not expire.
         self.description = description  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The description of the authorization.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetAppsAuthoritiesRequest, self).to_map()
@@ -29423,14 +34571,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class SetAppsAuthoritiesResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Grants access permissions on a specified API to multiple apps.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetAppsAuthoritiesResponseBody, self).to_map()
@@ -29863,20 +35012,126 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SetDomainWebSocketStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SetGroupAuthAppCodeRequest(TeaModel):
+    def __init__(self, auth_app_code=None, group_id=None, security_token=None):
+        self.auth_app_code = auth_app_code  # type: str
+        self.group_id = group_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetGroupAuthAppCodeRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetGroupAuthAppCodeResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetGroupAuthAppCodeResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetGroupAuthAppCodeResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetGroupAuthAppCodeResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, api_ids=None, group_id=None, ip_control_id=None, security_token=None, stage_name=None):
+        # The ID of the request.
         self.api_ids = api_ids  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **PRE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
+        # The API IDs. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.ip_control_id = ip_control_id  # type: str
         self.security_token = security_token  # type: str
+        # *   This operation is intended for API callers.
+        # *   A maximum of 100 APIs can be bound at a time.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetIpControlApisRequest, self).to_map()
@@ -29909,14 +35164,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class SetIpControlApisResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Creates a binding relationship between specified access control lists (ACLs) and APIs.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetIpControlApisResponseBody, self).to_map()
@@ -29972,18 +35228,27 @@
             temp_model = SetIpControlApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetSignatureApisRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, security_token=None, signature_id=None, stage_name=None):
+        # The ID of the request.
         self.api_ids = api_ids  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **PRE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.signature_id = signature_id  # type: str
+        # *   This API is intended for API providers.
+        # *   This operation allows you to bind a signature key to an API. You can bind signature keys for up to 100 APIs at a time.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetSignatureApisRequest, self).to_map()
@@ -30016,14 +35281,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class SetSignatureApisResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Binds a signature key to APIs.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetSignatureApisResponseBody, self).to_map()
@@ -30079,18 +35345,26 @@
             temp_model = SetSignatureApisResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SetTrafficControlApisRequest(TeaModel):
     def __init__(self, api_ids=None, group_id=None, security_token=None, stage_name=None, traffic_control_id=None):
+        # The ID of the request.
         self.api_ids = api_ids  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
+        # *   This API is intended for API providers.
+        # *   This API allows you to bind a specific throttling policy to up to 100 APIs at a time.
         self.stage_name = stage_name  # type: str
+        # The API ID for the specified operation. Separate multiple API IDs with commas (,). A maximum of 100 API IDs can be entered.
         self.traffic_control_id = traffic_control_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetTrafficControlApisRequest, self).to_map()
@@ -30123,14 +35397,15 @@
         if m.get('TrafficControlId') is not None:
             self.traffic_control_id = m.get('TrafficControlId')
         return self
 
 
 class SetTrafficControlApisResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Binds a throttling policy to APIs.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SetTrafficControlApisResponseBody, self).to_map()
@@ -30407,19 +35682,31 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SwitchApiRequest(TeaModel):
     def __init__(self, api_id=None, description=None, group_id=None, history_version=None, security_token=None,
                  stage_name=None):
+        # The description of the switch operation.
         self.api_id = api_id  # type: str
+        # The ID of the request.
         self.description = description  # type: str
-        self.group_id = group_id  # type: str
+        # The name of the runtime environment. Valid values:
+        # 
+        # *   **RELEASE**\
+        # *   **TEST**\
+        self.group_id = group_id  # type: str
+        # *   This API is intended for API providers.
+        # *   The historical version can be obtained through the DescribeHistoryApis API.****\
+        # *   Only APIs that have been published more than once have historical versions to switch to.
+        # *   This operation can only be performed on running APIs. Use caution when performing this operation because the operation cannot be undone after it has been completed and takes effect within 5 seconds.
+        # *   The switch operation is in essence a publish operation, and the reason for this operation must be provided.
         self.history_version = history_version  # type: str
         self.security_token = security_token  # type: str
+        # The historical version you want to switch to.
         self.stage_name = stage_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SwitchApiRequest, self).to_map()
@@ -30456,14 +35743,15 @@
         if m.get('StageName') is not None:
             self.stage_name = m.get('StageName')
         return self
 
 
 class SwitchApiResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # Switches the definition of an API in a specified runtime environment to a historical version.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SwitchApiResponseBody, self).to_map()
@@ -30519,15 +35807,17 @@
             temp_model = SwitchApiResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TagResourcesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
+        # Adds tags to resources.
         self.key = key  # type: str
+        # TagResources
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(TagResourcesRequestTag, self).to_map()
@@ -30549,14 +35839,15 @@
             self.value = m.get('Value')
         return self
 
 
 class TagResourcesRequest(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, security_token=None, tag=None):
         self.resource_id = resource_id  # type: list[str]
+        # The operation that you want to perform. Set the value to **TagResources**.
         self.resource_type = resource_type  # type: str
         self.security_token = security_token  # type: str
         self.tag = tag  # type: list[TagResourcesRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
@@ -30658,16 +35949,20 @@
             temp_model = TagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UntagResourcesRequest(TeaModel):
     def __init__(self, all=None, resource_id=None, resource_type=None, security_token=None, tag_key=None):
+        # The ID of the request.
         self.all = all  # type: bool
         self.resource_id = resource_id  # type: list[str]
+        # The key of tag N.
+        # 
+        # Valid values of N: `1 to 20.`
         self.resource_type = resource_type  # type: str
         self.security_token = security_token  # type: str
         self.tag_key = tag_key  # type: list[str]
 
     def validate(self):
         pass
 
@@ -30702,14 +35997,15 @@
         if m.get('TagKey') is not None:
             self.tag_key = m.get('TagKey')
         return self
 
 
 class UntagResourcesResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # UntagResources
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UntagResourcesResponseBody, self).to_map()
@@ -30763,7 +36059,114 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ValidateVpcConnectivityRequest(TeaModel):
+    def __init__(self, instance_id=None, security_token=None, vpc_access_id=None):
+        self.instance_id = instance_id  # type: str
+        self.security_token = security_token  # type: str
+        self.vpc_access_id = vpc_access_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ValidateVpcConnectivityRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, connected=None, ip_type=None, request_id=None):
+        self.connected = connected  # type: bool
+        self.ip_type = ip_type  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ValidateVpcConnectivityResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ValidateVpcConnectivityResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ValidateVpcConnectivityResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO` & `alibabacloud_cloudapi20160714_py2-3.0.0/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudapi20160714-py2
-Version: 2.2.9
+Version: 3.0.0
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.9/setup.py` & `alibabacloud_cloudapi20160714_py2-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudapi20160714_py2.
 
-Created on 13/10/2022
+Created on 31/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudapi20160714"
 NAME = "alibabacloud_cloudapi20160714_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CloudAPI (20160714) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

