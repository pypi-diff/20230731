# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.945.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.945.tar", last modified: Fri Jul 28 00:37:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.946.tar", last modified: Mon Jul 31 00:38:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.945.tar` & `tencentcloud-sdk-python-tione-3.0.946.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51244 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12673 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   531149 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22102 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   144266 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-28 00:37:45.000000 tencentcloud-sdk-python-tione-3.0.945/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    62673 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15130 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   609461 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22102 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   144266 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-31 00:38:05.000000 tencentcloud-sdk-python-tione-3.0.946/README.rst
```

### Comparing `tencentcloud-sdk-python-tione-3.0.945/setup.py` & `tencentcloud-sdk-python-tione-3.0.946/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/tione_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,14 +114,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateNotebook(self, request):
+        """创建Notebook
+
+        :param request: Request instance for CreateNotebook.
+        :type request: :class:`tencentcloud.tione.v20211111.models.CreateNotebookRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.CreateNotebookResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateNotebook", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateNotebookResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def CreateNotebookImage(self, request):
+        """保存镜像
+
+        :param request: Request instance for CreateNotebookImage.
+        :type request: :class:`tencentcloud.tione.v20211111.models.CreateNotebookImageRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.CreateNotebookImageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateNotebookImage", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateNotebookImageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateOptimizedModel(self, request):
         """保存优化模型
 
         :param request: Request instance for CreateOptimizedModel.
         :type request: :class:`tencentcloud.tione.v20211111.models.CreateOptimizedModelRequest`
         :rtype: :class:`tencentcloud.tione.v20211111.models.CreateOptimizedModelResponse`
 
@@ -298,14 +344,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DeleteNotebook(self, request):
+        """删除Notebook
+
+        :param request: Request instance for DeleteNotebook.
+        :type request: :class:`tencentcloud.tione.v20211111.models.DeleteNotebookRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.DeleteNotebookResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteNotebook", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteNotebookResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DeleteNotebookImageRecord(self, request):
+        """删除notebook镜像保存记录
+
+        :param request: Request instance for DeleteNotebookImageRecord.
+        :type request: :class:`tencentcloud.tione.v20211111.models.DeleteNotebookImageRecordRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.DeleteNotebookImageRecordResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteNotebookImageRecord", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteNotebookImageRecordResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DeleteTrainingModel(self, request):
         """删除模型
 
         :param request: Request instance for DeleteTrainingModel.
         :type request: :class:`tencentcloud.tione.v20211111.models.DeleteTrainingModelRequest`
         :rtype: :class:`tencentcloud.tione.v20211111.models.DeleteTrainingModelResponse`
 
@@ -896,14 +988,106 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeNotebook(self, request):
+        """Notebook详情
+
+        :param request: Request instance for DescribeNotebook.
+        :type request: :class:`tencentcloud.tione.v20211111.models.DescribeNotebookRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.DescribeNotebookResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeNotebook", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeNotebookResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeNotebookImageKernels(self, request):
+        """查询镜像kernel
+
+        :param request: Request instance for DescribeNotebookImageKernels.
+        :type request: :class:`tencentcloud.tione.v20211111.models.DescribeNotebookImageKernelsRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.DescribeNotebookImageKernelsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeNotebookImageKernels", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeNotebookImageKernelsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeNotebookImageRecords(self, request):
+        """查看notebook镜像保存记录
+
+        :param request: Request instance for DescribeNotebookImageRecords.
+        :type request: :class:`tencentcloud.tione.v20211111.models.DescribeNotebookImageRecordsRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.DescribeNotebookImageRecordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeNotebookImageRecords", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeNotebookImageRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeNotebooks(self, request):
+        """Notebook列表
+
+        :param request: Request instance for DescribeNotebooks.
+        :type request: :class:`tencentcloud.tione.v20211111.models.DescribeNotebooksRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.DescribeNotebooksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeNotebooks", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeNotebooksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeTrainingFrameworks(self, request):
         """训练框架列表
 
         :param request: Request instance for DescribeTrainingFrameworks.
         :type request: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingFrameworksRequest`
         :rtype: :class:`tencentcloud.tione.v20211111.models.DescribeTrainingFrameworksResponse`
 
@@ -1126,14 +1310,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def ModifyNotebook(self, request):
+        """修改Notebook
+
+        :param request: Request instance for ModifyNotebook.
+        :type request: :class:`tencentcloud.tione.v20211111.models.ModifyNotebookRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.ModifyNotebookResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyNotebook", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyNotebookResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def ModifyNotebookTags(self, request):
+        """修改Notebook标签
+
+        :param request: Request instance for ModifyNotebookTags.
+        :type request: :class:`tencentcloud.tione.v20211111.models.ModifyNotebookTagsRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.ModifyNotebookTagsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyNotebookTags", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyNotebookTagsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ModifyServiceGroupWeights(self, request):
         """更新推理服务组流量分配
 
         :param request: Request instance for ModifyServiceGroupWeights.
         :type request: :class:`tencentcloud.tione.v20211111.models.ModifyServiceGroupWeightsRequest`
         :rtype: :class:`tencentcloud.tione.v20211111.models.ModifyServiceGroupWeightsResponse`
 
@@ -1195,14 +1425,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def StartNotebook(self, request):
+        """启动Notebook
+
+        :param request: Request instance for StartNotebook.
+        :type request: :class:`tencentcloud.tione.v20211111.models.StartNotebookRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.StartNotebookResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StartNotebook", params, headers=headers)
+            response = json.loads(body)
+            model = models.StartNotebookResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def StartTrainingTask(self, request):
         """启动模型训练任务
 
         :param request: Request instance for StartTrainingTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.StartTrainingTaskRequest`
         :rtype: :class:`tencentcloud.tione.v20211111.models.StartTrainingTaskResponse`
 
@@ -1241,14 +1494,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def StopCreatingImage(self, request):
+        """停止保存镜像
+
+        :param request: Request instance for StopCreatingImage.
+        :type request: :class:`tencentcloud.tione.v20211111.models.StopCreatingImageRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.StopCreatingImageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StopCreatingImage", params, headers=headers)
+            response = json.loads(body)
+            model = models.StopCreatingImageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def StopModelAccelerateTask(self, request):
         """停止模型加速任务
 
         :param request: Request instance for StopModelAccelerateTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.StopModelAccelerateTaskRequest`
         :rtype: :class:`tencentcloud.tione.v20211111.models.StopModelAccelerateTaskResponse`
 
@@ -1262,14 +1538,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def StopNotebook(self, request):
+        """停止Notebook
+
+        :param request: Request instance for StopNotebook.
+        :type request: :class:`tencentcloud.tione.v20211111.models.StopNotebookRequest`
+        :rtype: :class:`tencentcloud.tione.v20211111.models.StopNotebookResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("StopNotebook", params, headers=headers)
+            response = json.loads(body)
+            model = models.StopNotebookResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def StopTrainingTask(self, request):
         """停止模型训练任务
 
         :param request: Request instance for StopTrainingTask.
         :type request: :class:`tencentcloud.tione.v20211111.models.StopTrainingTaskRequest`
```

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,20 +43,26 @@
 
 # CAM内部错误。
 FAILEDOPERATION_CAMFAILURE = 'FailedOperation.CAMFailure'
 
 # 调用集群失败。
 FAILEDOPERATION_CALLCLUSTERFAIL = 'FailedOperation.CallClusterFail'
 
+# 查询计费白名单失败
+FAILEDOPERATION_CHECKBILLINGWHITELISTFAILED = 'FailedOperation.CheckBillingWhiteListFailed'
+
 # 尚未开通CLS日志服务，请开前往开通。
 FAILEDOPERATION_CLSSERVICENOTACTIVED = 'FailedOperation.ClsServiceNotActived'
 
 # 集群访问失败。
 FAILEDOPERATION_CLUSTERQUERYFAILED = 'FailedOperation.ClusterQueryFailed'
 
+# 导出Notebook镜像失败
+FAILEDOPERATION_CREATEIMAGEFAILED = 'FailedOperation.CreateImageFailed'
+
 # 启动实例失败。
 FAILEDOPERATION_CREATEJOBINSTANCEFAILED = 'FailedOperation.CreateJobInstanceFailed'
 
 # cos client 内部错误。
 FAILEDOPERATION_DCCOSCLIENTERR = 'FailedOperation.DCCosClientErr'
 
 # 创建内部异步任务失败。
@@ -88,14 +94,17 @@
 
 # 数据反序列化错误。
 FAILEDOPERATION_DCUNMARSHALDATAERR = 'FailedOperation.DCUnmarshalDataErr'
 
 # 数据集操作不支持。
 FAILEDOPERATION_DCUNSUPPORTEDOPERATION = 'FailedOperation.DCUnsupportedOperation'
 
+# 删除Notebook实例存储失败。
+FAILEDOPERATION_DELETENOTEBOOKSTORAGEFAILED = 'FailedOperation.DeleteNotebookStorageFailed'
+
 # 名称重复。
 FAILEDOPERATION_DUPLICATENAME = 'FailedOperation.DuplicateName'
 
 # 训练任务名称已存在，请更换名称
 FAILEDOPERATION_DUPLICATENAMETASKISCREATING = 'FailedOperation.DuplicateNameTaskIsCreating'
 
 # 数据库执行错误。
@@ -112,14 +121,20 @@
 
 # 操作失败，用户类型异常。
 FAILEDOPERATION_INVALIDUSERTYPE = 'FailedOperation.InvalidUserType'
 
 # 密钥管理系统服务未开通，请先开通腾讯云密钥管理系统服务。
 FAILEDOPERATION_KMSKEYNOTOPEN = 'FailedOperation.KmsKeyNotOpen'
 
+# 变更计费配置失败。
+FAILEDOPERATION_MODIFYBILLINGINSTANCEBATCHFAILED = 'FailedOperation.ModifyBillingInstanceBatchFailed'
+
+# 修改计费统计的资源关联标签失败
+FAILEDOPERATION_MODIFYRESOURCEBILLINGTAGSFAILED = 'FailedOperation.ModifyResourceBillingTagsFailed'
+
 # 移动模型目录失败。
 FAILEDOPERATION_MOVEMODELDIRFAILED = 'FailedOperation.MoveModelDirFailed'
 
 # 没有空闲免费桶。
 FAILEDOPERATION_NOFREEBUCKET = 'FailedOperation.NoFreeBucket'
 
 # 没有权限。
@@ -139,14 +154,17 @@
 
 # 根据标签查询资源失败。
 FAILEDOPERATION_QUERYMODELSBYTAGSFAILED = 'FailedOperation.QueryModelsByTagsFailed'
 
 # 查询计费价格失败。
 FAILEDOPERATION_QUERYPRICEFAILED = 'FailedOperation.QueryPriceFailed'
 
+# 查询资源组名称失败。
+FAILEDOPERATION_QUERYRESOURCEGROUPNAMESFAILED = 'FailedOperation.QueryResourceGroupNamesFailed'
+
 # 查询计费项详情失败。
 FAILEDOPERATION_QUERYRESOURCESPECFAILED = 'FailedOperation.QueryResourceSpecFailed'
 
 # 查询计费项失败。
 FAILEDOPERATION_QUERYSPECSFAILED = 'FailedOperation.QuerySpecsFailed'
 
 # 查询标签服务失败。
@@ -154,20 +172,32 @@
 
 # 记录不存在。
 FAILEDOPERATION_RECORDNOTFOUND = 'FailedOperation.RecordNotFound'
 
 # 存储库有绑定的实例，请先删除绑定的实例。
 FAILEDOPERATION_REPOBINDBYINSTANCE = 'FailedOperation.RepoBindByInstance'
 
+# 停止实例失败。
+FAILEDOPERATION_STOPJOBINSTANCEFAILED = 'FailedOperation.StopJobInstanceFailed'
+
 # 密钥服务访问失败，请重试。
 FAILEDOPERATION_STSQUERYFAILED = 'FailedOperation.StsQueryFailed'
 
 # 实例启动失败。
 FAILEDOPERATION_TIMEDOUT = 'FailedOperation.Timedout'
 
+# 解绑标签失败。
+FAILEDOPERATION_UNBINDINGTAGSFAILED = 'FailedOperation.UnBindingTagsFailed'
+
+# 当前任务后台提交重试中，不允许操作停止，请稍后再试。
+FAILEDOPERATION_UNSUBMITNOTALLOWTOSTOP = 'FailedOperation.UnSubmitNotAllowToStop'
+
+# 解冻失败。
+FAILEDOPERATION_UNFREEZEBILLFAILED = 'FailedOperation.UnfreezeBillFailed'
+
 # 未知的实例规格。
 FAILEDOPERATION_UNKNOWNINSTANCETYPE = 'FailedOperation.UnknownInstanceType'
 
 # 数据解析失败。
 FAILEDOPERATION_UNMARSHALDATA = 'FailedOperation.UnmarshalData'
 
 # 内部错误。
@@ -214,14 +244,17 @@
 
 # 未提交状态禁止停止
 INTERNALERROR_UNSUBMITTEDSTATUSNOTALLOWSTOP = 'InternalError.UnSubmittedStatusNotAllowStop'
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
+# 接口过滤条件"运行状态"与"计费状态"不能同时存在。
+INVALIDPARAMETER_FILTERKEYSTATUSCONFLICTWITHCHARGESTATUS = 'InvalidParameter.FilterKeyStatusConflictWithChargeStatus'
+
 # 模型包不符合规范。
 INVALIDPARAMETER_MODELFILEINVALID = 'InvalidParameter.ModelFileInvalid'
 
 # 无效的接口。
 INVALIDPARAMETER_TGWINVALIDINTERFACE = 'InvalidParameter.TgwInvalidInterface'
 
 # 无效的请求包体。
@@ -238,14 +271,17 @@
 
 # 名称不合法。
 INVALIDPARAMETERVALUE_BADNAME = 'InvalidParameterValue.BadName'
 
 # 请设置日志集、日志主题ID。
 INVALIDPARAMETERVALUE_CLSCONFIGREQUIRED = 'InvalidParameterValue.ClsConfigRequired'
 
+# 存储库重复配置，请移除重复的存储库配置后重试。
+INVALIDPARAMETERVALUE_CODEREPODUPLICATED = 'InvalidParameterValue.CodeRepoDuplicated'
+
 # 存储库不存在。
 INVALIDPARAMETERVALUE_CODEREPONOTFOUND = 'InvalidParameterValue.CodeRepoNotFound'
 
 # 不支持的标注类型。
 INVALIDPARAMETERVALUE_DCANNOTATIONTYPE = 'InvalidParameterValue.DCAnnotationType'
 
 # 存储桶参数错误。
@@ -280,32 +316,47 @@
 
 # 训练任务镜像不存在。
 INVALIDPARAMETERVALUE_IMAGENOTFOUND = 'InvalidParameterValue.ImageNotFound'
 
 # 无效的过滤器。
 INVALIDPARAMETERVALUE_INVALIDFILTER = 'InvalidParameterValue.InvalidFilter'
 
+# 生命周期脚本无效。
+INVALIDPARAMETERVALUE_LIFECYCLENOTFOUND = 'InvalidParameterValue.LifecycleNotFound'
+
 # 参数值数量超过限制。
 INVALIDPARAMETERVALUE_LIMITEXCEEDED = 'InvalidParameterValue.LimitExceeded'
 
 # 操作不允许。
 INVALIDPARAMETERVALUE_NOTALLOW = 'InvalidParameterValue.NotAllow'
 
+# 裸金属资源组不支持创建Notebook
+INVALIDPARAMETERVALUE_NOTALLOWEDTOCREATENOTEBOOKWITHBAREMETALRESOURCEGROUP = 'InvalidParameterValue.NotAllowedToCreateNotebookWithBareMetalResourceGroup'
+
 # 分页查询limit超出限制
 INVALIDPARAMETERVALUE_PAGELIMITEXCEEDED = 'InvalidParameterValue.PageLimitExceeded'
 
 # RDMA配置不合法
 INVALIDPARAMETERVALUE_RDMACONFIGILLEGAL = 'InvalidParameterValue.RDMAConfigIllegal'
 
 # 资源配置不合法
 INVALIDPARAMETERVALUE_RESOURCECONFIGILLEGAL = 'InvalidParameterValue.ResourceConfigIllegal'
 
+# 子网不存在。
+INVALIDPARAMETERVALUE_SUBNETNOTFOUND = 'InvalidParameterValue.SubnetNotFound'
+
+# 未找到当前日志主题。
+INVALIDPARAMETERVALUE_TOPICNOTFOUND = 'InvalidParameterValue.TopicNotFound'
+
 # 裸金属类型资源组不支持配置输入数据
 INVALIDPARAMETERVALUE_UNSUPPORTEDDATACONFIG = 'InvalidParameterValue.UnsupportedDataConfig'
 
+# Notebook卷大小只能增加，如需减小容量请重新创建实例。
+INVALIDPARAMETERVALUE_VOLUMESHRINKNOTALLOW = 'InvalidParameterValue.VolumeShrinkNotAllow'
+
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 操作被拒绝。
@@ -316,23 +367,29 @@
 
 # 计费平台出错
 OPERATIONDENIED_BILLINGEXCEPTION = 'OperationDenied.BillingException'
 
 # 按量计费资源售罄。
 OPERATIONDENIED_BILLINGSTATUSRESOURCEINSUFFICIENT = 'OperationDenied.BillingStatusResourceInsufficient'
 
+# IP不合法。
+OPERATIONDENIED_IPILLEGAL = 'OperationDenied.IpIllegal'
+
 # 觅影资源包余额不足，请先充值。
 OPERATIONDENIED_MIYINGBALANCEINSUFFICIENT = 'OperationDenied.MIYINGBalanceInsufficient'
 
 # 网段不合法。
 OPERATIONDENIED_NETWORKCIDRILLEGAL = 'OperationDenied.NetworkCidrIllegal'
 
 # 操作不允许
 OPERATIONDENIED_NOTALLOW = 'OperationDenied.NotAllow'
 
+# 存量Notebook不支持保存
+OPERATIONDENIED_NOTSUPPORTSAVEIMAGE = 'OperationDenied.NotSupportSaveImage'
+
 # 预付费资源组余量不足。
 OPERATIONDENIED_RESOURCEGROUPINSUFFICIENT = 'OperationDenied.ResourceGroupInsufficient'
 
 # 子网不合法。
 OPERATIONDENIED_SUBNETILLEGAL = 'OperationDenied.SubnetIllegal'
 
 # 白名单免费配额不足。
```

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20211111/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -2646,14 +2646,444 @@
     def _deserialize(self, params):
         if params.get("Service") is not None:
             self._Service = Service()
             self._Service._deserialize(params.get("Service"))
         self._RequestId = params.get("RequestId")
 
 
+class CreateNotebookImageRequest(AbstractModel):
+    """CreateNotebookImage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Kernels: 要保存的kernel数组
+        :type Kernels: list of str
+        :param _ImageInfo: 镜像信息
+        :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
+        :param _NotebookId: notebook id
+        :type NotebookId: str
+        """
+        self._Kernels = None
+        self._ImageInfo = None
+        self._NotebookId = None
+
+    @property
+    def Kernels(self):
+        return self._Kernels
+
+    @Kernels.setter
+    def Kernels(self, Kernels):
+        self._Kernels = Kernels
+
+    @property
+    def ImageInfo(self):
+        return self._ImageInfo
+
+    @ImageInfo.setter
+    def ImageInfo(self, ImageInfo):
+        self._ImageInfo = ImageInfo
+
+    @property
+    def NotebookId(self):
+        return self._NotebookId
+
+    @NotebookId.setter
+    def NotebookId(self, NotebookId):
+        self._NotebookId = NotebookId
+
+
+    def _deserialize(self, params):
+        self._Kernels = params.get("Kernels")
+        if params.get("ImageInfo") is not None:
+            self._ImageInfo = ImageInfo()
+            self._ImageInfo._deserialize(params.get("ImageInfo"))
+        self._NotebookId = params.get("NotebookId")
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
+class CreateNotebookImageResponse(AbstractModel):
+    """CreateNotebookImage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
+class CreateNotebookRequest(AbstractModel):
+    """CreateNotebook请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 名称。不超过60个字符，仅支持中英文、数字、下划线"_"、短横"-"，只能以中英文、数字开头
+        :type Name: str
+        :param _ChargeType: 计算资源付费模式 ，可选值为：
+PREPAID：预付费，即包年包月
+POSTPAID_BY_HOUR：按小时后付费
+        :type ChargeType: str
+        :param _ResourceConf: 计算资源配置
+        :type ResourceConf: :class:`tencentcloud.tione.v20211111.models.ResourceConf`
+        :param _LogEnable: 是否上报日志
+        :type LogEnable: bool
+        :param _RootAccess: 是否ROOT权限
+        :type RootAccess: bool
+        :param _AutoStopping: 是否自动停止
+        :type AutoStopping: bool
+        :param _DirectInternetAccess: 是否访问公网
+        :type DirectInternetAccess: bool
+        :param _ResourceGroupId: 资源组ID(for预付费)
+        :type ResourceGroupId: str
+        :param _VpcId: Vpc-Id
+        :type VpcId: str
+        :param _SubnetId: 子网Id
+        :type SubnetId: str
+        :param _VolumeSourceType: 存储的类型。取值包含： 
+    FREE:    预付费的免费存储
+    CLOUD_PREMIUM： 高性能云硬盘
+    CLOUD_SSD： SSD云硬盘
+    CFS:     CFS存储，包含NFS和turbo
+        :type VolumeSourceType: str
+        :param _VolumeSizeInGB: 存储卷大小，单位GB
+        :type VolumeSizeInGB: int
+        :param _VolumeSourceCFS: CFS存储的配置
+        :type VolumeSourceCFS: :class:`tencentcloud.tione.v20211111.models.CFSConfig`
+        :param _LogConfig: 日志配置
+        :type LogConfig: :class:`tencentcloud.tione.v20211111.models.LogConfig`
+        :param _LifecycleScriptId: 生命周期脚本的ID
+        :type LifecycleScriptId: str
+        :param _DefaultCodeRepoId: 默认GIT存储库的ID
+        :type DefaultCodeRepoId: str
+        :param _AdditionalCodeRepoIds: 其他GIT存储库的ID，最多3个
+        :type AdditionalCodeRepoIds: list of str
+        :param _AutomaticStopTime: 自动停止时间，单位小时
+        :type AutomaticStopTime: int
+        :param _Tags: 标签配置
+        :type Tags: list of Tag
+        :param _DataConfigs: 数据配置
+        :type DataConfigs: list of DataConfig
+        :param _ImageInfo: 镜像信息
+        :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
+        :param _ImageType: 镜像类型
+        :type ImageType: str
+        """
+        self._Name = None
+        self._ChargeType = None
+        self._ResourceConf = None
+        self._LogEnable = None
+        self._RootAccess = None
+        self._AutoStopping = None
+        self._DirectInternetAccess = None
+        self._ResourceGroupId = None
+        self._VpcId = None
+        self._SubnetId = None
+        self._VolumeSourceType = None
+        self._VolumeSizeInGB = None
+        self._VolumeSourceCFS = None
+        self._LogConfig = None
+        self._LifecycleScriptId = None
+        self._DefaultCodeRepoId = None
+        self._AdditionalCodeRepoIds = None
+        self._AutomaticStopTime = None
+        self._Tags = None
+        self._DataConfigs = None
+        self._ImageInfo = None
+        self._ImageType = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def ChargeType(self):
+        return self._ChargeType
+
+    @ChargeType.setter
+    def ChargeType(self, ChargeType):
+        self._ChargeType = ChargeType
+
+    @property
+    def ResourceConf(self):
+        return self._ResourceConf
+
+    @ResourceConf.setter
+    def ResourceConf(self, ResourceConf):
+        self._ResourceConf = ResourceConf
+
+    @property
+    def LogEnable(self):
+        return self._LogEnable
+
+    @LogEnable.setter
+    def LogEnable(self, LogEnable):
+        self._LogEnable = LogEnable
+
+    @property
+    def RootAccess(self):
+        return self._RootAccess
+
+    @RootAccess.setter
+    def RootAccess(self, RootAccess):
+        self._RootAccess = RootAccess
+
+    @property
+    def AutoStopping(self):
+        return self._AutoStopping
+
+    @AutoStopping.setter
+    def AutoStopping(self, AutoStopping):
+        self._AutoStopping = AutoStopping
+
+    @property
+    def DirectInternetAccess(self):
+        return self._DirectInternetAccess
+
+    @DirectInternetAccess.setter
+    def DirectInternetAccess(self, DirectInternetAccess):
+        self._DirectInternetAccess = DirectInternetAccess
+
+    @property
+    def ResourceGroupId(self):
+        return self._ResourceGroupId
+
+    @ResourceGroupId.setter
+    def ResourceGroupId(self, ResourceGroupId):
+        self._ResourceGroupId = ResourceGroupId
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def SubnetId(self):
+        return self._SubnetId
+
+    @SubnetId.setter
+    def SubnetId(self, SubnetId):
+        self._SubnetId = SubnetId
+
+    @property
+    def VolumeSourceType(self):
+        return self._VolumeSourceType
+
+    @VolumeSourceType.setter
+    def VolumeSourceType(self, VolumeSourceType):
+        self._VolumeSourceType = VolumeSourceType
+
+    @property
+    def VolumeSizeInGB(self):
+        return self._VolumeSizeInGB
+
+    @VolumeSizeInGB.setter
+    def VolumeSizeInGB(self, VolumeSizeInGB):
+        self._VolumeSizeInGB = VolumeSizeInGB
+
+    @property
+    def VolumeSourceCFS(self):
+        return self._VolumeSourceCFS
+
+    @VolumeSourceCFS.setter
+    def VolumeSourceCFS(self, VolumeSourceCFS):
+        self._VolumeSourceCFS = VolumeSourceCFS
+
+    @property
+    def LogConfig(self):
+        return self._LogConfig
+
+    @LogConfig.setter
+    def LogConfig(self, LogConfig):
+        self._LogConfig = LogConfig
+
+    @property
+    def LifecycleScriptId(self):
+        return self._LifecycleScriptId
+
+    @LifecycleScriptId.setter
+    def LifecycleScriptId(self, LifecycleScriptId):
+        self._LifecycleScriptId = LifecycleScriptId
+
+    @property
+    def DefaultCodeRepoId(self):
+        return self._DefaultCodeRepoId
+
+    @DefaultCodeRepoId.setter
+    def DefaultCodeRepoId(self, DefaultCodeRepoId):
+        self._DefaultCodeRepoId = DefaultCodeRepoId
+
+    @property
+    def AdditionalCodeRepoIds(self):
+        return self._AdditionalCodeRepoIds
+
+    @AdditionalCodeRepoIds.setter
+    def AdditionalCodeRepoIds(self, AdditionalCodeRepoIds):
+        self._AdditionalCodeRepoIds = AdditionalCodeRepoIds
+
+    @property
+    def AutomaticStopTime(self):
+        return self._AutomaticStopTime
+
+    @AutomaticStopTime.setter
+    def AutomaticStopTime(self, AutomaticStopTime):
+        self._AutomaticStopTime = AutomaticStopTime
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
+    @property
+    def DataConfigs(self):
+        return self._DataConfigs
+
+    @DataConfigs.setter
+    def DataConfigs(self, DataConfigs):
+        self._DataConfigs = DataConfigs
+
+    @property
+    def ImageInfo(self):
+        return self._ImageInfo
+
+    @ImageInfo.setter
+    def ImageInfo(self, ImageInfo):
+        self._ImageInfo = ImageInfo
+
+    @property
+    def ImageType(self):
+        return self._ImageType
+
+    @ImageType.setter
+    def ImageType(self, ImageType):
+        self._ImageType = ImageType
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._ChargeType = params.get("ChargeType")
+        if params.get("ResourceConf") is not None:
+            self._ResourceConf = ResourceConf()
+            self._ResourceConf._deserialize(params.get("ResourceConf"))
+        self._LogEnable = params.get("LogEnable")
+        self._RootAccess = params.get("RootAccess")
+        self._AutoStopping = params.get("AutoStopping")
+        self._DirectInternetAccess = params.get("DirectInternetAccess")
+        self._ResourceGroupId = params.get("ResourceGroupId")
+        self._VpcId = params.get("VpcId")
+        self._SubnetId = params.get("SubnetId")
+        self._VolumeSourceType = params.get("VolumeSourceType")
+        self._VolumeSizeInGB = params.get("VolumeSizeInGB")
+        if params.get("VolumeSourceCFS") is not None:
+            self._VolumeSourceCFS = CFSConfig()
+            self._VolumeSourceCFS._deserialize(params.get("VolumeSourceCFS"))
+        if params.get("LogConfig") is not None:
+            self._LogConfig = LogConfig()
+            self._LogConfig._deserialize(params.get("LogConfig"))
+        self._LifecycleScriptId = params.get("LifecycleScriptId")
+        self._DefaultCodeRepoId = params.get("DefaultCodeRepoId")
+        self._AdditionalCodeRepoIds = params.get("AdditionalCodeRepoIds")
+        self._AutomaticStopTime = params.get("AutomaticStopTime")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self._Tags.append(obj)
+        if params.get("DataConfigs") is not None:
+            self._DataConfigs = []
+            for item in params.get("DataConfigs"):
+                obj = DataConfig()
+                obj._deserialize(item)
+                self._DataConfigs.append(obj)
+        if params.get("ImageInfo") is not None:
+            self._ImageInfo = ImageInfo()
+            self._ImageInfo._deserialize(params.get("ImageInfo"))
+        self._ImageType = params.get("ImageType")
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
+class CreateNotebookResponse(AbstractModel):
+    """CreateNotebook返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook标志
+        :type Id: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Id = None
+        self._RequestId = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
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
+        self._Id = params.get("Id")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateOptimizedModelRequest(AbstractModel):
     """CreateOptimizedModel请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5075,14 +5505,130 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class DeleteNotebookImageRecordRequest(AbstractModel):
+    """DeleteNotebookImageRecord请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RecordId: 记录id
+        :type RecordId: str
+        """
+        self._RecordId = None
+
+    @property
+    def RecordId(self):
+        return self._RecordId
+
+    @RecordId.setter
+    def RecordId(self, RecordId):
+        self._RecordId = RecordId
+
+
+    def _deserialize(self, params):
+        self._RecordId = params.get("RecordId")
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
+class DeleteNotebookImageRecordResponse(AbstractModel):
+    """DeleteNotebookImageRecord返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
+class DeleteNotebookRequest(AbstractModel):
+    """DeleteNotebook请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook id
+        :type Id: str
+        """
+        self._Id = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
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
+class DeleteNotebookResponse(AbstractModel):
+    """DeleteNotebook返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteTrainingModelRequest(AbstractModel):
     """DeleteTrainingModel请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8042,14 +8588,453 @@
             for item in params.get("Services"):
                 obj = Service()
                 obj._deserialize(item)
                 self._Services.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeNotebookImageKernelsRequest(AbstractModel):
+    """DescribeNotebookImageKernels请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _NotebookId: notebook id
+        :type NotebookId: str
+        """
+        self._NotebookId = None
+
+    @property
+    def NotebookId(self):
+        return self._NotebookId
+
+    @NotebookId.setter
+    def NotebookId(self, NotebookId):
+        self._NotebookId = NotebookId
+
+
+    def _deserialize(self, params):
+        self._NotebookId = params.get("NotebookId")
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
+class DescribeNotebookImageKernelsResponse(AbstractModel):
+    """DescribeNotebookImageKernels返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Kernels: 镜像kernel数组
+        :type Kernels: list of str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Kernels = None
+        self._RequestId = None
+
+    @property
+    def Kernels(self):
+        return self._Kernels
+
+    @Kernels.setter
+    def Kernels(self, Kernels):
+        self._Kernels = Kernels
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
+        self._Kernels = params.get("Kernels")
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeNotebookImageRecordsRequest(AbstractModel):
+    """DescribeNotebookImageRecords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _NotebookId: notebook id
+        :type NotebookId: str
+        :param _Offset: 位移值
+        :type Offset: int
+        :param _Limit: 日志限制
+        :type Limit: int
+        :param _Filters: 状态筛选
+        :type Filters: list of Filter
+        """
+        self._NotebookId = None
+        self._Offset = None
+        self._Limit = None
+        self._Filters = None
+
+    @property
+    def NotebookId(self):
+        return self._NotebookId
+
+    @NotebookId.setter
+    def NotebookId(self, NotebookId):
+        self._NotebookId = NotebookId
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+
+    def _deserialize(self, params):
+        self._NotebookId = params.get("NotebookId")
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
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
+class DescribeNotebookImageRecordsResponse(AbstractModel):
+    """DescribeNotebookImageRecords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 总条数
+        :type TotalCount: int
+        :param _NotebookImageRecords: 镜像保存记录
+        :type NotebookImageRecords: list of NotebookImageRecord
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._NotebookImageRecords = None
+        self._RequestId = None
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
+    def NotebookImageRecords(self):
+        return self._NotebookImageRecords
+
+    @NotebookImageRecords.setter
+    def NotebookImageRecords(self, NotebookImageRecords):
+        self._NotebookImageRecords = NotebookImageRecords
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
+        self._TotalCount = params.get("TotalCount")
+        if params.get("NotebookImageRecords") is not None:
+            self._NotebookImageRecords = []
+            for item in params.get("NotebookImageRecords"):
+                obj = NotebookImageRecord()
+                obj._deserialize(item)
+                self._NotebookImageRecords.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeNotebookRequest(AbstractModel):
+    """DescribeNotebook请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook id
+        :type Id: str
+        """
+        self._Id = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
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
+class DescribeNotebookResponse(AbstractModel):
+    """DescribeNotebook返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _NotebookDetail: 详情
+        :type NotebookDetail: :class:`tencentcloud.tione.v20211111.models.NotebookDetail`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._NotebookDetail = None
+        self._RequestId = None
+
+    @property
+    def NotebookDetail(self):
+        return self._NotebookDetail
+
+    @NotebookDetail.setter
+    def NotebookDetail(self, NotebookDetail):
+        self._NotebookDetail = NotebookDetail
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
+        if params.get("NotebookDetail") is not None:
+            self._NotebookDetail = NotebookDetail()
+            self._NotebookDetail._deserialize(params.get("NotebookDetail"))
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeNotebooksRequest(AbstractModel):
+    """DescribeNotebooks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Offset: 偏移量，默认为0
+        :type Offset: int
+        :param _Limit: 每页返回的实例数，默认为10
+        :type Limit: int
+        :param _Order: 输出列表的排列顺序。取值范围：ASC：升序排列 DESC：降序排列。默认为DESC
+        :type Order: str
+        :param _OrderField: 根据哪个字段排序，如：CreateTime、UpdateTime，默认为UpdateTime
+        :type OrderField: str
+        :param _Filters: 过滤器，eg：[{ "Name": "Id", "Values": ["nb-123456789"] }]
+
+取值范围
+Name（名称）：notebook1
+Id（notebook ID）：nb-123456789
+Status（状态）：Starting / Running / Stopped / Stopping / Failed / SubmitFailed
+ChargeType（计费类型）：PREPAID（预付费）/ POSTPAID_BY_HOUR（后付费）
+ChargeStatus（计费状态）：NOT_BILLING（未开始计费）/ BILLING（计费中）/ BILLING_STORAGE（存储计费中）/ARREARS_STOP（欠费停止）
+DefaultCodeRepoId（默认代码仓库ID）：cr-123456789
+AdditionalCodeRepoId（关联代码仓库ID）：cr-123456789
+LifecycleScriptId（生命周期ID）：ls-12312312311312
+        :type Filters: list of Filter
+        :param _TagFilters: 标签过滤器，eg：[{ "TagKey": "TagKeyA", "TagValue": ["TagValueA"] }]
+        :type TagFilters: list of TagFilter
+        """
+        self._Offset = None
+        self._Limit = None
+        self._Order = None
+        self._OrderField = None
+        self._Filters = None
+        self._TagFilters = None
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
+    def Order(self):
+        return self._Order
+
+    @Order.setter
+    def Order(self, Order):
+        self._Order = Order
+
+    @property
+    def OrderField(self):
+        return self._OrderField
+
+    @OrderField.setter
+    def OrderField(self, OrderField):
+        self._OrderField = OrderField
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+    @property
+    def TagFilters(self):
+        return self._TagFilters
+
+    @TagFilters.setter
+    def TagFilters(self, TagFilters):
+        self._TagFilters = TagFilters
+
+
+    def _deserialize(self, params):
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        self._Order = params.get("Order")
+        self._OrderField = params.get("OrderField")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        if params.get("TagFilters") is not None:
+            self._TagFilters = []
+            for item in params.get("TagFilters"):
+                obj = TagFilter()
+                obj._deserialize(item)
+                self._TagFilters.append(obj)
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
+class DescribeNotebooksResponse(AbstractModel):
+    """DescribeNotebooks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _NotebookSet: 详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type NotebookSet: list of NotebookSetItem
+        :param _TotalCount: 总条数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._NotebookSet = None
+        self._TotalCount = None
+        self._RequestId = None
+
+    @property
+    def NotebookSet(self):
+        return self._NotebookSet
+
+    @NotebookSet.setter
+    def NotebookSet(self, NotebookSet):
+        self._NotebookSet = NotebookSet
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
+        if params.get("NotebookSet") is not None:
+            self._NotebookSet = []
+            for item in params.get("NotebookSet"):
+                obj = NotebookSetItem()
+                obj._deserialize(item)
+                self._NotebookSet.append(obj)
+        self._TotalCount = params.get("TotalCount")
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeTrainingFrameworksRequest(AbstractModel):
     """DescribeTrainingFrameworks请求参数结构体
 
     """
 
 
 class DescribeTrainingFrameworksResponse(AbstractModel):
@@ -11678,14 +12663,435 @@
     def _deserialize(self, params):
         if params.get("Service") is not None:
             self._Service = Service()
             self._Service._deserialize(params.get("Service"))
         self._RequestId = params.get("RequestId")
 
 
+class ModifyNotebookRequest(AbstractModel):
+    """ModifyNotebook请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook id
+        :type Id: str
+        :param _Name: 名称
+        :type Name: str
+        :param _ChargeType: 计算资源付费模式 ，可选值为：
+PREPAID：预付费，即包年包月
+POSTPAID_BY_HOUR：按小时后付费
+        :type ChargeType: str
+        :param _ResourceConf: 计算资源配置
+        :type ResourceConf: :class:`tencentcloud.tione.v20211111.models.ResourceConf`
+        :param _LogEnable: 是否上报日志
+        :type LogEnable: bool
+        :param _AutoStopping: 是否自动停止
+        :type AutoStopping: bool
+        :param _DirectInternetAccess: 是否访问公网
+        :type DirectInternetAccess: bool
+        :param _RootAccess: 是否ROOT权限
+        :type RootAccess: bool
+        :param _ResourceGroupId: 资源组ID(for预付费)
+        :type ResourceGroupId: str
+        :param _VpcId: Vpc-Id
+        :type VpcId: str
+        :param _SubnetId: 子网Id
+        :type SubnetId: str
+        :param _VolumeSizeInGB: 存储卷大小，单位GB
+        :type VolumeSizeInGB: int
+        :param _VolumeSourceType: 存储的类型。取值包含： 
+    FREE:    预付费的免费存储
+    CLOUD_PREMIUM： 高性能云硬盘
+    CLOUD_SSD： SSD云硬盘
+    CFS:     CFS存储，包含NFS和turbo
+        :type VolumeSourceType: str
+        :param _VolumeSourceCFS: CFS存储的配置
+        :type VolumeSourceCFS: :class:`tencentcloud.tione.v20211111.models.CFSConfig`
+        :param _LogConfig: 日志配置
+        :type LogConfig: :class:`tencentcloud.tione.v20211111.models.LogConfig`
+        :param _LifecycleScriptId: 生命周期脚本的ID
+        :type LifecycleScriptId: str
+        :param _DefaultCodeRepoId: 默认GIT存储库的ID
+        :type DefaultCodeRepoId: str
+        :param _AdditionalCodeRepoIds: 其他GIT存储库的ID，最多3个
+        :type AdditionalCodeRepoIds: list of str
+        :param _AutomaticStopTime: 自动停止时间，单位小时
+        :type AutomaticStopTime: int
+        :param _Tags: 标签配置
+        :type Tags: list of Tag
+        :param _DataConfigs: 数据配置
+        :type DataConfigs: list of DataConfig
+        :param _ImageInfo: 镜像信息
+        :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
+        :param _ImageType: 镜像类型
+        :type ImageType: str
+        """
+        self._Id = None
+        self._Name = None
+        self._ChargeType = None
+        self._ResourceConf = None
+        self._LogEnable = None
+        self._AutoStopping = None
+        self._DirectInternetAccess = None
+        self._RootAccess = None
+        self._ResourceGroupId = None
+        self._VpcId = None
+        self._SubnetId = None
+        self._VolumeSizeInGB = None
+        self._VolumeSourceType = None
+        self._VolumeSourceCFS = None
+        self._LogConfig = None
+        self._LifecycleScriptId = None
+        self._DefaultCodeRepoId = None
+        self._AdditionalCodeRepoIds = None
+        self._AutomaticStopTime = None
+        self._Tags = None
+        self._DataConfigs = None
+        self._ImageInfo = None
+        self._ImageType = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def ChargeType(self):
+        return self._ChargeType
+
+    @ChargeType.setter
+    def ChargeType(self, ChargeType):
+        self._ChargeType = ChargeType
+
+    @property
+    def ResourceConf(self):
+        return self._ResourceConf
+
+    @ResourceConf.setter
+    def ResourceConf(self, ResourceConf):
+        self._ResourceConf = ResourceConf
+
+    @property
+    def LogEnable(self):
+        return self._LogEnable
+
+    @LogEnable.setter
+    def LogEnable(self, LogEnable):
+        self._LogEnable = LogEnable
+
+    @property
+    def AutoStopping(self):
+        return self._AutoStopping
+
+    @AutoStopping.setter
+    def AutoStopping(self, AutoStopping):
+        self._AutoStopping = AutoStopping
+
+    @property
+    def DirectInternetAccess(self):
+        return self._DirectInternetAccess
+
+    @DirectInternetAccess.setter
+    def DirectInternetAccess(self, DirectInternetAccess):
+        self._DirectInternetAccess = DirectInternetAccess
+
+    @property
+    def RootAccess(self):
+        return self._RootAccess
+
+    @RootAccess.setter
+    def RootAccess(self, RootAccess):
+        self._RootAccess = RootAccess
+
+    @property
+    def ResourceGroupId(self):
+        return self._ResourceGroupId
+
+    @ResourceGroupId.setter
+    def ResourceGroupId(self, ResourceGroupId):
+        self._ResourceGroupId = ResourceGroupId
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def SubnetId(self):
+        return self._SubnetId
+
+    @SubnetId.setter
+    def SubnetId(self, SubnetId):
+        self._SubnetId = SubnetId
+
+    @property
+    def VolumeSizeInGB(self):
+        return self._VolumeSizeInGB
+
+    @VolumeSizeInGB.setter
+    def VolumeSizeInGB(self, VolumeSizeInGB):
+        self._VolumeSizeInGB = VolumeSizeInGB
+
+    @property
+    def VolumeSourceType(self):
+        return self._VolumeSourceType
+
+    @VolumeSourceType.setter
+    def VolumeSourceType(self, VolumeSourceType):
+        self._VolumeSourceType = VolumeSourceType
+
+    @property
+    def VolumeSourceCFS(self):
+        return self._VolumeSourceCFS
+
+    @VolumeSourceCFS.setter
+    def VolumeSourceCFS(self, VolumeSourceCFS):
+        self._VolumeSourceCFS = VolumeSourceCFS
+
+    @property
+    def LogConfig(self):
+        return self._LogConfig
+
+    @LogConfig.setter
+    def LogConfig(self, LogConfig):
+        self._LogConfig = LogConfig
+
+    @property
+    def LifecycleScriptId(self):
+        return self._LifecycleScriptId
+
+    @LifecycleScriptId.setter
+    def LifecycleScriptId(self, LifecycleScriptId):
+        self._LifecycleScriptId = LifecycleScriptId
+
+    @property
+    def DefaultCodeRepoId(self):
+        return self._DefaultCodeRepoId
+
+    @DefaultCodeRepoId.setter
+    def DefaultCodeRepoId(self, DefaultCodeRepoId):
+        self._DefaultCodeRepoId = DefaultCodeRepoId
+
+    @property
+    def AdditionalCodeRepoIds(self):
+        return self._AdditionalCodeRepoIds
+
+    @AdditionalCodeRepoIds.setter
+    def AdditionalCodeRepoIds(self, AdditionalCodeRepoIds):
+        self._AdditionalCodeRepoIds = AdditionalCodeRepoIds
+
+    @property
+    def AutomaticStopTime(self):
+        return self._AutomaticStopTime
+
+    @AutomaticStopTime.setter
+    def AutomaticStopTime(self, AutomaticStopTime):
+        self._AutomaticStopTime = AutomaticStopTime
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
+    @property
+    def DataConfigs(self):
+        return self._DataConfigs
+
+    @DataConfigs.setter
+    def DataConfigs(self, DataConfigs):
+        self._DataConfigs = DataConfigs
+
+    @property
+    def ImageInfo(self):
+        return self._ImageInfo
+
+    @ImageInfo.setter
+    def ImageInfo(self, ImageInfo):
+        self._ImageInfo = ImageInfo
+
+    @property
+    def ImageType(self):
+        return self._ImageType
+
+    @ImageType.setter
+    def ImageType(self, ImageType):
+        self._ImageType = ImageType
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._Name = params.get("Name")
+        self._ChargeType = params.get("ChargeType")
+        if params.get("ResourceConf") is not None:
+            self._ResourceConf = ResourceConf()
+            self._ResourceConf._deserialize(params.get("ResourceConf"))
+        self._LogEnable = params.get("LogEnable")
+        self._AutoStopping = params.get("AutoStopping")
+        self._DirectInternetAccess = params.get("DirectInternetAccess")
+        self._RootAccess = params.get("RootAccess")
+        self._ResourceGroupId = params.get("ResourceGroupId")
+        self._VpcId = params.get("VpcId")
+        self._SubnetId = params.get("SubnetId")
+        self._VolumeSizeInGB = params.get("VolumeSizeInGB")
+        self._VolumeSourceType = params.get("VolumeSourceType")
+        if params.get("VolumeSourceCFS") is not None:
+            self._VolumeSourceCFS = CFSConfig()
+            self._VolumeSourceCFS._deserialize(params.get("VolumeSourceCFS"))
+        if params.get("LogConfig") is not None:
+            self._LogConfig = LogConfig()
+            self._LogConfig._deserialize(params.get("LogConfig"))
+        self._LifecycleScriptId = params.get("LifecycleScriptId")
+        self._DefaultCodeRepoId = params.get("DefaultCodeRepoId")
+        self._AdditionalCodeRepoIds = params.get("AdditionalCodeRepoIds")
+        self._AutomaticStopTime = params.get("AutomaticStopTime")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self._Tags.append(obj)
+        if params.get("DataConfigs") is not None:
+            self._DataConfigs = []
+            for item in params.get("DataConfigs"):
+                obj = DataConfig()
+                obj._deserialize(item)
+                self._DataConfigs.append(obj)
+        if params.get("ImageInfo") is not None:
+            self._ImageInfo = ImageInfo()
+            self._ImageInfo._deserialize(params.get("ImageInfo"))
+        self._ImageType = params.get("ImageType")
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
+class ModifyNotebookResponse(AbstractModel):
+    """ModifyNotebook返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
+class ModifyNotebookTagsRequest(AbstractModel):
+    """ModifyNotebookTags请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: Notebook Id
+        :type Id: str
+        :param _Tags: Notebook修改标签集合
+        :type Tags: list of Tag
+        """
+        self._Id = None
+        self._Tags = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self._Tags.append(obj)
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
+class ModifyNotebookTagsResponse(AbstractModel):
+    """ModifyNotebookTags返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class ModifyServiceGroupWeightsRequest(AbstractModel):
     """ModifyServiceGroupWeights请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -11768,14 +13174,989 @@
     def _deserialize(self, params):
         if params.get("ServiceGroup") is not None:
             self._ServiceGroup = ServiceGroup()
             self._ServiceGroup._deserialize(params.get("ServiceGroup"))
         self._RequestId = params.get("RequestId")
 
 
+class NotebookDetail(AbstractModel):
+    """类型NotebookDetail
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook  ID
+        :type Id: str
+        :param _Name: notebook 名称
+        :type Name: str
+        :param _LifecycleScriptId: 生命周期脚本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LifecycleScriptId: str
+        :param _PodName: Pod-Name
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PodName: str
+        :param _UpdateTime: Update-Time
+        :type UpdateTime: str
+        :param _DirectInternetAccess: 是否访问公网
+        :type DirectInternetAccess: bool
+        :param _ResourceGroupId: 预付费专用资源组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceGroupId: str
+        :param _Tags: 标签配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of Tag
+        :param _AutoStopping: 是否自动停止
+        :type AutoStopping: bool
+        :param _AdditionalCodeRepoIds: 其他GIT存储库，最多3个，单个
+长度不超过512字符
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AdditionalCodeRepoIds: list of str
+        :param _AutomaticStopTime: 自动停止时间，单位小时
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AutomaticStopTime: int
+        :param _ResourceConf: 资源配置
+        :type ResourceConf: :class:`tencentcloud.tione.v20211111.models.ResourceConf`
+        :param _DefaultCodeRepoId: 默认GIT存储库，长度不超过512字符
+        :type DefaultCodeRepoId: str
+        :param _EndTime: 训练输出
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: str
+        :param _LogEnable: 是否上报日志
+        :type LogEnable: bool
+        :param _LogConfig: 日志配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogConfig: :class:`tencentcloud.tione.v20211111.models.LogConfig`
+        :param _VpcId: VPC ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcId: str
+        :param _SubnetId: 子网ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SubnetId: str
+        :param _Status: 任务状态
+        :type Status: str
+        :param _RuntimeInSeconds: 运行时长
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RuntimeInSeconds: int
+        :param _CreateTime: 创建时间
+        :type CreateTime: str
+        :param _StartTime: 训练开始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param _ChargeStatus: 计费状态，eg：BILLING计费中，ARREARS_STOP欠费停止，NOT_BILLING不在计费中
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChargeStatus: str
+        :param _RootAccess: 是否ROOT权限
+        :type RootAccess: bool
+        :param _BillingInfos: 计贺金额信息，eg:2.00元/小时
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BillingInfos: list of str
+        :param _VolumeSizeInGB: 存储卷大小 （单位时GB，最小10GB，必须是10G的倍数）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VolumeSizeInGB: int
+        :param _FailureReason: 失败原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FailureReason: str
+        :param _ChargeType: 计算资源付费模式 (- PREPAID：预付费，即包年包月 - POSTPAID_BY_HOUR：按小时后付费)
+        :type ChargeType: str
+        :param _InstanceTypeAlias: 后付费资源规格说明
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceTypeAlias: str
+        :param _ResourceGroupName: 预付费资源组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceGroupName: str
+        :param _VolumeSourceType: 存储的类型。取值包含： 
+    FREE:        预付费的免费存储
+    CLOUD_PREMIUM： 高性能云硬盘
+    CLOUD_SSD： SSD云硬盘
+    CFS:     CFS存储，包含NFS和turbo
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VolumeSourceType: str
+        :param _VolumeSourceCFS: CFS存储的配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VolumeSourceCFS: :class:`tencentcloud.tione.v20211111.models.CFSConfig`
+        :param _DataConfigs: 数据配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataConfigs: list of DataConfig
+        :param _Message: notebook 信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param _DataSource: 数据源来源，eg：WeData_HDFS
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataSource: str
+        :param _ImageInfo: 镜像信息
+        :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
+        :param _ImageType: 镜像类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageType: str
+        """
+        self._Id = None
+        self._Name = None
+        self._LifecycleScriptId = None
+        self._PodName = None
+        self._UpdateTime = None
+        self._DirectInternetAccess = None
+        self._ResourceGroupId = None
+        self._Tags = None
+        self._AutoStopping = None
+        self._AdditionalCodeRepoIds = None
+        self._AutomaticStopTime = None
+        self._ResourceConf = None
+        self._DefaultCodeRepoId = None
+        self._EndTime = None
+        self._LogEnable = None
+        self._LogConfig = None
+        self._VpcId = None
+        self._SubnetId = None
+        self._Status = None
+        self._RuntimeInSeconds = None
+        self._CreateTime = None
+        self._StartTime = None
+        self._ChargeStatus = None
+        self._RootAccess = None
+        self._BillingInfos = None
+        self._VolumeSizeInGB = None
+        self._FailureReason = None
+        self._ChargeType = None
+        self._InstanceTypeAlias = None
+        self._ResourceGroupName = None
+        self._VolumeSourceType = None
+        self._VolumeSourceCFS = None
+        self._DataConfigs = None
+        self._Message = None
+        self._DataSource = None
+        self._ImageInfo = None
+        self._ImageType = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def LifecycleScriptId(self):
+        return self._LifecycleScriptId
+
+    @LifecycleScriptId.setter
+    def LifecycleScriptId(self, LifecycleScriptId):
+        self._LifecycleScriptId = LifecycleScriptId
+
+    @property
+    def PodName(self):
+        return self._PodName
+
+    @PodName.setter
+    def PodName(self, PodName):
+        self._PodName = PodName
+
+    @property
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
+    def DirectInternetAccess(self):
+        return self._DirectInternetAccess
+
+    @DirectInternetAccess.setter
+    def DirectInternetAccess(self, DirectInternetAccess):
+        self._DirectInternetAccess = DirectInternetAccess
+
+    @property
+    def ResourceGroupId(self):
+        return self._ResourceGroupId
+
+    @ResourceGroupId.setter
+    def ResourceGroupId(self, ResourceGroupId):
+        self._ResourceGroupId = ResourceGroupId
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
+    @property
+    def AutoStopping(self):
+        return self._AutoStopping
+
+    @AutoStopping.setter
+    def AutoStopping(self, AutoStopping):
+        self._AutoStopping = AutoStopping
+
+    @property
+    def AdditionalCodeRepoIds(self):
+        return self._AdditionalCodeRepoIds
+
+    @AdditionalCodeRepoIds.setter
+    def AdditionalCodeRepoIds(self, AdditionalCodeRepoIds):
+        self._AdditionalCodeRepoIds = AdditionalCodeRepoIds
+
+    @property
+    def AutomaticStopTime(self):
+        return self._AutomaticStopTime
+
+    @AutomaticStopTime.setter
+    def AutomaticStopTime(self, AutomaticStopTime):
+        self._AutomaticStopTime = AutomaticStopTime
+
+    @property
+    def ResourceConf(self):
+        return self._ResourceConf
+
+    @ResourceConf.setter
+    def ResourceConf(self, ResourceConf):
+        self._ResourceConf = ResourceConf
+
+    @property
+    def DefaultCodeRepoId(self):
+        return self._DefaultCodeRepoId
+
+    @DefaultCodeRepoId.setter
+    def DefaultCodeRepoId(self, DefaultCodeRepoId):
+        self._DefaultCodeRepoId = DefaultCodeRepoId
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
+    def LogEnable(self):
+        return self._LogEnable
+
+    @LogEnable.setter
+    def LogEnable(self, LogEnable):
+        self._LogEnable = LogEnable
+
+    @property
+    def LogConfig(self):
+        return self._LogConfig
+
+    @LogConfig.setter
+    def LogConfig(self, LogConfig):
+        self._LogConfig = LogConfig
+
+    @property
+    def VpcId(self):
+        return self._VpcId
+
+    @VpcId.setter
+    def VpcId(self, VpcId):
+        self._VpcId = VpcId
+
+    @property
+    def SubnetId(self):
+        return self._SubnetId
+
+    @SubnetId.setter
+    def SubnetId(self, SubnetId):
+        self._SubnetId = SubnetId
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def RuntimeInSeconds(self):
+        return self._RuntimeInSeconds
+
+    @RuntimeInSeconds.setter
+    def RuntimeInSeconds(self, RuntimeInSeconds):
+        self._RuntimeInSeconds = RuntimeInSeconds
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
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
+    def ChargeStatus(self):
+        return self._ChargeStatus
+
+    @ChargeStatus.setter
+    def ChargeStatus(self, ChargeStatus):
+        self._ChargeStatus = ChargeStatus
+
+    @property
+    def RootAccess(self):
+        return self._RootAccess
+
+    @RootAccess.setter
+    def RootAccess(self, RootAccess):
+        self._RootAccess = RootAccess
+
+    @property
+    def BillingInfos(self):
+        return self._BillingInfos
+
+    @BillingInfos.setter
+    def BillingInfos(self, BillingInfos):
+        self._BillingInfos = BillingInfos
+
+    @property
+    def VolumeSizeInGB(self):
+        return self._VolumeSizeInGB
+
+    @VolumeSizeInGB.setter
+    def VolumeSizeInGB(self, VolumeSizeInGB):
+        self._VolumeSizeInGB = VolumeSizeInGB
+
+    @property
+    def FailureReason(self):
+        return self._FailureReason
+
+    @FailureReason.setter
+    def FailureReason(self, FailureReason):
+        self._FailureReason = FailureReason
+
+    @property
+    def ChargeType(self):
+        return self._ChargeType
+
+    @ChargeType.setter
+    def ChargeType(self, ChargeType):
+        self._ChargeType = ChargeType
+
+    @property
+    def InstanceTypeAlias(self):
+        return self._InstanceTypeAlias
+
+    @InstanceTypeAlias.setter
+    def InstanceTypeAlias(self, InstanceTypeAlias):
+        self._InstanceTypeAlias = InstanceTypeAlias
+
+    @property
+    def ResourceGroupName(self):
+        return self._ResourceGroupName
+
+    @ResourceGroupName.setter
+    def ResourceGroupName(self, ResourceGroupName):
+        self._ResourceGroupName = ResourceGroupName
+
+    @property
+    def VolumeSourceType(self):
+        return self._VolumeSourceType
+
+    @VolumeSourceType.setter
+    def VolumeSourceType(self, VolumeSourceType):
+        self._VolumeSourceType = VolumeSourceType
+
+    @property
+    def VolumeSourceCFS(self):
+        return self._VolumeSourceCFS
+
+    @VolumeSourceCFS.setter
+    def VolumeSourceCFS(self, VolumeSourceCFS):
+        self._VolumeSourceCFS = VolumeSourceCFS
+
+    @property
+    def DataConfigs(self):
+        return self._DataConfigs
+
+    @DataConfigs.setter
+    def DataConfigs(self, DataConfigs):
+        self._DataConfigs = DataConfigs
+
+    @property
+    def Message(self):
+        return self._Message
+
+    @Message.setter
+    def Message(self, Message):
+        self._Message = Message
+
+    @property
+    def DataSource(self):
+        return self._DataSource
+
+    @DataSource.setter
+    def DataSource(self, DataSource):
+        self._DataSource = DataSource
+
+    @property
+    def ImageInfo(self):
+        return self._ImageInfo
+
+    @ImageInfo.setter
+    def ImageInfo(self, ImageInfo):
+        self._ImageInfo = ImageInfo
+
+    @property
+    def ImageType(self):
+        return self._ImageType
+
+    @ImageType.setter
+    def ImageType(self, ImageType):
+        self._ImageType = ImageType
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._Name = params.get("Name")
+        self._LifecycleScriptId = params.get("LifecycleScriptId")
+        self._PodName = params.get("PodName")
+        self._UpdateTime = params.get("UpdateTime")
+        self._DirectInternetAccess = params.get("DirectInternetAccess")
+        self._ResourceGroupId = params.get("ResourceGroupId")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self._Tags.append(obj)
+        self._AutoStopping = params.get("AutoStopping")
+        self._AdditionalCodeRepoIds = params.get("AdditionalCodeRepoIds")
+        self._AutomaticStopTime = params.get("AutomaticStopTime")
+        if params.get("ResourceConf") is not None:
+            self._ResourceConf = ResourceConf()
+            self._ResourceConf._deserialize(params.get("ResourceConf"))
+        self._DefaultCodeRepoId = params.get("DefaultCodeRepoId")
+        self._EndTime = params.get("EndTime")
+        self._LogEnable = params.get("LogEnable")
+        if params.get("LogConfig") is not None:
+            self._LogConfig = LogConfig()
+            self._LogConfig._deserialize(params.get("LogConfig"))
+        self._VpcId = params.get("VpcId")
+        self._SubnetId = params.get("SubnetId")
+        self._Status = params.get("Status")
+        self._RuntimeInSeconds = params.get("RuntimeInSeconds")
+        self._CreateTime = params.get("CreateTime")
+        self._StartTime = params.get("StartTime")
+        self._ChargeStatus = params.get("ChargeStatus")
+        self._RootAccess = params.get("RootAccess")
+        self._BillingInfos = params.get("BillingInfos")
+        self._VolumeSizeInGB = params.get("VolumeSizeInGB")
+        self._FailureReason = params.get("FailureReason")
+        self._ChargeType = params.get("ChargeType")
+        self._InstanceTypeAlias = params.get("InstanceTypeAlias")
+        self._ResourceGroupName = params.get("ResourceGroupName")
+        self._VolumeSourceType = params.get("VolumeSourceType")
+        if params.get("VolumeSourceCFS") is not None:
+            self._VolumeSourceCFS = CFSConfig()
+            self._VolumeSourceCFS._deserialize(params.get("VolumeSourceCFS"))
+        if params.get("DataConfigs") is not None:
+            self._DataConfigs = []
+            for item in params.get("DataConfigs"):
+                obj = DataConfig()
+                obj._deserialize(item)
+                self._DataConfigs.append(obj)
+        self._Message = params.get("Message")
+        self._DataSource = params.get("DataSource")
+        if params.get("ImageInfo") is not None:
+            self._ImageInfo = ImageInfo()
+            self._ImageInfo._deserialize(params.get("ImageInfo"))
+        self._ImageType = params.get("ImageType")
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
+class NotebookImageRecord(AbstractModel):
+    """镜像保存记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RecordId: 保存记录ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecordId: str
+        :param _ImageUrl: 镜像地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageUrl: str
+        :param _Status: 状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: str
+        :param _CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _Message: 状态信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param _InstanceId: 实例ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param _Kernels: kernel数组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Kernels: list of str
+        """
+        self._RecordId = None
+        self._ImageUrl = None
+        self._Status = None
+        self._CreateTime = None
+        self._Message = None
+        self._InstanceId = None
+        self._Kernels = None
+
+    @property
+    def RecordId(self):
+        return self._RecordId
+
+    @RecordId.setter
+    def RecordId(self, RecordId):
+        self._RecordId = RecordId
+
+    @property
+    def ImageUrl(self):
+        return self._ImageUrl
+
+    @ImageUrl.setter
+    def ImageUrl(self, ImageUrl):
+        self._ImageUrl = ImageUrl
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def Message(self):
+        return self._Message
+
+    @Message.setter
+    def Message(self, Message):
+        self._Message = Message
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def Kernels(self):
+        return self._Kernels
+
+    @Kernels.setter
+    def Kernels(self, Kernels):
+        self._Kernels = Kernels
+
+
+    def _deserialize(self, params):
+        self._RecordId = params.get("RecordId")
+        self._ImageUrl = params.get("ImageUrl")
+        self._Status = params.get("Status")
+        self._CreateTime = params.get("CreateTime")
+        self._Message = params.get("Message")
+        self._InstanceId = params.get("InstanceId")
+        self._Kernels = params.get("Kernels")
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
+class NotebookSetItem(AbstractModel):
+    """Notebook列表元素
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook ID
+        :type Id: str
+        :param _Name: notebook 名称
+        :type Name: str
+        :param _ChargeType: 计费模式
+        :type ChargeType: str
+        :param _ResourceConf: 资源配置
+        :type ResourceConf: :class:`tencentcloud.tione.v20211111.models.ResourceConf`
+        :param _ResourceGroupId: 预付费资源组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceGroupId: str
+        :param _VolumeSizeInGB: 存储卷大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VolumeSizeInGB: int
+        :param _BillingInfos: 计费金额信息，eg：2.00元/小时 (for后付费)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BillingInfos: list of str
+        :param _Tags: 标签配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of Tag
+        :param _CreateTime: 创建时间
+        :type CreateTime: str
+        :param _StartTime: 启动时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StartTime: str
+        :param _UpdateTime: 更新时间
+        :type UpdateTime: str
+        :param _RuntimeInSeconds: 运行时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RuntimeInSeconds: int
+        :param _ChargeStatus: 计费状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChargeStatus: str
+        :param _Status: 状态
+        :type Status: str
+        :param _FailureReason: 错误原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FailureReason: str
+        :param _EndTime: 结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EndTime: str
+        :param _PodName: Pod名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PodName: str
+        :param _InstanceTypeAlias: 后付费资源规格名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceTypeAlias: str
+        :param _ResourceGroupName: 预付费资源组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceGroupName: str
+        :param _AutoStopping: 是否自动终止
+        :type AutoStopping: bool
+        :param _AutomaticStopTime: 自动停止时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AutomaticStopTime: int
+        :param _VolumeSourceType: 存储的类型。取值包含： 
+    FREE:        预付费的免费存储
+    CLOUD_PREMIUM： 高性能云硬盘
+    CLOUD_SSD： SSD云硬盘
+    CFS:     CFS存储，包含NFS和turbo
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VolumeSourceType: str
+        :param _VolumeSourceCFS: CFS存储的配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VolumeSourceCFS: :class:`tencentcloud.tione.v20211111.models.CFSConfig`
+        :param _Message: notebook 信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param _UserTypes: notebook用户类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserTypes: list of str
+        """
+        self._Id = None
+        self._Name = None
+        self._ChargeType = None
+        self._ResourceConf = None
+        self._ResourceGroupId = None
+        self._VolumeSizeInGB = None
+        self._BillingInfos = None
+        self._Tags = None
+        self._CreateTime = None
+        self._StartTime = None
+        self._UpdateTime = None
+        self._RuntimeInSeconds = None
+        self._ChargeStatus = None
+        self._Status = None
+        self._FailureReason = None
+        self._EndTime = None
+        self._PodName = None
+        self._InstanceTypeAlias = None
+        self._ResourceGroupName = None
+        self._AutoStopping = None
+        self._AutomaticStopTime = None
+        self._VolumeSourceType = None
+        self._VolumeSourceCFS = None
+        self._Message = None
+        self._UserTypes = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def ChargeType(self):
+        return self._ChargeType
+
+    @ChargeType.setter
+    def ChargeType(self, ChargeType):
+        self._ChargeType = ChargeType
+
+    @property
+    def ResourceConf(self):
+        return self._ResourceConf
+
+    @ResourceConf.setter
+    def ResourceConf(self, ResourceConf):
+        self._ResourceConf = ResourceConf
+
+    @property
+    def ResourceGroupId(self):
+        return self._ResourceGroupId
+
+    @ResourceGroupId.setter
+    def ResourceGroupId(self, ResourceGroupId):
+        self._ResourceGroupId = ResourceGroupId
+
+    @property
+    def VolumeSizeInGB(self):
+        return self._VolumeSizeInGB
+
+    @VolumeSizeInGB.setter
+    def VolumeSizeInGB(self, VolumeSizeInGB):
+        self._VolumeSizeInGB = VolumeSizeInGB
+
+    @property
+    def BillingInfos(self):
+        return self._BillingInfos
+
+    @BillingInfos.setter
+    def BillingInfos(self, BillingInfos):
+        self._BillingInfos = BillingInfos
+
+    @property
+    def Tags(self):
+        return self._Tags
+
+    @Tags.setter
+    def Tags(self, Tags):
+        self._Tags = Tags
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
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
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
+    def RuntimeInSeconds(self):
+        return self._RuntimeInSeconds
+
+    @RuntimeInSeconds.setter
+    def RuntimeInSeconds(self, RuntimeInSeconds):
+        self._RuntimeInSeconds = RuntimeInSeconds
+
+    @property
+    def ChargeStatus(self):
+        return self._ChargeStatus
+
+    @ChargeStatus.setter
+    def ChargeStatus(self, ChargeStatus):
+        self._ChargeStatus = ChargeStatus
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def FailureReason(self):
+        return self._FailureReason
+
+    @FailureReason.setter
+    def FailureReason(self, FailureReason):
+        self._FailureReason = FailureReason
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
+    def PodName(self):
+        return self._PodName
+
+    @PodName.setter
+    def PodName(self, PodName):
+        self._PodName = PodName
+
+    @property
+    def InstanceTypeAlias(self):
+        return self._InstanceTypeAlias
+
+    @InstanceTypeAlias.setter
+    def InstanceTypeAlias(self, InstanceTypeAlias):
+        self._InstanceTypeAlias = InstanceTypeAlias
+
+    @property
+    def ResourceGroupName(self):
+        return self._ResourceGroupName
+
+    @ResourceGroupName.setter
+    def ResourceGroupName(self, ResourceGroupName):
+        self._ResourceGroupName = ResourceGroupName
+
+    @property
+    def AutoStopping(self):
+        return self._AutoStopping
+
+    @AutoStopping.setter
+    def AutoStopping(self, AutoStopping):
+        self._AutoStopping = AutoStopping
+
+    @property
+    def AutomaticStopTime(self):
+        return self._AutomaticStopTime
+
+    @AutomaticStopTime.setter
+    def AutomaticStopTime(self, AutomaticStopTime):
+        self._AutomaticStopTime = AutomaticStopTime
+
+    @property
+    def VolumeSourceType(self):
+        return self._VolumeSourceType
+
+    @VolumeSourceType.setter
+    def VolumeSourceType(self, VolumeSourceType):
+        self._VolumeSourceType = VolumeSourceType
+
+    @property
+    def VolumeSourceCFS(self):
+        return self._VolumeSourceCFS
+
+    @VolumeSourceCFS.setter
+    def VolumeSourceCFS(self, VolumeSourceCFS):
+        self._VolumeSourceCFS = VolumeSourceCFS
+
+    @property
+    def Message(self):
+        return self._Message
+
+    @Message.setter
+    def Message(self, Message):
+        self._Message = Message
+
+    @property
+    def UserTypes(self):
+        return self._UserTypes
+
+    @UserTypes.setter
+    def UserTypes(self, UserTypes):
+        self._UserTypes = UserTypes
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._Name = params.get("Name")
+        self._ChargeType = params.get("ChargeType")
+        if params.get("ResourceConf") is not None:
+            self._ResourceConf = ResourceConf()
+            self._ResourceConf._deserialize(params.get("ResourceConf"))
+        self._ResourceGroupId = params.get("ResourceGroupId")
+        self._VolumeSizeInGB = params.get("VolumeSizeInGB")
+        self._BillingInfos = params.get("BillingInfos")
+        if params.get("Tags") is not None:
+            self._Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self._Tags.append(obj)
+        self._CreateTime = params.get("CreateTime")
+        self._StartTime = params.get("StartTime")
+        self._UpdateTime = params.get("UpdateTime")
+        self._RuntimeInSeconds = params.get("RuntimeInSeconds")
+        self._ChargeStatus = params.get("ChargeStatus")
+        self._Status = params.get("Status")
+        self._FailureReason = params.get("FailureReason")
+        self._EndTime = params.get("EndTime")
+        self._PodName = params.get("PodName")
+        self._InstanceTypeAlias = params.get("InstanceTypeAlias")
+        self._ResourceGroupName = params.get("ResourceGroupName")
+        self._AutoStopping = params.get("AutoStopping")
+        self._AutomaticStopTime = params.get("AutomaticStopTime")
+        self._VolumeSourceType = params.get("VolumeSourceType")
+        if params.get("VolumeSourceCFS") is not None:
+            self._VolumeSourceCFS = CFSConfig()
+            self._VolumeSourceCFS._deserialize(params.get("VolumeSourceCFS"))
+        self._Message = params.get("Message")
+        self._UserTypes = params.get("UserTypes")
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
 class OcrLabelInfo(AbstractModel):
     """OCR场景标签列表
 
     """
 
     def __init__(self):
         r"""
@@ -12258,14 +14639,116 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ResourceConf(AbstractModel):
+    """Notebook资源参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Cpu: cpu 处理器资源, 单位为1/1000核 (for预付费)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Cpu: int
+        :param _Memory: memory 内存资源, 单位为1M (for预付费)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Memory: int
+        :param _Gpu: gpu Gpu卡资源，单位为1单位的GpuType，例如GpuType=T4时，1 Gpu = 1/100 T4卡，GpuType=vcuda时，1 Gpu = 1/100 vcuda-core (for预付费)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Gpu: int
+        :param _GpuType: GpuType 卡类型 vcuda, T4,P4,V100等 (for预付费)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GpuType: str
+        :param _InstanceType: 计算规格 (for后付费)，可选值如下：
+TI.S.LARGE.POST: 4C8G 
+TI.S.2XLARGE16.POST:  8C16G 
+TI.S.2XLARGE32.POST:  8C32G 
+TI.S.4XLARGE32.POST:  16C32G
+TI.S.4XLARGE64.POST:  16C64G
+TI.S.6XLARGE48.POST:  24C48G
+TI.S.6XLARGE96.POST:  24C96G
+TI.S.8XLARGE64.POST:  32C64G
+TI.S.8XLARGE128.POST : 32C128G
+TI.GN10.2XLARGE40.POST: 8C40G V100*1 
+TI.GN10.5XLARGE80.POST:  18C80G V100*2 
+TI.GN10.10XLARGE160.POST :  32C160G V100*4
+TI.GN10.20XLARGE320.POST :  72C320G V100*8
+TI.GN7.8XLARGE128.POST: 32C128G T4*1 
+TI.GN7.10XLARGE160.POST: 40C160G T4*2 
+TI.GN7.20XLARGE320.POST: 80C320G T4*4
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceType: str
+        """
+        self._Cpu = None
+        self._Memory = None
+        self._Gpu = None
+        self._GpuType = None
+        self._InstanceType = None
+
+    @property
+    def Cpu(self):
+        return self._Cpu
+
+    @Cpu.setter
+    def Cpu(self, Cpu):
+        self._Cpu = Cpu
+
+    @property
+    def Memory(self):
+        return self._Memory
+
+    @Memory.setter
+    def Memory(self, Memory):
+        self._Memory = Memory
+
+    @property
+    def Gpu(self):
+        return self._Gpu
+
+    @Gpu.setter
+    def Gpu(self, Gpu):
+        self._Gpu = Gpu
+
+    @property
+    def GpuType(self):
+        return self._GpuType
+
+    @GpuType.setter
+    def GpuType(self, GpuType):
+        self._GpuType = GpuType
+
+    @property
+    def InstanceType(self):
+        return self._InstanceType
+
+    @InstanceType.setter
+    def InstanceType(self, InstanceType):
+        self._InstanceType = InstanceType
+
+
+    def _deserialize(self, params):
+        self._Cpu = params.get("Cpu")
+        self._Memory = params.get("Memory")
+        self._Gpu = params.get("Gpu")
+        self._GpuType = params.get("GpuType")
+        self._InstanceType = params.get("InstanceType")
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
 class ResourceConfigInfo(AbstractModel):
     """资源配置
 
     """
 
     def __init__(self):
         r"""
@@ -14782,14 +17265,72 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class StartNotebookRequest(AbstractModel):
+    """StartNotebook请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook id
+        :type Id: str
+        """
+        self._Id = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
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
+class StartNotebookResponse(AbstractModel):
+    """StartNotebook返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class StartTrainingTaskRequest(AbstractModel):
     """StartTrainingTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -14984,14 +17525,72 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class StopCreatingImageRequest(AbstractModel):
+    """StopCreatingImage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RecordId: 镜像保存记录ID
+        :type RecordId: str
+        """
+        self._RecordId = None
+
+    @property
+    def RecordId(self):
+        return self._RecordId
+
+    @RecordId.setter
+    def RecordId(self, RecordId):
+        self._RecordId = RecordId
+
+
+    def _deserialize(self, params):
+        self._RecordId = params.get("RecordId")
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
+class StopCreatingImageResponse(AbstractModel):
+    """StopCreatingImage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class StopModelAccelerateTaskRequest(AbstractModel):
     """StopModelAccelerateTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -15068,14 +17667,72 @@
 
     def _deserialize(self, params):
         self._ModelAccTaskId = params.get("ModelAccTaskId")
         self._AsyncTaskId = params.get("AsyncTaskId")
         self._RequestId = params.get("RequestId")
 
 
+class StopNotebookRequest(AbstractModel):
+    """StopNotebook请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: notebook id
+        :type Id: str
+        """
+        self._Id = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
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
+class StopNotebookResponse(AbstractModel):
+    """StopNotebook返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
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
+        self._RequestId = params.get("RequestId")
+
+
 class StopTrainingTaskRequest(AbstractModel):
     """StopTrainingTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.945/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.946/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.945/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.946/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.945
+Version: 3.0.946
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.945/README.rst` & `tencentcloud-sdk-python-tione-3.0.946/README.rst`

 * *Files identical despite different names*

