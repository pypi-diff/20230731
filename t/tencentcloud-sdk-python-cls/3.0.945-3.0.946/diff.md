# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.945.tar", last modified: Fri Jul 28 00:24:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.946.tar", last modified: Mon Jul 31 00:23:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.945.tar` & `tencentcloud-sdk-python-cls-3.0.946.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)    81890 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9048 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   499532 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-28 00:24:50.000000 tencentcloud-sdk-python-cls-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)    81890 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9048 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   499514 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-31 00:23:02.000000 tencentcloud-sdk-python-cls-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-31 00:23:01.000000 tencentcloud-sdk-python-cls-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-cls-3.0.945/setup.py` & `tencentcloud-sdk-python-cls-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4539,35 +4539,35 @@
 
     def __init__(self):
         r"""
         :param _SrcTopicId: 源日志主题
         :type SrcTopicId: str
         :param _Name: 任务名称
         :type Name: str
-        :param _EnableFlag: 任务启动状态.  1正常开启,  2关闭
+        :param _EnableFlag: 任务启动状态.  1开启,  2关闭
         :type EnableFlag: int
         :param _DstResource: 定时SQL分析目标日志主题
         :type DstResource: :class:`tencentcloud.cls.v20201016.models.ScheduledSqlResouceInfo`
         :param _ScheduledSqlContent: 查询语句
         :type ScheduledSqlContent: str
         :param _ProcessStartTime: 调度开始时间,Unix时间戳，单位ms
         :type ProcessStartTime: int
-        :param _ProcessType: 调度类型，1:持续运行 2:指定调度结束时间
+        :param _ProcessType: 调度类型，1:持续运行 2:指定时间范围
         :type ProcessType: int
         :param _ProcessPeriod: 调度周期(分钟)
         :type ProcessPeriod: int
         :param _ProcessTimeWindow: 单次查询的时间窗口
         :type ProcessTimeWindow: str
         :param _ProcessDelay: 执行延迟(秒)
         :type ProcessDelay: int
         :param _SrcTopicRegion: 源topicId的地域信息
         :type SrcTopicRegion: str
         :param _ProcessEndTime: 调度结束时间，当ProcessType=2时为必传字段, Unix时间戳，单位ms
         :type ProcessEndTime: int
-        :param _SyntaxRule: 语法规则。 默认值为0。0：Lucene语法，1：CQL语法  
+        :param _SyntaxRule: 查询语法规则。 默认值为0。0：Lucene语法，1：CQL语法  
         :type SyntaxRule: int
         """
         self._SrcTopicId = None
         self._Name = None
         self._EnableFlag = None
         self._DstResource = None
         self._ScheduledSqlContent = None
@@ -14083,15 +14083,15 @@
 
     def __init__(self):
         r"""
         :param _TaskId: 任务ID
         :type TaskId: str
         :param _SrcTopicId: 源日志主题
         :type SrcTopicId: str
-        :param _EnableFlag: 任务启动状态.   1正常开启,  2关闭
+        :param _EnableFlag: 任务启动状态.   1开启,  2关闭
         :type EnableFlag: int
         :param _DstResource: 定时SQL分析的目标日志主题
         :type DstResource: :class:`tencentcloud.cls.v20201016.models.ScheduledSqlResouceInfo`
         :param _ScheduledSqlContent: 查询语句
         :type ScheduledSqlContent: str
         :param _ProcessPeriod: 调度周期(分钟)
         :type ProcessPeriod: int
@@ -15743,15 +15743,15 @@
         :type Status: int
         :param _EnableFlag: 任务启用状态，1开启,  2关闭
         :type EnableFlag: int
         :param _ScheduledSqlContent: 查询语句
         :type ScheduledSqlContent: str
         :param _ProcessStartTime: 调度开始时间
         :type ProcessStartTime: str
-        :param _ProcessType: 调度类型，1:持续运行 2:指定调度结束时间
+        :param _ProcessType: 调度类型，1:持续运行 2:指定时间范围
         :type ProcessType: int
         :param _ProcessEndTime: 调度结束时间，当process_type=2时为必传字段
         :type ProcessEndTime: str
         :param _ProcessPeriod: 调度周期(分钟)
         :type ProcessPeriod: int
         :param _ProcessTimeWindow: 查询的时间窗口. @m-15m, @m，意为近15分钟
         :type ProcessTimeWindow: str
```

### Comparing `tencentcloud-sdk-python-cls-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.945/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.946/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.946/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.945/README.rst` & `tencentcloud-sdk-python-cls-3.0.946/README.rst`

 * *Files identical despite different names*

