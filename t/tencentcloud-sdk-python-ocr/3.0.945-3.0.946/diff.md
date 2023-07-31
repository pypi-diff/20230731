# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.945.tar", last modified: Fri Jul 28 00:32:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.946.tar", last modified: Mon Jul 31 00:33:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.945.tar` & `tencentcloud-sdk-python-ocr-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115943 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   821044 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:32:55.000000 tencentcloud-sdk-python-ocr-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   113546 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   807406 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:33:08.000000 tencentcloud-sdk-python-ocr-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/setup.py` & `tencentcloud-sdk-python-ocr-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,14 @@
 
 # Config不是有效的JSON格式。
 INVALIDPARAMETER_CONFIGFORMATERROR = 'InvalidParameter.ConfigFormatError'
 
 # 图片解码失败。
 INVALIDPARAMETER_ENGINEIMAGEDECODEFAILED = 'InvalidParameter.EngineImageDecodeFailed'
 
-# 无效的GTIN。
-INVALIDPARAMETER_INVALIDGTINERROR = 'InvalidParameter.InvalidGTINError'
-
 # 任务创建失败，文件URL非法。
 INVALIDPARAMETERVALUE_FILEURLILLEGALERROR = 'InvalidParameterValue.FileUrlIllegalError'
 
 # 参数值错误。
 INVALIDPARAMETERVALUE_INVALIDPARAMETERVALUELIMIT = 'InvalidParameterValue.InvalidParameterValueLimit'
 
 # 开票金额或校验码参数值错误。
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1353,41 +1353,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
-    def QueryBarCode(self, request):
-        """库源服务调整，该接口在2023年6月1日将正式下线。
-
-        本接口支持条形码备案信息查询，返回条形码查询结果的相关信息，包括产品名称、产品英文名称、品牌名称、规格型号、宽度、高度、深度、关键字、产品描述、厂家名称、厂家地址、企业社会信用代码13个字段信息。
-
-        产品优势：直联中国物品编码中心，查询结果更加准确、可靠。
-
-        :param request: Request instance for QueryBarCode.
-        :type request: :class:`tencentcloud.ocr.v20181119.models.QueryBarCodeRequest`
-        :rtype: :class:`tencentcloud.ocr.v20181119.models.QueryBarCodeResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("QueryBarCode", params, headers=headers)
-            response = json.loads(body)
-            model = models.QueryBarCodeResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
     def QuotaInvoiceOCR(self, request):
         """本接口支持定额发票的发票号码、发票代码、金额(大小写)、发票消费类型、地区及是否有公司印章等关键字段的识别。
 
         默认接口请求频率限制：5次/秒。
 
         :param request: Request instance for QuotaInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.QuotaInvoiceOCRRequest`
@@ -2421,39 +2394,14 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
-
-
-    def VerifyEnterpriseFourFactors(self, request):
-        """库源服务调整，该接口在2023年6月1日将正式下线。
-
-        此接口基于企业四要素授权“姓名、证件号码、企业标识、企业全称”，验证企业信息是否一致。
-
-        :param request: Request instance for VerifyEnterpriseFourFactors.
-        :type request: :class:`tencentcloud.ocr.v20181119.models.VerifyEnterpriseFourFactorsRequest`
-        :rtype: :class:`tencentcloud.ocr.v20181119.models.VerifyEnterpriseFourFactorsResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("VerifyEnterpriseFourFactors", params, headers=headers)
-            response = json.loads(body)
-            model = models.VerifyEnterpriseFourFactorsResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def VerifyOfdVatInvoiceOCR(self, request):
         """本接口支持OFD格式的增值税电子普通发票和增值税电子专用发票的识别，返回发票代码、发票号码、开票日期、验证码、机器编号、密码区，购买方和销售方信息，包括名称、纳税人识别号、地址电话、开户行及账号，以及价税合计、开票人、收款人、复核人、税额、不含税金额等字段信息。
 
         :param request: Request instance for VerifyOfdVatInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.VerifyOfdVatInvoiceOCRRequest`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.946/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2734,59 +2734,14 @@
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._OperateUrl = params.get("OperateUrl")
         self._RequestId = params.get("RequestId")
 
 
-class Detail(AbstractModel):
-    """企业四要素核验结果
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Result: 企业四要素核验结果状态码
-        :type Result: int
-        :param _Desc: 企业四要素核验结果描述
-        :type Desc: str
-        """
-        self._Result = None
-        self._Desc = None
-
-    @property
-    def Result(self):
-        return self._Result
-
-    @Result.setter
-    def Result(self, Result):
-        self._Result = Result
-
-    @property
-    def Desc(self):
-        return self._Desc
-
-    @Desc.setter
-    def Desc(self, Desc):
-        self._Desc = Desc
-
-
-    def _deserialize(self, params):
-        self._Result = params.get("Result")
-        self._Desc = params.get("Desc")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class DetectedWordCoordPoint(AbstractModel):
     """单字在原图中的坐标，以四个顶点坐标表示，以左上角为起点，顺时针返回。
 
     """
 
     def __init__(self):
         r"""
@@ -11454,234 +11409,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ProductDataRecord(AbstractModel):
-    """商品码信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ProductName: 产品名称
-        :type ProductName: str
-        :param _EnName: 产品名称(英文)
-        :type EnName: str
-        :param _BrandName: 品牌名称
-        :type BrandName: str
-        :param _Type: 规格型号
-        :type Type: str
-        :param _Width: 宽度，单位毫米
-        :type Width: str
-        :param _Height: 高度，单位毫米
-        :type Height: str
-        :param _Depth: 深度，单位毫米
-        :type Depth: str
-        :param _KeyWord: 关键字
-        :type KeyWord: str
-        :param _Description: 简短描述
-        :type Description: str
-        :param _ImageLink: 图片链接
-        :type ImageLink: list of str
-        :param _ManufacturerName: 厂家名称
-        :type ManufacturerName: str
-        :param _ManufacturerAddress: 厂家地址
-        :type ManufacturerAddress: str
-        :param _FirmCode: 企业社会信用代码
-        :type FirmCode: str
-        :param _CheckResult: 表示数据查询状态
-checkResult	状态说明
-1	 经查，该商品条码已在中国物品编码中心注册
-2	经查，该厂商识别代码已在中国物品编码中心注册，但编码信息未按规定通报。
-3	经查，该厂商识别代码已于xxxxx注销，请关注产品生产日期。
-4	经查，该企业以及条码未经条码中心注册，属于违法使用
--1	经查，该商品条码被冒用
--2	经查，该厂商识别代码已在中国物品编码中心注册，但该产品已经下市
-S001                未找到该厂商识别代码的注册信息。
-S002		该厂商识别代码已经在GS1注册，但编码信息未通报
-S003		该商品条码已在GS1通报
-S004		该商品条码已注销
-S005		数字不正确。GS1前缀（3位国家/地区代码）用于特殊用途。
-E001		完整性失败：此GTIN的长度无效。
-E002		完整性失败：校验位不正确。
-E003		完整性失败：字符串包含字母数字字符。
-E004		数字不正确。GS1前缀（3位国家/地区代码）不存在。
-E005		数字不正确。GS1前缀（3位国家/地区代码）用于特殊用途。
-E006		数字不正确。尚未分配该GS1公司前缀。
-E008	        经查，该企业厂商识别代码以及条码尚未通报
-        :type CheckResult: str
-        :param _CategoryCode: UNSPSC分类码
-        :type CategoryCode: str
-        """
-        self._ProductName = None
-        self._EnName = None
-        self._BrandName = None
-        self._Type = None
-        self._Width = None
-        self._Height = None
-        self._Depth = None
-        self._KeyWord = None
-        self._Description = None
-        self._ImageLink = None
-        self._ManufacturerName = None
-        self._ManufacturerAddress = None
-        self._FirmCode = None
-        self._CheckResult = None
-        self._CategoryCode = None
-
-    @property
-    def ProductName(self):
-        return self._ProductName
-
-    @ProductName.setter
-    def ProductName(self, ProductName):
-        self._ProductName = ProductName
-
-    @property
-    def EnName(self):
-        return self._EnName
-
-    @EnName.setter
-    def EnName(self, EnName):
-        self._EnName = EnName
-
-    @property
-    def BrandName(self):
-        return self._BrandName
-
-    @BrandName.setter
-    def BrandName(self, BrandName):
-        self._BrandName = BrandName
-
-    @property
-    def Type(self):
-        return self._Type
-
-    @Type.setter
-    def Type(self, Type):
-        self._Type = Type
-
-    @property
-    def Width(self):
-        return self._Width
-
-    @Width.setter
-    def Width(self, Width):
-        self._Width = Width
-
-    @property
-    def Height(self):
-        return self._Height
-
-    @Height.setter
-    def Height(self, Height):
-        self._Height = Height
-
-    @property
-    def Depth(self):
-        return self._Depth
-
-    @Depth.setter
-    def Depth(self, Depth):
-        self._Depth = Depth
-
-    @property
-    def KeyWord(self):
-        return self._KeyWord
-
-    @KeyWord.setter
-    def KeyWord(self, KeyWord):
-        self._KeyWord = KeyWord
-
-    @property
-    def Description(self):
-        return self._Description
-
-    @Description.setter
-    def Description(self, Description):
-        self._Description = Description
-
-    @property
-    def ImageLink(self):
-        return self._ImageLink
-
-    @ImageLink.setter
-    def ImageLink(self, ImageLink):
-        self._ImageLink = ImageLink
-
-    @property
-    def ManufacturerName(self):
-        return self._ManufacturerName
-
-    @ManufacturerName.setter
-    def ManufacturerName(self, ManufacturerName):
-        self._ManufacturerName = ManufacturerName
-
-    @property
-    def ManufacturerAddress(self):
-        return self._ManufacturerAddress
-
-    @ManufacturerAddress.setter
-    def ManufacturerAddress(self, ManufacturerAddress):
-        self._ManufacturerAddress = ManufacturerAddress
-
-    @property
-    def FirmCode(self):
-        return self._FirmCode
-
-    @FirmCode.setter
-    def FirmCode(self, FirmCode):
-        self._FirmCode = FirmCode
-
-    @property
-    def CheckResult(self):
-        return self._CheckResult
-
-    @CheckResult.setter
-    def CheckResult(self, CheckResult):
-        self._CheckResult = CheckResult
-
-    @property
-    def CategoryCode(self):
-        return self._CategoryCode
-
-    @CategoryCode.setter
-    def CategoryCode(self, CategoryCode):
-        self._CategoryCode = CategoryCode
-
-
-    def _deserialize(self, params):
-        self._ProductName = params.get("ProductName")
-        self._EnName = params.get("EnName")
-        self._BrandName = params.get("BrandName")
-        self._Type = params.get("Type")
-        self._Width = params.get("Width")
-        self._Height = params.get("Height")
-        self._Depth = params.get("Depth")
-        self._KeyWord = params.get("KeyWord")
-        self._Description = params.get("Description")
-        self._ImageLink = params.get("ImageLink")
-        self._ManufacturerName = params.get("ManufacturerName")
-        self._ManufacturerAddress = params.get("ManufacturerAddress")
-        self._FirmCode = params.get("FirmCode")
-        self._CheckResult = params.get("CheckResult")
-        self._CategoryCode = params.get("CategoryCode")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class PropOwnerCertOCRRequest(AbstractModel):
     """PropOwnerCertOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12107,101 +11842,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class QueryBarCodeRequest(AbstractModel):
-    """QueryBarCode请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _BarCode: 条形码
-        :type BarCode: str
-        """
-        self._BarCode = None
-
-    @property
-    def BarCode(self):
-        return self._BarCode
-
-    @BarCode.setter
-    def BarCode(self, BarCode):
-        self._BarCode = BarCode
-
-
-    def _deserialize(self, params):
-        self._BarCode = params.get("BarCode")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class QueryBarCodeResponse(AbstractModel):
-    """QueryBarCode返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _BarCode: 条码
-        :type BarCode: str
-        :param _ProductDataRecords: 条码信息数组
-        :type ProductDataRecords: list of ProductDataRecord
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._BarCode = None
-        self._ProductDataRecords = None
-        self._RequestId = None
-
-    @property
-    def BarCode(self):
-        return self._BarCode
-
-    @BarCode.setter
-    def BarCode(self, BarCode):
-        self._BarCode = BarCode
-
-    @property
-    def ProductDataRecords(self):
-        return self._ProductDataRecords
-
-    @ProductDataRecords.setter
-    def ProductDataRecords(self, ProductDataRecords):
-        self._ProductDataRecords = ProductDataRecords
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._BarCode = params.get("BarCode")
-        if params.get("ProductDataRecords") is not None:
-            self._ProductDataRecords = []
-            for item in params.get("ProductDataRecords"):
-                obj = ProductDataRecord()
-                obj._deserialize(item)
-                self._ProductDataRecords.append(obj)
-        self._RequestId = params.get("RequestId")
-
-
 class QuestionBlockObj(AbstractModel):
     """数学试题识别结构化对象
 
     """
 
     def __init__(self):
         r"""
@@ -26467,136 +26115,14 @@
         self._Address = params.get("Address")
         if params.get("RegNumResult") is not None:
             self._RegNumResult = BizLicenseVerifyResult()
             self._RegNumResult._deserialize(params.get("RegNumResult"))
         self._RequestId = params.get("RequestId")
 
 
-class VerifyEnterpriseFourFactorsRequest(AbstractModel):
-    """VerifyEnterpriseFourFactors请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RealName: 姓名
-        :type RealName: str
-        :param _IdCard: 证件号码（公司注册证件号）
-        :type IdCard: str
-        :param _EnterpriseName: 企业全称
-        :type EnterpriseName: str
-        :param _EnterpriseMark: 企业标识（注册号，统一社会信用代码）
-        :type EnterpriseMark: str
-        """
-        self._RealName = None
-        self._IdCard = None
-        self._EnterpriseName = None
-        self._EnterpriseMark = None
-
-    @property
-    def RealName(self):
-        return self._RealName
-
-    @RealName.setter
-    def RealName(self, RealName):
-        self._RealName = RealName
-
-    @property
-    def IdCard(self):
-        return self._IdCard
-
-    @IdCard.setter
-    def IdCard(self, IdCard):
-        self._IdCard = IdCard
-
-    @property
-    def EnterpriseName(self):
-        return self._EnterpriseName
-
-    @EnterpriseName.setter
-    def EnterpriseName(self, EnterpriseName):
-        self._EnterpriseName = EnterpriseName
-
-    @property
-    def EnterpriseMark(self):
-        return self._EnterpriseMark
-
-    @EnterpriseMark.setter
-    def EnterpriseMark(self, EnterpriseMark):
-        self._EnterpriseMark = EnterpriseMark
-
-
-    def _deserialize(self, params):
-        self._RealName = params.get("RealName")
-        self._IdCard = params.get("IdCard")
-        self._EnterpriseName = params.get("EnterpriseName")
-        self._EnterpriseMark = params.get("EnterpriseMark")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class VerifyEnterpriseFourFactorsResponse(AbstractModel):
-    """VerifyEnterpriseFourFactors返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _State: 核验一致性（1:一致，2:不一致，3:查询无记录）
-        :type State: int
-        :param _Detail: 核验结果明细，7：企业法人/负责人，6：企业股东，5：企
-业管理人员，-21：企业名称与企业标识不符，-22：姓名不一致，-23：证件号码不一致，-24：企业名称不一致，-25：企业标识不一致
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Detail: :class:`tencentcloud.ocr.v20181119.models.Detail`
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._State = None
-        self._Detail = None
-        self._RequestId = None
-
-    @property
-    def State(self):
-        return self._State
-
-    @State.setter
-    def State(self, State):
-        self._State = State
-
-    @property
-    def Detail(self):
-        return self._Detail
-
-    @Detail.setter
-    def Detail(self, Detail):
-        self._Detail = Detail
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._State = params.get("State")
-        if params.get("Detail") is not None:
-            self._Detail = Detail()
-            self._Detail._deserialize(params.get("Detail"))
-        self._RequestId = params.get("RequestId")
-
-
 class VerifyOfdVatInvoiceOCRRequest(AbstractModel):
     """VerifyOfdVatInvoiceOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.946/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.946/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.945/README.rst` & `tencentcloud-sdk-python-ocr-3.0.946/README.rst`

 * *Files identical despite different names*

