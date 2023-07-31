# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.945.tar", last modified: Fri Jul 28 00:24:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.946.tar", last modified: Mon Jul 31 00:22:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.945.tar` & `tencentcloud-sdk-python-clb-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89989 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)   508306 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:24:28.000000 tencentcloud-sdk-python-clb-3.0.945/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89989 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)   507898 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:22:42.000000 tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-clb-3.0.945/setup.py` & `tencentcloud-sdk-python-clb-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.945/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3196,17 +3196,16 @@
 注意：当指定VIP创建内网实例、或公网IPv6 BGP实例时，若VIP不属于指定VPC子网的网段内时，会创建失败；若VIP已被占用，也会创建失败。
         :type Vip: str
         :param _BandwidthPackageId: 带宽包ID，指定此参数时，网络计费方式（InternetAccessible.InternetChargeType）只支持按带宽包计费（BANDWIDTH_PACKAGE）。
         :type BandwidthPackageId: str
         :param _ExclusiveCluster: 独占型实例信息。若创建独占型的内网负载均衡实例，则此参数必填。
         :type ExclusiveCluster: :class:`tencentcloud.clb.v20180317.models.ExclusiveCluster`
         :param _SlaType: 创建性能容量型实例。
-<ul><li>若需要创建性能容量型实例，则此参数必填，且取值为：SLA，表示创建按量计费模式下的默认规格的性能容量型实例。
-<ul><li>默认为普通规格的性能容量型实例，SLA对应超强型1规格。
-<li>当您开通了超大型规格的性能容量型时，SLA对应超强型4规格。超大型规格的性能容量型正在内测中，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category)。</li></ul></li><li>若需要创建共享型实例，则无需填写此参数。</li></ul>
+<ul><li>若需要创建性能容量型实例，则此参数必填，且取值为：SLA，表示超强型1规格。
+<ul><li>当您开通了超大型规格的性能容量型时，SLA对应超强型4规格。如需超大型规格的性能容量型，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category)。</li></ul></li><li>若需要创建共享型实例，则无需填写此参数。</li></ul>
         :type SlaType: str
         :param _ClientToken: 用于保证请求幂等性的字符串。该字符串由客户生成，需保证不同请求之间唯一，最大值不超过64个ASCII字符。若不指定该参数，则无法保证请求的幂等性。
         :type ClientToken: str
         :param _SnatPro: 是否支持绑定跨地域/跨Vpc绑定IP的功能。
         :type SnatPro: bool
         :param _SnatIps: 开启绑定跨地域/跨Vpc绑定IP的功能后，创建SnatIp。
         :type SnatIps: list of SnatIp
@@ -15367,17 +15366,16 @@
 
     """
 
     def __init__(self):
         r"""
         :param _LoadBalancerId: lb的字符串ID
         :type LoadBalancerId: str
-        :param _SlaType: 升级为性能容量型，固定取值为SLA。SLA表示升级为默认规格的性能容量型实例。
-<ul><li>当您开通了普通规格的性能容量型时，SLA对应超强型1规格。普通规格的性能容量型正在内测中，请提交 [内测申请](https://cloud.tencent.com/apply/p/hf45esx99lf)。</li>
-<li>当您开通了超大型规格的性能容量型时，SLA对应超强型4规格。超大型规格的性能容量型正在内测中，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category)。</li></ul>
+        :param _SlaType: 升级为性能容量型，固定取值为SLA。SLA表示超强型1规格。
+当您开通了超大型规格的性能容量型时，SLA对应超强型4规格。如需超大型规格的性能容量型，请提交[工单申请](https://console.cloud.tencent.com/workorder/category)。
         :type SlaType: str
         """
         self._LoadBalancerId = None
         self._SlaType = None
 
     @property
     def LoadBalancerId(self):
```

### Comparing `tencentcloud-sdk-python-clb-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.946/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.945/README.rst` & `tencentcloud-sdk-python-clb-3.0.946/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.945/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.946/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

