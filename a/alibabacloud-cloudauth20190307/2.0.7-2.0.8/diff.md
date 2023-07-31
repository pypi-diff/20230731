# Comparing `tmp/alibabacloud_cloudauth20190307-2.0.7.tar.gz` & `tmp/alibabacloud_cloudauth20190307-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.0.7.tar", last modified: Fri Jul 14 01:44:38 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cloudauth20190307-2.0.8.tar", last modified: Mon Jul 31 08:03:23 2023, max compression
```

## Comparing `alibabacloud_cloudauth20190307-2.0.7.tar` & `alibabacloud_cloudauth20190307-2.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/
--rw-r--r--   0 root         (0) root         (0)      801 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77649 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/client.py
--rw-r--r--   0 root         (0) root         (0)   129660 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 01:44:38.000000 alibabacloud_cloudauth20190307-2.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2837 2023-07-14 01:44:37.000000 alibabacloud_cloudauth20190307-2.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/
+-rw-r--r--   0 root         (0) root         (0)      846 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78731 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307/client.py
+-rw-r--r--   0 root         (0) root         (0)   131145 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-31 08:03:23.000000 alibabacloud_cloudauth20190307-2.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-07-31 08:03:22.000000 alibabacloud_cloudauth20190307-2.0.8/setup.py
```

### Comparing `alibabacloud_cloudauth20190307-2.0.7/ChangeLog.md` & `alibabacloud_cloudauth20190307-2.0.8/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-14 Version: 2.0.7
+- For 2019-03-07.
+
 2023-05-18 Version: 2.0.6
 - For 2019-03-07.
 
 2022-11-02 Version: 2.0.5
 - For 2019-03-07.
 
 2022-10-17 Version: 2.0.4
```

### Comparing `alibabacloud_cloudauth20190307-2.0.7/LICENSE` & `alibabacloud_cloudauth20190307-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.7/PKG-INFO` & `alibabacloud_cloudauth20190307-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudauth20190307
-Version: 2.0.7
+Version: 2.0.8
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.0.7/README-CN.md` & `alibabacloud_cloudauth20190307-2.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.7/README.md` & `alibabacloud_cloudauth20190307-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/client.py` & `alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1280,56 +1280,66 @@
     def init_face_verify_with_options(
         self,
         request: cloudauth_20190307_models.InitFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.InitFaceVerifyResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.birthday):
+            query['Birthday'] = request.birthday
         if not UtilClient.is_unset(request.callback_token):
             query['CallbackToken'] = request.callback_token
         if not UtilClient.is_unset(request.callback_url):
             query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.cert_name):
             query['CertName'] = request.cert_name
         if not UtilClient.is_unset(request.cert_no):
             query['CertNo'] = request.cert_no
         if not UtilClient.is_unset(request.cert_type):
             query['CertType'] = request.cert_type
         if not UtilClient.is_unset(request.certify_id):
             query['CertifyId'] = request.certify_id
+        if not UtilClient.is_unset(request.certify_url_style):
+            query['CertifyUrlStyle'] = request.certify_url_style
         if not UtilClient.is_unset(request.certify_url_type):
             query['CertifyUrlType'] = request.certify_url_type
         if not UtilClient.is_unset(request.encrypt_type):
             query['EncryptType'] = request.encrypt_type
         if not UtilClient.is_unset(request.face_contrast_picture_url):
             query['FaceContrastPictureUrl'] = request.face_contrast_picture_url
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.meta_info):
             query['MetaInfo'] = request.meta_info
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.mode):
+            query['Mode'] = request.mode
         if not UtilClient.is_unset(request.oss_bucket_name):
             query['OssBucketName'] = request.oss_bucket_name
         if not UtilClient.is_unset(request.oss_object_name):
             query['OssObjectName'] = request.oss_object_name
         if not UtilClient.is_unset(request.outer_order_no):
             query['OuterOrderNo'] = request.outer_order_no
         if not UtilClient.is_unset(request.procedure_priority):
             query['ProcedurePriority'] = request.procedure_priority
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
+        if not UtilClient.is_unset(request.read_img):
+            query['ReadImg'] = request.read_img
         if not UtilClient.is_unset(request.return_url):
             query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_id):
             query['SceneId'] = request.scene_id
         if not UtilClient.is_unset(request.suitable_type):
             query['SuitableType'] = request.suitable_type
         if not UtilClient.is_unset(request.user_id):
             query['UserId'] = request.user_id
+        if not UtilClient.is_unset(request.validity_date):
+            query['ValidityDate'] = request.validity_date
         if not UtilClient.is_unset(request.voluntary_customized_content):
             query['VoluntaryCustomizedContent'] = request.voluntary_customized_content
         body = {}
         if not UtilClient.is_unset(request.auth_id):
             body['AuthId'] = request.auth_id
         if not UtilClient.is_unset(request.crop):
             body['Crop'] = request.crop
@@ -1360,56 +1370,66 @@
     async def init_face_verify_with_options_async(
         self,
         request: cloudauth_20190307_models.InitFaceVerifyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudauth_20190307_models.InitFaceVerifyResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.birthday):
+            query['Birthday'] = request.birthday
         if not UtilClient.is_unset(request.callback_token):
             query['CallbackToken'] = request.callback_token
         if not UtilClient.is_unset(request.callback_url):
             query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.cert_name):
             query['CertName'] = request.cert_name
         if not UtilClient.is_unset(request.cert_no):
             query['CertNo'] = request.cert_no
         if not UtilClient.is_unset(request.cert_type):
             query['CertType'] = request.cert_type
         if not UtilClient.is_unset(request.certify_id):
             query['CertifyId'] = request.certify_id
+        if not UtilClient.is_unset(request.certify_url_style):
+            query['CertifyUrlStyle'] = request.certify_url_style
         if not UtilClient.is_unset(request.certify_url_type):
             query['CertifyUrlType'] = request.certify_url_type
         if not UtilClient.is_unset(request.encrypt_type):
             query['EncryptType'] = request.encrypt_type
         if not UtilClient.is_unset(request.face_contrast_picture_url):
             query['FaceContrastPictureUrl'] = request.face_contrast_picture_url
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.meta_info):
             query['MetaInfo'] = request.meta_info
         if not UtilClient.is_unset(request.mobile):
             query['Mobile'] = request.mobile
+        if not UtilClient.is_unset(request.mode):
+            query['Mode'] = request.mode
         if not UtilClient.is_unset(request.oss_bucket_name):
             query['OssBucketName'] = request.oss_bucket_name
         if not UtilClient.is_unset(request.oss_object_name):
             query['OssObjectName'] = request.oss_object_name
         if not UtilClient.is_unset(request.outer_order_no):
             query['OuterOrderNo'] = request.outer_order_no
         if not UtilClient.is_unset(request.procedure_priority):
             query['ProcedurePriority'] = request.procedure_priority
         if not UtilClient.is_unset(request.product_code):
             query['ProductCode'] = request.product_code
+        if not UtilClient.is_unset(request.read_img):
+            query['ReadImg'] = request.read_img
         if not UtilClient.is_unset(request.return_url):
             query['ReturnUrl'] = request.return_url
         if not UtilClient.is_unset(request.scene_id):
             query['SceneId'] = request.scene_id
         if not UtilClient.is_unset(request.suitable_type):
             query['SuitableType'] = request.suitable_type
         if not UtilClient.is_unset(request.user_id):
             query['UserId'] = request.user_id
+        if not UtilClient.is_unset(request.validity_date):
+            query['ValidityDate'] = request.validity_date
         if not UtilClient.is_unset(request.voluntary_customized_content):
             query['VoluntaryCustomizedContent'] = request.voluntary_customized_content
         body = {}
         if not UtilClient.is_unset(request.auth_id):
             body['AuthId'] = request.auth_id
         if not UtilClient.is_unset(request.crop):
             body['Crop'] = request.crop
```

### Comparing `alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307/models.py` & `alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1390,21 +1390,23 @@
         self,
         device_risk: str = None,
         device_token: str = None,
         identity_info: str = None,
         material_info: str = None,
         passed: str = None,
         sub_code: str = None,
+        success: str = None,
     ):
         self.device_risk = device_risk
         self.device_token = device_token
         self.identity_info = identity_info
         self.material_info = material_info
         self.passed = passed
         self.sub_code = sub_code
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1419,14 +1421,16 @@
             result['IdentityInfo'] = self.identity_info
         if self.material_info is not None:
             result['MaterialInfo'] = self.material_info
         if self.passed is not None:
             result['Passed'] = self.passed
         if self.sub_code is not None:
             result['SubCode'] = self.sub_code
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DeviceRisk') is not None:
             self.device_risk = m.get('DeviceRisk')
         if m.get('DeviceToken') is not None:
@@ -1435,14 +1439,16 @@
             self.identity_info = m.get('IdentityInfo')
         if m.get('MaterialInfo') is not None:
             self.material_info = m.get('MaterialInfo')
         if m.get('Passed') is not None:
             self.passed = m.get('Passed')
         if m.get('SubCode') is not None:
             self.sub_code = m.get('SubCode')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class DescribeFaceVerifyResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -2767,90 +2773,104 @@
         return self
 
 
 class InitFaceVerifyRequest(TeaModel):
     def __init__(
         self,
         auth_id: str = None,
+        birthday: str = None,
         callback_token: str = None,
         callback_url: str = None,
         cert_name: str = None,
         cert_no: str = None,
         cert_type: str = None,
         certify_id: str = None,
+        certify_url_style: str = None,
         certify_url_type: str = None,
         crop: str = None,
         encrypt_type: str = None,
         face_contrast_picture: str = None,
         face_contrast_picture_url: str = None,
         ip: str = None,
         meta_info: str = None,
         mobile: str = None,
+        mode: str = None,
         model: str = None,
         oss_bucket_name: str = None,
         oss_object_name: str = None,
         outer_order_no: str = None,
         procedure_priority: str = None,
         product_code: str = None,
+        read_img: str = None,
         return_url: str = None,
         scene_id: int = None,
         suitable_type: str = None,
         user_id: str = None,
+        validity_date: str = None,
         voluntary_customized_content: str = None,
     ):
         self.auth_id = auth_id
+        self.birthday = birthday
         self.callback_token = callback_token
         self.callback_url = callback_url
         self.cert_name = cert_name
         self.cert_no = cert_no
         self.cert_type = cert_type
         self.certify_id = certify_id
+        self.certify_url_style = certify_url_style
         self.certify_url_type = certify_url_type
         self.crop = crop
         self.encrypt_type = encrypt_type
         self.face_contrast_picture = face_contrast_picture
         self.face_contrast_picture_url = face_contrast_picture_url
         self.ip = ip
         self.meta_info = meta_info
         self.mobile = mobile
+        self.mode = mode
         self.model = model
         self.oss_bucket_name = oss_bucket_name
         self.oss_object_name = oss_object_name
         self.outer_order_no = outer_order_no
         self.procedure_priority = procedure_priority
         self.product_code = product_code
+        self.read_img = read_img
         self.return_url = return_url
         self.scene_id = scene_id
         self.suitable_type = suitable_type
         self.user_id = user_id
+        self.validity_date = validity_date
         self.voluntary_customized_content = voluntary_customized_content
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_id is not None:
             result['AuthId'] = self.auth_id
+        if self.birthday is not None:
+            result['Birthday'] = self.birthday
         if self.callback_token is not None:
             result['CallbackToken'] = self.callback_token
         if self.callback_url is not None:
             result['CallbackUrl'] = self.callback_url
         if self.cert_name is not None:
             result['CertName'] = self.cert_name
         if self.cert_no is not None:
             result['CertNo'] = self.cert_no
         if self.cert_type is not None:
             result['CertType'] = self.cert_type
         if self.certify_id is not None:
             result['CertifyId'] = self.certify_id
+        if self.certify_url_style is not None:
+            result['CertifyUrlStyle'] = self.certify_url_style
         if self.certify_url_type is not None:
             result['CertifyUrlType'] = self.certify_url_type
         if self.crop is not None:
             result['Crop'] = self.crop
         if self.encrypt_type is not None:
             result['EncryptType'] = self.encrypt_type
         if self.face_contrast_picture is not None:
@@ -2859,54 +2879,64 @@
             result['FaceContrastPictureUrl'] = self.face_contrast_picture_url
         if self.ip is not None:
             result['Ip'] = self.ip
         if self.meta_info is not None:
             result['MetaInfo'] = self.meta_info
         if self.mobile is not None:
             result['Mobile'] = self.mobile
+        if self.mode is not None:
+            result['Mode'] = self.mode
         if self.model is not None:
             result['Model'] = self.model
         if self.oss_bucket_name is not None:
             result['OssBucketName'] = self.oss_bucket_name
         if self.oss_object_name is not None:
             result['OssObjectName'] = self.oss_object_name
         if self.outer_order_no is not None:
             result['OuterOrderNo'] = self.outer_order_no
         if self.procedure_priority is not None:
             result['ProcedurePriority'] = self.procedure_priority
         if self.product_code is not None:
             result['ProductCode'] = self.product_code
+        if self.read_img is not None:
+            result['ReadImg'] = self.read_img
         if self.return_url is not None:
             result['ReturnUrl'] = self.return_url
         if self.scene_id is not None:
             result['SceneId'] = self.scene_id
         if self.suitable_type is not None:
             result['SuitableType'] = self.suitable_type
         if self.user_id is not None:
             result['UserId'] = self.user_id
+        if self.validity_date is not None:
+            result['ValidityDate'] = self.validity_date
         if self.voluntary_customized_content is not None:
             result['VoluntaryCustomizedContent'] = self.voluntary_customized_content
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AuthId') is not None:
             self.auth_id = m.get('AuthId')
+        if m.get('Birthday') is not None:
+            self.birthday = m.get('Birthday')
         if m.get('CallbackToken') is not None:
             self.callback_token = m.get('CallbackToken')
         if m.get('CallbackUrl') is not None:
             self.callback_url = m.get('CallbackUrl')
         if m.get('CertName') is not None:
             self.cert_name = m.get('CertName')
         if m.get('CertNo') is not None:
             self.cert_no = m.get('CertNo')
         if m.get('CertType') is not None:
             self.cert_type = m.get('CertType')
         if m.get('CertifyId') is not None:
             self.certify_id = m.get('CertifyId')
+        if m.get('CertifyUrlStyle') is not None:
+            self.certify_url_style = m.get('CertifyUrlStyle')
         if m.get('CertifyUrlType') is not None:
             self.certify_url_type = m.get('CertifyUrlType')
         if m.get('Crop') is not None:
             self.crop = m.get('Crop')
         if m.get('EncryptType') is not None:
             self.encrypt_type = m.get('EncryptType')
         if m.get('FaceContrastPicture') is not None:
@@ -2915,34 +2945,40 @@
             self.face_contrast_picture_url = m.get('FaceContrastPictureUrl')
         if m.get('Ip') is not None:
             self.ip = m.get('Ip')
         if m.get('MetaInfo') is not None:
             self.meta_info = m.get('MetaInfo')
         if m.get('Mobile') is not None:
             self.mobile = m.get('Mobile')
+        if m.get('Mode') is not None:
+            self.mode = m.get('Mode')
         if m.get('Model') is not None:
             self.model = m.get('Model')
         if m.get('OssBucketName') is not None:
             self.oss_bucket_name = m.get('OssBucketName')
         if m.get('OssObjectName') is not None:
             self.oss_object_name = m.get('OssObjectName')
         if m.get('OuterOrderNo') is not None:
             self.outer_order_no = m.get('OuterOrderNo')
         if m.get('ProcedurePriority') is not None:
             self.procedure_priority = m.get('ProcedurePriority')
         if m.get('ProductCode') is not None:
             self.product_code = m.get('ProductCode')
+        if m.get('ReadImg') is not None:
+            self.read_img = m.get('ReadImg')
         if m.get('ReturnUrl') is not None:
             self.return_url = m.get('ReturnUrl')
         if m.get('SceneId') is not None:
             self.scene_id = m.get('SceneId')
         if m.get('SuitableType') is not None:
             self.suitable_type = m.get('SuitableType')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
+        if m.get('ValidityDate') is not None:
+            self.validity_date = m.get('ValidityDate')
         if m.get('VoluntaryCustomizedContent') is not None:
             self.voluntary_customized_content = m.get('VoluntaryCustomizedContent')
         return self
 
 
 class InitFaceVerifyResponseBodyResultObject(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_cloudauth20190307-2.0.7/alibabacloud_cloudauth20190307.egg-info/PKG-INFO` & `alibabacloud_cloudauth20190307-2.0.8/alibabacloud_cloudauth20190307.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudauth20190307
-Version: 2.0.7
+Version: 2.0.8
 Summary: Alibaba Cloud ID Verification (20190307) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudauth20190307-2.0.7/setup.py` & `alibabacloud_cloudauth20190307-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudauth20190307.
 
-Created on 14/07/2023
+Created on 31/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudauth20190307"
 NAME = "alibabacloud_cloudauth20190307" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ID Verification (20190307) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
```

